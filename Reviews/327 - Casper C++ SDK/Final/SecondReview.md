Grant Proposal | [327 - Casper C++ SDK](https://portal.devxdao.com/public-proposals/327)
------------ | -------------
Milestone | 3 second submission
Milestone Title | Final
OP | numlock
Reviewer | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details
This is the final milestone of the grant.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The following methods will be implemented:

- C++ version of CLType primitives
- C++ version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects
- ED25519/SECP256K1 key pairs  Wrappers
- PutDeploy RPC call implemented
- Refactoring C++ SDK calls to return Casper Domaine Specific Objects

**Acceptance criteria:**

- C++ version of CLType primitives
- C++ version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects 
- ED25519/SECP256K1 key pairs  Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects

**Additional notes regarding submission from OP:**

Requirements of the last milestone is also complete.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/yusufketen/casper-cpp-sdk | b9f9bd9


# Install & Usage Testing Procedure and Findings

## Installation

Following the instructions in the [README](https://github.com/yusufketen/casper-cpp-sdk) of the porject, reviewer was able to successfully build the source code for this milestone for both the Debug and Release builds on Ubuntu 20.04. Also, it is observed that the project builds on MacOS and Windows aswell. Logs for ubuntu can be found below: 

[Debug Build Logs](SecondReviewassets/debugbuildlogs.md)

[Release Build Logs](SecondReviewassets/releasebuildlogs.md)

[Install Build Logs](SecondReviewassets/installbuildlogs.md)

## Overall Impression of usage testing

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Project contains sufficient enough unit tests. Following the instrucrions in the [README](https://github.com/yusufketen/casper-cpp-sdk) of the porject, reviewer was able to successfully run tests successfully. Log files for unittests can be found below: 

[Tests Build Logs](SecondReviewassets/testbuildlogs.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code-level documentation is sufficient enough for this milestone of the project. It has proper comments for all critical classes and methods. Low-level code documentation allows auto generation of documentation aswell.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

README.md includes clear information about the build and installation of the SDK.

Along with build instructions, there are instructions that allow users to run examples automatically. Everything works fine except the put deploy call, and it's expected that the put deploy call won't automatically run without a private key of an account. Also, the repository includes `/example/` folder, which has code samples that show how to use every RPC call. How to run code samples is instructed in the README. The examples run as expected.

The usage instructions and examples are sufficient; however, it can even be better if "put deploy call" could be run manually as well. This can be solved by giving a path of the private key to the script, as it's done in tests. Manuel usage testing was successful for all examples and RPC calls. Usage documentation is good enough, but it can be improved by giving more examples or explenation to every call especially for "put deploy call".

Sufficient instructions are given to be able to generate auto documentation with `doxygen`. The reviewer successfully generated and was able to view the documentation after using these instructions.

As stated in previous milestones and the first review of this milestone, auto-generation of the documentation without manual user invocation can give a better experience.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

Coverage of code documentation is good enough. Build and Install instructions are clear and the reviewer was able to apply them successfully.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains CONTRIBUTING and SECURITY policie which leads to The Code of Conduct. Pull requests and Issues are enabled on the repository.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The source code is well-written and very clear. General best coding practices are used throughout the project. Code includes good enough comments as well.

# Final Conclusion

Project meets the coding standards of DEVxDAO and acceptance criteria.

The documentation is good enough as it is now. It can be improved along with the reviewers notes.

Project has very detailed and comprehensive unit test coverage. All tests work successfully.

The project has multiplatform support and has instructions for Linux, Windows and MacOS

Reviewer recommends that this submission should PASS with NOTES.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
