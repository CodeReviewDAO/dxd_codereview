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

Reviewer used an Ubuntu 22.04.2 LTS GitPod instance, an Ubuntu 20.04 GitHub Workspaces instance, a local Pardus 21.5 GNU/Linux local instance and a macOS Ventura 13.1.1 system for doing this review.

Before starting the review, the project was missing many of its components. To fix those, reviewer tried to find a contact information about OP and found one of their email address in their GitHub profile and asked them to contact him to fix the issues. However, OP did not respond to that email. After some days, reviewer also created an issue on the repository asking them the same question and this time OP responded and got into contact to fix the issues.

Then, when asked, OP was not aware of what the review was for and did not recall submitting anything for review. After telling them what CRDAO does and who DEVxDAO is, OP stated that they did not know about them before contacting the reviewer and this project was submitted directly to Casper Network. Eventually, after discussions, they made changes to the repository to comply with the review requirements.

These types of communication problems can result in further problems in the review process.

## Overall Impression of usage testing

Reviewer first installed the prerequisites for the project on the GitPod instance then tried to run the build with the given instructions in the README. However, this does not yield any further results since running `make build-contract` always returned errors. After checking multiple times, reviewer changed to a GitHub Workspaces instance where all of the progress also halted at the build step. After that, trying the code on Pardus GNU/Linux and finally a macOS system did not end in a different state.

After working around the code and build scripts, reviewer understood the problem was laying under the missing `wasm32-unknown-unknown` target. Reviewer then manually installed the target using the `rustup target add wasm32-unknown-unknown` command and ran the make script again which resulted in a successful build. This information needs to be added to the build instructions.

- [Build logs](assets/build.md)

Documentation has sufficient installation instructions.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS


# Unit / Automated Testing

Unit tests are present and sufficiently cover the functionality required by the acceptance criteria.

- [Unit tests logs](assets/unittests.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS


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

On the other hand, some parts of the code are stored as Gists on GitHub and do not have a license. These were not submitted in the grant review and was provided to reviewer by the OP. Discussing this with OP did not result to a full conclusion and the code still stays as Gists instead of their own repositories. It is not clear that whether these files should be incorporated into the main repository or stay as their own. Since the OP has valid justifications for this, the issue should further be addressed by DEVxDAO.

Additional code provided as Gists by OP can be reached at these links:
- https://gist.github.com/k3rn3lpanicc/af78301897a513a70b61de3cf6ad37ac
- https://gist.github.com/k3rn3lpanicc/976f048998865659f531a127e3c4fa43

In its current state, reviewer gives the resolution of PASS with Notes.

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

At the beginning of the review, there were many missing parts and communication problems that resulted in a train of failure points. Reviewer assisted OP on working on these missing parts and eventually the project came to a desirable state for a review standpoint. Some licensing issues needs attention for the source code.

Because of these reasons, reviewer suggests a resolution of PASS with Notes.


# Recommendation

Recommendation | PASS with Notes
------------ | -------------
