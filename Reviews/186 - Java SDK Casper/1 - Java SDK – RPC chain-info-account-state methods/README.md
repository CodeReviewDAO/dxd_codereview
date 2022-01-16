Grant Proposal | [186 - Java SDK Casper](https://portal.devxdao.com/public-proposals/186)
------------ | -------------
Milestone | 1
Milestone Title | Java SDK – RPC chain/info/account/state methods
OP | ReDC
Reviewer | Muhammet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Source code in our own public Gitbhub repository;
- Unit-tests;
- Documentation.

**Acceptance criteria:**

- Setup a concurrent connection with many RPC nodes
- Implement the encoding/decoding schemes to translate from/to JSON and Java objects
- Implement the chain/info/account/state methods as per casper-node 1.3 specs
  - chain_get_block
  - chain_get_block_transfers
  - chain_get_state_root_hash
  - chain_get_era_info_by_switch_block
  - info_get_deploy
  - info_get_peers
  - info_get_status
  - account_put_deploy
  - state_get_item
  - state_get_balance
  - state_get_auction_info
  - state_get_account_info
  - state_get_dictionary_info

**Additional notes regarding submission from OP:**

Please find the Java code togehter with the unit tests and the documentation for the Java Casper SDK in our github repository: https://github.com/syntifi/casper-sdk

Note that this SDK follows the 1.3 node specification. The package has been published in the Github maven repository and can be added in another project following the instructions in the README file.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/syntifi/casper-sdk | dae8bd0

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/syntifi/casper-sdk, reviewer was able to [successfully build the source code and run the tests](build-and-test.md) for this milestone on Ubuntu 20.04 in a cloud environment. Because there was no published maven package on the central repository, the reviewer installed the library by using the locally built artifact, and manually resolving the missing dependencies, on a newly created project. Then the reviewer was ale to run queries against a node on the Casper Network and get valid responses.

## Overall Impression of usage testing

The project builds without errors, and the project functionality meets/exceeds the acceptance criteria and operates without errors. However, the reviewer thinks that the documentation still has room for improvement regarding the installation and execution instructions for example by fixing small method call mismatches on the given examples and by providing the central maven repository information for the library.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total number of 87 tests, covering both positive and negative paths. The tests are configured to run automatically by means of automated actions on the repository. However, the reviewer thinks that the tests are heavily focused on the positive paths, thus highly suggests increasing the number of the negative path tests

[Tests Run](test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that the critical functions of the code-base has an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Reviewer has observed that the project has detailed documentation for usage with examples, along with the installation, build and test instructions. However, the reviewer finds the installation through custom package repository less than ideal, and thus highly suggests publishing a package on the central maven repository and updating the instructions accordingly.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License. However, the promised license on the grant proposal is MIT, so proper action must be taken by the OP to correct this mismatch before the final milestone.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

## Contribution Policies

Pull requests and Issues are enabled on the repository, and the project contains CONTRIBUTING guidelines, but lacks a SECURITY policy. Because this is an SDK project which is meant to be used by many other projects, its security is especially important. Thus, the reviewer recommends preparing and publishing a proper SECURITY policy on the repository as soon as possible.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

Reviewer finds the code to be generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. The SDK is well-documented and has an acceptable level of tests.

However, **no description, website, or topics provided for the repository**, which cripples the discoverability of the project. Moreover, although it is qn OSI-approved license, the project's license mismatches the one promised on the proposal, which needs to be fixed before the final milestone.

The project also lacks a security policy, and is observed to be heavily focused on the positive paths in its unit tests. Furthermore, it is not published on the central package repository of the language, making it harder to install and use.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------

