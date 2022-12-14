Grant Proposal | [705 - Casper .NET Client Libraries & Web Library](https://portal.devxdao.com/public-proposals/705)
------------ | -------------
Milestone | 1-4
Milestone Title | Client Library for CEP-47 (Deprecated)
OP | Michael Steuer | MAKE
Reviewer | Muhammed Didin <mdidin80@gmail.com>


# Milestone Details

The review will cover all the milestones' criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

A library that can be imported into .NET projects that deploys contracts in ERC-20 and CEP-47 formats.


**Acceptance criteria:**

Library can be included in a project and provide interfaces to all standard functions of CEP-47 non-fungible token contracts

**Additional notes regarding submission from OP:**

This library is an extension of the Casper .NET SDK that provides easy to use client classes for the Casper ERC20 and CEP47 smart contracts.
Usage is explained in the Docs/Examples directory of the repo. The library is available via nuget here: https://www.nuget.org/packages/Casper.Network.SDK.Clients/1.1.0

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-net-sdk-clients| 689f3bb


# Install & Usage Testing Procedure and Findings
It is stated in the README that .NET 5.0 or higher must be installed to use this library. The reviewer used this library on a macOS Monterey device with .NET 7.0.100 installed.

This library is published as a nuget package in [nuget](nuget.org). Following the instructions in the README, the reviewer query `dotnet add package Casper.Network.SDK.Clients` command to add a reference to the Clients library in the project via `dotnet cli tool`. The reviewer used the example scripts placed under `Docs/Examples` folder by the development team to ensure the project meets to the acceptance criteria. 


## Overall Impression of usage testing

Documentation provides sufficient installation instructions. The reviewer easily set up the environment to build the project using these.

The project ran as intended and posted the specific information mentioned in the acceptance criteria. These were observed:

- [The result of installing CEP-47 example](assets/install_cep47.txt)

Install CEP-47 example deploy: https://testnet.cspr.live/contract-package/7372b0514253b0f662a5fd98dc1da9022c65ebd5babfdd20fc9b380b1b88f67a


- [The result of installing ERC-20 example](assets/install_erc20.txt)

Install ERC-20 example deploy: https://testnet.cspr.live/contract/f684c8ba46073eaa063213290eae726e4c78e5c041f86d84145db3943dad9787

- [The result of calling CEP-47 example](assets/call_cep47.txt)

Call CEP-47 example deploy: https://testnet.cspr.live/deploy/101a0df1ddb76c90f268a269e0bffc12200a09c6f0e310ebab66a5163f4cf341

- [The result of calling ERC-20 example](assets/call_erc20.txt)

Call ERC-20 example deploy: https://testnet.cspr.live/deploy/be15b6699d50fd2dd49e686b519ab88d5fc12c5a29d362fc68b0a00355aff7b4


The project meets the acceptance criteria for these milestones.


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has 53 automated tests and all tests PASS for this milestone running on ubuntu machine by the [GitHub Actions](https://github.com/make-software/casper-net-sdk-clients/actions/runs/3574518972/jobs/6009882965). Automated tests cover critical functionality.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code is now overall well documented, and almost all classes and critical functions have acceptable code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project documentation is sufficient to  The reviewer was able to complete the necessary operations following the information provided by the documentation.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation is sufficient for this milestone.


# Open Source Practices

## Licenses

The Project is released under the Apache 2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project has CONTRIBUTING and SECURITY policies that link to a Code of Conduct. Also, Pull Requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

The source code is well-written and documented. General best coding practices are used throughout the project. The project is committed to GitHub and both the unit tests and the manual tests are passed.


# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. Also, the code is well-documented and open to public participation. 


# Recommendation

Recommendation | PASS
------------ | -------------
