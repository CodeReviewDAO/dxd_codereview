
Grant Proposal | [50 - 721 Standard - Transpiler](https://portal.devxdao.com/public-proposals/50)
------------ | -------------
Milestone | 3
Milestone Title | Audit Smart Contracts
OP | VDAO
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the 3rd milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Deliverable: Audited Smart contracts for review on Casper testnet

**Acceptance criteria:**

Acceptance Criteria :External Review, Passing Tests, Deployed to Testnet with transaction tests.

**Additional notes regarding submission from OP:**

All milestones completed. Thank you for review and consideration.

https://github.com/Herasoft/CSPR-721-DEVxDAO-Grant

https://github.com/Herasoft/CSPR-721-DEVXDAO-GRANT-RUST-BASE

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Herasoft/CSPR-721-DEVXDAO-GRANT-RUST-BASE | 23535c3

The [front-end repository](https://github.com/Herasoft/CSPR-721-DEVxDAO-Grant) mentioned in the submission notes is part of the next milestone, and thus will be omitted for this review.

# Install & Usage Testing Procedure and Findings

The reviewer followed the instructions on the README of the project to build the project, and run the automated tests, but it was observed that **the README of the project lacks deployment and usage instructions and examples.** Moreover, the acceptance criteria, in the reviewer's opinion, is not ideal for an acceptance review as it doesn't tell anything about the specific functionalities to be checked/provided although it is not in the scope of this review.

* [build](assets/build.md)
* [test](assets/test.md)

The reviewer was then [able to deploy](https://testnet.cspr.live/deploy/731d4f9848905ac4937be9c9c2a8512cd0b785b13b8b35bd1bfdab4d4844f6c7) the contract onto the Casper Testnet, based on his experience, after inspecting certain test case arguments of the project.

The procedure was carried out on Ubuntu 20.04 in the cloud. [A deployment on the Testnet](https://testnet.cspr.live/deploy/25f248e18cba3d7a1d6da5adba8a95991cbd044dab94db6d1b7dff57f8849c3a) was also submitted by the OP to meet the acceptance criteria, and it was observed to be a successful deployment.

## Overall Impression of usage testing

It was observed that the project builds and passes the automated tests successfully, **but the documentation does not provide sufficient installation/execution instructions** although it is possible to deploy the smart contract based on previous experience. Moreover **the submission lacks the contract audit which was one of the acceptance criteria.**

Thus, the reviewer thinks that this part of the review should PASS with Notes only because it is a non-final milestone, the contract was successfully deployed despite the lack of the instructions, and the audit criterion is not a functional requirement and it was communicated to be not needed on top of its vague way of wording.

Overall, the documentation must be improved to include instructions and examples for installation/deployment and usage before the final milestone, and the job poster and/or the grant-giving body should decide if the audit is actually needed, and accept/pass the submission on this condition as this review focuses on the standard definition of done required by the DxD, and the open-source guidelines and standards endorsed by the DxD and the CRDAO.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

The project has sufficient tests covering both the positive and the negative paths. The reviewer observed that all of the tests successfully pass.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

**The code-level documentation of the project has been observed to be extremely sparse** although the function names seem to be self-explanatory to some extent. **The code-level documentation must be improved before the final milestone,** with comments for all code portions for the critical functionality.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

**Project Documentation has been observed to be extremely sparse, and must be improved with proper deployment and usage instructions and examples before teh final milestone.** It currently has only the very basic instructions for building and testing.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are extremely sparse, and must be improved significantly before the final milestone.

# Open Source Practices

## Licenses

The Project is correctly released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. However, the project has no contribution or security policy. Moreover, the repository has no description, website, or topics, hindering its discoverability.

Although they are not causes for a failure, the reviewer highly suggests improving these points.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and has an acceptable level of tests.

# Final Conclusion

First of all, the reviewer would like to note that this review was put on hold on OP's request and within knowledge of the job poster, to give the OP enough time to improve certain points of the submission to meet the requirements, due to certain difficulties experienced by the OP. The reviewer thanks the OP for the improvements done during that time frame, based on the guidance provided as courtesy of the CRDAO.

The project builds and passes automated tests which proves basic functionality of the smart contract, but both the project-level and the code-level documentation must be improved significantly before the final milestone as per the notes in the relevant sections of this review, the standard definition of done of the DxD, and the open-source guidelines presented by the DxD proposal #185.

The non-functional and not-well-defined requirement of audit has been considered out of scope of this review, and should be taken into account by the grant-giving body instead.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------


