
Grant Proposal | [267 - Casper .NET C# SDK](https://portal.devxdao.com/public-proposals/267)
------------ | -------------
Milestone | 3
Milestone Title | Final Version
OP | Michael Steuer | <michael@make.software>
Reviewer | Hatice Kaya <haticekaya@protonmail.com>

# Milestone Details
This is the third milestone of grant. 
The review will cover the third milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

In addition to Alpha and Beta requirements, the project is complete, all unit tests pass, all methods have detailed Documentation and the project is available as a package via NuGet

**Acceptance criteria:**

- the C# SDK is feature complete, including the alpha and beta milestones, and discretionary convenience methods and types 
- all unit tests pass 
- all methods have detailed Documentation 
- the C# SDK is available as a package via NuGet

**Additional notes regarding submission from OP:**

All final acceptance criteria have been met.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-net-sdk | f2227ad

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-net-sdk, reviewer was able to successfully build the source code for this milestone, and test is successfully passed.

[267_3_Build.md](assets/267_3_Build.md)

## Overall Impression of usage testing

By following the provided instructions on the repository, the reviewer was able to install the SDK and successfully run the test.


Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS 

# Unit / Automated Testing

Project contains 155 unit tests that can be executed from the console. 
The reviewer has observed that all tests run successfully without errors. 

Test Results can be found in the folder next to this review: [267_3_TestResults.md](assets/267_3_TestResults.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS 
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation

The reviewer has observed that the project has immense code-level documentation with properly formatted summaries and comments on the critical classes and methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project Documentation was great for usage. It was also observed that there are multiple example tutorials with step by step explanations.

Requirement | Finding
------------ | -------------
  Usage Documented | PASS
  Example Documented | PASS


## Overall Conclusion on Documentation

Well organized and comprehensive.

# Open Source Practices

## Licenses

The Project is released under the Apache License 2.0.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution and a security policy.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS


# Coding Standards

## General Observations

Code is generally well-structured and readable. 
The project has been committed to GitHub and both 155 unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS
------------ | -------------
