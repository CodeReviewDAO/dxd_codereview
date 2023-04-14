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

Reviewer used an Ubuntu 22.04.2 LTS GitPod instance, an Ubuntu 20.04 GitHub Workspaces instance, a local Pardus 21.5 GNU/Linux local instance and finally a macOS system for doing this review.

Before starting the review, the project was missing many of its components. To fix those, reviewer tried to find a contact information about OP and found one of theirs email address in their GitHub profile and asked them to contact him to fix the issues. However, OP did not respond to that email. After some days, reviewer also created an issue on the repository asking them the same question and this time OP responded and got into contact to fix the issues.

Then, when asked, OP was not aware of what the review was for and did not recall submitting anything for review. After telling them what CRDAO does and who DEVxDAO is, OP stated that they did not know about them before contacting the reviewer and this project was submitted directly to Casper Network. Eventually, after discussions, they made changes to the repository to comply with the review requirements.

These types of communication problems can result in further problems in the review process. Reviewer suggests that we determine an official way to get in touch with the OP of the projects so that the reviews do not fail on simpler fixes.

## Overall Impression of usage testing

Reviewer first installed the prerequisites for the project on the GitPod instance then tried to run the build with the given instructions in the README. However, this does not yield any further results since running `make build-contract` always returned errors. After checking multiple times, reviewer changed to a GitHub Workspaces instance where all of the progress also halted at the build step. After that, trying the code on Pardus GNU/Linux and finally a macOS system did not end in a different state. Since in its current form the project does not properly build, it fails the requirements.

Documentation has sufficient installation instructions.

Since the build fails, there is no way to check if the functionality meets the acceptance criteria and operates without error.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL


# Unit / Automated Testing

Unit tests also met their demise since the build fails.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL


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

On the other hand, some parts of the code are stored as Gists on GitHub and do not have a license. Discussing this with OP did not result to a full conclusion and the code still stays as Gists instead of their own repositories. These does not comply with the requirements of the review.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

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

At the beginning of the review, there were many missing parts and communication problems that resulted in a train of failure points, which ultimately undermined the success of this review. While OP worked on many of the missing parts, it was not enough to make the project run correctly. While the improvements can fix the further underlying issues in the code, the long review process should come to an end and a decision should be made. Because of these reasons, reviewer decided that this review should FAIL.


# Recommendation

Recommendation | FAIL
------------ | -------------
