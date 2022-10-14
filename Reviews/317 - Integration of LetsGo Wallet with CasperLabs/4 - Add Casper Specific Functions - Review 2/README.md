Grant Proposal | [317 - Integration of LetsGo Wallet with CasperLabs](https://portal.devxdao.com/public-proposals/317)
------------ | -------------
Milestone | 4
Milestone Title | Add Casper Specific Functions
OP | A1Labs
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Continuing the build of the system, this milestone will allow users to perform casper blockchain specific functions, including: Add / Manage Associated Keys, Set Action Thresholds, Casper Tokens (similar to the ERC20) (sending and receiving), Delegate Tokens (Staking), Undelegate Tokens (Unstake). This milestone may require assistance of the casper team to ensure its entirety at the time of development.

Existing open source code does not connect any of this to the system to give the bots ability to send / receive / generate keys, etc. That needs to be programmed for their coin into the bot system. We will be using some of their repos in this milestone, including the casper signer. However, we are not re-inventing the wheel, we are integrating those services with the bot to work in the same way as other coins

We will deliver:
- Add / Manage Associated Keys
- Set Action Threshods
- Casper Tokens (similar to the ERC20) (sending and receiving)
- Delegate Tokens (Staking)
- Undelegate Tokens (Unstake)

**Acceptance criteria:**

The milestone will be accepted when following will be implemented.

- User can generate new keys via BIP39 standard
- User can restore keys via BIP39 standard
- User can import existing keys from another format
- Website will verify appropriate keys
- Casper Signer integration to sign transactions

Upon completion of this milestone, a code review will be requested pursuant to coding standards (https://portal.devxdao.com/app/proposal/185) and definition of done (https://portal.devxdao.com/app/proposal/196) as well as an internal audit from Casper Labs

**Additional notes regarding submission from OP:**

- User can generate new keys via BIP39 standard
- User can restore keys via BIP39 standard
- User can import existing keys from another format
- Website will verify appropriate keys

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/CasperGoApp/CasperSpecificChainFunctions | f924c67

*Note:* This milestone was submitted as a separate repository and later merged into the main one.


# Install & Usage Testing Procedure and Findings

OP provided an installation environment on a remote server that uses Ubuntu 20.04.5 LTS for the reviewer. Together with OP, reviewer was successfully able to install the project according to the instructions provided in the README without errors. The installation instructions are very detailed but requirements are very long. Talking to OP, they stated that they are planning to move to an installation script in future milestones to ease this process.

![](assets/install-1.png)
![](assets/install-2.png)
![](assets/install-3.png)


## Overall Impression of usage testing

This project has many milestones. For this milestone, usage testing was achieved with unit tests. All test cases cover the acceptance criteria and there were no errors.

These tests should also be tested again manually after Milestone 5 as a note.

The project also allows sign in using Casper Signer and a website to verify appropriate keys. Reviewer was able to successfully sign in to the webpage, send some CSPR using the page and verify the keys. Here are some screenshots from these operations:

![](assets/casper-signer-connect.png)
![](assets/casper-signer-send.png)
![](assets/casper-signer-validation.png)
![](assets/transaction-sent.png)
![](assets/deployment.png)

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Unit tests cover all critical functionality required for this milestone's acceptance criteria.

- [Unit test logs](assets/unit-tests.md)

*Note:* Unit tests for this milestone has been put into the main repository and tests were done using those.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code is well documented. However, the quality of code comments are mediocre. They are mostly single words or for very obvious operations that can easily be understood by just looking at the code. These need improvements in the following milestones.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Installation documentation is well prepared and useful. Further documentation does not exist and needs to be implemented in future milestones.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

Code documentation needs improvements and project documentation needs to be added.

# Open Source Practices

## Licenses

The project is licensed under MIT license.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policies. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is well prepared and general best practices for implementation are used throughout the source code.


# Final Conclusion

The project would benefit greatly from a Continuous Integration (CI) Action on GitHub.

Build process is tedious. A build script would make installation process automated and less prone to user errors.

Code documentation is not of high quality and further project documentation is needed.

Because of these reasons, reviewer suggests a resolution of PASS with Notes for this milestone.


# Recommendation

Recommendation | PASS with Notes
------------ | -------------
