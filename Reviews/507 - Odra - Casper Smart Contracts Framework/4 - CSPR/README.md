Grant Proposal | [507 - Odra - Casper Smart Contracts Framework](https://portal.devxdao.com/public-proposals/507)
------------ | -------------
Milestone | 4
Milestone Title | CSPR
OP | Maciej Zieliński
Reviewers | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**


Milestone #4 is all about supporting CSPR transfers. We will develop the Wrapped CSPR Contract and modules for handling CSPR transfers ready to be used via the standard library.

**Acceptance criteria:**

- next version of odra is released to the http://crates.io.
- developers have a clear way of handling CSPR transfers and holding CSPR in smart contract.
- Wrapped CSPR is included into the standard library.

**Additional notes regarding submission from OP:**

This milesone is implemented and released as Odra `0.2.0`.

Since the last submission we introduced series of changes:

- One of the response we got from reviewers of the previous milestones (and other developers) was "large complexity due to large amount of repositories". We have addressed that and rearranged code. Now it's just 2 repositories: https://github.com/odradev/odra and https://github.com/odradev/cargo-odra

- We optimized build times.

- CSPR handling functions are now available. Entry point can be marked as "payable" now and accept CSPR tokens. As an example we implemented Time Lock Wallet: https://github.com/odradev/odra/blob/0.2.0/examples/src/tlw.rs. To see Wrapped CSPR with ERC20 interface is also implemented, see: https://github.com/odradev/odra/blob/0.2.0/modules/src/wrapped_native.rs.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/odradev/odra | aa6351c

# Install & Usage Testing Procedure and Findings

Following the instructions in the [README](https://github.com/odradev/odra) of the project, reviewer was able to successfully install the project along with it's dependencies, and run the tests for this milestone on Ubuntu 20.04. There are a lot of links to other repositories and sites, but it can be better to have more explanation about them in the README of the project instead of just linking to other repositories. Also, adding a requirement.txt and using it to install prerequisities might be useful too.

[Build Logs](assets/cargoodralogs.md)

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions. Build instructions are giving required information but can be enhanced and more clear by detailing each step. Same as installation instrutctions this part also needs improvements in the reviewer's opinion . The project functionality meets/exceeds the acceptance criteria and operates without errors.

[Example Build Logs](assets/examplebuildlogs.md)

[Example Test Logs](assets/exampletestlogs.md)

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has sufficient amount of tests, covering both positive and negative paths. All tests run successfully.

[Test Logs](assets/justtestlogs.md)
[Actions](https://github.com/odradev/odra/actions/runs/3533097352/jobs/5928283489)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The critical functions of the project have an acceptable level of code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has sufficient documentation coverage for usage with examples, along with the installation, build and test instructions. The README of the project links to other sites or repos for the instructions, but it is better to have more instructions and explanations in the README of the project instead of just linking. 

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

In the reviewer's opinion, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository, and the project contains a CONTRIBUTING and a SECURITY policy. CODE OF CONDUCT can be added.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project published publicly on GitHub. Project documentation is sufficient enough as general. Unit test coverage is good enough but can be improved, and all test run successfully.

Corresponding version of odra released to the http://crates.io.

Cspr transfer is implementd

# Final Conclusion

The project meets the milestone acceptance criteria. Install and usage instructions are sufficient but they are a bit confusing as they have a lot of linking to other repositories and sites. Tests run successfully.

Thus, in the reviewers' opinion, this submission should PASS with Notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
