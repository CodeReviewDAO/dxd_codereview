Grant Proposal | [513 - On-Chain MVPR](https://portal.devxdao.com/public-proposals/513)
------------ | -------------
Milestone | 4
Milestone Title | Variable Repository
OP | Michael Steuer
Reviewer | Ömer ÇAKMAK <farukomercakmak@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- A KYC contract built on the Casper network
- A JavaScript client that can install the KYC token, interact with all its interfaces, and facilitate E2E testing
- Documentation associated with the above

**Acceptance criteria:**

- KYC contract can be installed on the Casper Network
- KYC results can be captured and matched against unique VA identifiers
- JS Client enables installation, usage and testing of the contract

**Additional notes regarding submission from OP:**

Please find the release notes for milestones #2 and #4 here: https://github.com/make-software/dao-contracts/releases/tag/milestone-2-4

Release Notes:

This release contains the following smart contracts:

- Variable Repository - keeps track of system parameters,
- Variable Repository Voter - allows voting on system parameters,
- Admin Contract - central contract, that enables the upgrade of the whole system,
- KYC NFT - keeps track of accounts that passed the KYC process,
- KYC Voter - allows performing a KYC process and mints KYC NFT,
- VA NFT - keeps track of accounts that are VAs.
- Onboarding Voter - allows to onboard new VAs and mints VA NFT.

Notes for the DEVxDAO:
- This code fully realizes milestone #2: Variable Repository.
- This code fully realizes milestone #4: KYC Contract.
- It contains a large part of the voting code required for milestone #5: Voting Contract. A full code will be the subject of the next release.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/dao-contracts/tree/milestone-2-4 | 7c24f46


# Install & Usage Testing Procedure and Findings

The reviewer used the Pardus GNU/Linux 21.2 (twenty-one) local machine for this review.

The README provides installation instructions, but no prerequisites are specified. It is understood from the terminal output that [rust] and revelant [cargo] packages should be loaded. The reviewer installed them using the steps on the official [Rust page](https://www.rust-lang.org/tools/install):

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Note: Rust install logs [here](assets/install_rust.log)

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | PASS / FAIL / PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes

# Unit / Automated Testing

_Summarize the result of the unit testing / automated testing / integration testing provided in the Milestone. Feel free to include
automated test output, either as text, image or other artifact. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS / FAIL / PASS with Notes
Unit Tests - At least one negative path test | PASS / FAIL / PASS with Notes
Unit Tests - Additional path tests | PASS / FAIL / PASS with Notes

# Documentation

### Code Documentation

Reviewer found the code to be well documented. 

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

_Summarize the project level documentation you encountered. This covers the information provided in the README for the project, 
as well any exampled provided. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

foc@foc:~/dao-contracts$ make docs >> docs.log
  Downloaded bit-set v0.5.2
  Downloaded getrandom v0.2.4
  Downloaded log v0.4.14
  Downloaded fnv v1.0.7
  Downloaded either v1.6.1
....
warning: `casper-dao-contracts` (lib doc) generated 6 warnings
    Finished dev [unoptimized + debuginfo] target(s) in 54.31s
     Opening /home/foc/dao-contracts/target/doc/casper_dao_contracts/index.html

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

A little more sample and usage information is needed.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project does not contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

_Provide any general observations about the project you want to add to your review. These can be subjective in nature as well, and do not
contribute to your recommendation to pass or fail the submission._

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
