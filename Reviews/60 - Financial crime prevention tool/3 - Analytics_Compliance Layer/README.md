Grant Proposal | [60 - Financial crime prevention and risk intelligence on-chain tool](https://portal.devxdao.com/public-proposals/60)
------------ | -------------
Milestone | 3
Milestone Title | Analytics/Compliance Layer
OP | Aberto
Reviewer | Mikael  Grouwet <m.grouwet@gmail.com>



# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Data analytics and compliance layer with functionalities to spot potential fraud and/or financial crime

**Acceptance criteria:**

- Incorporate an open source data visualization interface (eg. Kibana, Graphana) and provide a couple of analytics charts


**Additional notes regarding submission from OP:**
There was a major code refactor on the ORI project:
1. The project now is broken into several modules
    - ori-api (containing the REST API and database models)
    - ori-chains (contiaining the crawlers for different chains)
    - ori-client (a simple java client to use ori-api)
    - ori-dashboard (the deliverable for this milestone)
    - ori-frontend (the deliverable for the previous milestone)
    - ori-risk-metric (the module responsible for the risk metric calculations)
    - ori-shared (an implementation of DTO objects)
2. We migrated from a no-sql persistency layer (Elastic Search) to Postgresql together with hibernate
3. All dockers, jars are built with ./mvwn package command
4. The front-end also has been modified to add the capability to choose the chain
5. An ETH crawler has also been added to the project

**Notes from previous review**

With respect to this milestone specifically, after compiling the project and crawling the blockchain to populate the database (note that this might take a while) it is possible to access a preloaded dashboard after running the appropriate docker file through localhost:8088 with login: admin and password:admin (or any other value specified to the docker container running the dashboard)
**REST API**
- Swagger-ui: http://localhost:8080/q/swagger-ui/
- Swagger file: http://localhost:8080/swagger

**GraphQL API**
- GraphQL-ui: http://localhost:8080/q/graphql-ui/
- Schema: http://localhost:8080/graphql/schema.graphql

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/syntifi/ori/tree/main/ori-dashboard | 118a181

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of the repositoty : https://github.com/syntifi/ori and the file provided as a guide for this milestone
https://github.com/syntifi/ori/blob/main/TLDR-CSPR.md

the reviewer was able to :

1- Install required dependencies on an Ubuntu 20.04 cloud server:

```console
Java 11 or above
Maven (3.8.1 or above)
Docker
Docker compose (version 1.29.2 or above)
Node.js (>=14.0.0) 
```

2. Test and build the project on an Ubuntu 20.04 cloud server

```bash
~/reviews/ori$ ./mvnw clean compile

```

Output : [60-3 clean-compile](assets/build.md "build")



3. Build libs, jars and images

```bash
~/reviews/ori$ ./mvnw package -DskipTests
```

Output:  [60-3 package](assets/build_libs.md "build_libs")


4. Create a docker network ori

```bash
~/reviews/ori$ docker network create ori
```

5. Start postgresql and api modules (docker images)

```bash
~/reviews/ori$ docker-compose -f ./ori-api/src/main/docker/docker-compose-jvm.yml up -d
Creating docker_ori-postgresql_1 ... done
Creating docker_ori-api_1        ... done
```

the reviewer was able to verify that the 2 docker images were up :

```bash
docker-compose -f ori-api/src/main/docker/docker-compose-jvm.yml ps
         Name                        Command              State                    Ports
----------------------------------------------------------------------------------------------------------
docker_ori-api_1          /deployments/run-java.sh        Up      0.0.0.0:8080->8080/tcp,:::8080->8080/tcp
docker_ori-postgresql_1   docker-entrypoint.sh postgres   Up      0.0.0.0:5432->5432/tcp,:::5432->5432/tcp
```

6. Launch the crawler for CSPR chain

```bash
~/reviews/ori$ docker-compose -f ./ori-chains/ori-cspr/src/main/docker/docker-compose.yml up -d
Creating docker_ori-cspr_1 ... done
```

the reviewer was able to verify that the docker image was up :

 ```bash
 ~/reviews/ori$ docker-compose -f ori-chains/ori-cspr/src/main/docker/docker-compose.yml ps
      Name              Command        State   Ports
----------------------------------------------------
docker_ori-cspr_1   /cnb/process/web   Up
 ```
The reviewer was then able to check crawling is up and running using the following command line :

 ```bash
docker-compose -f ori-chains/ori-cspr/src/main/docker/docker-compose.yml logs -f
 ```
![crawling](assets/crawling.png "crawling CSPR")

The crawler took a long time (at least a day) to populate the database.
The crawler retrieves all the blocks, accounts and transactions of the CSPR chain from Genesis (via RPC calls). 
The OP also offered the alternative to use an image with a database containing only recent blocks.
the reviewer wanted to make sure that the crawler completed the whole process of populating the data without errors.

7. Access the front-end

The reviewer was able to check that the front end webapp is up and running.
He could then access it using the url : http://server_ip_address:8080
![front_end](assets/front_end.png "front_end")

8. Check the database was populated 

The reviewer used  pgAdmin program to check the datas was successfully injected by the crawling process :
He verified 3 main tables :
   
   * Account :

   ![account](assets/account.png "account") 

   * Block:

   ![block](assets/block.png "block")
   
   * Transaction:

   ![transaction](assets/transaction.png "transaction")
   


9. Start the dashboard

```bash
~/reviews/ori$ docker-compose -f ori-dashboard/docker/docker-compose.yml up -d
Creating docker_dashboard_1 ... done
```

The reviewer was then able to check the dashboard is up and running using the following command line :

```bash
~/reviews/ori$ docker-compose -f ori-dashboard/docker/docker-compose.yml ps
       Name                   Command               State                        Ports
--------------------------------------------------------------------------------------------------------
docker_dashboard_1   sh ./docker/entrypoint.sh   Up (healthy)   0.0.0.0:8088->8088/tcp,:::8088->8088/tcp
```




### Testing the dashboard

This review focuses on the dashboard part. 
The dashboard module uses the Apache Superset which is an open source data visualization and exploration platform. 
It is used here to have data analysis on transactions in the Casper blockchain.
These analysis can be used for coin tracing for example (used in AML).
the dashboard is currently limited to transactions analysis but can be extended to explore other datas  such as blocks, validators etc ...
In this review,  we will carry out test scenarios on the following dashboard features :

- Transactions Monitor
- Charts 

1. Access the dashboard

The reviewer was able to connect to the dashboard using the login credentials provided in the Additional notes above.

![login](assets/dashboard/login.png "login")


2. Transactions Monitor
 
The reviewer was then able to load the transactions monitor  

![login](assets/dashboard/transaction_monitor_1.png "login")


The page displays a chart representing the coin flows (limited to 100 rows) and  informations like :

- Top 10 outflows
- Top 10 inflows
- Total amount
- Total transactions


#### Filtering

The reviewer was able to filter datas using :

**'From Account' filter :**

From Account = account-hash-8c15bba2d147859c7b7a8f43028eeb4d3c9571c6e36dfecc97c77463d3af08cd

The dashboard was successfully loaded with all the transactions having this account as source

![filter1](assets/dashboard/transaction_monitor_2.png "filter1")


**'To Account' filter :**

From Account =  account-hash-00005f6d67c5303c206f5e678f4eb52703dc0665a7d08a12c8c6b55867da654d

The dashboard was successfully loaded with all the transactions having this account as recipient

![filter2](assets/dashboard/transaction_monitor_3.png "filter2")


#### Adding filters

The dashboard offers the possibility to add to the fields used to filter transaction datas.
The reviewer was able to add a new filter on the amount of transaction. 

![filter3](assets/dashboard/transaction_monitor_4.png "filter3")

Then he applied this filter with the value = 11 500 000 000 (motes). The datas was successfully loaded.

![filter4](assets/dashboard/transaction_monitor_5.png "filter4")


3- Charts

3.1 Displaying and updating charts

The dashboard offers the possibility of adding charts to visualize  transaction datas.

There are already 5 configured charts (embedded in the Transaction Monitor): 

![charts1](assets/dashboard/charts_1.png "charts1")

The reviewer was able to load all of these charts and apply changes to them.

* Example with coin flow chart : 

![charts2](assets/dashboard/charts_2.png "charts2")

The reviewer changed the 'Metric' filter from 'Count' to 'MAX':

![charts3](assets/dashboard/charts_3.png "charts3")

The  coin flow chart was updated accodingly. 

![charts4](assets/dashboard/charts_4.png "charts4")

The reviewer increased the 'Row limit' filter from 10 to 10000 rows (transaction hashes) and was able to update the chart:

![charts5](assets/dashboard/charts_5.png "charts5")

3.2 Adding new charts

The tool offers the possibility of adding many types of charts to explore transaction datas.

![charts6](assets/dashboard/charts_6.png "charts6")

The reviewer was able to add a new 'Pie' chart reflecting the transactions having a given amount.

![charts7](assets/dashboard/charts_7.png "charts7")



## Overall Impression of usage testing
The reviewer was able to build the project and the dashboard component following the instructions given in the README files on the repository.
**However, the OP is encouraged to add examples of data analysis performed when using the dashboard in the module main page. This will allow a quick understanding of the objective of the module.
It would also be desirable to mention the use of 'Apache Superset' platform in the project (with a link to the projet repository) and to add complete test scenarios in this module to allow any user to easily test the plateform**


Requirement | Finding
------------ | -------------
Project builds and runs without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS 


# Unit / Automated Testing
This part of the project uses Apache superSet to perform data analysis and exploration. 
There are currently no tools to perform automated tests on this platform. the reviewer was limited to running the above test scenarios.

Based on last review , the project contained only 24 unit tests accross all its modules . 
An effort has been made to improve the test coverage of the project which now has 107 unit tests.
The tests can be executed from the console and cover both positive and negative test paths.


```bash
~/reviews/ori$ ./mvnw test
```

Output : [60-3 unit_test](assets/unit_tests.md "tests")

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

A commendable effort has been made to document the project code following the remarks made on this point in the reviews of milestone 1. The code is now overall well documented  and almost all classes and critical functions have acceptable code-level documentation.


Requirement | Finding
------------ | -------------
Code documentation | PASS

### Project Documentation

the project documentation is generally sufficient and the instructions for building and running project The OP is encouragedmodules are clear. 
**However, it is desirable to add, within each module of the project, a detailled description of the component and its critical functions.
In order to give a quick undesrstaing of the whole project,  The OP is encouraged to add a brief description of what the project is about and its objectives. The reviewer had first to install and run the project and navigate through the different modules to get an idea of the purpose of the project.
The OP could add a diagram (simple package uml diagram) illustrating the links between the different modules.**

Requirement | Finding
------------ | -------------
Project Documentation | PASS with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient. The OP is encouraged to provide detailed documentation  on the general usage of the project and its different modules.

# Open Source Practices

## Licenses

The Project is released under the MIT License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub and all 107 unit tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. 
**The reviewer spent a significant amount of time understanding the usefulness of the project and the its features.
The reviewer thus draws the OP's attention to the need to improve the general documentation of the project and its modules during the next milestones.**

In the reviewer's opinion, this submission should PASS with Notes

# Recommendation

Recommendation | PASS with Notes
------------ | -------------

