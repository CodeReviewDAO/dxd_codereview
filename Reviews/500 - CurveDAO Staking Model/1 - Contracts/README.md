Grant Proposal | [500 - CurveDAO Staking Model](https://portal.devxdao.com/public-proposals/500)
------------ | -------------
Milestone | 1
Milestone Title | Contracts
OP | CaptainBernardo
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

**Deliverables**
The following contracts split up into crates:
- ChildStreamer
- CurvePool
- CurveRewards
- CurveTokenV1-V3 (The logic is built on top of the previous version so all versions need to be ported)
- ERC20-CRV
- ERC20-LP (likely just reuse our LP token crate)
- FeeDistributor
- GaugeController
- LiquidityGauge V1-V4 (The logic is built on top of the previous version so all versions need to be ported)
- LiquidityGauge Reward
- Minter
- Pausable
- RewardClaimer
- RewardsOnlyGuage
- RewardStream
- Synthetic-RewardsDistributionReceipient
- Synthetix Staking Contracts (either Arcadia’s version or a new one)
- UnitVault
- VestingEscrow
- VestingEscrowFactory
- VestingEscrowSimple
- VotingEscrow

**Acceptance criteria:**


Due to the complexity of this, we will just deploy a version of this contract that’s set up to work with a testnet instance of Casper Swap

CRDAO: Verification of this milestone will include a suite of unit tests for each contract.  Due to the complexity of bootstrapping this system, our team will provide a test environment with a running version of casper swap

**Additional notes regarding submission from OP:**

 Completed per acceptance criteria

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-Curve-DAO | e6ef46b .. a806de2

# Install & Usage Testing Procedure and Findings

_Provide a detailed review of your install and usage testing of the project. Highlight any issues setting up the project,
including shortcomings in the documentation/setup instructions. Test the usage of the project against the Acceptance Criteria
provided for the grant milestone._

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

_Summarize the code level documentation you encountered. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Code Documented | PASS / FAIL / PASS with Notes

### Project Documentation

_Summarize the project level documentation you encountered. This covers the information provided in the README for the project, 
as well any exampled provided. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Usage Documented | PASS / FAIL / PASS with Notes
Example Documented | PASS / FAIL / PASS with Notes

## Overall Conclusion on Documentation

_Summarize your review of the documentation in this project, including code, usage and examples_

# Open Source Practices

## Licenses

The project is released under Apache-2.0 license, which is an OSI-approved open-source license, and it is the same license promised on the DxD proposal.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains CONTRIBUTING, SECURITY and CODE OF CONDUCT policies. Pull requests and Issues are enabled on the repositories and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

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
