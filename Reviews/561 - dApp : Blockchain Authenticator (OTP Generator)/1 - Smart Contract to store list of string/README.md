Grant Proposal | [561 - dApp : Blockchain Authenticator (OTP Generator)](https://portal.devxdao.com/public-proposals/561)
------------ | -------------
Milestone | 1
Milestone Title | Smart Contract to store list of string
OP | mikael-g
Reviewers | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**


Smart contract to create/update the secret codes needed to generate the one-time password.
The data stored in the blockchain will be used by the webapp in Milestone#2 

The first implementation of the smart contract will be done on the Casper’s blockchain

**Acceptance criteria:**

Rust contract to store a list of CLString under the named key “blockchain-authenticator”.

There are 2 parameters :
* method (type : CLString) : add or del
* keys (type : CLList<CLString>) : list of CLString to store on the blockchain. The string must be formatted as follow : "[ID];[DATA]"

To call the contract, use "ModuleBytes"

When you call the “add” method, the keys are added (or updated) to the existing keys.
When you call the “del” method, the keys are removed from the existing keys. If you try to remove a non-existing key, nothing happen

The smartcontract will come with a set of tests that will :
- check the existence of the named key
- check a missing parameter
- add an element
- remove an element
- update an element
- remove a non-existing element

You'll also be able to see the information on cspr.live (eg : https://testnet.cspr.live/uref/uref-b4bfa9ba4952840e54e52f00c694d8b8a515567a828acc860e134267b4abc131-007)

Note : The data is encrypted by the webapp (Milestone#2), to test this contract you can store non-encrypted data.

**Additional notes regarding submission from OP:**

All informations are provided in the README of the repo

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/blockchain-authenticator-contract | 9462d0b

# Install & Usage Testing Procedure and Findings

Following the instructions in the [README](https://github.com/caspercommunityio/blockchain-authenticator-contract) of the project, reviewer was able to successfully build the source code and run the tests for this milestone on Ubuntu 20.04. The reviewer able to install dependencies by following the provided links but it would be better to have direct instructions on the README of the project instead of linking.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions. Build instructions are giving required information but can be enhanced and more clear by detailing each step. The project functionality meets/exceeds the acceptance criteria and operates without errors. The reviewer was able to run the example put deploy command successfully by following the instructions on the README.

[Build Logs](assets/makecontractlogs.md)

[Put Deploy Example Output](assets/exampledeploy.md)

[cspr.live link of the example deploy](https://testnet.cspr.live/deploy/c15a386c98adadad561f2a557e33346e746d3ab9a8348d914a611ef71117a2a7)


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total 9 tests, covering both positive and negative paths.

Although the implemented tests are already in very good state, they can be enchanted and more test can be added.

[Test Logs](assets/maketestlogs.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
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

The Project is released under the MIT License.

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

The project meets the milestone acceptance criteria. Install and usage instructions are sufficient. Tests run successfully.

Thus, in the reviewers' opinion, this submission should PASS.

# Recommendation

Recommendation | PASS
------------ | -------------
