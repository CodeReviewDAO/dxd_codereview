
Grant Proposal | [338 - Casper Swift SDK](https://portal.devxdao.com/public-proposals/338)
------------ | -------------
Milestone | 3
Milestone Title | Swift version of Casper Domain Objects
OP | Huy Tran
Reviewer | M. Chad ABAHMANE

## Details & Acceptance Criteria

This is the third milestone of the grant.

**Details of what will be delivered in milestone:**
- Swift version of CLType primitives
- Swift version for Casper Domain Specific Objects
- Serialization of Casper Domain Specific Objects

**Acceptance criteria**: 

- Swift version of CLType primitives
- Swift version for Casper Domain Specific Objects
- Serialization of Casper Domain Specific Objects
- Unit test full coverage


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/hienbui9999/CasperSDKInSwift | d40c158

# Install & Usage Testing Procedure and Findings

The reviewer  was able to build the project using the command line instructions given in the README file on the repository.
The reviewer was also able to load the whole project into Xcode IDE and successfully build it. 

## Overall Impression of usage testing

The reviewer was able to build the project following the instructions given in the README file and using an Xcode IDE.
The documentation provides sufficient installation/build instructions.

**However, despite the build being successful, the build console shows a lot of warnings that can indicate  potential problems in the code or in the libraries used by the SDK.
The OP is encouraged to fix these warnings for the next milestone**.


Requirement | Finding
------------ | -------------
Project builds without errors | PASS with notes
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

[338_3_Build.md](assets/338_3_Build.md)
# Code / Unit / Automated Testing

## Code

The reviewer was able to verify that all the [CLType primitives](https://casper.network/docs/design/serialization-standard#clvalue) are implemented in the  project.
The project also contains most of the Casper domain objects and entities (Deploy, Block, DeployExecutable, Era, Validator etc...) implemented in Swift.
The reviewer was also able to verify the presence of  byte serialization functions for all CLType primitives and Casper domain objects (related to sending a deploy to the network: Deploy, Block, DeployExecutable etc...).

## Unit / Automated Testing

Project contains 125 tests and 89 of them are for milestone 3. 
All the tests can be executed from the console or from the Xcode IDE. Tests cover both the positive and the negative paths,
The reviewer was able to verify test coverage for byte serialization of all CLTypes and Casper domain objects.
The reviewer has observed that [all tests run successfully](assets/test.md) without errors. 


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation
A commendable effort has been made to document the project code following the remarks made on this point in the review of milestone 2.
The code is overall well documented now and almost all critical functions designed for milestone 3 have acceptable code-level documentation.
Requirement | Finding
------------ | -------------
Code Documented | PASS 

### Project Documentation

The reviewer has observed that the project has a very acceptable level of documentation. The documentation is sufficient to understand the SDK project. There are also code examples that simplify the understanding of critical functions of the SDK.
Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient. 

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the project repository. The project has a contribution and a security policy. 
Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS 


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub and all 125 unit tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.
The SDK is well-documented and has an acceptable level of tests.
**The reviewer recommands to fix the warning that appears when building the project.**
In the reviewer's opinion, this submission should pass with notes.
# Recommendation

Recommendation | PASS with notes
------------ | -------------

