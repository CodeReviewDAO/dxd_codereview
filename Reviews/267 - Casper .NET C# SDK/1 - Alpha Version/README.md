
Grant Proposal | [267 - Casper .NET C# SDK](https://portal.devxdao.com/public-proposals/267)
------------ | -------------
Milestone | 1
Milestone Title | Alpha Version
OP | Michael Steuer | MAKE
Reviewer | Robert Carbone <codereview@robertcarbone.com>

# Milestone Details
This is the first milestone of grant. 
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Scaffolding of C# SDK project, public on GitHub, 
and able to connect to a Casper Node and execute and return response for at least 1 method

**Acceptance criteria:**

- C# SDK project is available on public GitHub repository
- When instantiated, can connect to a Casper node
- When connected, it can make at least 1 method call and return a response

**Additional notes regarding submission from OP:**


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-net-sdk | 39cd6a3

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-net-sdk, the reviewer was able to successfully install the library. The reviewer was also able to successfully build the source code for this milestone by using the build script furnished in the root and readme of the repository. 

## Overall Impression of usage testing

The code was very well laid out and pretty printed for easy reading. Things were aligned nicely and it was easy to understand what was happening in the libraries as everything was also named very appropriately. In this milestone usage testing is not part of the requirement. 
Still things look to be on a promising track for future milestones where this criteria is more mission critical. 

Requirement | Finding
------------ | -------------

                           C# SDK project is available on public GitHub repository | PASS
                                   When instantiated, can connect to a Casper node | PASS
          When connected, it can make at least 1 method call and return a response | PASS
                                                     Project builds without errors | PASS
             Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
                                                      Can connect to a Casper node | PASS

# Unit / Automated Testing

Project contains 41 unit tests that can be executed from the console. 
The reviewer has observed that all tests run successfully without errors. 

Test Results can be found in the folder next to this review: 267_1_TestResults.txt

Requirement | Finding
------------ | -------------
Unit Tests - Sufficient | PASS

# Documentation

### Code Documentation

Code Documentation was acceptable for this stage of the project. 

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project Documentation was acceptable for this stage of the project. 

Requirement | Finding
------------ | -------------
  Usage Documented | PASS


## Overall Conclusion on Documentation

Very well Done. 

# Open Source Practices

## Licenses

The Project is correctly released under the Apache License 2.0

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Sufficient for the current state of the project. 

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is fantastically well-structured and readable. 
The project has been committed to GitHub and all 41 unit tests pass. 

# Final Conclusion

The project meets and exceeds our standards and exceeds the functionality required to m
eet the milestone acceptance criteria in the grant application.
Resounding PASS.

# Recommendation

Recommendation | PASS
------------ | -------------



