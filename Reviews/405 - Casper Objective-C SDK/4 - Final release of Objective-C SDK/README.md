Grant Proposal | [405 - Casper Objective-C SDK](https://portal.devxdao.com/public-proposals/405)
------------ | -------------
Milestone | 4
Milestone Title | Final release of Objective-C SDK
OP | Huy Tran
Reviewer | Yusuf Keten

# Milestone Details
The review will cover the 4th milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- ED25519/SECP256K1 key pairs Wrappers
- PutDeploy RPC call implemented
- Refactoring Objective-C SDK calls to return Casper Domaine Specific Objects

**Acceptance criteria:**

- ED25519/SECP256K1 key pairs Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects

**Additional notes regarding submission from OP:**

- ED25519/SECP256K1 key pairs Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/tqhuy2018/Casper-ObjectiveC-sdk | 1c38f00


# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of the repository(https://github.com/tqhuy2018/Casper-ObjectiveC-sdk), the reviewer was able to successfully build the source code on a macOS Monterey 12.3 Mac using Xcode version 13.3.

[Build Logs](assets/build-run.md)

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Project contains 425 unit tests that can be executed from the console. The reviewer has observed that all tests run successfully without errors.

[Test Logs](assets/test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has detailed documentation for the installation, build and test instructions.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, code-level documentation is sufficient.  The OP has improved the documentation from the last milestone as suggested in the review. The usage and example documentation is added to the project. Also, key pair generation and key pair wrapping implementation are extensively documented.

# Open Source Practices

## Licenses

The project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository, and the project contains a CONTRIBUTING and a SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. The project is committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

Thus, in the reviewer's opinion, this submission should pass.

# Recommendation

Recommendation | PASS
------------ | -------------
