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

## Install

In accordance with DEVxDAO's request, there will be no review conducted for the local build and installation procedures in this milestone. This exclusion was explicitly mentioned in the job posting and subsequently communicated with DEVxDAO administrators. Additionally, the reviewer is unable to assess the accuracy and reliability of the installation and execution documentation, despite the presence of detailed instructions in the repository. Therefore, both of these aspects will be designated as Not Applicable in the final assessment table.

## Usage Testing

The testing and evaluation of the prototype were performed on the servers provided by the OP for this purpose. The reviewer used the dedicated review environment to assess the prototype submitted in this milestone.

### Login, Authoriztation & Account Procedures

The reviewer successfully accessed the test review environment specified in the account information table given in the README by following the instructions. Once logged in, the reviewer proceeded to the account page by clicking on the username located in the top right corner. By following link under Casper Account Details, the reviewer was directed to the Casper account page, where they observed the most recent action of adding a delegate right to the Casper DID Management Smart Contract.

The reviewer followed the instructions provided to verify the delegate rights from the Casper Smart Contract. The reviewer navigated to the delegates dictionary within the DID contract. Using the account-hash of the specified user (`user1`), the reviewer searched for it within the dictionary and found that the SBP account-hash is listed as a delegate of the `user1` account.

### Invoice Verification

After logging in, the reviewer navigated to the invoices overview page and clicked on "Add New Invoice" to create a new invoice. Then, entered the required necessary data. When prompted to trade the invoice, the reviewer selected "No" to proceed with the invoice verification use case. The reviewer entered the customer details and clicked on "Create Invoice" to finalize the creation of the invoice within the system. The reviewer was then presented with a detailed overview page displaying the specific invoice. By clicking on "BLOCKCHAIN REF," the reviewer was directed to the IPFS representation of the invoice. Accessing the "Invoices" section in the left navigation menu, the reviewer confirmed that the new invoice had been successfully added to the system.

### Smart Billing

The reviewer navigated to the contract overview page and clicked on "Add New Contract" to initiate the creation of a new contract. Contract details were entered. Supplier data was pre-filled to match the user data. The reviewer filled in the customer details and moved to the next page. Ensuring compliance with the requirement, the reviewer provided the necessary milestones, making sure that the sum of all milestones matched the full value of the contract. Without adding additional milestones, the reviewer selected "No" to place the invoice on the marketplace. Once everything was entered, the reviewer saved the info. The contract was successfully created. The reviewer clicked on "Sign and Submit" to proceed. Upon signing, the contract switched to the "Active" state, allowing milestones to be reached. The reviewer marked the first milestone as completed, which marked the respective milestone as completed with its date. This also caused the creation of an invoice. The created was put on its finalized state. The contract remained open until all respective invoices were paid, indicating the completion of all milestones.

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | N/A
Documentation provides sufficient installation/execution instructions | N/A
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes


# Unit / Automated Testing

As per the request from DEVxDAO, installation of the project was not carried out during the review process. Consequently, the reviewer faced limitations in conducting unit tests for the assessment. Since unit tests typically require a properly installed project environment, the absence of installation prevented the reviewer from executing and evaluating the unit tests effectively. Therefore, due to the specific instruction from DEVxDAO, the reviewer was unable to perform the required unit tests as part of the project evaluation.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A


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
