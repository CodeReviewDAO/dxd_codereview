Grant Proposal | [346 - Blockcerts on Casper (with Verifiable Credentials and Open Badges capability)](https://portal.devxdao.com/public-proposals/346)
------------ | -------------
Milestone | 1
Milestone Title | Enable Issuing Casper Blockcerts (Open Badges) - Submission 2
OP | Zan McNaught
Reviewer | Yusuf Keten

# Milestone Details
The review will cover the 1st milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

– Set up either Casper JS SDK or REST API

– Generate or obtain a list of major nodes with high uptime

– Point Casper JS SDK or REST API to major nodes and check functionality

– Fork https://github.com/blockchain-certificates/cert-tools

– Add OP's previously proprietary backwards-compatible upgrades

– Enable instantiation of Casper-compatible Blockcerts (Open Badges version)

– Fork https://github.com/blockchain-certificates/cert-issuer 

– Enable signed transactions in order to issue Casper Blockcerts (Open Badges version)

**Acceptance criteria:**

A user will be able to instantiate and issue a batch of Casper Blockcerts (Open Badges). When issued, that batch’s hash will be written to the Casper blockchain. With a properly configured validator (Milestone #3), this hash will be usable for validating Casper Blockcerts.

**Additional notes regarding submission from OP:**

– BE SURE TO ONLY REVIEW THE "v2" BRANCH!!! The "master" branch is part of a future milestone. 

– Reviewers can follow the "Casper-specific Instructions" in the README and ignore the rest (which applies to Bitcoin and Ethereum issuing).

– When you issue a Casper Blockcert, you can find its transaction ID (txid) in the logs.

– If you get a signature error, just try again a couple times or change the Casper RPC Node IP Address.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/amazanzan/casper-cert-issuer/tree/v2 | 900b371


# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of repository, the reviewer was able to successfully build the source code on Ubuntu 20.04.

[Build Logs](assets/build-run.md)

Sample deploy: https://testnet.cspr.live/deploy/f91f32eb87b5afb8cae67c9117ae0a3530621825a30d655191c6f3a96318fb2c

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Documentation provides sufficient installation/execution instructions | PASS
Project builds without errors | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The reviewer was able to successfully run the unit tests. The bash script provided in the README file was not able to run the unit tests. However, they can be run manually by running with Python. The project has unit tests for all critical classes and methods. However, the OP is encouraged to fix the test script and add more Casper-specific both positive and negative unit tests.

[Test Logs](assets/test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods. However, the OP is encouraged to add more documentation to the tests and the project.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

README.md has sufficient basic usage instructions/samples for the implemented methods which are sufficient for this early milestone. Reviewer highly suggests enriching the project-level documentation with additional information on the project's usage.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. 

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. The project as committed to GitHub. Both the unit tests and the manual tests pass. 

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are certain points noted above that could be improved on the project.

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
