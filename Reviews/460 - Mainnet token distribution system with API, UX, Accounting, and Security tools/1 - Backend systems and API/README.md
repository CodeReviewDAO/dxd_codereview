Grant Proposal | [460 - Mainnet token distribution system with API, UX, Accounting, and Security tools](https://portal.devxdao.com/public-proposals/460)
------------ | -------------
Milestone | 1
Milestone Title | Backend systems and API - Submission 1
OP | LedgerLeap
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The first of 2 milestones will deliver the system backend environment for CSPR distribution. This includes the ability to generate keys for API access and whitelist the IPs able to use these keys. The system will also assess daily and per transaction rate limits. A token transfer system will send CSPR mainnet tokens if the key is valid, the IP of the request is approved, and the transfer does not surpass rate limits. Keyholders will also provide the address to which the CSPR tokens will go. All transfers will be recorded in a database along with the pertinent security information to verify the sender. The API will have clear error codes for invalid requests. The first milestone expects to have 2 developers assigned for 8 to 9 days to build these features in an optimal way that supports the next milestone built on top.

**Acceptance criteria:**

The environment will support installation, and testing will begin by registering an API key and IP address. Once registered, the system will allow a test send of CSPR by submitting a request including the key, recipient address, and amount of CSPR. The system will check the rate limit logic, then send CSPR and log the transaction if approved.

**Additional notes regarding submission from OP:**

The URL of the backend API staging deployment is at: https://api.casperfyre.com/  
Backend API has been updated and finished to include all required endpoints, throttling, security, documentation, and unit tests. Some test orders have been executed using a test account with 500 CSPR initially deposited. Transactions purposefully meant to succeed have been verified on chain.  
This simple use guide can be followed:
 - Any user can register to use the portal and verify their account application.
 - Your admin must accept your application from the admin panel. Staging credentials for an admin account will be provided discretely.
 - After your application is accepted and your account is active, you can create new API keys, wallets, and whitelist your company IP addresses.
 - Upon account activation, a wallet and API key is automatically issued and displayed on your dashboard. The IP address you applied from will also automatically be added to your whitelist.
 - Deposit some CSPR to your wallet. All keys are kept encrypted and recoverable using server software keys.
 - Use/test the public facing API using the automatically generated documentation found in your dashboard settings as a reference.
A full description and usage guide instruction can be found at https://github.com/ledgerleapllc/casperfyre-backend/blob/main/README.md

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/ledgerleapllc/casperfyre-backend | 1dd0d51


# Install & Usage Testing Procedure and Findings

_Provide a detailed review of your install and usage testing of the project. Highlight any issues setting up the project,
including shortcomings in the documentation/setup instructions. Test the usage of the project against the Acceptance Criteria
provided for the grant milestone._

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

Code documentation is very well prepared and is of high quality. All critical functionality of the code is commented. Many other helping comments and documentation are provided within the code and they are well prepared and detailed.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Reviewer was able to generate the necessary documentation provided with the instructions. The documentation includes key components, how to install and run the proect and usage examples.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation for the project is sufficient for this milestone.


# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING and SECURITY policies. Pull requests and Issues are enabled on the repository and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project. Overall sufficient work is done.


# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
