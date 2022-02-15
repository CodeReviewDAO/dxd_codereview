
Grant Proposal | [338 - Casper Swift SDK](https://portal.devxdao.com/public-proposals/338)
------------ | -------------
Milestone | 2
Milestone Title | Beta version
OP | Huy Tran
Reviewer | Muhammet Kara

# Milestone Details
This is the second milestone of grant. 
The review will cover the second milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The following RPC methods will be fully implemented in the Swift SDK:
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
- Documentation are available for all critical classes and methods.

**Additional notes regarding submission from OP:**

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/hienbui9999/CasperSDKInSwift | 4d65207

# Install & Usage Testing Procedure and Findings

The reviewer observed that, following the instructions in the README of https://github.com/hienbui9999/CasperSDKInSwift, it was possible to successfully install the library, and run queries against a node on the Casper Network. The reviewer also observed that it was possible to [successfully build the source code](assets/build.md) for this milestone by using the commands given on the README of the repository.

## Overall Impression of usage testing

It was observed that the project builds without errors, documentation provides sufficient installation/execution instructions, project functionality meets/exceeds acceptance criteria and operates without error, and it is possible to query the network by using the SDK.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Project contains 130 tests that can be executed from the console, covering both the positive and the negative paths, and the reviewer has observed that [all tests run successfully](assets/test.md) without errors. **The reviewer praises the OP for taking the notes from the review of the previous milestone seriously, and improving the test coverage of the project significantly since then.**

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code documentation was acceptable for this stage of the project, however it is recommended to improve the code-level documentation by covering all critical functions with standard comments which allow auto-generation of documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Project Documentation was observed to be extensive with sufficient usage documentation and examples.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient. **However the code-level documentation has room for improvement although it is acceptable for this non-final milestone, which was also noted in the previous review, but observed to be not acted on yet.**

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution and a security policy. However, **it was observed that the OP didn't act on the notes from this section of the previous review, and the repository still lacks relevant tags, hindering its discoverability.**

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub and all unit tests pass.

# Final Conclusion

The project meets/exceeds the functional requirements, and is generally in a very good shape in terms of open-source guidelines. However, **the code-level documentation is suggested to be improved. Adding relevant tags to the code repository is also highly recommended.**

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------

