Grant Proposal | [354 - 1.4.2 Upgrades to Uniswap](https://portal.devxdao.com/public-proposals/354)
------------ | -------------
Milestone | 2
Milestone Title | Test Upgrades
OP | david
Reviewer | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Tests will be upgraded using the new test runner and architecture where applicable.

A 5000 advance payment is requested for this.

**Acceptance criteria:**

Smart contract tests will be upgraded to use the new test runner features and we will add tests that can (finally) verify return values for inter-contract communications.

**Additional notes regarding submission from OP:**

These are now using:

casper-contract = "1.4.4"
casper-engine-test-support = "2.2.0"
casper-execution-engine = "2.0.0"
casper-types = "1.5.0"
casper-hashing = "1.4.3"

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core | 651bb08
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router | 838ec27

# Install & Usage Testing Procedure and Findings

By following the instructions in both READMEs reviewer tried to build projects but encountered some typos, which caused the build to fail, but the reviewer manually fixed them and built both projects, and informed OP about them.

### `CasperLabs-UniswapV2-Core`

In the [README](https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core) following line has a typo that needs to be fixed:

"sudo apt-key add casper-repo-pubkey.ascr", "r" at the end of the command should be removed.

### `CasperLabs-UniswapV2-Router`

In the [README](https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router) following line has a typo that needs to be fixed:

"sudo apt-key add casper-repo-pubkey.ascr", "r" at the end of the command should be removed.

In addition to the typo in install instructions, there is a typo that needs to be fixed in [Makefile](https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router/blob/main/Makefile). In the first line of Makefile, the Core repo path has an upper-lower case typo; otherwise, the build gives errors. The typo can be fixed as follows:

"uniswap_core_directory = ../CasperLabs-UniswapV2-core"  -> "uniswap_core_directory = ../CasperLabs-UniswapV2-Core"

## Overall Impression of usage testing

### `CasperLabs-UniswapV2-Core`

After fixing typos mentioned by the reviewer, the reviewer was able to build the project. The reviewer contacted the OP, and the OP will fix those typos. In the reviewer's opinion, this part should Pass with Notes because after fixing the minor typos, this repository meets the acceptance criteria and builds successfully. Here are the logs for "make build" and "make test" commands: 

[CoreBuildLogs](assets/corebuildlogs.md)
[CoreTestLogs](assets/coretestlogs.md)

Requirement | Finding
------------ | -------------
Project builds without errors | PASS WITH NOTES
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS WITH NOTES

### `CasperLabs-UniswapV2-Router`

After fixing typos mentioned by the reviewer, the reviewer was able to build the project. The reviewer contacted the OP, and the OP will fix those typos, but after the building reviewer encountered errors while issuing the "make test" command to run tests. This is a test milestone and the final milestone of the project, so tests should run successfully as a part of the acceptance criteria. In the reviewer's opinion, this part should FAIL because after fixing the minor typos, the reviewer managed to build the project but encountered errors while running tests, so this repository does not meet acceptance criteria. Here are the logs for "make build" and "make test" commands:

[RouterBuildLogs](assets/routerbuildlogs.md)
[RouterTestLogs](assets/routertestlogs.md)

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

### `CasperLabs-UniswapV2-Core`

The project has unit tests for all critical classes and methods. [CI Actions](https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core/actions/runs/2741059743/jobs/4296943773) was active on the GitHub repository. The reviewer checked the tests in CI Actions, and they were executed on without errors. The reviewer ran tests manually by following the instructions on the README of the project, and they were completed successfully too. Here is the test logs:

[CoreTestLogs](assets/coretestlogs.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

### `CasperLabs-UniswapV2-Router`

The project has unit tests written for all critical classes and methods. CI Actions was not active on the GitHub repository. Reviewer ran tests manually by following the instructions on the README of the project and encountered multiple "error[E0308]: mismatched types" errors. Even though the repository has tests, they don't run successfully, so in the reviewer's opinion, this part should fail. Here is the test logs:

[RouterTestLogs](assets/routertestlogs.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

# Documentation

### Code Documentation

The code has a sufficient amount of inline comments and low-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

### `CasperLabs-UniswapV2-Core`

The README file provides the necessary information to overview the project quickly. The README has a sufficient amount of instructions usage documentation overall.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

### `CasperLabs-UniswapV2-Router`

The README file provides the necessary information to overview the project quickly. The README has a sufficient amount of instructions usage documentation overall.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

In the reviewer's opinion, the typos in the install instructions documentation for the project is sufficient for this milestone.

# Open Source Practices

## Licenses

### `CasperLabs-UniswapV2-Core`

The Project is released under the GNU General Public License v3.0.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

### `CasperLabs-UniswapV2-Router`

The Project is released under the GNU General Public License v3.0.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Both of the projects contain a CONTRIBUTING and SECURITY policy that links to a Code of Conduct. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The code is well written and has a sufficient amount of comments as general on both repositories.

### `CasperLabs-UniswapV2-Core`

This part of the project meets the acceptance criteria. Code repo is available, test scripts have been written and included in the repository, and CI Actions are active. Source code is well written and has a sufficient amount of code-level documentation. The reviewer reported a minor typo that needs to be fixed, and after that, there will be no issues with this repository.

### `CasperLabs-UniswapV2-Router`

This part of the project does not meet the acceptance criteria. The code repository is available, and test scripts have been written and included in the repository, but the tests can't be executed without errors. Source code is well written and has a sufficient amount of code-level documentation. The reviewer reported a minor typo that needs to be fixed, and after that, there will be no issues with this repository.

# Final Conclusion

The reviewer recommends that this submission should FAIL as it fails to execute tests on one of the repositories. This is the final milestone of the proposal, and this milestone is related to tests, and tests should run without errors as a part of acceptance criteria too.

# Recommendation

Recommendation | FAIL
------------ | -------------
