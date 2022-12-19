Grant Proposal | [499 - Solana Endpoint for Boosty Labs Bridge](https://portal.devxdao.com/public-proposals/499)
------------ | -------------
Milestone | 1
Milestone Title | Solana Contracts for Bridge & Integration Testing - Submission 1
OP | RengoLabs
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Deliverables:
Clone the Ethereum Contract to Solana.
Integrate Boosty’s oracle/validator system.

We request half the value of this milestone in advance per #191, resolution relating to “MILESTONE PAYMENTS”.

**Acceptance criteria:**

Users can send bridge tokens through Boosty’s Ethereum and Casper contracts.  These contracts will be deployed to solana testnet and mainnet with the rest of the Boosty Bridge hits those phases but that is out of scope for this grant.

CRDAO will be evaluating the solana contracts and test suite for the contracts only.  Integration tests will be bundled with Boosty's original grant.

**Additional notes regarding submission from OP:**

Per completion criteria

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-Solana-bridge | cf2f3c5


# Install & Usage Testing Procedure and Findings

Setup is simple and very easy with the instruction provided in the README.

- [Installation logs](assets/installation.md)

## Overall Impression of usage testing

Since these are smart contracts, usage testing is done with unit tests.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

All automated unit tests PASS for this milestone. Tests cover critical functionality. Reviewer successfully ran all automated tests on an Ubuntu 20.04.4 LTS machine. Overall quality of tests are sufficient. Test output is below.

- [Test logs](assets/test.md)


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code is well documented. Critical functionality is properly explained and lots of additional comments exist.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project documentation is sufficient and useful. Reviewer was able to complete necessary operations following the information provided by the documentation.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation is sufficient for this milestone.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING and SECURITY policies, and the optional CODE OF CONDUCT policy. Pull requests and Issues are enabled on the repository and the project is set up for public participation.


Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project. Overall sufficient work is done.

# Final Conclusion

Project provides the acceptance criteria for the milestone it covers. Unit tests are well prepared and useful for helping understand how different usage scenarios can be executed. Documentation is sufficient. Code documentation is also good but with coming milestones, any newer additions are welcomed and would be beneficial. Coding practices used in the project are of good quality. Because of its sufficient deliverables, reviewer suggests the project to PASS.

# Recommendation

Recommendation | PASS
------------ | -------------
