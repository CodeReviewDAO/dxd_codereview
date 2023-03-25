Grant Proposal | [357 - Curios - Casper NFT issuance platform integration](https://portal.devxdao.com/public-proposals/357)
------------ | -------------
Milestone | 1-3
Milestone Title | CEP47 Integration Build Out - Submission 1
OP | david
Reviewer | Muhammed Didin <mdidin80@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**


**Acceptance criteria:**

- Contract can be deployed and interacted with 
- NFTs can be minted, burned and transferred 
- Casper NFTs provide same functionality as ERC-721 tokens

**Additional notes regarding submission from OP:**

Code base is the Google Lambda integration to their backend.

This means that existing closed source features of the the NFT platform is now enabled for the code:
https://www.youtube.com/watch?v=HMZE_hfg_ck

Again, the repo itself is just the open source integration into a closed source project.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://bitbucket.org/grantnpowell/casper-integration/src/master | 7a3a6bb


# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of the repository, the reviewer was able to successfully build and run the source code and use the project on macOS Monterey.

### Install
The reviewer queried `npm i` command into _command-line-integraion/js_additional_integration_ directory to install the dependencies into project. 

[Full Install Logs](assets/install.txt)

Please note that the project frontend is not suitable for building on a local computer, as it is a  Casper integration into the Curious NFT Issuance Platform.

### Usage

Queries successfully works for deploy, mint and transfer tokens.

[Full Deploy Logs](assets/deploy.txt)

[Full Mint Logs](assets/mint.txt)

[Full Transfer Logs](assets/transfer.txt)

Sample Mint Deploy: https://testnet.cspr.live/deploy/121aa2a6534367c45352f428abe9a9674d57aef0786f95626f364608c1e97761


Sample Transfer Deploy: https://testnet.cspr.live/deploy/44b7463d90230d0f17ef62bff5b701f13a6820136d016e5d2c625c0923c1da77




## Overall Impression of usage testing

The project installs without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The reviewer was able to successfully run the e2e tests. The bash script provided in the README file was able to run the unit tests. The project has sufficient amount of tests.

[Full Test Logs](assets/test.txt)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Properly formatted inline comments on the critical classes and the methods are added to the project. The reviewer thinks that there is a sufficient amount of code documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The README file has sufficient basic usage instructions for the implemented methods. The reviewer was able to use the project using project documentation. Please note that there is one more milestone of this project that has an acceptance criteria as follows: 
- Full, Clear, Documentation Provided


Requirement | Finding
------------ | -------------
Usage Documented | PASS 
Example Documented | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, the project has sufficient documentation. 

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project has Contributing and Security Policies and a Code of Conduct.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project has well-structured and readable code. Code and project documentation is sufficient and they provide the necessary information to use the program. The project complies with open source standards.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. 

Thus, in the reviewer's opinion, this submission should PASS.

# Recommendation

Recommendation | PASS
------------ | -------------

