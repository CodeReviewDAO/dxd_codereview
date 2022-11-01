Grant Proposal | [295 - Casper Scala SDK](https://portal.devxdao.com/public-proposals/295)
------------ | -------------
Milestone | 4 - Second Submission
Milestone Title | Final release of Scala SDK
OP | Mustapha Chad ABAHMANE <elmabahma@gmail.com>
Reviewers | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- ED25519/SECP256K1 key pairs  Wrappers
- PutDeploy RPC call implemented
- Refactoring Scala SDK calls to return Casper Domaine Specific Objects
- Scala SDK  published as a package via Maven and SBT

**Acceptance criteria:**

- ED25519/SECP256K1 key pairs  Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects
- Scala SDK  available as a package via Maven and SBT
- Unit tests

**Additional notes regarding submission from OP:**

Final milestone with following :

- PuDeploy RPC call implemented 

- Casper Keys wrappers and key management via CLPublicKey and KeyPair objects 

- full test coverage for casper key management  and PutDeploy RPC call 

- Scala SDK is  available in remote repositories for Maven and SBT


Notes for this second submission:

GitHub repository for this submission : 

https://github.com/abahmanem/casper-scala-sdk


- added the two missing methods and fixed the issues raised in the review: https://github.com/djhahe/dxd_codereview/tree/scala-sdk-differential-evaluation/Reviews/295%20-%20Casper%20Scala%20SDK/Differential%20evaluation%20of%20Scala%20SDK

- fixed the issues raised in: https://github.com/caspercommunityio/casper-scala-sdk/pulls

- Replaced Json fasterXml with Scala Circe library

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/abahmanem/casper-scala-sdk | a6943b8

# Install & Usage Testing Procedure and Findings

Following the instructions in the [README](https://github.com/abahmanem/casper-scala-sdk) of the project, reviewer was able to successfully build the source code and run the tests for this milestone on Ubuntu 20.04. The reviewer was also able to install the project as a dependency on a newly created project from maven, and run the queries successfully.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions. Build instructions are giving required information but can be enhabced and more clear by detailing each step. The project functionality meets/exceeds the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total 198 tests, covering both positive and negative paths. Automated actions on the repository is active. 

Although the implemented tests are already in very good state, as mentioned in the previous review, **the remaining test stubs marked as TODO should also be implemented for full coverage**, as this is the final milestone of the project.

[Test Logs](secondreviewassets/testlogs.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

The critical functions of the project have an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation. Also, auto-generated documentation is created and included in repository.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has compherensive documentation coverage for usage with examples, along with the installation, build and test instructions.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, this review should pass.

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

The project published publicly on GitHub. Project documentation is sufficient enough as general. Unit test coverage is good enough, and all test run successfully. 

Issues that have been mentioned, and created by the previous reviewers.

# Final Conclusion

The project meets the milestone acceptance criteria. The SDK is well-documented and has extensive automated tests except a few test stubs missing implementation.

Thus, in the reviewers' opinion, this submission should PASS.

# Recommendation

Recommendation | PASS
------------ | -------------
