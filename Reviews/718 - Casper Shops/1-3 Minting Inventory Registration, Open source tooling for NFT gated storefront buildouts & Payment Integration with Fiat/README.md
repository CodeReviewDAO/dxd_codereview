Grant Proposal | [718 - Casper Shops](https://portal.devxdao.com/public-proposals/718)
------------ | -------------
Milestone | 1:3
Milestone Title | Payment Integration with Fiat (200 hours) - Submission 2
OP | droplinked
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Payment system integration via Stripe with CSPR<>Fiat converter

**Acceptance criteria:**

Live integration with CasperPunks Shop

**Additional notes regarding submission from OP:**

We've completed the full smart contract related to Casper Shops aside from paying with the Casper Token - this needs a peg to the USD but we are exploring options with our team.

Aside, we are working with the team at CasperPunks to deploy the front end of the shop UI that is turnkey with the Casper Wallet that enables token gating goods with customizable rulesets based on Casper initiated NFT's.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/FLATLAY/droplinked_casper | e11fdb8


# Install & Usage Testing Procedure and Findings

Reviewer used an Ubuntu 22.04.2 LTS GitPod instance for doing this review.

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

Main parts of the source code includes many descriptive comments but this is not the case for other source files. Also, current comments are a bit on the shorter side. Some polish is recommended for future updates.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

At the start of the review, only some basic comments about how to run the project were in the documentation. After discussing this with OP, they vastly improved the documentation and included many additional information that would be greatly beneficial for the users of the project.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation is sufficient for both the code and the project.

# Open Source Practices

## Licenses

At the start of the review, the project did not have any license file. On DEVxDAO Portal, only the license for research and documents are stated and they are to be a Creative Commons license. This issue was discussed with OP. They ended up licensing their source code with MIT License but this is not present in the original grant. This should be taken as a note for future reviews.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

## Contribution Policies

At the start of the review, contribution policies were missing from the repository. After discussing this with OP and guiding them on how to create those, the appropriate policies were created and other contribution components were enabled.

The project contains CONTRIBUTING and SECURITY policies. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Source code is well written, easily readable, and conforms to good coding practices overall.


# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_


# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
