Grant Proposal | [507 - Odra - Casper Smart Contracts Framework](https://portal.devxdao.com/public-proposals/507)
------------ | -------------
Milestone | 2
Milestone Title | MVP Part 2
OP | Maciej Zieliński
Reviewer | Zoltán Róbert Lovas <zoltan@casperlabs.io>, Karan Dhareshwar (karan@casperlabs.io)

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The goal of this milestone is to develop:
- MockVM to provide debugging features (with breakpoints) and unit-tests not just for whole contracts, but also particular parts and modules.
- a complete example of ERC20 implementation.

**Acceptance criteria:**

version is 0.1.0 released to the http://crates.io, - it is possible to write simple smart contracts and test them using CasperVM.

**Additional notes regarding submission from OP:**

- We have also provided a console tool called Cargo Odra, that simplifies development process.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/odradev/odra | 3905380


# Install & Usage Testing Procedure and Findings

To install/use the project the suggested method is getting `cargo-odra`.
[Cargo-odra cannot be installed from cargo](assets/cargo-odra-install.md).
Multiple reviewers failed the installation of `cargo-odra` from cargo, and so tried to install from source which is possible. Even after getting the installation of `cargo-odra` to a success, none of the reviewers managed to get actually get a WASM build out of the system, which is an important and promoted functionality. 

The odra-cargo Makefile test (test-project-generation) is written for apt, which is not on the reviewers linux distribution. Following said commands instructions (which are also the ones described in the cargo-odra repository as the intended use) results in a failure at `cargo odra test -b casper-latest`.
[cargo odra casper backend failure](assets/cargo-odra-casper-backend-build.md).

## Overall Impression of usage testing

Currently `cargo-odra` is not in working state. Installation is problematic, and usage fails. The system cannot compile a WASM and hence cannot test against CasperVM (which is the imported execution engine from Casper). This is a failure of milestone acceptance criteria.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

The provided repositories each contain multiple unit tests, each of them compile and end with the expected results.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The documentation in the codebase is minimal in some parts of the codes, while completely missing in other parts. A consideration is that to oversee the whole project the reviewer needs to look at multiple repositories each with different degrees of documentation, but all of them being inadequate for optimal use.
It needs to be stated that documentation is supposedly a part of a later milestone (#3). 

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

The usage of the project is only detailed in a few commands and lines that are not enough as it is to produce a viable prodct. The most prominent  or useful part of this is a .gif embedded into the README.md of the repository that demonstrates the intended usage of `cargo-odra`.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

The documentation is not enough to use the project in any viable capacity. The developer intends to create the documentation in a later milestone (#3). 

# Open Source Practices

## Licenses

The repository contains an MIT license as stated in the original proposal.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

No contributing, security policy, or code of conduct was found. 
Issues and Pull requests are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

# Coding Standards

## General Observations

The proposals milestone 2 acceptance criteria is as follows:
- version is 0.2.0 released to the http://crates.io,
- Rust debugger can be used to debug smart contracts and tests,
- standard library is initialized with the ERC20 contract and can be used to develop custom tokens.

But the review job criteria and milestone #2 goal are:
- version is 0.1.0 released to the http://crates.io, - it is possible to write simple smart contracts and test them using CasperVM.
- It is possible to develop and debug smart contract against the fast mock virtual machine.
- ERC20 contract is available as an example and can be used as a starting point for the development.

The project is found in multiple different repositories making it easier to get lost.
cargo-odra is a part of the project which is a cargo tool. This tool was not stated in the original proposal. 

# Final Conclusion

Based on problematic installation, failing tool, inability to test against the intended use case, and failed milestone the reviwer recommends the current state of the project to fail this review.

# Recommendation

Recommendation | FAIL
------------ | -------------
