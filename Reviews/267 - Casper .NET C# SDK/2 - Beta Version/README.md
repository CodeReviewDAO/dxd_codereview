Grant Proposal | [267 - Casper .NET C# SDK](https://portal.devxdao.com/public-proposals/267)
------------ | -------------
Milestone | 2
Milestone Title | Beta Version
OP | Michael Steuer <michael@make.software>
Reviewer | Hatice Kaya <haticekaya@protonmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

In addition to Alpha requirements, the project now implements all available RPC methods, all available Casper types

**Acceptance criteria:**

- all RPC methods can be called and return an appropriate response
- all Casper Types are available in the C# SDK

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-net-sdk | f2227ad

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-net-sdk, reviewer was
able to successfully build the source code for this milestone, and RPC queries using the provided SDK.

## Overall Impression of usage testing

By following the provided instructions on the repository, the reviewer was able to install the SDK, run basic queries and get proper responses.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Can make some basic RPC calls | PASS

# Unit / Automated Testing

The project has 155 tests in total, with positive, negative, and additional paths. The reviewer has observed that all tests pass when run by using the command given on the README.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that the project has extensive code-level documentation with properly formatted summaries and comments on the critical classes and methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has extensive documentation for usage. It was also observed that there are multiple example tutorials with step by step explanations.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS
------------ | -------------

