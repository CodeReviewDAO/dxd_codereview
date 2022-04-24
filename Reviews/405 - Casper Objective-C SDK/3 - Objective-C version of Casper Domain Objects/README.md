Grant Proposal | [405 - Casper Objective-C SDK](https://portal.devxdao.com/public-proposals/405)
------------ | -------------
Milestone | 3
Milestone Title | Objective-C version of Casper Domain Objects - Submission 1
OP | Huy Tran
Reviewer | Yusuf Keten

# Milestone Details
The review will cover the 3rd milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Objective-C version of CLType primitives
- Objective-C version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects

**Acceptance criteria:**

- Objective-C version of CLType primitives
- Objective-C version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects 
- Unit test full coverage

**Additional notes regarding submission from OP:**

- Objective-C version of CLType primitives
- Objective-C version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects 
- Unit test full coverage

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/tqhuy2018/Casper-ObjectiveC-sdk | [7ca37b3](https://github.com/tqhuy2018/Casper-ObjectiveC-sdk/commit/7ca37b39cbde390eb4b003ce2f36c3c5d0ad4113)


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

The project has unit tests for most of the critical classes and methods. Nonetheless, the unit tests are not comprehensive. Some of the unit tests are not active although they are covering the functionality. In the reviewer's opinion, the OP is highly motivated to improve the unit tests. Current tests are better than the previous milestone tests. To sum up, the OP is strongly encouraged to improve the unit tests and enable the inactive test cases until the last milestone.

[Test Logs](assets/test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has detailed documentation for the installation, build and test instructions. However, the OP is strongly encouraged to add more detail about the usage of the project. It is expected that other projects will use the SDK. Therefore, the documentation must be updated to include the usage instructions until the project is in the final milestone.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

In the reviewer's opinion, code-level documentation is sufficient. However, the usage documentation is not enough. The OP is strongly encouraged to add more detail about the usage of the project until the project is in the final milestone.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

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

Code is generally well-structured and very readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are certain points noted above that could be improved on the project. **Especially, the OP must improve the unit tests, enable the inactive test cases, and add usage documentation(how to use the SDK in an Objective-C/Swift project) until the final milestone.**

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
