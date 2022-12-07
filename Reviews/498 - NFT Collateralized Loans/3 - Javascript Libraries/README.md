Grant Proposal | [498 - NFT Collateralized Loans](https://portal.devxdao.com/public-proposals/498)
------------ | -------------
Milestone | 3
Milestone Title | Javascript Libraries
OP | CaptainBernardo
Reviewer | Zoltán Róbert Lovas <zoltan@casperlabs.io>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Deliverables
Javascript libraries that interface with the contracts
Automated testing for the contracts

We request half the value of this milestone in advance per #191, resolution regarding “MILESTONE PAYMENTS”.

**Acceptance criteria:**

A user will be able to call the contracts from node.js or a website.

CRDAO: Verification for this milestone will be a suite of unit tests for each endpoint.

**Additional notes regarding submission from OP:**

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-LiquidNFT | eb03989


# Install & Usage Testing Procedure and Findings

Installation and usage testing is well documented in the repository's README files. The flow of installation in step by step and mentions most probable error points.
[Compilation runs successfully](assets/js-install.md).

## Overall Impression of usage testing

Starting with [installation to casper-testnet](assets/npm-install-cmd.md) the testing is on point with ways to test functionality manually and automatically.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The testing framework is extensive.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Documentation in the codebase is present in a manner that is enough to read and understand codes function.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Each sub-project is well documented.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Every directory which corresponds to what is in essence its own subproject is well documented with step by step workflows and lists of possible error and the way of usage.

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

Code quality is good with each project part being well documented. Code compiles, tests pass, OpenSource standards are held.

# Final Conclusion

The project is in working order as to milestone and can be considered as a success.

# Recommendation

Recommendation | PASS
------------ | -------------
