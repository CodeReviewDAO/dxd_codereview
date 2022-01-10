Grant Proposal | [295 - Casper Scala SDK](https://portal.devxdao.com/public-proposals/295)
------------ | -------------
Milestone | 2
Milestone Title | Fully implemented and tested Scala SDK
OP | Mustapha Chad ABAHMANE <elmabahma@gmail.com>
Reviewer | Muhammet Kara <muhammetk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

-  RPC methods Fully implemented in the Scala SDK  and available on a public GitHub repository.
    
   RPC methods to be implemented:
 
     info_get_deploy 
     info_get_status 
     chain_get_block_transfers 
     chain_get_block
     chain_get_era_info_by_switch_block    
     state_get_item
     state_get_dictionary_item
     state_get_balance
     state_get_auction_info


- Unit tests full coverage
- Full documentation of the SDK

**Acceptance criteria:**

- Following methods of  the SDK project fully implemented and will return when called: 
      
     info_get_deploy 
     info_get_status 
     chain_get_block_transfers 
     chain_get_block
     chain_get_era_info_by_switch_block    
     state_get_item
     state_get_dictionary_item
     state_get_balance
     state_get_auction_info

- Unit test full coverage

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/casper-scala-sdk | c465841

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/caspercommunityio/casper-scala-sdk, reviewer was able to successfully build the source code and run the tests for this milestone on Ubuntu 20.04. The reviewer was also able to install the published maven package of the project (`io.caspercommunity:casperscala-sdk_3:1.0.1`) as a dependency on a newly created project, and run queries against a node on the Casper Network and get valid responses.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, the project functionality meets/exceeds the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total number of 128 tests, covering both positive and negative paths. The tests are configured to run automatically by means of automated actions on the repository. Although there are some tests still existing just as a stub, and marked as TODO, the implemented tests are already in very good state, in the reviewer's opinion. The reviewer praises the OP for the extensive coverage of the tests on the project.

[Tests Run](test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that the critical functions of the code-base has an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation. It was also observed that the project has an already generated copy of this documentation on the repository, and the command to regenerate the documentation is provided on the README.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Reviewer has observed that the project has detailed documentation for usage with examples, along with the installation, build and test instructions.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

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

Reviewer finds the code to be generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. The SDK is well-documented and has extensive automated tests. However, **no description, website, or topics provided for the repository**, which cripples the discoverability of the project. Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
