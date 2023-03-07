Grant Proposal | [498 - NFT Collateralized Loans](https://portal.devxdao.com/public-proposals/498)
------------ | -------------
Milestone | 2
Milestone Title | Code Review Based on Ethereum Contract Audit
OP | CaptainBernardo
Reviewers | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Deliverables
Code Review will be done on the ethereum contracts and fixes will be done on Casper Contracts as well.

We request half the value of this milestone in advance per #191, resolution regarding “MILESTONE PAYMENTS”.

**Acceptance criteria:**

A copy of the ethereum contract audit.
A pair of git hashes for commits before and after with all the issues addressed.

**Additional notes regarding submission from OP:**

https://github.com/Rengo-Labs/CasperLabs-LiquidNFT/commit/fc78deb067322ce69bc463df7f3ceef5c139de8c

With the explainer: 
We worked in parallel with the solidity team for LiquidNFTs and have implemented fixes from the solidity audit.  All that needs to be checked is the audit and the linked PR
https://github.com/wise-foundation/liquidnfts-audit-scope/blob/master/audit/LiquidLocker_Audit.pdf

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-LiquidNFT | 71c879c

# Install & Usage Testing Procedure and Findings

Following the instructions in the [README](https://github.com/Rengo-Labs/CasperLabs-LiquidNFT) of the project, reviewer was able to successfully build the source code and run the tests for this milestone on Ubuntu 20.04. The reviewer able to install dependencies by following the instructions too.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions. Build instructions are giving required information but can be enhanced and more clear by detailing each step. The project functionality meets/exceeds the acceptance criteria and operates without errors. The reviewer was able to run the example put deploy command successfully by following the instructions on the README. Changes have been made after the audit so it meets the acceptance criteria.

[Contract Build](assets/makeall.md)

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total 12 tests, covering both positive and negative paths.

Although the implemented tests are already in very good state, they can be enchanted and more test can be added.

[Test Logs](assets/testlogs.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

The critical functions of the project have an acceptable level of code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has sufficient documentation coverage for usage with examples, along with the installation, build and test instructions.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

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

The project published publicly on GitHub. Project documentation is sufficient enough as general. Unit test coverage is good enough but can be improved, and all test run successfully. 


# Final Conclusion

The project meets the milestone acceptance criteria. Install and usage instructions are sufficient. Tests run successfully. Commit hash with the changes after audit and the audit files can be found below.

[Commit](https://github.com/Rengo-Labs/CasperLabs-LiquidNFT/commit/fc78deb067322ce69bc463df7f3ceef5c139de8c)

[Audit file](https://github.com/wise-foundation/liquidnfts-audit-scope/blob/master/audit/LiquidLocker_Audit.pdf)

Thus, in the reviewers' opinion, this submission should PASS.

# Recommendation

Recommendation | PASS
------------ | -------------
