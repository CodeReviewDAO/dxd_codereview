Grant Proposal | [670 - DotOracle - the first decentralized bridge for fungible tokens and NFTs](https://portal.devxdao.com/public-proposals/670)
------------ | -------------
Milestone | 1
Milestone Title | Bridge for fungible tokens
OP | AuroraNguyen
Reviewer | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Decentralized multiparty computation protocol for bridge validators to govern the bridge
Deploy a set of customized wrapped tokens on Casper for ERC20 & native tokens from EVM chains including Ethereum, BSC, Avalanche, MoonBeam, Okex, Fantom, Matic
A decentralized consensus protocol for the DotOracle bridge validators to validate bridge transactions made by users on EVM chains and mint corresponding wrapped tokens on Casper. Note that this process is decentralized and any changes in the protocol require the agreement of all validators.
DotOracle bridge front-end at https://bridge.dotoracle.network
Documentation for partners to integrate DotOracle bridge to provide service on Casper blockchain

**Acceptance criteria:**

DotOracle bridge launch that allows users to transfer assets back and forth from between Ethereum, Avalanche, BSC, MoonBeam, and OKC Chain, to Casper blockchain. Users use our DotOracle bridge service on https://bridge.dotoracle.network and will receive wrapped tokens on the Casper blockchain.
The DotOracle bridge is secured by a decentralized validator network, each validator of the network needs to lock DTO as bonding to secure the network
Announcements:
a.  DotOracle mainnet is live:
	https://twitter.com/DoTOracle/status/1531200689879166977?s=20&t=G7_-fAfjnS9TeTsM46Vnow
https://twitter.com/Casper_Hodlers/status/1533086345966526466?s=20&t=G7_-fAfjnS9TeTsM46Vnow
b. $DTO, $FRAX, $DAI are added to DotOracle Bridge:
	https://twitter.com/DoTOracle/status/1537024189705555969?s=20&t=G7_-fAfjnS9TeTsM46Vnow
https://twitter.com/casperinsider/status/1538921298965184512?s=20&t=G7_-fAfjnS9TeTsM46Vnow
c. 5 chains and 15+ tokens supported
https://twitter.com/DoTOracle/status/1540336978691883008?s=20&t=G7_-fAfjnS9TeTsM46Vnow
d. Integrated OKC Chain (OKEX) on DotOracle bridge
https://twitter.com/DoTOracle/status/1543829740930273280?s=20&t=G7_-fAfjnS9TeTsM46Vnow

**Additional notes regarding submission from OP:**

This submission is for the first milestone. The submission consists:
https://github.com/dotoracle/dto-validator: the code used for running validators 
https://github.com/dotoracle/bridge-contracts: the bridge contracts deployed on EVM-compatible chains: Ethereum, BSC, Avalaunche, MoonBeam, OKC 
https://github.com/dotoracle/casper-erc20: the wrapped token contract on Casper 
https://github.com/dotoracle/casper-contract-hash: the configuration for which token contracts can be bridged back and forth between Casper and EVM chains 
https://github.com/dotoracle/packages: utility packages

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/dotoracle/dto-validator | 1633259
https://github.com/dotoracle/bridge-contracts | df92c75
https://github.com/dotoracle/casper-erc20 | f8e16d2
https://github.com/dotoracle/casper-contract-hash | a53f0d5
https://github.com/dotoracle/packages | 0df6321

# Install & Usage Testing Procedure and Findings

### `dto-validator`

Repo was missing many instructions at the beginning and the reviewer sent a guide to OP to update the project's repos. OP updated this repo and informed the reviewer. Repos still had issues and the reviewer gave another feedback to OP before proceeding the final review.
By following the instructions in the [README](https://github.com/dotoracle/dto-validator) of the repository, the build has failed at first step. Install and usage examples still need improvements.

[npm install](assets/validatornpminstall.md)

### `bridge-contracts`

Repo was missing many instructions at the beginning and the reviewer sent a guide to OP to update the project's repos. OP updated this repo and informed the reviewer. Repos still had issues and the reviewer gave another feedback to OP before proceeding the final review.

By following the instructions in the [README](https://github.com/dotoracle/bridge-contracts) of the repository, the build has failed at first step. Install and usage examples still need improvements.

[npm i](assets/bridgenpmi.md)

### `casper-erc20`

Repo was missing many instructions at the beginning and the reviewer sent a guide to OP to update the project's repos. OP updated this repo and informed the reviewer. Repos still had issues and the reviewer gave another feedback to OP before proceeding the final review.

By following the instructions in the [README](https://github.com/dotoracle/casper-erc20) of the repository. The reviewer was able to build the project.

[make prepare](assets/ercmakeprepare.md)

[make build-contract](assets/ercmakebuildcontract.md)

### `casper-contract-hash`

This type of repo does not need build instructions but repo readme should be improved and more information should be added.

### `packages`

Repo is basically for of the original CASPER repo ,however it is submitted as a part of the project and It should meets the DEVxDAO and CRDAO standards and repo is missing main README.md so there is no general information or instruction included.

## Overall Impression of usage testing

### `dto-validator`

The project repository is missing usage examples or usage instructions.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

### `bridge-contracts`

The project repository has one example script but ıt needs more explanation and instruction. Also, repo should have more usage examples.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

### `casper-erc20`

The repository is a fork of original CASPER repository. There are examples forked from the original repository ,however examples are missing instructions. Instruction and How TOs should be added to repository. 

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

### `casper-contract-hash`

Requirement | Finding
------------ | -------------
Project builds without errors | N/A
Documentation provides sufficient installation/execution instructions | N/A
Project functionality meets/exceeds acceptance criteria and operates without error | N/A

### `packages`

Repo is missing main README.md so there is no general information or instruction included for usage examples.

Requirement | Finding
------------ | -------------
Project builds without errors | N/A
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

### `dto-validator`

The repository is missing tests and test instructions.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

### `bridge-contracts`

Tests could not run because of the dependency error retrieved at build step.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

### `casper-erc20`

Test instructions are given ,and tests run successfully. The repository has 22 tests total. Test coverage can be improved.

[make test](assets/ercmaketest)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

### `casper-contract-hash`

Tests or instructions not given. Reviewer thinks that this type of repository might not need tests.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/a
Unit Tests - Additional path tests | N/A

### `packages`

Testing instructions are missing.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

# Code Analysis & CI Facilities

The project doesn't have any continuous integration (CI) or code-analysis facilities on any of its repositories. As both are crucial for protecting the project against regressions and software decay as well as errors due to untested code changes, the reviewer recommends setting up at least one code analysis (similar to CodeQL) and one CI measure to the project, which would ideally run on every pull request and commit on the `main` or `mainnet` branch.

Requirement | Finding
------------ | -------------
Code Analysis | FAIL
Continuous Integration | FAIL

# Documentation

### Code Documentation

#### `dto-validator`

Api folder has acceptable level of code documentation. Other parts of the project need improvements on code level documentatıon. All critical fucntions should be commented and documented. As this is the first milestone of the project ,the reviewer thinks that this part should pass with notes.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

#### `bridge-contracts`

All critical functions and classes of the project should have comments. As general repository is poor on code level documentation and need improvements.

Requirement | Finding
------------ | -------------
Code Documented | FAIL

#### `casper-erc20`

Repository has sufficient code level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

#### `casper-contract-hash`

The reviewer thinks that this repository does not need high amount of code level documentation as 2 files included in this repository are config files ,however comments can be added

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

#### `packages`

Project does not have any code level documentation 

Requirement | Finding
------------ | -------------
Code Documented | FAIL

### Project Documentation

#### `dto-validator`

The project repository is missing usage examples or usage instructions.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL 
Example Documented | FAIL

#### `bridge-contracts`

The project repository has one example script but ıt needs more explanation and instruction. Also, repo should have more usage examples.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL 
Example Documented | FAIL

#### `casper-erc20`

Examples are forked from the original CASPER repository but no instructions added to README.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL 
Example Documented | FAIL

#### `casper-contract-hash`

Repository only have config files. README of the project needs more explanation about where they are used etc.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL 
Example Documented | FAIL

#### `packages`

README is missing in the repository.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL 
Example Documented | FAIL

## Overall Conclusion on Documentation

In the reviewer's opinion, the project documentation is poor at its current state and needs improvements. 

# Open Source Practices

## Licenses

### `dto-validator`

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

### `bridge-contracts`

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

### `casper-erc20`

The Project is released under the Apache-2.0 License ,however its mentioned as MIT on the DEVxDAO portal so this should be changed or negotiated with DEVxDAO

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

### `casper-contract-hash`

The repository does not have any licence

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

### `packages`

The repository does not have any licence

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

## Contribution Policies

### `dto-validator`

The project has Contributing policy. Security Policies and a Code of Conduct should be added to repository. Issues and pull requests are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

### `bridge-contracts`

The project has Contributing policy. Security Policies and a Code of Conduct should be added to repository. Issues and pull requests are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

### `casper-erc20`

Contributing policy, Security Policies and a Code of Conduct should be added to repository. Issues should be enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

### `casper-contract-hash`

Contributing policy, Security Policies and a Code of Conduct should be added to repository. Issues and pull requests should be enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

### `packages`

Contributing policy, Security Policies and a Code of Conduct should be added to repository. Issues and pull requests should be enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

# Coding Standards

## Dependencies

The project has a number of dependencies with high or critical-level security vulnerabilities, which are recommended to be fixed as soon as possible. Reviewer highly suggests enabling dependency checks on the project's repositories to be alerted about such vulnerabilities in the future.

### `dto-validator`

Dependency | Vulnerability | Severity
------------ | ------------- | -------------
libp2p | [CVE-2022-23487](https://github.com/advisories/GHSA-f44q-634c-jvwv) | High

### `bridge-contracts`

Dependency | Vulnerability | Severity
------------ | ------------- | -------------
@openzeppelin/contracts | [CVE-2021-41264](https://github.com/advisories/GHSA-5vp3-v4hc-gx76) | Critical
@openzeppelin/contracts | [CVE-2021-27290](https://github.com/advisories/GHSA-fg47-3c2x-m2wr) | Critical
@openzeppelin/contracts-upgradeable | [CVE-2022-35961](https://github.com/advisories/GHSA-4h98-2769-gh6h) | High
@openzeppelin/contracts-upgradeable | [CVE-2022-31198](https://github.com/advisories/GHSA-xrc4-737v-9q75) | High
@openzeppelin/contracts-upgradeable | [CVE-2022-31172](https://github.com/advisories/GHSA-4g63-c64m-25w9) | High
@openzeppelin/contracts-upgradeable | [CVE-2022-31170](https://github.com/advisories/GHSA-qh9x-gcfh-pcrw) | High
@openzeppelin/contracts | [CVE-2021-46320](https://github.com/advisories/GHSA-88g8-f5mf-f5rj) | High

### `casper-erc20`

Dependency | Vulnerability | Severity
------------ | ------------- | -------------
wee_alloc | [GHSA-rc23-xxgq-x27g](https://github.com/advisories/GHSA-rc23-xxgq-x27g) | Critical
zeroize_derive | [CVE-2021-45706](https://github.com/advisories/GHSA-c5hx-w945-j4pq) | Critical
regex | [CVE-2022-24713](https://github.com/advisories/GHSA-m5pq-gvj9-9vr8) | High
time | [CVE-2020-26235](https://github.com/advisories/GHSA-wcg3-cvx6-7396) | Moderate
num-bigint | [GHSA-v935-pqmr-g8v9](https://github.com/advisories/GHSA-v935-pqmr-g8v9) | Moderate

### `casper-contract-hash`

Dependency | Vulnerability | Severity
------------ | ------------- | -------------
N/A | N/A | N/A

### `packages`

Dependency | Vulnerability | Severity
------------ | ------------- | -------------
webpack | [CVE-2023-28154](https://github.com/advisories/GHSA-hc6q-2mpp-qw7j) | High

##CodeQL

### `dto-validator`

File | Vulnerability | Severity
------------ | ------------- | -------------
api/main.js | [js/request-forgery](https://github.com/furkanahmetk/dto-validator/security/code-scanning/1) | Critical

## General Observations

### `dto-validator`

The project has sufficient structure. Low-level code documentation and project documentation should be improved. Project does not build and run successfully. The project does not fully complies with open source standards and should be updated according to the reviewer's suggestions.

### `bridge-contracts`

The Project has many dependency vulnerabilities and one Code vulnerability that needs to fixed. Code level documentation should be added to project. Project does not build successfully with given instructions. The project does not fully complies with open source standards and should be updated according to the reviewer's suggestions.

### `casper-erc20`

The project has multiple dependency vulnerabilities that need to be fixed. Code level documentation is sufficient. Project builds and runs successfully. The project does not fully complies with open source standards and should be updated according to the reviewer's suggestions.

### `casper-contract-hash`

The Repository only have config files. The project does not complies with open source standards and should be updated according to the reviewer's suggestions.

### `packages`

The repository is missing a README file ,so there are no general instructions. Code level documentation of the project should be improved. The project does not complies with open source standards and should be updated according to the reviewer's suggestions.

# Final Conclusion

`dto-validator`, `bridge-contracts` , `casper-erc20` repositories have good shape but they need improvements as mentioned in the related sections. `casper-contract-hash`, `packages` repositories need proper repository structure. 

`dto-validator`, `bridge-contracts` does not build. If instructions are missing or incorrect they need to be fixed. 

Although not a cause for an overall failure, the project lacks the code analysis and the CI facilities, which are very important for long term success of an open-source project.

Thus, in the reviewer's opinion, this submission should FAIL.

# Recommendation

Recommendation | FAIL
------------ | -------------

