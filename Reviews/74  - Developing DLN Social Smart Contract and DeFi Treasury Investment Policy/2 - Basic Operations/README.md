Grant Proposal | [28 - Validator Information Standard](https://portal.devxdao.com/public-proposals/28)
------------ | -------------
Milestone | 2
Milestone Title | Sample Implementation
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
https://github.com/dlndao/Casper_ERC20/ | d77e027

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

The reviewer could not start the development server for the React and could not manually test the client:

```
Error: error:0308010C:digital envelope routines::unsupported
    at new Hash (node:internal/crypto/hash:67:19)
    at Object.createHash (node:crypto:130:10)
    at module.exports (/home/dtai/Casper_ERC20/client/node_modules/webpack/lib/util/createHash.js:135:53)
    at NormalModule._initBuildHash (/home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:417:16)
    at handleParseError (/home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:471:10)
    at /home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:503:5
    at /home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:358:12
    at /home/dtai/Casper_ERC20/client/node_modules/loader-runner/lib/LoaderRunner.js:373:3
    at iterateNormalLoaders (/home/dtai/Casper_ERC20/client/node_modules/loader-runner/lib/LoaderRunner.js:214:10)
    at iterateNormalLoaders (/home/dtai/Casper_ERC20/client/node_modules/loader-runner/lib/LoaderRunner.js:221:10)
/home/dtai/Casper_ERC20/client/node_modules/react-scripts/scripts/start.js:19
  throw err;
  ^

Error: error:0308010C:digital envelope routines::unsupported
    at new Hash (node:internal/crypto/hash:67:19)
    at Object.createHash (node:crypto:130:10)
    at module.exports (/home/dtai/Casper_ERC20/client/node_modules/webpack/lib/util/createHash.js:135:53)
    at NormalModule._initBuildHash (/home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:417:16)
    at /home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:452:10
    at /home/dtai/Casper_ERC20/client/node_modules/webpack/lib/NormalModule.js:323:13
    at /home/dtai/Casper_ERC20/client/node_modules/loader-runner/lib/LoaderRunner.js:367:11
    at /home/dtai/Casper_ERC20/client/node_modules/loader-runner/lib/LoaderRunner.js:233:18
    at context.callback (/home/dtai/Casper_ERC20/client/node_modules/loader-runner/lib/LoaderRunner.js:111:13)
    at /home/dtai/Casper_ERC20/client/node_modules/react-scripts/node_modules/babel-loader/lib/index.js:59:103 {
  opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
  library: 'digital envelope routines',
  reason: 'unsupported',
  code: 'ERR_OSSL_EVP_UNSUPPORTED'
}
```

## Overall Impression of usage testing

There was a Rust package build error that the reviewer identified which was communicated to the submitter and fixed.  There was also a build issue with node-sass and Node 17 on ubuntu that the reviewer identified that's fixed with a version update in npm/yarn which is a minor fix.  A major security flaw was discovered in the ERC-20 contract that was fixed in issue #32 of the official reference implementation `https://github.com/casper-ecosystem/erc20` which needs to be picked up.

Documentation is relatively sparse but sufficient for the current milestone. The reviewer could not get the client project running.

Requirement | Finding
------------ | -------------
Project builds and runs without errors | FAIL
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

Project contains 7 unit smart contract tests that can be executed from the console. Tests cover both positive and negative test paths.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code documentation is sparse to non-existant on the contract.  Code documentation is minimal on the javascript client.

Requirement | Finding
------------ | -------------
Contract Documented | FAIL
JS Client Documentation | PASS

### Project Documentation

README.md has body of command line usage documentation.  

Requirement | Finding
------------ | -------------
Usage Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should not pass.

# Open Source Practices

## Licenses

The Project is missing a license file.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

## Contribution Policies

The project does not contain a CONTRIBUTING policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

# Coding Standards

## General Observations

This project needs to first meet minimal requirements and fix both the build and smart contract security issues before being resubmitted.

# Final Conclusion

The project should not pass in its current state.

# Recommendation

Recommendation | FAIL
------------ | -------------

