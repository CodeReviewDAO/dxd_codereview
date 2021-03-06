Grant Proposal | [72 - CasperHolders Interact with the Casper Network](https://portal.devxdao.com/public-proposals/72)
------------ | -------------
Milestone | 1
Milestone Title | Release the code to GitHub and deploy the website
OP | Killian
Reviewer | Michael Steuer <michael@make.software>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- The project will be released on GitHub with the current license.
- Website will be deployed on production for both testnet and mainnet.

**Acceptance criteria:**

- Share the GitHub & website link with the community.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/casperholders/casperholdersfront | c112926
https://github.com/casperholders/casperholdersapi | 425af5c
https://github.com/casperholders/casperholderscore | 80a32ff

### Changes

Repository | New Revision | New commits | Content
------------ | ------------- | ------------- | -------------
https://github.com/casperholders/casperholdersfront | c60a380a000d452a3c87dcda0de02713c2802a05 | 5 | Fix potential integer overflow <br> Added documentation & Integration tests
https://github.com/casperholders/casperholdersapi | 671a6c37b17a87b3cd4dbaf89fd8d921b176027c | 12 | Removed console logs <br> Removed hardcoded urls <br> Added docs / fix http codes / add swagger ui <br> Added tests with Jest
https://github.com/casperholders/casperholderscore | 49eb969489c9461c24bf457c3e545e1bd8b1bce6 | 9 | Added documentation link <br> Fix potential integer overflow <br> add tests <br> add docs



# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/casperholders/casperholdersfront, reviewer was
able to successfully build and run that project, as well as the backend API in https://github.com/casperholders/casperholdersapi
Upon first run, no errors were produced during compilation, and the CasperHolders site became available
at http://localhost:8080/. Smoke-testing the site did not result in any noteworthy error messages or notices in the JS console. 
While testing all the advertised functionality (checking balances, transferring, (un)staking, etc.) no errors were encountered and
everything worked as advertised. 

Requirement | Finding
------------ | -------------
Project builds and runs without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
API Endpoints work without error | IMPLICIT PASS 

# Unit / Automated Testing

None of the three projects contained any automated or unit tests.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

## Changes

Requirement | Changes
------------ | -------------
Unit Tests - At least one positive path test | CasperFront / API / Core test all critical paths
Unit Tests - At least one negative path test | CasperFront / API / Core test all critical paths
Unit Tests - Additional path tests | Coverage for respectively the Front / Core / Api : 84% / 85% / 86% 

# Documentation

Considering the deliverable contains multiple project repositories, each will be evaluated separately below

## CasperHoldersAPI

### Code Documentation

The code in the API project is essentially comment/documentation free

### Changes
This is now fixed. The API contains Jest tests units and JSDoc documentation + swagger ui to test the api locally

Requirement | Finding
------------ | -------------
Low level function documentation | FAIL

### Project Documentation

The README.md file provides minimum but sufficient documentation on how to install and run the project, build a docker image
and deploy with Kubernetes (even though it indicates that the Kubernetes deployment configuration is proprietary and will only work
for OP)

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS

### API Documentation

As an API project, API end point documentation is required. This project does not contain any API documentation.

### Changes
This is now fixed. The API contains a swagger & swagger ui to test the api locally (and also JSDoc documentation)

Requirement | Finding
------------ | -------------
API documentation | FAIL

## CasperHoldersFront

### Code Documentation

The code in the Front End project is essentially comment/documentation free. While many areas of the code should not require
extensive commenting (such as view markup, etc.), the business logic that interacts with the blockchain, wallets and 
tokens should contain comments/documentation.

### Changes
This is now fixed. The project contains JSDoc documentation

Requirement | Finding
------------ | -------------
Low level function documentation | FAIL

### Project Documentation

The README.md file provides sufficient documentation on how to install and run the project, build a docker image
and deploy with Kubernetes (even though it indicates that the Kubernetes deployment configuration is proprietary and will only work
for OP). It additionally explains the architecture and interaction between the 3 repositories that make up the project.

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS

### API Documentation

N/A

Requirement | Finding
------------ | -------------
API documentation | N/A

## CasperHoldersCore

### Code Documentation

The code in this project, which as a core library provides much of the API for the CasperHoldersFront project, is well
documented and each function has a clear description of its use, parameters and output.

Requirement | Finding
------------ | -------------
Low level function documentation | PASS

### Project Documentation

The README.md file provides documentation on how to install the library into another project, and presents a link
to documentation of the core library that leads to a `404 Not Found`. It does not provide documentation on building or testing
the library.

### Changes
This is now fixed. I've added the link to the documentation in the readme.

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | FAIL

### API Documentation

As the Core API library of the project, this sub-project should have detailed API documentation. While the code is well documented in-line,
no API documentation is provided for developers to use the Core API library. A dead link suggests that it may exist, but it cannot 
be verified by the reviewer.

### Changes
This is now fixed. I've added the link to the documentation in the readme and redirect users to the test folder for exemples.

Requirement | Finding
------------ | -------------
API documentation | FAIL

## Overall Conclusion on Documentation

Given the number of FAILs above, the overall conclusion has to be that this project falls short of the expected level of documentation.

# Open Source Practices

## Licenses

Each of the projects is released under the Apache 2.0 License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Each of the projects has CONTRIBUTING policy as well as a CODE OF CONDUCT for contributors. Issues and Pull Requests are enabled
for each project.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

OP's code is clean and readable. It would benefit from including comments. Negative patterns/issues that were observed:
- debugging / console.log code left in production code (e.g. https://github.com/casperholders/casperholdersapi/blob/425af5c8631dc7e45e1bf1cebfeebc39cbaace85/routes/deploy.js#L41-L43)
  - This is now fixed
- local testing related execution paths hardcoded, rather than environment based configuration (e.g. https://github.com/casperholders/casperholdersapi/blob/425af5c8631dc7e45e1bf1cebfeebc39cbaace85/routes/deploy.js#L15)
  - This is now fixed
- Integer overflow susceptible code. The code here: https://github.com/casperholders/casperholderscore/blob/80a32ffc88e7fb201e106a20e593f38883592cbd/src/services/helpers/currencyUtils.js#L14 and here: https://github.com/casperholders/casperholderscore/blob/80a32ffc88e7fb201e106a20e593f38883592cbd/src/services/helpers/currencyUtils.js#L24 
  is guaranteed to overflow when a large enough CSPR/motes amount is passed to it.
  - This is now fixed (Hopefully)
- absolutely no test coverage
  - This is now fixed. (84%+ on all three projects)
- optimistic coding, for example: https://github.com/casperholders/casperholderscore/blob/80a32ffc88e7fb201e106a20e593f38883592cbd/src/services/deploys/abstractSmartContractStoredByHashDeployParameters.js#L49 can throw exceptions but is not handling exceptions. 
  - This is **not** fixed. See https://github.com/casperholders/casperholderscore/issues/4

# Final Conclusion

The project is already live at https://casperholders.io and provides the functionality described in the grant application
and milestone acceptance criteria.
The deliverable falls short in the following areas:
* Documentation
* Automated/Unit Testing
* Code quality / potential bugs outlined above

# Recommendation

Recommendation | PASS (with notes)
------------ | -------------

Based on the shortcomings identified above, this project should **FAIL** code review. However, since the project is already
live and performs the base functionality it sets out to provide, the Reviewer recommends that the Voting Associates **PASS** this milestone
**with notes**: 

_The shortcoming need to be addressed before the submission of a final milestone in this project, in order for that milestone to pass._

### FOOTNOTES
- While it is possible to clone to project and set up another
instance of CasperHolders, under a different name and/or domain, and point it to another validator node, this project as delivered
is designed to benefit exclusively one validator at the time, and in its current iteration, only the OP. 
This observation does not affect the code review acceptance.
  - This will be fixed in the first milestone of the next Grant (#135)

