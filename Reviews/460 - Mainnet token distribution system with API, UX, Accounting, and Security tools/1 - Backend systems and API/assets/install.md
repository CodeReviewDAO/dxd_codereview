```sh
@ggurbet ➜ /workspaces/casperfyre-backend (main) $ sudo mysql -u root
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 12
Server version: 8.0.29-0ubuntu0.20.04.3 (Ubuntu)

Copyright (c) 2000, 2022, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'crdao';
Query OK, 0 rows affected (0.05 sec)

mysql> create database casperfyre;
Query OK, 1 row affected (0.05 sec)

mysql> exit
Bye
@ggurbet ➜ /workspaces/casperfyre-backend (main) $ sudo mkdir /var/www
@ggurbet ➜ /workspaces/casperfyre-backend (main) $ cd /var/www/
@ggurbet ➜ /var/www $ sudo git clone https://github.com/ledgerleapllc/casperfyre-backend casperfyre-api
Cloning into 'casperfyre-api'...
remote: Enumerating objects: 1565, done.
remote: Counting objects: 100% (349/349), done.
remote: Compressing objects: 100% (160/160), done.
remote: Total 1565 (delta 220), reused 299 (delta 184), pack-reused 1216
Receiving objects: 100% (1565/1565), 14.62 MiB | 13.03 MiB/s, done.
Resolving deltas: 100% (979/979), done.
```

