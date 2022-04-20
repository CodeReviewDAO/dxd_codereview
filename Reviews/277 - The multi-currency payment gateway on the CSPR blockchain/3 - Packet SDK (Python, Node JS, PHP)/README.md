Grant Proposal | [277 - The multi-currency payment gateway on the CSPR blockchain](https://portal.devxdao.com/public-proposals/277)
------------ | -------------
Milestone | 3
Milestone Title | Packet SDK (Python, Node JS, PHP)
OP | Huy Tran <tqhuy2018@gmail.com>
Reviewer | Killian Hascoet <killianh@live.fr>

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

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/DHFinance/dhf-pay-php | 6c100a7
https://github.com/DHFinance/phf-pay-python | bc8ada9
https://github.com/DHFinance/dhf-pay-php | 8da03ad



# Install & Usage Testing Procedure and Findings

## JS

Missing the command to install the dependencies before launching the test / build command.

Unit tests are useless, they only asserts what the mock return. The reviewer ask the OP to do integration tests.

The SDK lack specific error types and a huge security issue was discovered.

## PHP

The published sdk on composer is different from the source code (it includes some debug var_dump).

Unit tests are useless, they only asserts what the mock return. The reviewer ask the OP to do integration tests.

The SDK lack specific error types and a huge security issue was discovered.

## Python

Local installation require root privileges.

Unit tests are useless, they only asserts what the mock return. The reviewer ask the OP to do integration tests.

The SDK lack specific error types and a huge security issue was discovered.

## Overall Impression of usage testing

The JS SDK build is OK.

The PHP SDK build is OK.

The Python SDK build is OK, **but it requires root permission not sure why**.

```sh
python3 setup.py install
running install
error: can't create or remove files in install directory

The following error occurred while trying to add or remove files in the
installation directory:

    [Errno 13] Permission denied: '/usr/local/lib/python3.9/dist-packages/test-easy-install-16630.write-test'

The installation directory you specified (via --install-dir, --prefix, or
the distutils default setting) was:

    /usr/local/lib/python3.9/dist-packages/

Perhaps your account does not have write access to this directory?  If the
installation directory is a system-owned directory, you may need to sign in
as the administrator or "root" account.  If you do not have administrative
access to this machine, you may wish to choose a different installation
directory, preferably one that is listed in your PYTHONPATH environment
variable.

For information on other options, you may wish to consult the
documentation at:

  https://setuptools.readthedocs.io/en/latest/easy_install.html

Please make the appropriate changes for your system and try again.
```

However, I asked the OP to improve the documentation over the whole review timeframe and they did.

Unfortunately, all sdk failed because of a security issue and the tests are useless because it only tests what the mock return.

I will only disclose the security issue to the Original CRDAO Members that wants to for security purpose. 

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

All tests passed on the 3 SDK. However, the tests can be improved by adding more tests & negative paths one especially.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

# Documentation

### Code Documentation

The code documentation is sufficient on all 3 sdk.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project documentation was improved a lot during the review. It still needs some improvement on the JS SDK & Python SDK.

The JS SDK readme lack the commands to install the dependencies before running the tests / build commands.

The python SDK local installation command require a root permission.

The PHP usage example for getting a single payment is missing the parameter.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL
Example Documented | FAIL 

## Overall Conclusion on Documentation

The 3 SDK are pretty simple however there was a lot of documentation issues that where resolved during the timeframe of the review.

There's still some documentation problems.

The documentation FAIL it still needs some improvements.

# Open Source Practices

## Licenses

Each SDK are released under Apache License 2.0 like stated in the grant.

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

The project documentations needs to be improved.
The code needs to implement specifics error types to improve the developer experience.
The tests need to be rewritten.
The security issue(s) needs to be fixed ASAP.

# Final Conclusion

The reviewer asked multiple time the OP to improve the documentation & error handling.
The OP fixed the most of the documentation in the different repos.
The reviewer started to test the examples of the JS SDK when he discovered a security issue hence failing the whole review.

The review status is a FAIL because of the useless tests / multiple fixes asked to the OP on a small project like this and the security issue. 

# Recommendation

Recommendation | FAIL
------------ | -------------
