
Grant Proposal | [338 - Casper Swift C# SDK](https://portal.devxdao.com/public-proposals/338)
------------ | -------------
Milestone | 1
Milestone Title | Connecting to a Casper node
OP | Huy Tran
Reviewer | Muhammet Kara

# Milestone Details
This is the first milestone of grant. 
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- First version of Swift SDK: Swift SDK project available on a public GitHub repository
- Following methods of the API fully implemented and will return when called by the SDK:
   * chain_get_state_root_hash
   *  info_get_peers  
- Unit tests

**Acceptance criteria:**

- Swift SDK project available on a public GitHub repository
- Following methods of the API fully implemented and will return when called:
   * chain_get_state_root_hash
   *  info_get_peers  
- Unit tests

**Additional notes regarding submission from OP:**

There will be some warnings when build the project, in the code belonging to milestone2, in which many of them are warnings of declaring variables but not put used, just because I create the variables and intend to use them later when I handle the method in detail.

In the previous version I used latest Swift library to handle asynchronous handling the POST request for sending method (info_get_state_root_hash or info_get_peers). But the latest Swift library required the MacOS version 12.0, which is quite new, and in Github the version for MacOS is just 11.6 then the test fails.

I have just adjusted the code, changed the Swift library and way to handle the asynchronous call to support earlier versions for Mac devices (from MacOs10.14.4, iOS from 10.0,watchOS 5.3 ,tvOS 12.3) and now all devices can run the code without error.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/hienbui9999/CasperSDKInSwift | 1779dac

# Install & Usage Testing Procedure and Findings

The reviewer observed that, following the instructions in the README of https://github.com/hienbui9999/CasperSDKInSwift, it was possible to successfully install the library, and run queries against a node on the Casper Network. The reviewer also observed that it was possible to [successfully build the source code](assets/build.md) for this milestone by using the commands given on the README of the repository.

## Overall Impression of usage testing

It was observed that the project builds without errors, documentation provides sufficient installation/execution instructions, project functionality meets/exceeds acceptance criteria and operates without error, and it is possible to query the network by using the SDK.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Can connect to a Casper node | PASS

# Unit / Automated Testing

Project contains 74 tests that can be executed from the console, and the reviewer has observed that [all tests run successfully](assets/test.md) without errors. However, it was also observed that the tests heavily focus on the positive paths, so the OP must improve the test coverage to remedy this situation before the final milestone.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code documentation was acceptable for this stage of the project, however it is recommended to improve the code-level documentation by covering all critical functions with standard comments which allow auto-generation of documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Project Documentation was acceptable for this stage of the project, with examples on the README.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient. However the code-level documentation has room for improvement although it is acceptable for this early milestone.

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution and a security policy. However, the repository lacks relevant tags, hindering its discoverability.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub and all unit tests pass.

# Final Conclusion

The project meets/exceeds the functional requirements, and is generally in a very good shape in terms of open-source guidelines. However, the test coverage needs to be extended to include more negative paths tests, and the code-level documentation is suggested to be improved.

Thus, in the reviewers opinion, this submission should pass with notes.


# Recommendation

Recommendation | PASS with Notes
------------ | -------------