```sh
@ggurbet ➜ /var/www/casperfyre-api $ sudo ./setup.sh
Setting up CasperFYRE API..

Press enter to continue >Please have your database and vhost details ready before starting this setup.



Your email address (Admin email)
Your email: crdao@ggurbet.com
Please enter the main URL of this server (eg. casperfyre.com)
Main domain URL: ggurbet.com
API domain URL: Please enter the API URL of this server (eg. api.casperfyre.com)
api.ggurbet.com
Node IP: Please enter a known validator IP. Default (18.219.70.138)

Database host: Please enter your database hostname. Default (localhost)

Please enter your database user. Default (root) 
Database username: 
Please enter your database password. 
Database password: 
Generating entropy...
./setup.sh: line 71: warning: command substitution: ignored null byte in input
./setup.sh: line 73: warning: command substitution: ignored null byte in input
Keys created
Configuring...
Checking for required software...
Installing Apache2

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Reading package lists...
Building dependency tree...
Reading state information...
The following additional packages will be installed:
  apache2-bin apache2-data apache2-utils libaprutil1-dbd-sqlite3
  libaprutil1-ldap libjansson4 liblua5.2-0 ssl-cert
Suggested packages:
  apache2-doc apache2-suexec-pristine | apache2-suexec-custom ufw
  openssl-blacklist
The following NEW packages will be installed:
  apache2 apache2-bin apache2-data apache2-utils libaprutil1-dbd-sqlite3
  libaprutil1-ldap libjansson4 liblua5.2-0 ssl-cert
0 upgraded, 9 newly installed, 0 to remove and 0 not upgraded.
Need to get 1,691 kB of archives.
After this operation, 7,527 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1-dbd-sqlite3 amd64 1.6.1-4ubuntu2 [10.5 kB]
Get:2 http://archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1-ldap amd64 1.6.1-4ubuntu2 [8,736 B]
Get:3 http://archive.ubuntu.com/ubuntu focal/main amd64 libjansson4 amd64 2.12-1build1 [28.9 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal/main amd64 liblua5.2-0 amd64 5.2.4-1.1build3 [106 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-bin amd64 2.4.41-4ubuntu3.12 [1,181 kB]
Get:6 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-data all 2.4.41-4ubuntu3.12 [159 kB]
Get:7 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-utils amd64 2.4.41-4ubuntu3.12 [84.5 kB]
Get:8 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2 amd64 2.4.41-4ubuntu3.12 [95.6 kB]
Get:9 http://archive.ubuntu.com/ubuntu focal/main amd64 ssl-cert all 1.0.39 [17.0 kB]
Preconfiguring packages ...
Fetched 1,691 kB in 0s (15.1 MB/s)
                                  Selecting previously unselected package libaprutil1-dbd-sqlite3:amd64.
(Reading database ... 71108 files and directories currently installed.)
Preparing to unpack .../0-libaprutil1-dbd-sqlite3_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1-dbd-sqlite3:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libaprutil1-ldap:amd64.
Preparing to unpack .../1-libaprutil1-ldap_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1-ldap:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libjansson4:amd64.
Preparing to unpack .../2-libjansson4_2.12-1build1_amd64.deb ...
Unpacking libjansson4:amd64 (2.12-1build1) ...
Selecting previously unselected package liblua5.2-0:amd64.
Preparing to unpack .../3-liblua5.2-0_5.2.4-1.1build3_amd64.deb ...
Unpacking liblua5.2-0:amd64 (5.2.4-1.1build3) ...
Selecting previously unselected package apache2-bin.
Preparing to unpack .../4-apache2-bin_2.4.41-4ubuntu3.12_amd64.deb ...
Unpacking apache2-bin (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package apache2-data.
Preparing to unpack .../5-apache2-data_2.4.41-4ubuntu3.12_all.deb ...
Unpacking apache2-data (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package apache2-utils.
Preparing to unpack .../6-apache2-utils_2.4.41-4ubuntu3.12_amd64.deb ...
Unpacking apache2-utils (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package apache2.
Preparing to unpack .../7-apache2_2.4.41-4ubuntu3.12_amd64.deb ...
Unpacking apache2 (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package ssl-cert.
Preparing to unpack .../8-ssl-cert_1.0.39_all.deb ...
Unpacking ssl-cert (1.0.39) ...
Setting up libaprutil1-ldap:amd64 (1.6.1-4ubuntu2) ...
Setting up libaprutil1-dbd-sqlite3:amd64 (1.6.1-4ubuntu2) ...
Setting up libjansson4:amd64 (2.12-1build1) ...
Setting up ssl-cert (1.0.39) ...
Setting up liblua5.2-0:amd64 (5.2.4-1.1build3) ...
Setting up apache2-data (2.4.41-4ubuntu3.12) ...
Setting up apache2-utils (2.4.41-4ubuntu3.12) ...
Setting up apache2-bin (2.4.41-4ubuntu3.12) ...
Setting up apache2 (2.4.41-4ubuntu3.12) ...
Enabling module mpm_event.
Enabling module authz_core.
Enabling module authz_host.
Enabling module authn_core.
Enabling module auth_basic.
Enabling module access_compat.
Enabling module authn_file.
Enabling module authz_user.
Enabling module alias.
Enabling module dir.
Enabling module autoindex.
Enabling module env.
Enabling module mime.
Enabling module negotiation.
Enabling module setenvif.
Enabling module filter.
Enabling module deflate.
Enabling module status.
Enabling module reqtimeout.
Enabling conf charset.
Enabling conf localized-error-pages.
Enabling conf other-vhosts-access-log.
Enabling conf security.
Enabling conf serve-cgi-bin.
Enabling site 000-default.
Created symlink /etc/systemd/system/multi-user.target.wants/apache2.service → /lib/systemd/system/apache2.service.
Created symlink /etc/systemd/system/multi-user.target.wants/apache-htcacheclean.service → /lib/systemd/system/apache-htcacheclean.service.
invoke-rc.d: could not determine current runlevel
invoke-rc.d: policy-rc.d denied execution of start.
Processing triggers for systemd (245.4-4ubuntu3.17) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.9) ...

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Reading package lists...
Building dependency tree...
Reading state information...
software-properties-common is already the newest version (0.99.9.8).
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
PHP installed
Installing Casper Client
deb https://repo.casperlabs.io/releases bionic main
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  3179  100  3179    0     0   6307      0 --:--:-- --:--:-- --:--:--  6295
Warning: apt-key output should not be parsed (stdout is not a terminal)
OK

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Hit:1 http://archive.ubuntu.com/ubuntu focal InRelease
Get:2 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Hit:3 https://cli.github.com/packages stable InRelease
Hit:4 https://packages.microsoft.com/repos/microsoft-ubuntu-focal-prod focal InRelease
Get:5 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Hit:6 http://ppa.launchpad.net/xapienz/curl34/ubuntu focal InRelease
Hit:7 https://repo.anaconda.com/pkgs/misc/debrepo/conda stable InRelease
Get:8 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Get:9 https://repo.casperlabs.io/releases bionic InRelease [3,170 B]
Get:11 https://repo.casperlabs.io/releases bionic/main amd64 Packages [5,548 B]
Hit:10 https://packagecloud.io/github/git-lfs/ubuntu focal InRelease
Fetched 345 kB in 1s (234 kB/s)
Reading package lists...
Building dependency tree...
Reading state information...
All packages are up to date.

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Reading package lists...
Building dependency tree...
Reading state information...
The following NEW packages will be installed:
  casper-client
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 3,720 kB of archives.
After this operation, 18.2 MB of additional disk space will be used.
Get:1 https://repo.casperlabs.io/releases bionic/main amd64 casper-client amd64 1.5.0-0+bionic [3,720 kB]
Fetched 3,720 kB in 1s (6,758 kB/s)
                                   Selecting previously unselected package casper-client.
(Reading database ... 71810 files and directories currently installed.)
Preparing to unpack .../casper-client_1.5.0-0+bionic_amd64.deb ...
Unpacking casper-client (1.5.0-0+bionic) ...
Setting up casper-client (1.5.0-0+bionic) ...

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Reading package lists...
Building dependency tree...
Reading state information...
curl is already the newest version (7.68.0-1ubuntu2.12).
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
Enabling module rewrite.
To activate the new configuration, you need to run:
  service apache2 restart
Enabling module headers.
To activate the new configuration, you need to run:
  service apache2 restart
Considering dependency setenvif for ssl:
Module setenvif already enabled
Considering dependency mime for ssl:
Module mime already enabled
Considering dependency socache_shmcb for ssl:
Enabling module socache_shmcb.
Enabling module ssl.
See /usr/share/doc/apache2/README.Debian.gz on how to configure SSL and create self-signed certificates.
To activate the new configuration, you need to run:
  service apache2 restart
 * Restarting Apache httpd web server apache2
AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.0.1. Set the 'ServerName' directive globally to suppress this message
   ...done.
No composer.lock file present. Updating dependencies to latest instead of installing from lock file. See https://getcomposer.org/install for more information.
Loading composer repositories with package information
Info from https://repo.packagist.org: #StandWithUkraine
Updating dependencies
Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - Root composer.json requires make-software/casper-php-sdk dev-master -> satisfiable by make-software/casper-php-sdk[dev-master].
    - make-software/casper-php-sdk dev-master requires php >=7.4 -> your php version (7.3.27) does not satisfy that requirement.

Loading composer repositories with package information
Updating dependencies
Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - Root composer.json requires make-software/casper-php-sdk dev-master -> satisfiable by make-software/casper-php-sdk[dev-master].
    - make-software/casper-php-sdk dev-master requires php >=7.4 -> your php version (7.3.27) does not satisfy that requirement.

./setup.sh: line 215: crontab: command not found
Installing crontab
./setup.sh: line 221: crontab: command not found
./setup.sh: line 222: crontab: command not found
./setup.sh: line 223: crontab: command not found
./setup.sh: line 224: crontab: command not found
./setup.sh: line 225: crontab: command not found
[+] Done

Please note, you will still need to setup emailer credentials information in your .env before the email scheduler will work.

BACKUP YOUR MASTER KEY --> bdd41fb4106462282dc2ca774d1992b0
Wallet keys/token balances will be lost if this key is lost.
```

