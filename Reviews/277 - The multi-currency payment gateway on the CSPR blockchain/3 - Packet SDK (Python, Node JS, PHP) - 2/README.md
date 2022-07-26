Grant Proposal | [277 - The multi-currency payment gateway on the CSPR blockchain](https://portal.devxdao.com/public-proposals/277)
------------ | -------------
Milestone | 3
Milestone Title | Packet SDK (Python, Node JS, PHP) - Submission 2
OP | Huy Tran <tqhuy2018@gmail.com>
Reviewer | Yusuf Keten <ketenyusuf@gmail.com>

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

? Add Integration tests

? Add more nagative path tests

? Fix security bugs

? Fix bugs wrong price calculation on frontend

? Fix bug Permission request when install Python

? Complete the documentation

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/DHFinance/dhf-pay-php | 1cf8f10
https://github.com/DHFinance/phf-pay-python | dcf8721
https://github.com/DHFinance/dhf-pay-js | e46a18f


# Install & Usage Testing Procedure and Findings
All of the SDKs are installed and tested successfully. The OP has fixed the previous bugs as mentioned in the first submission. The reviewer observed that the SDKs are working as expected.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The reviewer has observed that all tests run successfully without errors. However, the tests should be improved by adding more tests.

[JS Test Logs](assets/js-test.md)

[PHP Test Logs](assets/php-test.md)

[Python Unit Test Logs](assets/python-unit-test.md)

[Python Integration Test Logs](assets/python-integration-test.md)


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

The code documentation is sufficient on all of the SDKs.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The OP has improved the project documentation from the first submission. The reviewer observed that the project documentation is sufficient for the project. However, the OP is highly encouraged to improve the usage documentations.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, the documentations can be improved. Overall, the OP is highly encouraged to improve the documentation.

# Open Source Practices

## Licenses

All of the SDKs are released under Apache License 2.0 as stated in the grant.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. The project is committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are certain points noted above that could be improved on the project.

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
