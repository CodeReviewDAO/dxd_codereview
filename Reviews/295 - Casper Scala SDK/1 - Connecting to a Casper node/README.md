Grant Proposal | [295 - Casper Scala SDK](https://portal.devxdao.com/public-proposals/295)
------------ | -------------
Milestone | 1
Milestone Title | Connecting to a Casper node
OP | Mustapha Chad ABAHMANE <elmabahma@gmail.com>
Reviewer | Muhammet Kara <muhammetk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- First version of Scala SDK : Scala SDK project available on a public GitHub repository
- Following methods of the API fully implemented and will return when called by the SDK :
  * chain_get_state_root_hash
  * info_get_peers
- Unit tests

**Acceptance criteria:**

- Scala SDK project available on a public GitHub repository
- Following methods of the API fully implemented and will return when called :
  * chain_get_state_root_hash
  * info_get_peers
- Unit tests

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/casper-scala-sdk | e9c577d

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/caspercommunityio/casper-scala-sdk, reviewer was able to successfully build the source code for this milestone on Ubuntu 20.04.

## Overall Impression of usage testing

The project builds successfully without errors, and reviewer has observed that it can connect to a Casper node, and run the basic queries required by the milestone. However, there are no packages published for the project which can be added as a maven dependency although the README has the instructions giving the impression that it is possible to do. Reviewer acknowledges that it is not explicitly required by this early milestone, but still highly suggests publishing a sonatype package for the repository for ease of installation and usage as soon as possible.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS (Improvements recommended)
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Can connect to a Casper node | PASS

# Unit / Automated Testing

Project contains 36 unit tests that can be executed from the console. Tests cover both positive and negative test paths. The reviewer has [observed](assets/test-run.md) that all tests run successfully without errors.

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

README.md has sufficient basic usage instructions/samples for the implemented methods which is sufficient for this early milestone. Reviewer highly suggests enriching the project-level documentation with more comprehensive usage examples reflecting common scenarios before the final milestone.

Requirement | Finding
------------ | -------------
Usage Documented | PASS (Improvements suggested)
Example Documented | PASS (Improvements suggested)

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

# Open Source Practices

## Licenses

The Project is released under the MIT license. However, the link to the license at the bottom of the README is observed to be broken. Reviewer thinks that such a link on the README is unnecessary, but it needs to be fixed if the author chooses to keep it.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. However, there is no CONTRIBUTING policy or code of conduct. Moreover, the project has no security policy. Reviewer recommends adding the aforementioned policies to the project before the final milestone.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS (Improvements suggested)

# Coding Standards

## General Observations

Code is generally well-structured and very readable. However, the project on GitHub doesn't have any static analysis or build actions. Reviewer recommends adding proper CI functionality to the project to maintain a certain quality and to avoid future regressions.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are certain points noted above which could be improved on the project. Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS (request for improvements)
------------ | -------------
