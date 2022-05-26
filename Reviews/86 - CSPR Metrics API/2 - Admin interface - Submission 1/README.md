Grant Proposal | [86 - 2 - CSPR Metrics API and Historical Archive for Services, Daps and Analytics](https://portal.devxdao.com/public-proposals/86)
------------ | -------------
Milestone | 2
Milestone Title | Admin interface - Submission 1
OP | Daniel Halford
Reviewer | Yasin Yalcin <yalcinyasin14@gmail.com>


## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Admin Interface

**Acceptance criteria:**

- Web interface ready to be used by administrator, allow full control and precise adjustments. API protected endpoint if required.


**Additional changes:**

- Complete rework and optimisation of all code base
- Crawler shaped to production level, additional multi-thread mechanics implemented
- Significant improvement in crawling process and speed
- Front page and user interface upgraded, functionality improved and ready for entertainment
- Increased test coverage
- Documentation updated
- API endpoints were improved and redesigned

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/a3mc/Casper-Metrics| ec4ff67

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of the repository : https://github.com/a3mc/Casper-Metrics/blob/master/docs/INSTALLATION.md

First of all , Reviewer started with installing the required dependencies.

```console
Docker 
PM2
Node v16.14.2
MySQL 8.x
Redis 

```

**Test and build the project:**

**System Preparation**

**Create user:**

```bash
  $ adduser Yasin
```

**Add user to docker group :**

```bash
  $ sudo usermod -aG docker Yasin
```

**For simplicity of this demo guide add user to sudo group as well:**

```bash
  $ sudo usermod -aG sudo Yasin
```

**Disconnect session and login back to activate new groups membership, install dependency ( for JWT generation optionally add pwgen package ):**

```bash
  $ sudo apt update && sudo apt-get install mysql-client git wget
```

**Build latest redis-cli: ( we use a default port here )**

```bash
  $ cd ~
  $ wget http://download.redis.io/redis-stable.tar.gz
  $ tar xvzf redis-stable.tar.gz
  $ cd redis-stable
  $ make
  $ cp src/redis-cli /usr/local/bin/
  $ chmod 755 /usr/local/bin/redis-cli
```

**Create folder for MySQL configuration and storage:**

```bash
  $ mkdir -p $HOME/.mysql/casper-metrics-mysql/conf.d
  $ mkdir -p $HOME/.mysql/casper-metrics-mysql/db
```

**Create and populate MySQL configuration file: ( we will point docker here )**

```bash
cat <<EOF > $HOME/.mysql/casper-metrics-mysql/conf.d/my.cnf
[mysqld]
user                         = mysql
log_error = /tmp/error.log
key_buffer_size              = 16M
myisam-recover-options       = BACKUP
max_connections              = 250
max_binlog_size              = 100M
innodb_buffer_pool_size      = 4G
innodb_buffer_pool_instances = 8
innodb_log_file_size         = 128M
table_open_cache             = 2677
open_files_limit             = 5355
EOF
```

```bash
  $ docker run --name casper-metrics-mysql -e MYSQL_ROOT_PASSWORD=password123 -e MYSQL_DATABASE=mainnet -e MYSQL_USER=apiuser -e MYSQL_PASSWORD=password123 --restart=always -d -p 0.0.0.0:3306:3306/tcp --volume=/$HOME/.mysql/casper-metrics-mysql/conf.d:/etc/mysql/conf.d --volume=/$HOME/.mysql/casper-metrics-mysql/db:/var/lib/mysql mysql:latest
```

**Check if database ready, should see 250 as set in configuration:**

```bash
  $ mysql -u apiuser -p -h 127.0.0.1 -P 3306 -e 'show global variables like "max_connections"';
```

**Switch auth method for users, we need this to ensure password authentification works as expected:**

```bash
  $ mysql -u root -p -h 127.0.0.1 -P 3306 -e "ALTER USER 'apiuser'@'%' IDENTIFIED WITH mysql_native_password BY 'password123';"
  $ mysql -u root -p -h 127.0.0.1 -P 3306 -e "ALTER USER 'root'@'%'    IDENTIFIED WITH mysql_native_password BY 'password123';"
```

**Deploy Redis:**

```bash
  $ docker run --name casper-metrics-redis --restart=always -d -p 127.0.0.1:6379:6379 redis
```

**Import database**

**flush Redis**

```bash
  $ redis-cli -n 0 flushdb
```

**Download database dump:**

```bash
  $ cd ~ && wget http://161.97.84.146/mysqldump_30_Apr_2022_13_33_19.sql
```

**Import in to previously created mainnet db:**

```bash
  $ docker exec -i casper-metrics-mysql mysql -u"root" -p"password123" mainnet < mysqldump_30_Apr_2022_13_33_19.sql
```

**Check last block ( 743151 ) and availability:**

```bash
  $ mysql -u apiuser -p -h 127.0.0.1 -P 3306 -e 'use mainnet; select id from Block ORDER BY id desc LIMIT 1';
```

**Adjust NodeJS version, currently v16.14.2, in this example we will use nvm script:**

```bash
  $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

**Export nvm path:**

```bash
  export NVM_DIR="$HOME/.nvm"
  [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

**Install required version and make default:**

```bash
  $ nvm install v16.14.2 && node --version
```

**Install PM2:**

```bash
  $ npm install -g pm2 && pm2 --version
```

**Install backend ( crawler & API )**

```bash
  $ cd ~
  $ git clone https://github.com/a3mc/Casper-Metrics.git
  $ cd Casper-Metrics/
  $ npm install
```

**We will use example.env as reference:**

```bash
  $ cp example.env .env
```

**Edit .env and adjust for your setup, in this demo we just need to generate JWT_SECRET, for example by using pwgen tool:**

```bash
  $ pwgen -N 1 -s 96
  $ nano .env
```

**Prepare database:**

```bash
  $ npm run migrate
```

**Run tests:**

```bash
  $ npm run test
```

**Start backend and check logs:**

```bash
  $ npm run start && pm2 logs all
```

**Install Public Web Interface**

**Here, in this example for testing or development we will use ng:**

```bash
  $ npm install -g @angular/cli
```
```bash
 $ cd ~
  $ git clone https://github.com/a3mc/Casper-Metrics-Front.git
  $ cd Casper-Metrics-Front
  $ npm install
  ```
 
**Run with ng, it will take a while. Deploying this way is good for debugging, UI will act slow, be patient.**

```bash
  $ ng serve
```

**Install Administrator Web Interface**

**Open new session in a separate terminal window ( we keep ng running )**

```bash
  $ cd ~
  $ git clone https://github.com/a3mc/Casper-Metrics-Admin.git
  $ cd Casper-Metrics-Admin/
  $ npm install
```

**Use ng to serve administrator interface:**

```bash
  $ ng serve
```

**If deployed remotely, to access all modules build tunnel as in example, or connect <IP:<PORT> directly ( not recommended ):**

```bash
  $ ssh <host> -L 4300:127.0.0.1:4300  -L 4200:127.0.0.1:4200  -L 3000:127.0.0.1:3000 -N
```
4300 - Public Front
  
4200 - Administrator UI
  
3000 - API


Outputs:
  
Deploy Redis and MySQL in docker
 
![img.jpeg](Assets/1.jpeg)
![img.jpeg](Assets/2.jpeg)
 
Migration of database
  
![img.jpeg](Assets/3.jpeg)
 
Run tests Result
  
![img.jpeg](Assets/4.jpeg)
 
Start backend 
  
![img.jpeg](Assets/5.jpeg)
 
Check logs
  
![img.jpeg](Assets/6.jpeg)
 
Run Casper-Metrics-Front
  
![img.jpeg](Assets/7.jpeg)
 
Run Casper-Metrics-Admin
  
![img.jpeg](Assets/8.jpeg)
 
Interface of front in local
  
![img.jpeg](Assets/9.jpeg)
 
Interface of Admin in local
  
![img.jpeg](Assets/10.jpeg)





## Overall Impression of usage testing
The reviewer was able to build and run the project with following the instructions. And also the documentation provides adequate installation/execution instructions for different scenarios. The reviewer thinks that the project functionality will meet the acceptance criteria.


Requirement | Finding
------------ | -------------
Project builds and runs without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS 


# Unit / Automated Testing

After following the instructions given in the README in the project and installing the requirements and adding the necessary configuration settings, the tests were run. No error was received during the tests. The tests cover both positive and negative test paths.


```bash
  $ npm run test
```
![img.jpeg](Assets/4.jpeg)


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer confirmed that all critical functions of the project are well documented and can be used for automated document generation.

Requirement | Finding
------------ | -------------
Code documentation | PASS

### Project Documentation

The reviewer observed that the project README has detailed usage documentation and project is generally well documented.

Requirement | Finding
------------ | -------------
Project Documentation | PASS

## Overall Conclusion on Documentation
The reviewer concluded that the project has sufficient comprehensive general documentation.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTION policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well structured and readable. Project is easy to set up from Github repository. The reviewer observed that he did not encounter any errors in the tests that would have required the project to fail the review.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. It also meets the standards required by the CRDAO. Thus, in the reviewer's opinion, this submission should PASS.

# Recommendation

Recommendation | PASS
------------ | -------------
