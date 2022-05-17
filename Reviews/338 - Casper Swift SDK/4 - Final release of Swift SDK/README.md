Grant Proposal | [338 - Casper Swift SDK](https://portal.devxdao.com/public-proposals/338)
------------ | -------------
Milestone | 4
Milestone Title | Final release of Swift SDK
OP | Huy Tran
Reviewer | Muhammet Kara

## Details & Acceptance Criteria

This is the 4th and the final milestone of the grant.

**Details of what will be delivered in milestone:**

- ED25519/SECP256K1 key pairs Wrappers
- PutDeploy RPC call implemented
- Refactoring Swift SDK calls to return Casper Domaine Specific Objects

**Acceptance criteria**: 

- ED25519/SECP256K1 key pairs Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/hienbui9999/CasperSDKInSwift | cdde4a3

# Install & Usage Testing Procedure and Findings

The reviewer  was able to build and install the project using the command line instructions given in the README file on the repository. It was also possible to run queries on the network by using the installed project.

## Overall Impression of usage testing

The reviewer observed that the project [builds](assets/build.md) without errors, documentation provides sufficient installation/execution instructions, and the project functionality meets/exceeds acceptance criteria and operates without error. There are few warnings encountered during a command-line/terminal run, but the OP's explanation for them on the README seems reasonable to the reviewer.


Requirement | Finding
------------ | -------------
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

It was observed that the project has a good amount of automated tests, covering both the positive and the negative paths. The reviewer was able to confirm that all of the [tests successfully pass](assets/test.md). 

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code is well documented with standard comments on critical functions, allowing auto-generation of the code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS 

### Project Documentation

The reviewer has observed that the project has a good level of overall documentation. The documentation is sufficient to understand the project. There are also code examples that simplify the understanding of critical functions of the SDK.

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

Code is generally well-structured and readable. The project has been committed to GitHub and all unit tests pass. However, some small white-space/styling inconsistencies were observed by the reviewer. Although these do not affect the functionality of the project, and are nowhere near a failure reason, OP is encouraged to fix them for the sake of readability of the code-base. 

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

The SDK is well-documented and has an acceptable level of tests, and the few warnings that appear during the build are explained by the OP on the README.

Although not a cause for failure, OP is encouraged to fix the very few styling and white-spacing inconsistencies in the code-base.

In the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------

