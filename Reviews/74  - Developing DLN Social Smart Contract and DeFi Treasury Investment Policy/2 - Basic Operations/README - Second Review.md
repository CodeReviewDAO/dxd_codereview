Grant Proposal | [74 - Developing DLN Social Smart Contract and DeFi Treasury Investment Policy](https://portal.devxdao.com/public-proposals/74)
------------ | -------------
Milestone | 2
Milestone Title | Basic Operations
OP | Dr. Adel
Reviewer | David Tai <dtaipublic@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Mint aUSDT	Internal token representing USDT stable token
- Mint aUSDC	Internal token representing BUSDC stable token
- Mint DLN	Internal token representing DLN stable token
- Mint DLNG (internal governance token)	Upon backing of users or protocol, DLNG is emitted
- Supports user deposits of assets	
- Supports redemption of internal assets for external assets

**Acceptance criteria:**

- Delivery will successfully find addresses on-chain and token balances of the test tokens in the user wallet

**Additional notes regarding submission from OP:**

Allows staking of internal assets
Allows the user to unstake internal assets with rewards
Allows users to back a proposal
Allows users to terminate backing
Fully functional interface

Those functions have been implemented as detailed in the updated document:
https://drive.google.com/file/d/1WfB48yO3aq6iLiNesdrerQ3nqZp10fyg/view?usp=sharing
The rest of the contracts have been added for the backing and un backing as well as saving the proposals on the chain.

We have experimented with a bit different approach for updating the proposals to be linked to the "a" tokens as opposed to the generic contract. 
While this approach has merits, we deduced that the single contract would be better. We are going to reintroduce the single contract next as we tie in the end-user UI next.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/dlndao/Casper_ERC20/ | 11bb5d3

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-account-info-contract, reviewer has with difficulty been able to build the project.

Automated testing for the ERC20 work but they are not specific to the project but rather mostly cover the ERC20 functionality:

```
running 7 tests
test erc20_tests::test_erc20_deploy ... ok
test erc20_tests::test_calling_construction - should panic ... ok
test erc20_tests::test_erc20_transfer ... ok
test erc20_tests::test_erc20_approve ... ok
test erc20_tests::test_erc20_transfer_too_much - should panic ... ok
test erc20_tests::test_erc20_transfer_from ... ok
test erc20_tests::test_erc20_transfer_from_too_much - should panic ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 2.74s

   Doc-tests erc20-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```

The reviewer was not able to build the project on OSX due to some sort of issue in post-css.  However, the reviewer was able to determine this was buildable under linux.  This, while not ideal can be addressed later.

## Overall Impression of usage testing

The casper signer has a whitelist of website internal to it.  To get this running, the reviewer had to install a custom version of the casper signer with modified whitelist.  When the project is live, the whitelist will be pushed to the casper signer repo.

The reviewer was able to get an explanation and video demo of the project.  The documentation is lacking on how to use the project but the video explanation is pretty clear and is included with this review.  The reviewer was able to replciate and confirm the side effects on the Casper blockchain testnet:

https://testnet.cspr.live/account/016cfd5ef2f0859fc9a2e4b43d6461d05d1ba7dfc57a4b9ed9ff6c2570b8e8e435

Documentation is relatively sparse but sufficient for the current milestone.

Requirement | Finding
------------ | -------------
Project builds and runs without errors | PASS on Linux
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Project contains 7 unit smart contract tests that can be executed from the console. Tests cover both positive and negative test paths.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Contract documentation is minimal but present.  Contract documentation should be improved with more detailed and standardized for ust.  Client documentation is minimal on the javascript client.  

Requirement | Finding
------------ | -------------
Contract Documented | PASS - should improve with more details compatible iwth rustdoc.
JS Client Documentation | PASS - should improve with more details compatible with one of the js/ts doc standards.

### Project Documentation

README.md has body of command line usage documentation.  Documentation references the incorrect contract hashes but the reviewer has brought this to the attention of the OP.

Requirement | Finding
------------ | -------------
Usage Documented | PASS - fix the incorrect testnet hashes

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should not pass.

# Open Source Practices

## Licenses

LICENSE file is present.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project does contains a CONTRIBUTING policy that links to a Code of Conduct policy.  Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project is functional but minimally documented.  The reviewer was able to replicate the video demo with the supplied build of hte casper signer.

# Final Conclusion

The project should pass in its current state with the notes addressed next review.

# Recommendation

Recommendation | PASS With Notes
------------ | -------------

