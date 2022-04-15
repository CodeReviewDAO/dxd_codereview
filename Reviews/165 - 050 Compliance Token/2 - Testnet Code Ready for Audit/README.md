
Grant Proposal | [165 - 050 Compliance Token](https://portal.devxdao.com/public-proposals/165)
------------ | -------------
Milestone | 2
Milestone Title | Testnet Code Ready for Audit
OP | futjr
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the 2nd milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

> public repo
> 050 smart contract codebase
> that compiles and is ready for audit
> Build notes and readme
> screen cast of the contract building

**Acceptance criteria:**

050 smart contract Testnet codebase that compiles and is available to audit.

**Additional notes regarding submission from OP:**

PreAuditCode base
Audit has been done.
Post Audit Fixes are in process.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Herasoft/CSPR-050-DEVxDAO-Grant | c66897b

# Install & Usage Testing Procedure and Findings

The reviewer tried to build the project following the instructions on the README, but failed with an error:
```
error: failed to parse manifest at `/workspace/.cargo/registry/src/github.com-1ecc6299db9ec823/uint-0.9.3/Cargo.toml`
```

The reviewer then informed the OP about the error, with tips for possible ways of fixing the issue, and waited until the deadline of this review job. As of the moment of submitting this review, it was not fixed yet. So, the reviewer will continue the review as best as he can, without the fix.

The following points are highly suggested to be fixed, based on this review:

- **The project does not build.**
- **The README of the project lacks deployment and usage instructions and examples.**
- **The README of the project lacks the instructions for installing the requirements for building and installing/deploying the project.**

The procedure was carried out on Ubuntu 20.04 in the cloud.

## Overall Impression of usage testing

It was observed that **the project fails to build**, following the instructions on its README, and **the documentation does not provide sufficient installation/execution instructions**. Moreover, the project does not give any information about what it is and what & how it is used for.

Thus, the reviewer thinks that this part of the review should FAIL mainly as the project fails to build although the shared video on the repository shows a build and test flow which was probably the case at a time in the past.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | NA

# Unit / Automated Testing

The project seems to have a number of tests covering both the positive and the negative paths, but **it was not possible to run them due to the build failure** noted in the previous section. Reviewer thinks that these tests would be enough for this milestone if the OP fixes the build failure, and makes sure the tests are still valid.

It was also observed that there are no CI features actively setup/used on the project's repository. **Reviewer recommends setting up proper CI actions** to protect the project from software erosion and regressions.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A

# Documentation

### Code Documentation

Project seems to have minimally acceptable level of code-level documentation in the rustdoc style, but the reviewer was not able to generate the documentation due to the build error mentioned earlier in teh review.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

**Project Documentation has been observed to be extremely sparse, and must be improved with proper deployment and usage instructions and examples, alogn with general information about the project.**

Requirement | Finding
------------ | -------------
Usage Documented | FAIL
Example Documented | FAIL


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are extremely sparse, and must be improved significantly. On the other hand, the code-level documentation seems to be at an acceptable level.

# Open Source Practices

## Licenses

The repository is correctly released under the Apache License 2.0, which is an OSI-approved open-source license.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repositories. However, **the project has no contribution or security policies**. Moreover, the repositories have **no description, website, or topics**, hindering its discoverability.

Although they are not causes for a failure, the reviewer highly suggests improving these points.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and seems to have an acceptable level of tests if they are proved to be running successfully after fixing the build error.

# Final Conclusion

It was observed that the project fails to build, the README of the project **lacks deployment and usage instructions and examples**, and its build instructions **do not have a proper section of requirements**. And it was observed that **the project fails to build**, following the instructions given.

The project seems to have a number of tests covering both the positive and the negative paths, but it was not possible to run them due to the build failure. Moreover, **there is no CI action** to automatically build and test the project over time and on changes.

**The project documentation is extremely sparse**, and must be improved with proper deployment and usage instructions and examples, along with general information about the project. The project also **lacks contribution and security policies**. Moreover, the project's repository has **no description, website, or topics**, hindering its discoverability.

Thus, in the reviewers opinion, this submission should FAIL.

# Recommendation

Recommendation | FAIL
------------ | -------------

