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

The reviewer followed the instructions on the README of the project to build and deploy to the Testnet, and test its functionality by running the tests. The procedure was carried out on Ubuntu 20.04.

At the first attempts of following the instructions, the reviewer encountered a number of issues/errors, mostly at the documentation level, causing the project to be not buildable/deployable/usable, which would normally result in a review with a FAIL recommendation. The reviewer provided the OP with the feedback coming out of these attempts. The OP fixed & improved the project and its documentation based on the feedback, and informed the reviewer that the project is now ready to be reviewed. The review presented here covers the latest version of the project which includes all of those fixes and the improvements.

Reviewer first installed the prerequisites by following the instructions on the main README, and then built and deployed the smart contracts by following the instructions on the README.

- [Build logs](assets/build.md)
- [TestNet deploy hashes](assets/deploy-hashes)

Then the reviewer observed the user interface in action, on the demo video provided by the OP.

![Curve DAO Usage Demo](assets/CurveDAODemo.gif)

Then the reviewer observed that it was possible to sign into the temporary installation connected to the smart contracts deployed on the TestNet, provided by the OP as promised on the respective milestone's acceptance criteria.

![Curve DAO Test Instance Connected](assets/CurveDAOTestInstance.png)

It was also observed that the Gauge Weight Vote menu was returning a blank screen, and the OP informed the reviewer that it is out of scope for this submission, and it would be a piece that will be completed by another project later.

## Overall Impression of usage testing

It was observed that the project builds and passes the automated tests successfully after the fixes and improvements by the OP, and the documentation provides sufficient installation/execution instructions. However, the reviewer thinks that the documentation still has room for improvement towards more explanations about the command parameters, better gas amount values on the sample commands, as well as more explanations covering the entirety of the project as it is a complex one which may be hard to understand, with many different smart contract units. It is also worth mentioning that no heavy/extensive testing on the UI was done during this review due to that part being in the scope of the next milestone of the project.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

The project has sufficient tests covering both the positive and the negative paths. Moreover, there is an easy to use helper script provided by the OP, which builds and deploys all contracts to the TestNet. The reviewer observed that all of the tests successfully pass.

The reviewer also observed that the project has CI facilities in place, automatically building and testing the smart contracts on every new commit. However, it was also observed that the CI action has been failing since a certain commit. **Although the reviewer doesn't consider this as a cause to fail the review because the builds and tests of the project actually succeeds when the instructions are followed; taking the complexity of the project into account, the reviewer highly suggests OP to fix the CI actions as soon as possible. Otherwise, there would be no way to know that the project is still buildable at a later date after new commits or dependency updates.**

[Test logs](assets/test.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that although the OP did an excellent job by documenting all smart contract functions on the README, **the code-level documentation for critical classes and functions is very thin, making it hard to have an easy-to-maintain code documentation which is auto-generated from the code-base. Thus, the reviewer recommends that much more code-level documentation to be added before the final milestone to improve the maintainability of such a complex project. Moreover, reviewer also recommends adding instructions for generation of the code-level documentation, or making necessary changes to make sure the code-level documentation is automatically generated and published on every commit.**

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Project Documentation was observed to be acceptable with usage documentation and examples. However, the reviewer thinks that it would be very useful to have documentation at the architecture level, documenting the "Why?"s and reasoning of the project's design decisions, as well as some less-technical documentation, explaining the project's nature and use cases.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are at an acceptable state, with room for further improvements. The code-level documentation is very thin based on the code comments although there is extensive documentation of functions on the README, thus needs to be improved before the final milestone.

The reviewer communicated the shortcomings of the documentation, along with further points of possible improvements which may not fall in the scope of this review, with the OP. OP acknowledged the feedback, and showed interest in working on further improvements.

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

Code is generally well-structured and readable. The project has been committed to GitHub, and has extensive tests.

# Final Conclusion

The project is generally in a very good shape in terms of open-source guidelines. Moreover, the project has extensive tests, and a sufficient level of documentation. The project also successfully builds and passes the automated tests, providing the promised functionality. However, the code-level documentation can be improved further based on the notes in the relevant sections of this review.

The reviewer also recommends the following points to be fixed/improved as soon as possible:
* A CI action that runs end-to-end tests by using NCTL should be added to the code repository.
* The build/text CI action to be fixed.
* Instructions to generate code-level documentation should be added to the documentation.
* Proper actions/config should be added to the repository to generate and publish code-level documentation upon every new commit.
* The sample commands need to be optimized and fixed to have proper gas amount values, and extensive explanations for each parameter, explaining not only "how" but also "why".
* The JS scripts for the end-to-end tests need to be improved to have better error & exception handling, with verbose feedback to the user. The script should also have proper measures against rate limiting on the RPC port of the connected node.
* The project documentation should be improved by adding documentation for the high-level design and architecture.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
