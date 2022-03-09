
Grant Proposal | [50 - 721 Standard - Transpiler](https://portal.devxdao.com/public-proposals/50)
------------ | -------------
Milestone | 4
Milestone Title | Deploy Contracts to Mainnet and Frontend to Production
OP | VDAO
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the 4th and the final milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Deliverable: Mainnet Deployed Contracts

**Acceptance criteria:**

Acceptance Criteria : Peer Reviewed Mainnet Deployed Contracts with working transactions

**Additional notes regarding submission from OP:**

All milestones completed. Thank you for review and consideration.

https://github.com/Herasoft/CSPR-721-DEVxDAO-Grant

https://github.com/Herasoft/CSPR-721-DEVXDAO-GRANT-RUST-BASE

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Herasoft/CSPR-721-DEVXDAO-GRANT-RUST-BASE | 23535c3
https://github.com/Herasoft/CSPR-721-DEVxDAO-Grant | eafc5e7

The reviewer finds the submission slightly confusing in terms of acceptance criteria as the title of the milestone, the milestone details, and the acceptance criteria don't seem to match. However, the reviewer will try to infer the essence of the submission as much as possible, and continue the review by focusing on the general definition of done and the open-source guidelines endorsed by the DxD and the CRDAO.

# Install & Usage Testing Procedure and Findings

## Base repository

The reviewer followed the instructions on the README of the project to build the project, and run the automated tests, but it was observed that **the README of the project lacks deployment and usage instructions and examples.** Moreover, the acceptance criteria, in the reviewer's opinion, is not ideal for an acceptance review as it doesn't tell anything about the specific functionalities to be checked/provided although it is not in the scope of this review.

* [build](assets/build.md)
* [test](assets/test.md)

The reviewer was then [able to deploy](https://testnet.cspr.live/deploy/731d4f9848905ac4937be9c9c2a8512cd0b785b13b8b35bd1bfdab4d4844f6c7) the contract onto the Casper Testnet, based on his experience, after inspecting certain test case arguments of the project.

The procedure was carried out on Ubuntu 20.04 in the cloud.

## Front-end

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

The project has sufficient tests covering both the positive and the negative paths. The reviewer observed that all of the tests successfully pass for the base repository. However, the front-end repository is in a direct failure status, causing the checks in this section not doable.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A

# Documentation

### Code Documentation

For the base repository: **The code-level documentation of the project has been observed to be extremely sparse** although the function names seem to be self-explanatory to some extent. **The code-level documentation must be improved for this submission to pass,** with comments for all code portions for the critical functionality.

The front-end repository seems to be in a better state with minimal code-level comments. Reviewer suggests OP to also make sure they are sufficient as part of their effort towards getting the front-end repository into shape.

Requirement | Finding
------------ | -------------
Code Documented | FAIL

### Project Documentation

Base repository: **Project Documentation has been observed to be extremely sparse, and must be improved with proper deployment and usage instructions and examples for this submission to pass.** It currently has only the very basic instructions for building and testing.

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

Pull requests and issues are enabled on the repositories. However, the project has no contribution or security policies. Moreover, the repositories have no description, website, or topics, hindering its discoverability.

Although they are not causes for a failure, the reviewer highly suggests improving these points.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and has an acceptable level of tests for the base repository. However, the front-end repository is in a direct failure state, rendering any observation in this section irrelevant.

# Final Conclusion

First of all, the reviewer would like to note that this review was put on hold on OP's request and within knowledge of the job poster, to give the OP enough time to improve certain points of the submission to meet the requirements, due to certain difficulties experienced by the OP. The reviewer thanks the OP for the improvements done during that time frame, based on the guidance provided as courtesy of the CRDAO.

The project's base repository builds and passes automated tests which proves basic functionality of the smart contract, but both the project-level and the code-level documentation must be improved significantly as per the notes in the relevant sections of this review, the standard definition of done of the DxD, and the open-source guidelines presented by the DxD proposal #185. Then it needs to be deployed on the Mainnet to meet the acceptance criteria.

The front-end repository of the project is in a direct failure state, and also needs to be improved significantly to meet the standard definition of done of the DxD, and the open-source guidelines presented by the DxD proposal #185. Then it needs to be deployed to a production environment by the OP.

Thus, in the reviewers opinion, this submission should FAIL.

# Recommendation

Recommendation | FAIL
------------ | -------------
