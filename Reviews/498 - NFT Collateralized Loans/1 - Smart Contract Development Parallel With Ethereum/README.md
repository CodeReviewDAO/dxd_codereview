Grant Proposal | [NFT Collateralized Loans](https://portal.devxdao.com/public-proposals/498)
------------ | -------------
Milestone | 1
Milestone Title | Smart Contract Development Parallel With Ethereum
OP | CaptainBernardo
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**


Deliverables
Some of this grant will go to pay for common RnD between both the Casper and Solana versions.
NFT Locker Contract
Contains NFT locking
Contains loan logic 
Contains defaulting logic
NFT Locker Factory
Deploys the locker contracts
We will add support for extended CEP47 -> ERC1155 via gap analysis
Documentation & Tests

**Acceptance criteria:**

Users can put up an NFT for collateral
Counter parties can make loans
Users can make payments
Counter parties can automatically get the NFT if a default occurs

CRDAO: Verification for this will be as a suite of unit tests for each contract.

**Additional notes regarding submission from OP:**

Completed per criteria

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-LiquidNFT | eb03989

# Install & Usage Testing Procedure and Findings

The reviewer followed the instructions on the README of the project to set it up, deploy to the Testnet, and test its functionality by running the end-to-end tests. The procedure was carried out on Ubuntu 20.04.

At the first attempts of following the instructions, the reviewer encountered a number of issues/errors, mostly at the documentation level, causing the project to be not buildable/deployable/usable, which would normally result in a review with a FAIL recommendation. The reviewer provided the OP with the feedback coming out of these attempts. The OP fixed & improved the project and its documentation based on the feedback, and informed the reviewer that the project is now ready to be reviewed. The review presented here covers the latest version of the project which includes all of those fixes and the improvements.

Since the OP did not provide an application with a UI which utilizes the smart contracts in the project, and the acceptance criteria of the milestone specifically instructs the CRDAO to do the verifications based on unit tests, the usage testing part of this review focuses on the unit and the end-to-end tests.

## Overall Impression of usage testing

It was observed that the project builds and passes the automated tests successfully after the quick fixes by the OP, and the documentation provides sufficient installation/execution instructions. However, the reviewer thinks that the documentation still has room for improvement towards further simplicity, clear explanations and sampel commands.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has sufficient tests covering both the positive and the negative paths. The reviewer observed that all of the tests successfully pass.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

All critical functions have been observed to have standard comments to provide the code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project Documentation was observed to be acceptable with usage documentation and examples. However, the reviewer thinks that more examples and use cases would be highly beneficial for the users of the project.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are at an acceptable state, with room for further improvements. The code-level documentation is sufficient.

The reviewer communicated the shortcomings of the documentation, along with further points of possible improvements which may not fall in the scope of this review, with the OP. OP acknowledged the feedback, and showed interest in working on further improvements.

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution policy. However, the project lacks a security policy, and the repository doesn't have the relevant tags, hindering its discoverability.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and has extensive tests.

# Final Conclusion

The project is generally in a very good shape in terms of open-source guidelines. Moreover, the project has extensive tests, and a sufficient level of documentation. The project also successfully builds and passes both the manual and the automated tests, providing the promised functionality. However, the project documentation can be improved further based on the notes in teh relevant sections of this review.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
