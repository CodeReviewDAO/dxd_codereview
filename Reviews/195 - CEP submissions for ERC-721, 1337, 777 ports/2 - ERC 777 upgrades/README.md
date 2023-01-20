Grant Proposal | [195 - 1.4 Upgrades and CEP submissions for ERC-721, 1337, and 777 ports](https://portal.devxdao.com/public-proposals/195)
------------ | -------------
Milestone | 2
Milestone Title | ERC 777 Upgrades
OP | David Tai
Reviewer | Zoltán Róbert Lovas <zoltan@casperlabs.io>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Wholesale replacement of deprecated ERC-20 with new 1.3 ERC-20 version now in pull request & review ( will have to wait until work on this is complete from casper's side, may take a few weeks)
- Figure out whether or not we are supporting ERC-1820 standard or using simple callbacks
- Work with Maciej to use the new ERC-20 crate (WIP) instead of copying all the ERC-20 code into the repo
- Events added
- Create a JS client
- Relevant Testing & Docs
- Release Crate
- Tests for Casper's internal backwards compatibility system (when defined)

**Acceptance criteria:**

ERC 777 is sufficiently similar enough to ERC-20 repos that technical reviewers sign off

**Additional notes regarding submission from OP:**

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-ERC777 | 054e6da


# Install & Usage Testing Procedure and Findings

Following the documentation installing and testing the project is easy and quick.

## Overall Impression of usage testing

Usage is in line with the expected quality and flow.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

There is an adaquate amount of tests that [run to completion with success.](assets/tests.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The codebase has enough documentation to help understand it.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project is extensively documented. Examples for intented usage are available.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation of the project(s) should be enough for most users to be able to assess, compile, deploy, and use the project.

# Open Source Practices

## Licenses

The repository contains an Apache-2.0 license.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Contributing, security policy, or code of conduct related documents are present. 
Issues and Pull requests are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Project holds up to the expected standards and has enough documentation and tutorials to be usable.

# Final Conclusion

The milestone is complete as per the acceptance criteria as it is sufficiently similar to the structure of ERC20, and passes all the general criterias (documentation, tests, etc.) as well. 

# Recommendation

Recommendation | PASS
------------ | -------------
