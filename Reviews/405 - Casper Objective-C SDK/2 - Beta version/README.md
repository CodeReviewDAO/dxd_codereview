Grant Proposal | [405 - Casper Objective-C SDK](https://portal.devxdao.com/public-proposals/405)
------------ | -------------
Milestone | 2
Milestone Title | Beta version
OP | Huy Tran
Reviewer | Yusuf Keten

# Milestone Details
The review will cover the 2nd milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The following RPC methods will be fully implemented in the Objective-C SDK:

     info_get_deploy 
     info_get_status 
     chain_get_block_transfers 
     chain_get_block
     chain_get_era_info_by_switch_block    
     state_get_item
     state_get_dictionary_item
     state_get_balance
     state_get_auction_info

These methods will return JSON arrays.

- Unit tests full coverage
- Full documentation of the SDK

**Acceptance criteria:**

Following methods of the SDK project fully implemented and will return when called: 
      
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
- Documentation are available for all critical classes and methods.

**Additional notes regarding submission from OP:**
Following methods of the SDK project fully implemented and will return when called: 
      
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
- Documentation are available for all critical classes and methods.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/tqhuy2018/Casper-ObjectiveC-sdk | [59b48a5](https://github.com/tqhuy2018/Casper-ObjectiveC-sdk/commit/59b48a5ed59dc54cb697eabbe01a2944c0d982e3)


# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of repository(https://github.com/tqhuy2018/Casper-ObjectiveC-sdk), the reviewer was able to successfully build the source code on a macOS Monterey 12.3 Mac using Xcode version 13.3.

[Build Logs](assets/build-run.md)

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has unit tests for all critical classes and methods. However, their coverage is not sufficient. Some of the unit tests are not comparing the expected result with the actual result. However, this is not blocking the milestone submission as the project is not in the final state. The OP is strongly encouraged to add more detail to the unit tests for the next milestone.

[Test Logs](assets/test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has a detailed documentation for usage with examples, along with the installation, build and test instructions.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation
In the reviewer's opinion, the project usage and code-level documentation are sufficient.

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

Code is generally well-structured and very readable. The project as committed to GitHub and both the unit tests and the manual tests pass. However, the unit tests should be improved to cover more cases. The reviewer recommends adding more units tests and extending the existing ones.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are certain points noted above that could be improved on the project. 

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with notes
------------ | -------------