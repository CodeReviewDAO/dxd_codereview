Grant Proposal | [410 - Dockerized NCTL](https://portal.devxdao.com/public-proposals/410) 
------------ |--------------------------------------------------------------------------
Milestone | 1                                                                        
Milestone Title | Docker Image and the Instructions                                                       
OP | Alex Kelly | MAKE 
Reviewer | Killian Hascoet <killianh@live.fr>                                              

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

_Dockerization of NCTL will be completed, and the new Docker image will be published on Docker Hub, along with the instructions on how to run it._

**Acceptance criteria:**

- NCTL docker image is available on Docker Hub
- It is possible to start a local network for testing, by following the provided instructions

**Additional notes regarding submission from OP:**

_https://github.com/make-software/casper-nctl-docker_

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-nctl-docker | 0496747


# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-nctl-docker/blob/master/BUILD.md, 
reviewer was able to successfully build the docker image and run the tests against it. 
The reviewer was also able to use the docker image published on docker hub, and run queries against the created network.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions,
the project functionality meets/exceeds the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Given the DOD :
- Integration tests with other systems are not required for software to be considered 'done'.

The project is an integration of multiple other systems not developed by the OP.
The reviewer was able to run the test suite provided against the locally built docker image.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The dockerfile is well documented.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project is well documented.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The project is released under the Apache License 2.0

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Final Conclusion

The project meets the functional requirements. The reviewer was able to build / run the tests and use the existing docker image.

Thus, in the reviewer's opinion, this submission should PASS with notes.

# Recommendation

Recommendation | PASS
------------ | -------------
