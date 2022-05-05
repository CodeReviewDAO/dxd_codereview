Grant Proposal | [469 - Casper Kotlin SDK](https://portal.devxdao.com/public-proposals/469)
------------ | -------------
Milestone | 1
Milestone Title | Beta version
OP | Huy Tran
Reviewer | Yusuf Keten

# Milestone Details
The review will cover the 1st milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- First version of Kotlin SDK: Kotlin SDK project available on a public GitHub repository

- Following methods fully implemented and will return when called by the SDK:
   * chain_get_state_root_hash
   *  info_get_peers  
   *  info_get_deploy 
   *  info_get_status 
   *  chain_get_block_transfers 
   *  chain_get_block
   *  chain_get_era_info_by_switch_block    
   *  state_get_item
   *  state_get_dictionary_item
   *  state_get_balance
   *  state_get_auction_info

- Unit tests full coverage

- Full documentation of the SDK

**Acceptance criteria:**

- Kotlin SDK project available on a public GitHub repository

- Following methods fully implemented:
   * chain_get_state_root_hash
   *  info_get_peers  
   *  info_get_deploy 
   *  info_get_status 
   *  chain_get_block_transfers 
   *  chain_get_block
   *  chain_get_era_info_by_switch_block    
   *  state_get_item
   *  state_get_dictionary_item
   *  state_get_balance
   *  state_get_auction_info

- Unit test full coverage

- Documentation are available for all critical classes and methods.

**Additional notes regarding submission from OP:**

- Kotlin SDK project available on a public GitHub repository

- Following methods fully implemented:
   * chain_get_state_root_hash
   *  info_get_peers  
   *  info_get_deploy 
   *  info_get_status 
   *  chain_get_block_transfers 
   *  chain_get_block
   *  chain_get_era_info_by_switch_block    
   *  state_get_item
   *  state_get_dictionary_item
   *  state_get_balance
   *  state_get_auction_info

- Unit test full coverage

- Documentation are available for all critical classes and methods.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/tqhuy2018/Casper-Kotlin-sdk | 3d83454

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/tqhuy2018/Casper-Kotlin-sdk, the reviewer was
able to successfully build the source code for this milestone.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

``` sh
Downloaded from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.1/commons-lang-2.1.jar (208 kB at 490 kB/s)
[INFO] Building jar: /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/target/consoleApp-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:29 min
[INFO] Finished at: 2022-05-04T16:14:19+03:00
[INFO] ------------------------------------------------------------------------
```

[Build Logs - mvn clean package](assets/mvn-clean-package.md)

[Build Logs - mvn package](assets/mvn-package.md)

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has unit tests for all critical classes and methods.

[Test Logs - mvn test](assets/mvn-test.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods. However, the OP is highly encouraged to improve the code documentation such as adding more detail to the documentation of the classes and methods.

Requirement | Finding
------------ | -------------
Low level function documentation | PASS with Notes

### Project Documentation

The README file is so readable and clear that it is a must-have for the project. It contains all the necessary information for the project build and execution. However, usage documentation is insufficient. This is not a reason for a failure, in the reviewer's opinion, at this non-final milestone. The reviewer recommends that the OP improve the usage documentation before the final milestone.

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS with Notes

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. The project also has CONTRIBUTING and SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project is committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are certain points noted above that could be improved on the project. 

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
