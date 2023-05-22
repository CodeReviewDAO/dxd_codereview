Grant Proposal | [645 - Smart Billing Platform Prototype](https://portal.devxdao.com/public-proposals/645)
------------ | -------------
Milestone | 3
Milestone Title | Backend prototype with frontend - Submission 1
OP | OpenSourceREMarketModel
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Developing a backend prototype along the user journeys and designing the most important screens.
- The backend prototype will be geared towards providing the functionality covered in the user journeys. It will contain a bridge to the Casper blockchain, allowing in particular the issuance and management of DIDs (tokens).

**Acceptance criteria:**

- An end-to-end backend prototype is built and ready to be demoed to reviewing entities. The most important screens are built (uploaded to GitHub).
- The backend prototype covers at least two of the three main user journeys as described in Milestone #1 but ignores special cases, edge cases, etc. The screens describe the most important elements of a frontend.

**Additional notes regarding submission from OP:**

The above repository contains the link for the code base for the prototype for Milestone 3 of Grant #645.  
The README.md file in the main directory contains detailed explanations for the code base as well as the review and usage process using the UI and API developed for this prototype.

A dedicated review environment has been created. It can be reached at:
The review environment can be reached as follows:

UI: https://app-sbpdxd-m3.shared-dev.noumenadigital.com/login  
API: https://api-sbpdxd-m3.shared-dev.noumenadigital.com  
Swagger: https://api-sbpdxd-m3.shared-dev.noumenadigital.com/swagger/

The users and the password for the environment, as well as the explanations for obtaining an Auth Token for the API are included in the main README.md file.

If there are any questions, please don’t hesitate to reach out.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/NoumenaDigital/sbp-dxd-m3 | 5b38955


# Install & Usage Testing Procedure and Findings

The reviewer used an Ubuntu 22.04.2 LTS GitPod instance and a local Pardus 21.5 GNU/Linux local instance for local installations. Usage testing was done on the servers provided by OP.

There were some out of date warnings at the beginning for building the frontend, which can be easily fixed and does not affect the build process.

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | PASS / FAIL / PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes


# Unit / Automated Testing

_Summarize the result of the unit testing / automated testing / integration testing provided in the Milestone. Feel free to include
automated test output, either as text, image or other artifact. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS / FAIL / PASS with Notes
Unit Tests - At least one negative path test | PASS / FAIL / PASS with Notes
Unit Tests - Additional path tests | PASS / FAIL / PASS with Notes


# Documentation

### Code Documentation

The code documentation for the project is well-prepared and of high quality. It provides thorough coverage of the codebase, making it easier for developers to understand and maintain the code. The comments and documentation throughout the code are helpful and demonstrate attention to detail. Overall, the code documentation is a valuable asset to the project, showcasing skill and professionalism.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project documentation is exemplary, characterized by its exceptional level of detail and professional presentation. It covers all aspects of the project, including the step-by-step process of building the application, testing methodologies, and deployment procedures. The documentation is written in a clear and concise manner, ensuring that users can easily follow the instructions and understand the project's workflow. The reviewer is highly impressed with the comprehensive nature of the documentation and believes it surpasses the necessary requirements for this project.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

The project's code documentation demonstrates a commendable level of thoroughness and organization, effectively addressing all crucial elements of the codebase. It provides comprehensive insights into the project's design, implementation, and usage, ensuring developers have the necessary information to work with the code effectively. The detailed documentation showcases the project team's commitment to delivering a comprehensive resource for users. Overall, the reviewer is satisfied with the documentation's quality and finds it to be more than adequate for the project's needs.


# Open Source Practices

## Licenses

The project is released under the Apache-2.0 license.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING and SECURITY policies. Pull requests and Issues are enabled on the repositories and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

The source code adheres to good coding practices, with a clear and organized structure that is easy to understand. The use of automated linting tools ensures that the code is free from common errors and inconsistencies, resulting in improved readability and maintainability. As a result, the codebase is of high quality and user-friendly, making it easy for developers to work with.


# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_


# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
