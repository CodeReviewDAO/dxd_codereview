Grant Proposal | [29 - Casper PHP SDK](https://portal.devxdao.com/public-proposals/29)
------------ | -------------
Milestone | 1
Milestone Title | Alpha Version
OP | Michael Steuer <michael@make.software>
Reviewer | David Tai <dtaipublic@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Scaffolding of PHP-SDK project, public on GitHub, loadable via Composer, and able to connect to a Casper Node and execute and return response for at least 1 method

**Acceptance criteria:**

- PHP-SDK project is available on public GitHub repository
- Can successfully be integrated into a project using Composer
- When instantiated, can connect to a Casper node
- When connected, it can make at least 1 method call and return a response

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-php-sdk | e1939ab

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-php-sdk, reviewer was
able to successfully build the source code for this milestone

## Overall Impression of usage testing

Currently there's only a very basic alpha version so there's not much to manually test other than writing a script to try and connect to a node.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Can connect to a Casper node | PASS

# Unit / Automated Testing

Unit tests will be included in milestone 3

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A

# Documentation

### Code Documentation

Code documentation is sparse, will be done in milestone 3

Requirement | Finding
------------ | -------------
Code Documented | Minimal

### Project Documentation

README.md has sufficient examples to construct your own testing script.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the Apache License

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

Recommendation | PASS (request for improvements)
------------ | -------------