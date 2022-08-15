Grant Proposal | [317 - Integration of LetsGo Wallet with CasperLabs](https://portal.devxdao.com/public-proposals/317)
------------ | -------------
Milestone | 1
Milestone Title | White Labeling of LetsGo Wallet (Chat Platform) - Submission 2
OP | A1Labs
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Using the base code and concepts from the LetsGo Wallet, we will make a version which is to be used in all future developments (specifically the ones in this proposal). The chat platform will be capable of multiple message delivery, delivery of digital content (photos, videos, contact cards) as well as standard messages and templated messages. This system will be based on a multi-language capable system, allowing for additions of new languages as desired. The core will be able to use several messaging systems (included in other milestones in this project) leveraging APIs for message delivery, allowing for a broader scope to be contributed by the open-source community Casper has been supporting / developing.

We will deliver:
- Forked, open-source version of LetsGo Wallet. This version will include:
    - Multiple message delivery
    - Digital content delivery (photos, videos, contact cards)
    - Templated messaging
    - Multilingual (human language) support
    - Internationalization-ready infrastructure
    - API integrations with Price Servers (Coin Gecko, Coin Market Cap, FIAT Exchange Rate Services), IPFS Gateways Internal Block Server APIs, Internal Bitcoin Server API, Internal DIVI Server API
- Landing Page website and project information

**Acceptance criteria:**

The submitted code base is:
- Capable of preparing multiple messages to multiple users
- Capable of preparing multimedia digital content
- Capable of sending messages with programmable templates
- Has at least 3 human language translations
- Has a table of strings for internationalization at-will
- Has functioning API integrations with Price Servers (Coin Gecko, Coin Market Cap, FIAT Exchange Rate Services), IPFS Gateways, Internal Block Server APIs, Internal Bitcoin Server API, Internal DIVI Server API

Upon completion of this milestone, a code review will be requested pursuant to coding standards (https://portal.devxdao.com/app/proposal/185) and definition of done (https://portal.devxdao.com/app/proposal/196).

**Additional notes regarding submission from OP:**

As requested, the repository in GitHub is established as a private repository; therefore, users who would like to review the code will need to provide their GitHub username to LetsGo to be added and have access for review and comments. DevxDao will provide a list of GitHub usernames for access to the private repository.

Created CasperGo website (https://caspergo.io)

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/my-repository/my-project | 1111aaaa


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

Code is well documented. However, the quality of code comments are subpar. They are mostly single words or 

Requirement | Finding
------------ | -------------
Code Documented | PASS / FAIL / PASS with Notes

### Project Documentation

_Summarize the project level documentation you encountered. This covers the information provided in the README for the project, 
as well any exampled provided. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Usage Documented | PASS / FAIL / PASS with Notes
Example Documented | PASS / FAIL / PASS with Notes

## Overall Conclusion on Documentation

_Summarize your review of the documentation in this project, including code, usage and examples_

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

The project would benefit greatly from a Continuous Integration (CI) Action on GitHub.

Build process is tedious. A build script would make installation process automated and less prone to user errors.


# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_


# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
