Grant Proposal | [186 - Java SDK Casper](https://portal.devxdao.com/public-proposals/186)
------------ | -------------
Milestone | 2
Milestone Title | Java SDK – ED25519/SECP256K1 key pairs
OP | ReDC
Reviewer | Chad (elmabahma@gmail.com)

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Source code in our own public Gitbhub repository;
- Unit-tests;
- Documentation

**Acceptance criteria:**

- Implements wrappers for key pairs under the curves ED25519 and SECP256K

**Additional notes regarding submission from OP:**

The implementation of the key pairs with the features such as reading pem files and signatures is available as an independent java project, under the repo:

https://github.com/syntifi/crypto-keys

and available on maven:
```xml
  <dependency>
        <groupId>com.syntifi.crypto</groupId>
        <artifactId>crypto-key-<SUBMODULE></artifactId>
        <version>VERSION</version>
   </dependency>
```
  

The implementation of the put_deploy, the service to create transfers and the relevant serialization procedures are still under the repository of milestone 1:
https://github.com/syntifi/casper-sdk

Also available on maven:
```xml
  <dependency>
    <groupId>com.syntifi.casper</groupId>
    <artifactId>casper-sdk</artifactId>
    <version>0.2.0</version>
</dependency>
```
## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/syntifi/casper-sdk| c463dae
https://github.com/syntifi/crypto-keys| e8ae3de



# Install & Usage Testing Procedure and Findings

Following the instructions in the readme files of the two repositories, the reviewer was able to:

1- build and run unit tests for the SDK:  [casper-sdk build and test](sdk-build-and-test.md)

2- build and run unit tests for the crypto module (key management) : [crypto-keys build and test](sdk-build-and-test.md)

The build and the tests were run on a MacOs Monterey 12.2.1 using the following tools:

- Java :
  ```bash
  java version "1.8.0_261"
  Java(TM) SE Runtime Environment (build 1.8.0_261-b12)
  Java HotSpot(TM) 64-Bit Server VM (build 25.261-b12, mixed mode)
  ```
- Maven :
````bash
Apache Maven 3.3.9 (bb52d8502b132ec0a5a3f4c09453c07478323dc5; 2015-11-10T17:41:47+01:00)
Java version: 1.8.0_261, vendor: Oracle Corporation
Default locale: fr_CH, platform encoding: UTF-8
OS name: "mac os x", version: "10.16", arch: "x86_64", family: "mac"

````
- Gradle:
````bash

------------------------------------------------------------
Gradle 7.4
------------------------------------------------------------

Build time:   2022-02-08 09:58:38 UTC
Revision:     f0d9291c04b90b59445041eaa75b2ee744162586
Kotlin:       1.5.31
Groovy:       3.0.9
Ant:          Apache Ant(TM) version 1.10.11 compiled on July 10 2021
JVM:          1.8.0_261 (Oracle Corporation 25.261-b12)
OS:           Mac OS X 10.16 x86_64
````

## Overall Impression of usage testing

The project builds without errors, documentation provides sufficient installation/execution instructions, and project functionality meets/exceeds acceptance criteria and operates without error.
Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Casper-sdk contains a total of 89 unit tests covering both positive and negative paths
Crypto-keys module contains 15 unit tests. The reviewer checked the presence of some unit tests on negative paths in this module.

The reviewer has checked the presence of unit tests for the functionalities related to the creation of  deploys,signing them (using crypto module) and sending
them to the network using the put-deploy RPC call which was added to the SDK in this milestone.


All these tests run successfully :

-  [casper-sdk unit test](casper-sdk-unit-tests.md)
-  [cryptos-key unit test](crypto-keys-unit-tests.md)


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that the critical functions of the code-base has an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The level of documentation on both projects is sufficient. The main page of the SDK project contains examples of using critical RPC functions.
The main page of the cryptos-keys module contains a 'how-to' detailing the main functionalities of 'key management' in the SDK.
The reviewer was able to import the maven libraries of the SDK and the crypto-key module, write and execute code snippets for both projects without too much difficulty.


Requirement | Finding
------------ | -------------
Usage Documented | PASS 
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

# Open Source Practices

## Licenses

Both projects are released under the Apache-2.0 License. 

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS 

## Contribution Policies

Pull requests and Issues are enabled on the repositories of both projects, they also contain CONTRIBUTING and SECURITY policies. 


Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Reviewer finds the code to be generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. 
In the reviewers opinion, this submission should PASS.

# Recommendation

Recommendation | PASS 
------------ | -------------

