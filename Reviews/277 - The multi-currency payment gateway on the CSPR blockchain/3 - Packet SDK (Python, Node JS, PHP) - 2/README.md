Grant Proposal | [277 - The multi-currency payment gateway on the CSPR blockchain](https://portal.devxdao.com/public-proposals/277)
------------ | -------------
Milestone | 3
Milestone Title | Packet SDK (Python, Node JS, PHP)
OP | Huy Tran 
Reviewer | Thham  <thham2022@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Packages SDK suitable for Python, Node JS, PHP languages

**Acceptance criteria:**

Complete SDK packages, ready to use with Python, Node JS, PHP

**Additional notes regarding submission from OP:**

Packages SDK suitable for Python, Node JS, PHP languages to integrate with Payment gateway.

PHP SDK https://github.com/DHFinance/dhf-pay-php

Python SDK https://github.com/DHFinance/phf-pay-python

NodeJS SDK https://github.com/DHFinance/dhf-pay-js

Add Integration tests, 
Add more nagative path tests, 
Fix security bugs, 
Fix bug Permission request when install Python, 
Complete the documentation.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/DHFinance/dhf-pay-php | 1cf8f10
https://github.com/DHFinance/phf-pay-python | 20b361c
https://github.com/DHFinance/dhf-pay-js | 1a029b6

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of repository (NodeJS, PHP, Python SDKs), there were some errors during the PHP SDK installation process due to incomplete documentation. After coordinating with the OP, the document has been updated and installed successfully. 

[Build Logs PHP](assets/install-php.md)

[Build Logs Python](assets/install-python.md)

[Build Logs NodeJS](assets/install-js.md)


## Overall Impression of usage testing

The SDKs documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

All tests passed on the 3 SDK. Unit tests a pretty simple and need to be improve, but integration test already covered most of functions.

[Test Logs for PHP SDK](assets/tests-php.md)

[Test Logs for Python SDK](assets/tests-python.md)

[Test Logs for NodeJS SDK](assets/tests-js.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

The code documentation is sufficient on all 3 sdk, with summaries and comments, especially on critical classes and methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The README file provides minimum but sufficient documentation on how to install and run the project.

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient.

# Open Source Practices

## Licenses

Each SDK are released under Apache License 2.0.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository, and the project contains a CONTRIBUTING and a SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. 

# Final Conclusion

The OP has fixed the issues raised in the first review: Add Integration tests, Add more nagative path tests, Fix security bugs, Fix bug Permission request when install Python, Complete the documentation. 

Unit tests a pretty simple and need to be improve, but integration test already covered most of functions.

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
