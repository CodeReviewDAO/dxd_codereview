Grant Proposal | [128 - ClearestStake staking asset manager for Node operators and groups](https://portal.devxdao.com/public-proposals/128)
------------ | -------------
Milestone | 2
Milestone Title | Development of user onboarding environment and user dashboards
OP | LedgerLeap
Reviewer | Muhammet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

This phase will deliver a front and back end system allowing recipients to receive secure invite links, powered by an emailer and verification process, where the user can accept a number of tokens from the system. Next, the user will create an account on the delivered registration process. User log in will also be delivered during this stage, support access to the user dashboard. This dashboard will be the heart of the system for users, showing an integrated pricing chart to show current convertible value of the user's token. The dashboard will also show every transaction on the users account in a clear accounting format for tracking and making tax calculations easy. Users will also have access to support and withdrawal function and forms, alerting admin and starting processes for support or distributions. Based on current resources and bandwidth, we expect to have a team of 3 developers, 1 engineer, and 1 project manager work a cumulative 420 hours for these deliverables. Because the team has other projects to balance time between, this milestone will require up to 60 days from the delivery of the prior milestone.

**Acceptance criteria:**

The following items will be delivered in the repository and also testable on a demonstration domain:

• Front-end built out in NEXT.JS for token-owner user views.
• User database will be delivered to support the other functions delivered in this phase.
• A test version of the invite system will allow a new user to claim their tokens by setting a password.
• Registration, password, and password reset will function.
• An IP logging system will be in place for all logins by token holders.
• An email verification system will function.
• User dashboard will be live and include sections to show balance, pricing, and transactions.
• User balance section will show live update of sample user test data with a converted price for token holdings and last distribution date for staking rewards.
• A withdrawal function will be deployed. This will be a form process designed to alert the admin to the need to process a user withdrawal. The front-end ONLY will be delivered in this phase. Admin side to be developed in next phase.
• A user invite system will support the addition of new users to the system by collecting their name, email, and starting balance. This system will send invites to the subject user for them to onboard themselves securely by setting a password. IPs will be logged. This system will recalculate the percentages of the master node total for all users to support the new user within the inflation credit system.
• User support system will be implemented, allowing a user to submit a ticket or question to admin and admin to have a dashboard and email alert.
• Admin side of withdrawal request system will support alerting admin of user, withdrawal request amount, and date for processing withdrawal requests.
• Withdrawing all tokens will be supported, removing users from the token inflation function.
• The admin dashboard will support tables for users and transactions, showing pertinent data such as token, converted price, percent of node, and last inflation rewards. Transactions will show data, type, and the subject user.
• User detail page will show the data and transactions attributed to a subject user, along with a log of all IPs used to access the system by the user.

Please see acceptance criteria as opposed to KPIs for the definition of done/delivered. KPIs are less applicable for this build as we are not measuring performance in this situation but rather the delivery of assets. The team will present the functionality of any and all systems detailed in the "Acceptance Criteria" section during a schedule zoom accessible to the public and record this session for proof of delivery.

**Additional notes regarding submission from OP:**

Repos updated for this Not 15th submission as per the CRDAO requirements.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/ledgerleapllc/cleareststake-frontend | d6fc357
https://github.com/ledgerleapllc/cleareststake-backend | 25ce75c

# Install & Usage Testing Procedure and Findings

Following the instructions in the README files of the frontend and the backend repositories of the project, reviewer was able to successfully build the source code, and make a test deploy for this milestone on the cloud in an `Ubuntu 20.04` environment, only after certain additional steps and modifications to the instructions noted below along with suggested improvements.

## Installation
### Documentation
* Backend and Frontend documentations provide `apache2` installation commands but it does not contain the virtual hosts configuration. 
* SSL configuration is missing
* Backend needs MySQL installation/configuration but the README does not cover it in a detailed way.
* The "laravel" database needs to be created before install.
* It would be good to add instructions on restarting the backend and the location of the logs to the README.
* The backend's .env file fields are clear but documentation does not explain it or provide example on it.

### Build
* The `npm install` command failed with an error for the frontend repository, and succeeded only after issuing the command as `npm install --legacy-peer-deps`.
* The `npm run build-export` command failed with an error for the frontend repository, and succeeded only after manually removing the `eslint .` part from the `build-export` script.


### Testing
* The cypress commands to run the integration/UI tests require additional dependencies not mentioned on the README.

## Usage Testing
Reviewer verified the basic login and logout functions and observed the full dashboard of the app successfully loaded on the test deploy.

![Test Deploy Login](/assets/01-login-test-deploy.png)
![Test Deploy Logged-in](/assets/02-logged-in-test-deploy.png)

Then the promised functionalities for the milestone were tested manually by using `Firefox 95.0 (64-bit)` as the browser, on the production deploy provided by the OP.

All functions were observed to be at an acceptable state except the following points observed by the reviewer, which need to be fixed before the final milestone of the project:

* Get Help / Ask a Question form gives an error when the Submit button is clicked. Due to this bug, the reviewer was not able to manually test certain parts of the functionality relying on this.
![Get Help Error](/assets/06-Get-Help-Form-Error-1.png)
![Get Help Error](/assets/07-Get-Help-Form-Error-2.png)

* Request Withdraw form gives an error when the Submit button is clicked. Due to this bug, the reviewer was not able to manually test certain parts of the functionality relying on this.
![Request Withdraw Error](/assets/09-Request-Withdraw-Error.png)
![Request Withdraw Error](/assets/10-Request-Withdraw-Error-2.png)

* On the Fund Sale screen, the number of users on the table doesn't match the number of users reported at the top of the page.
![Fund Sale screen](/assets/25-Admin-Fund-Sale.png)

* On the Fund Sale screen, entering the exact amount reported on the UI to the total value field causes an error (seen in red at the bottom of the page), and can be fixed only by manually adjusting the amounts on the individual rows.
![Fund Sale error](/assets/26-Admin-Fund-Sale-Filled.png)



Functionality | Finding
------------ | -------------
Front-end token-owner user views | PASS
User database | PASS
Test version of the invite system | PASS
Registration, password, and password reset | PASS
IP logging system | PASS
Email verification system | PASS
User dashboard with balance, pricing, and transactions | PASS
User balance section live-updates with a converted price for token holdings and last distribution date for staking rewards | PASS
Withdrawal function front-end form | PASS with Notes
User registration through the user invite system | PASS
The percentages of the master node total for all users recalculated after new user addition | PASS
User support system with admin dashboard and email alerts | N/A
Admin side of withdrawal request system will support alerting admin of user, withdrawal request amount, and date for processing withdrawal requests | N/A
Withdrawing all tokens will be supported, removing users from the token inflation function | N/A
The admin dashboard will support tables for users and transactions, showing pertinent data such as token, converted price, percent of node, and last inflation rewards. Transactions will show data, type, and the subject user | PASS
User detail page will show the data and transactions attributed to a subject user, along with a log of all IPs used to access the system by the user | PASS

## Overall Impression of usage testing

Both on the test deployment by the reviewer and the demo deployment provided by the OP, all of the major functionality is observed to be working properly except the points noted in the Usage Testing section above.

Although the reviewer was able to build and install the application only after the modifications and the extra steps mentioned earlier in the review, these are not reasons for a failure, in the reviewer's opinion, at this non-final milestone. Nonetheless, the reviewer recommends fixing the noted points, and revising and improving the documentation to cover these difficulties.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

Project contains UI and integration tests on the frontend side, and API tests on the backend side, covering the critical functionality. However, in the reviewers opinion, the test coverage is weak and heavily focused on the positive paths. Although the reviewer doesn't see this as a cause of failure for this non-final milestone, he thinks the test coverage needs to be improved significantly also by focusing on the negative path tests before the final milestone.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Code Analysis & CI Facilities

The project has automated code analysis setup on the frontend repository and continuous integration setup on the backend repository. The reviewer praises the OP for having these setup as they are crucial for any open-source project to resist regressions. However, it would be highly suggested to also add a UI test action to the frontend repository.

Requirement | Finding
------------ | -------------
Code Analysis | PASS
Continuous Integration | PASS with Notes

# Documentation

### Code Documentation

Code documentation is sparse on both the frontend and the backend side. Reviewer was able to generate the api documentation by using `phpDocumentor`, and observed that the code-level documentation for the critical functions needs to be improved although it is possible to to have a basic understanding of the code-base due to easy-to-understand structure and naming of the entities. Reviewer recommends improving the code-level documentation, and highly suggests adding proper instructions on the README to generate the api documentation and also to provide an auto-generated version of the documentation, updated on new commits on the `master` branch.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

README.md has sufficient general information about the project, along with installation instructions, and the usage documentation. However, in the reviewer's opinion, the installation instructions should be improved to allow the individuals who are not devops/systems engineers to install the app with ease.

Usage documentation is brief. The reviewer suggests detailing the usage documentation with specific usage scenarios and steps.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. The project also has a CONTRIBUTING policy and a security policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## Dependencies
The project has a number of dependencies with high or critical-level security vulnerabilities, which are recommended to be fixed as soon as possible. Reviewer highly suggests enabling dependency checks on the project's repositories to be alerted about such vulnerabilities in the future.

### Frontend

Dependency | Vulnerability | Severity
------------ | ------------- | -------------
follow-redirects | [CVE-2022-0155](https://github.com/advisories/GHSA-74fj-2j2h-c42q) | High
simple-get | [CVE-2022-0355](https://github.com/advisories/GHSA-wpg7-2c88-r8xv) | High
node-fetch | [CVE-2022-0235](https://github.com/advisories/GHSA-r683-j2x4-v87g) | High
next | [CVE-2021-43803](https://github.com/advisories/GHSA-25mp-g6fv-mqxx) | High
next | [CVE-2021-39178](https://github.com/advisories/GHSA-9gr3-7897-pp7m) | High
trim-newlines | [CVE-2021-33623](https://github.com/advisories/GHSA-7p7h-4mm5-852v) | High
glob-parent | [CVE-2020-28469](https://github.com/advisories/GHSA-ww39-953v-wcq6) | High
glob-parent | [CVE-2020-28469](https://github.com/advisories/GHSA-ww39-953v-wcq6) | High

## General Observations

Code is generally well-structured and readable. The project as committed to GitHub and both the automated tests and the manual tests pass. However, the project has a number of dependencies with high or critical-level security vulnerabilities.

# Final Conclusion

The project provides the most of the functionalities described in the grant application and milestone acceptance criteria. The reviewer praises the OP for the general stability and the fluid user experience of the app. The reviewer also would like to thank the OP for including the open-source policies, which are very important for the long-term sustainability of any open-source project, in the project's repositories.

However, the Get Help and the Request Withdraw forms are not working properly which hinders a user's ability to benefit the application. Moreover, the project has a number of dependencies with high-level security vulnerabilities. Both of these would be reasons for a failure if this was not a non-final milestone.

Although they are not causes for failure, the build and the installation instructions, as well as the usage documentation have some room for improvements. Moreover, the project build succeeds only after, even though they are minor, manual modifications.

The project also has a few small UI bugs which were noted at the relevant section of the review. Although these does not cripple any critical functionality, they are suggested to be fixed for a flawless user experience.

Thus, in the reviewer's opinion, this submission should PASS with Notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
