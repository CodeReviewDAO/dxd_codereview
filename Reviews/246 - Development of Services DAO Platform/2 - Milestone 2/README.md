Grant Proposal | [246 - Development of Services DAO Platform](https://portal.devxdao.com/public-proposals/246)
------------ | -------------
Milestone | 2
Milestone Title | Milestone 2
OP | Ekin Keçeci
Reviewer | Muhammet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Bid submission management
- Reputation management
- Voting Engine
- Authorization for three types of user(voter, member, admin)
- DEVxDAO portal integration

**Acceptance criteria:**

- Bid submission management must be developed
- Reputation management must be developed
- Voting Engine must be developed
- Authorization for user types must be checked. (voter, member, admin)

**Additional notes regarding submission from OP:**

Beta has been deployed on https://crdao.ossa.dev

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/EKON-YAZILIM/ServicesDAO | 3c36247

It was also observed that the project has one more repository which is not submitted together with the main repository above, but is an indispensable part of the project. Thus, it will also be included in this review as follows:

Repository | Revision Reviewed
------------ | -------------
https://github.com/EKON-YAZILIM/ServicesDAO_VotingEngine | 8221e05

# Install & Usage Testing Procedure and Findings

## Build

Following the instructions in the README of the project's repositories, the reviewer was able to successfully build the project for this milestone on Ubuntu 20.04 in a cloud environment as separate microservices:
* [DAO_ApiGateway](artifacts/build-DAO_ApiGateway.md)
* [DAO_DbService](artifacts/build-DAO_DbService.md)
* [DAO_IdentityService](artifacts/build-DAO_IdentityService.md)
* [DAO_LogService](artifacts/build-DAO_LogService.md)
* [DAO_NotificationService](artifacts/build-DAO_NotificationService.md)
* [DAO_WebPortal](artifacts/build-DAO_WebPortal.md)
* [DAO_ReputationService](artifacts/build-DAO_ReputationService.md)
* [DAO_VotingEngine](artifacts/build-DAO_VotingEngine.md)

## Installation

The reviewer was able to install the project on a test environment following the instructions on the repositories, only after certain changes and additions which are noted in the installation notes section below.

![Services DAO Portal Home](assets/01-PortalHome.png)

### Installation Notes
ServicesDAO's docker-compose file is simple and easily deployable, but the project's README file and the instructions seem to have some room for improvement.

Configs, covered poorly, that the reviewer had to find out by himself:
1. SMTP Configuration file
    * located at **DAO_NotificationService/appsettings.json**
2. DAO_WebPortal/appsettings.json contains **Service_ApiGateway_Url** field and its value is statically set to the developer's server address. This is **very critical information** but not provided in the README file. If you do not set this address correctly, your deployment will not run correctly.
3. Rabbitmq and MySQL passwords are static, and spread across many different files. Changing environment variable fields in the docker-compose file doesn't work.
    * Rabbitmq passwords:
    Except for the docker-compose files, files containing passwords are as follows.
    ```
    DAO_LogService/appsettings.json
    DAO_NotificationService/appsettings.json
    DAO_DbService/appsettings.test.json
    DAO_DbService/appsettings.json
    DAO_ApiGateway/appsettings.json
    DAO_IdentityService/appsettings.test.json
    DAO_IdentityService/appsettings.json
    DAO_WebPortal/appsettings.json
    ```
    * Mysql passwords: 
    Except for the docker-compose.test.yml files, files containing passwords are as follows.
    ```
    DAO_LogService/appsettings.json
    DAO_DbService/appsettings.test.json
    DAO_DbService/appsettings.json
    DAO_IdentityService/appsettings.test.json
    ```
    These passwords can easily be set with a simple find+sed command but the documentation does not cover this.

## Usage

The usage was first tested on the test deployment by the reviewer on a basic level, then judged based on the extensive usage of the beta deployment on https://crdao.ossa.dev

The reviewer was able to login to the portal with different user types (voter, member, admin), and see different options and views for each user type.

![Login as Voting Associate](assets/02-Login-VA.png)
![Login as Admin](assets/03-Login-Admin.png)
![Login as Associate](assets/04-Login-Member.png)

It was observed that the bid submission functionality exists and works on the portal.

![Bid Submission](assets/05-Bid-Submission.png)
![Bid Submission List](assets/06-Bid-Submitted.png)

The reviewer was able to see that different types of votes are taking place on the portal, producing proper outcomes as reputation minting and distribution and state changes of the jobs, evidencing the functionality of the voting engine and the reputation management.

![Voting](assets/07-Voting-In-Progress.png)
![Completed Votes](assets/08-Voting-Completed.png)
![Reputation Management](assets/09-Reputation-Management.png)

## Overall Impression of usage testing

The project builds without errors, and the project functionality meets/exceeds the acceptance criteria and operates without errors. However, the reviewer thinks that the documentation still has room for improvement regarding the installation and execution instructions especially on the points noted in the Installation Notes section.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Unit/automated testing will be checked in a later milestone.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that the critical functions of the code-base has an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Reviewer has observed that the project has detailed documentation for usage with examples, along with the installation, build and test instructions. However, the reviewer finds the installation through custom package repository less than ideal, and thus highly suggests publishing a package on the central maven repository and updating the instructions accordingly.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License. However, the promised license on the grant proposal is MIT, so proper action must be taken by the OP to correct this mismatch before the final milestone.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

## Contribution Policies

Pull requests and Issues are enabled on the repository, and the project contains CONTRIBUTING guidelines, but lacks a SECURITY policy. Because this is an SDK project which is meant to be used by many other projects, its security is especially important. Thus, the reviewer recommends preparing and publishing a proper SECURITY policy on the repository as soon as possible.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

Reviewer finds the code to be generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. The SDK is well-documented and has an acceptable level of tests.

However, **no description, website, or topics provided for the repository**, which cripples the discoverability of the project. Moreover, although it is qn OSI-approved license, the project's license mismatches the one promised on the proposal, which needs to be fixed before the final milestone.

The project also lacks a security policy, and is observed to be heavily focused on the positive paths in its unit tests. Furthermore, it is not published on the central package repository of the language, making it harder to install and use.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
