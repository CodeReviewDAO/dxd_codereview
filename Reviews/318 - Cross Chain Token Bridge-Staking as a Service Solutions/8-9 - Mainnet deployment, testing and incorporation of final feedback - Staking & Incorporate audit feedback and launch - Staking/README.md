Grant Proposal | [318 - Cross Chain Token Bridge/Staking as a Service Solutions](https://portal.devxdao.com/public-proposals/318)
------------ | -------------
Milestone | 8:9
Milestone Titles | Mainnet deployment, testing and incorporation of final feedback - Staking & Incorporate audit feedback and launch - Staking
OP | Nick Odio - EVP of Growth at Ferrum Network
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

## Details & Acceptance Criteria

### Milestone 8

**Details of what will be delivered in milestone:**

- Deploy staking on mainnet
- Incorporate audit feedback if audit is completed
- Conduct internal testing
- Share the staking mainnet deployment with DEVxDAO and incorporate the final feedback

**Acceptance criteria:**

- Smart Contract Deployment for traditional staking
- Casper compatible wallet integration
    1. Ability to proceed through staking flow as described below:
    2. Ability to deploy the pool.
    3. Ability to set and test staking Periods
    4. Ability to set mandatory lock and early withdrawal
    5. Ability to set and test reward redistribution of Early Withdrawal
    6. Ability to set and test rewards distribution for full maturity
- DEVxDAO signs off on mainnet testing

**Additional notes regarding submission from OP:**

https://mail.google.com/mail/u/0?ui=2&ik=f20012be9d&attid=0.2&permmsgid=msg-a:r7591766417104732950&view=att&disp=safe&realattid=f_lkh0pgph1

https://casper-staking-mainnet.netlify.app/

### Milestone 9

**Details of what will be delivered in milestone:**

- Incorporate final audit feedback
- Launching the traditional staking pool on production mainnet

**Acceptance criteria:**

- Sign-off on audit completion
- Launch on production mainnet
- Staking pool is live for users to stake

**Additional notes regarding submission from OP:**

https://mail.google.com/mail/u/0?ui=2&ik=f20012be9d&attid=0.2&permmsgid=msg-a:r7591766417104732950&view=att&disp=safe&realattid=f_lkh0pgph1

https://casper-staking-mainnet.netlify.app/

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/ferrumnet/casper_staking | 32d8e45


# Install & Usage Testing Procedure and Findings

Reviewer used an Ubuntu 22.04.2 LTS cloud instance on GitPod for this review.

Reviewer used the instructions in the `README` to successfully deploy the staking smart contract under `staking_contract` directory. There is also a brilliantly prepared GitHub workflow that automatically builds and deploys the app.

- [Build logs](assets/build.md)
- [GitHub Workflow Logs](assets/workflow.md)

After the installation, reviewer checked the acceptance criteria on the live server provided by OP.

The ability to deploy was checked with a developer. The configurations were updated and valid deploys were created without any problems. Below is a link to a deploy created during these tests:

- [Local deploy](https://cspr.live/deploy/ab1d448f51907dc63c71962dd842e77b219fcff61f4f8900a8f1bf7ccd32f3b5)

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | PASS / FAIL / PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes

# Unit / Automated Testing

Project has enough test cases that cover the critical functionality required for this milestone. There were some package dependencies for the test cases that were deprecated and would have caused security issues. Reviewer informed OP about this issue and they promptly updated their dependency lists and removed the problematic packages without breaking the tests.
It should also be added that, there are some minor warnings that can be updated for better compatibility and to prevent possible problems that can arise in the future. In its current state, unit tests are sufficient.

- [Unit Tests Logs](assets/test.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes


# Documentation

### Code Documentation

The code documentation exhibits a high level of quality and thoroughness, having been carefully prepared to offer comprehensive coverage of the entire codebase. Critical code functionality is properly covered with comments, making it easier for developers to comprehend and manage the code effectively.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

At the start of the review, there were no `README` file present in the root of the repository. After telling this issue to the developers, it is stated that the instructions are inside the `staking_contract` directory. Developers then moved this file into the root of the repository.

In its current state, project documentation is sufficient and provides adequate instructions and information

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Both code documentation and project documentation is sufficient. There are quite useful code comments for describing the corresponding methods. Project documentation provides satisfactory content to set up and deploy the project properly.


# Open Source Practices

## Licenses

The project is released under MIT license.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING, SECURITY and CODE OF CONDUCT policies. Pull requests and Issues are enabled on the repositories and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project.

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
