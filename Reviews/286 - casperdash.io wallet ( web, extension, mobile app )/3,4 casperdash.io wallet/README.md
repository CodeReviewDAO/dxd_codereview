
Grant Proposal | [286-3:4 casperdash.io wallet ( web, extension, mobile app )](https://portal.devxdao.com/app/proposal/286)
------------ | -------------
Milestone | 3:4
Milestone Title | Casperdash Mobile Wallet (IOS, Android) - Submission 1
OP | Kien Nguyen
Reviewer | Huy Tran

# Milestone Details
The review will cover the 3 and 4 milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone 3:**

IOS application
   
**Acceptance criteria:**

We will release a stable version working on mainnet and the app will be available in Apple App store marketplace.
- Dashboard ( View CRPR balance, send/receive CRPR )
- Tokens (ERC20)
- History
- NFTs
- Stacking
- Integrate with Ledger

**Details of what will be delivered in milestone 4:**

Android application
   
**Acceptance criteria:**

We will release a stable version working on mainnet and the app will be available in Google App store marketplace.
- Dashboard ( View CRPR balance, send/receive CRPR )
- Tokens (ERC20)
- History
- NFTs
- Stacking
- Integrate with Ledger

## Milestone Submission

The following milestones assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/CasperDash/casperdash-mobile-wallet/tree/main | 7dd8c37

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of repository, there were some errors during the installation process due to incomplete documentation. After coordinating with OP, the document has been updated and installed successfully. The reviewer was able to successfully build the source code on MacOS 11.5.2.

[Build Logs iOS](assets/Logs/CasperDash_BuildIOSLog.md)

[Build Logs Android](assets/Logs/CasperDash_BuildAndroidLog.md)

## Overall Impression of usage testing

The documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Documentation provides sufficient installation/execution instructions | PASS
Project builds without errors | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with notes

More detail about functionality

Requirement | Finding
------------ | ------------
View CSPR balance  | PASS with notes
Send/Receive CRPR  | PASS
View tokens (ERC20) balance | PASS
Add custom token by contract hash | PASS
View transfer transactions history | PASS with notes
View NFTs | PASS
Stacking Operations |PASS with notes
Ledger Integration  | PASS

Notes:
- Dashboard ( View CRPR balance, send/receive CRPR ): In View mode, the interface should remove 2 buttons to receive and send because these 2 buttons cannot be used.
- History: need to add CSPR Receive history, Stake history
- Stacking: When entering amount, it is not convenient because the keyboard is automatically hidden after each number of typing

Tested the app on Iphone13 (iOS 15.4.1) and Samsung Galaxy A70 (Android 9). See more screenshots [here](assets/)

# Unit / Automated Testing

The project has unit tests for all critical classes and methods. The reviewer was able to run all tests successfully.

[Test Logs](assets/Logs/CasperDash_TestLog.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | FAIL

# Documentation

### Code Documentation

The project has sufficient code-level documentation with summaries and comments, especially on critical classes and methods.

Requirement | Finding
------------ | -------------
Code Documented | Pass

### Project Documentation

The reviewer observed that the project README has detailed general and usage documentation. The project README includes an architecture section that describes the project architecture and the project's components.
The Example Documented section, after being requested, the OP added.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

The project is well documented and the reviewer has observed that the project README has detailed general, roadmap, and usage documentation.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. The project contains a CONTRIBUTING and SECURITY policy. 

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

There are some redundant comments, after coordinating with the OP, the OP has removed them.
Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. However, there are still some points that need improvement as mentioned above about functionality.

Thus, in the reviewer's opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with notes
------------ | -------------
