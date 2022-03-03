
Grant Proposal | [329 - 1 - Apache Camel Casper connector](https://portal.devxdao.com/public-proposals/329)
------------ | -------------
Milestone | 1
Milestone Title | Camel casper component : CasperProducer
OP | Chad | 
Reviewer | Alexandre Carvalho <adcarvalho@gmail.com>

# Milestone Details
This is the first milestone of grant. 
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Setting up the project on a public repository on GitHub
- Implementing CasperProducer  for sending message exchanges to the Casper endpoint
- Implementing all operations of Casper node 1.4 RPC library.
- Unit testing  CasperProducer

**Acceptance criteria:**

- Camel Casper component project available on a public repository on GitHub
- CasperProducer component fully implemented, tested and documented.
- All RPC operations of Casper node RPC library 1.4 implemented.
- Unit tests passing

**Additional notes regarding submission from OP:**

- Java SDK we wanted to use for this grant was not suitable for our developements.
 We delayed submission of milestone 1 until this Java SDK was published into maven repository: 
 
 https://github.com/syntifi/casper-sdk/

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/camel-casper | [346fcdf](https://github.com/caspercommunityio/camel-casper/tree/346fcdfdf52a7b16bf0ad2bd211e05326044aac4)

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/caspercommunityio/camel-casper, reviewer was able to successfully build the source code for this milestone, and all tests have successfully passed.

Build Results can be found here: [329_1_Build.md](resources/329_1_Build.md)

## Overall Impression of usage testing

By following the provided instructions on the repository, the reviewer was able to compile and successfully run the tests. On the other hand, the lack of a test coverage report made it more difficult to analyze the quality and range of the tests. The reviewer strongly suggest the use of a test coverage and results reporting plugins (e.g. Jacoco)

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes 

The Java SDK used in this project was developed for the casper node spec v1.3. That means two RPC requests (query_global_state and info_get_validator_changes) are unavailable. The OP implemented code to support those and it would require a minimal change as soon as the SDK provides them. For this reason the reviewer considers the acceptance criteria met, therefore the 'Pass with Notes' above.

# Unit / Automated Testing

Project contains 43 unit tests that can be executed from the console. 
The reviewer has observed that all tests run successfully without errors. 

Test Results can be found here: [329_1_TestResults.md](resources/329_1_Test_Results.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS 
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation

The reviewer has observed that the project has sufficient code-level documentation with summaries and comments at least on critical classes and methods. However, the reviewer thinks that the documentation still has room for improvement, finding that in some cases said summary consisted of only the name of the class, with no description of its function or usage.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Reviewer has observed that the project has detailed documentation for usage with examples, along with the installation, build and test instructions. 

Requirement | Finding
------------ | -------------
  Usage Documented | PASS
  Example Documented | PASS


## Overall Conclusion on Documentation

Based on the reviewer's findings, this should pass with notes and attention should be paid to code-level documentation on upcoming milestones. Javadoc fails to run and is required to properly publish packages to Maven Central following its standards. Javadoc results can be found here: [329_1_Javadoc_Results.md](resources/329_1_Javadoc_Results.md)

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution and a security policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is generally well-structured and readable, although attention should be paid to code formatting, spacing and general code organization. Some logical ordering of class contents (e.g., fields, constructors, getters/setters, other methods, etc) should be used throughout the project to improve its learnability and readability. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However it should improve its code-level documentation and overall coding standards before the final milestone. Also it should properly fix javadoc content and generation to be compliant with [Maven Central requirements](https://central.sonatype.org/publish/requirements/#why-do-we-have-requirements).

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------