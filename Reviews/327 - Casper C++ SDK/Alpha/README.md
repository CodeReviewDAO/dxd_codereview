
Grant Proposal | [327 - Casper C++ SDK](https://portal.devxdao.com/app/proposal/327)
------------ | -------------
Milestone | 1
Milestone Title | Alpha
OP | numlock
Reviewer | Huy Tran

# Milestone Details
This is the first milestone of grant. 
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Base project of C++ SDK will be created and published on a GitHub repository.
- Following methods of the API will be fully implemented and will return when called by the SDK:
   * chainGetStateRootHash
   * infoGetPeers

**Acceptance criteria:**

- C++ SDK project available on a public GitHub repository
- It will be possible to connect to a Casper node and retrieve information by using the implemented methods.
- Following methods of the API fully implemented and will return when called:
   * chainGetStateRootHash
   *  infoGetPeers

**Additional notes regarding submission from OP:**

SDK currently only runs on Linux systems. It will have multi platform support by the last milestone.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/yusufketen/casper-cpp-sdk | 373f347

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/yusufketen/casper-cpp-sdk, reviewer was able to successfully build the source code but fail to run test for this milestone on Ubuntu 20.04

## Overall Impression of usage testing

The project builds successfully without errors, but as the reviewer tries to to the test as described at https://github.com/yusufketen/casper-cpp-sdk#test and do the running example as described at https://github.com/yusufketen/casper-cpp-sdk#run-example, **the Auto build & test FAILS on the master branch.**

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

Since the test failed there is no test case implemented. The overall result for the test is **FAIL**.

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

README.md has sufficient basic usage instructions for the implemented methods which is sufficient for this early milestone. There is one Example folder with codes for doing examples. 

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS (good example but need to review and run again when the test pass)


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient. However the code-level documentation has room for improvement although it is acceptable for this early milestone.

# Open Source Practices

## Licenses

The Project is correctly released under the Apache License 2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. However, there is no CONTRIBUTING policy or code of conduct. Moreover, the project has no security policy. Reviewer recommends adding the aforementioned policies to the project before the final milestone.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and quite readable. Comments are good enough for each method.

# Final Conclusion

The project code seems to provide the functionality described in the grant application and milestone acceptance criteria. However, since the test failed right at the start when run the test command, in the reviewer's opinion, this submission should FAIL. 

# Recommendation

Recommendation | FAIL
------------ | -------------
