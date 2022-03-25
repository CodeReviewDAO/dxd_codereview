Grant Proposal | [51 - 1155 Standard - Transpiler](https://portal.devxdao.com/public-proposals/51)
------------ | -------------
Milestone | 4
Milestone Title | Deploy Contracts to Mainnet and Frontend to Production
OP | VDAO
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the 3rd milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Deliverable: Mainnet Deployed Contracts

**Acceptance criteria:**

Acceptance Criteria : Peer Reviewed Mainnet Deployed Contracts with working transactions

**Additional notes regarding submission from OP:**

All milestones completed.  Thank you for review and consideration.

https://github.com/Herasoft/CSPR-1155-DEVxDAO-Grant

https://github.com/Herasoft/CSPR-1155-DEVXDAO-GRANT-RUST-BASE

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Herasoft/CSPR-1155-DEVXDAO-GRANT-RUST-BASE | ecfd35e
https://github.com/Herasoft/CSPR-1155-DEVxDAO-Grant | fee879a

# Install & Usage Testing Procedure and Findings

## Base repo
The reviewer followed the instructions on the README of the project to build the project, and run the automated tests, but it was observed that **the README of the project lacks deployment and usage instructions and examples.** Moreover, the acceptance criteria, in the reviewer's opinion, is not ideal for an acceptance review as it doesn't tell anything about the specific functionalities to be checked/provided although it is not in the scope of this review.

* [build](assets/build.md)
* [test](assets/test.md)

The reviewer was then [able to deploy](https://testnet.cspr.live/deploy/12f4b816ee4046315bcda99835ed9647dfc4ed577c263e2e476c53c74acf3ab1) the contract onto the Casper Testnet, based on his experience, after inspecting certain test case arguments of the project.

The procedure was carried out on Ubuntu 20.04 in the cloud. **No Mainnet deployment hash was submitted by the OP, thus it was not checked by teh reviewer.**

## Front-end repo
The reviewer could not build or run the project's front-end as there is no README in the repository. If it was a separate submission, this would cause a direct failure.

## Overall Impression of usage testing

It was observed that the project builds and passes the automated tests successfully, **but the documentation does not provide sufficient installation/execution instructions** although it is possible to deploy the smart contract based on previous experience. Moreover **the submission lacks the Mainnet deploy hash, and the info about a peer review, which were part of the acceptance criteria.**


It was also observed that **the front-end repository is in a direct failure status**, and needs to be significantly improved by adding the necessary pieces of documentation which would be expected from an open-source project as per the DxD definition of done and the open-source guidelines and standards. The OP also needs to provide a functional deployment of the front-end accessible in a production environment.

Thus, the reviewer thinks that this part of the review should FAIL because it is the final milestone and the points mentioned above needs to be fixed before it can pass.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

The reviewer observed that all of the tests successfully pass, but the project have **tests focusing only on the positive paths**. **The tests need to be improved to cover also the negative paths **. Moreover, the front-end repository is in a direct failure status, causing the checks in this section not doable.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

# Documentation

### Code Documentation

**The code-level documentation of the project has been observed to be extremely sparse** although the function names seem to be self-explanatory to some extent. **The code-level documentation must be improved,** with comments for all code portions for the critical functionality, to allow auto-generation of the related documentation.

The front-end repository seems to be in a better state with minimal code-level comments. Reviewer suggests OP to also make sure they are sufficient as part of their effort towards getting the front-end repository into shape.

Requirement | Finding
------------ | -------------
Code Documented | FAIL

### Project Documentation

**Project Documentation has been observed to be extremely sparse, and must be improved with proper deployment and usage instructions and examples before the final milestone.** It currently has only the very basic instructions for building and testing.

Front-end repository is in a direct failure state as it completely lacks the project-level documentation.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL
Example Documented | FAIL


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are extremely sparse, and must be improved significantly on the base repository, and must be prepared from the ground up on the front-end repository, for this submission to pass.

# Open Source Practices

## Licenses

The base repository is correctly released under the Apache-2.0 License. **The front-end repository completely lacks a license.**

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

## Contribution Policies

Pull requests and issues are enabled on the repositories. However, **the project has no contribution or security policy**. Moreover, **the repositories have no description, website, or topics**, hindering their discoverability.

Although they are not causes for a failure, the reviewer highly suggests improving these points.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code on the base repository is generally well-structured and readable. The project has been committed to GitHub, and has successfully passing **tests**, but **focusing only on the positive paths**. Moreover, **the front-end repository is in a direct failure state**, rendering any observation in this section irrelevant.

# Final Conclusion

First of all, the reviewer would like to note that this review was put on hold on OP's request and within knowledge of the job poster, to give the OP enough time to improve certain points of the submission to meet the requirements, due to certain difficulties experienced by the OP. The reviewer thanks the OP for the improvements done during that time frame, based on the guidance provided as courtesy of the CRDAO.

The project's base repository builds and passes automated tests which proves basic functionality of the smart contract, but the tests need to be improved to also cover the negative paths. Moreover, both the project-level and the code-level documentation must be improved significantly as per the notes in the relevant sections of this review, the standard definition of done of the DxD, and the open-source guidelines presented by the DxD proposal #185. Then it needs to be deployed on the Mainnet to meet the acceptance criteria.

The front-end repository of the project is in a direct failure state, and also needs to be improved significantly to meet the standard definition of done of the DxD, and the open-source guidelines presented by the DxD proposal #185. Then it needs to be deployed to a production environment by the OP.

The non-functional and not-well-defined requirement of the peer review has been considered out of scope of this review, and should be taken into account by the grant-giving body instead.

Thus, in the reviewers opinion, this submission should FAIL.

# Recommendation

Recommendation | FAIL
------------ | -------------
