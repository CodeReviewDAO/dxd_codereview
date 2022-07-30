Grant Proposal | [86 - CSPR Metrics API and Historical Archive for Services, Daps and Analytics](https://portal.devxdao.com/app/proposal/86)
------------ | -------------
Milestone | 3
Milestone Title | Documentation, tests and improvements
OP | Daniel Halford
Reviewer | Furkan Ahmet Kara <furkanahmetkara.fk@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

As we have a clear picture how to collect and serve the metrics data, this milestone is important to ensure that system delivers correct results, includes all aspects and ready for production use. The following step includes the following.

**Acceptance criteria:**

- Check generated metrics in various ways to ensure it’s always accurate;
- Create technical documentation on the project;
- Create user documentation, explaining how to use API;
- Create unit and e2e tests to make sure no parts have errors;
- Add or alter the endpoints as requested by the community. This may include new metrics to track or more filters to add;
- Improve and validate caching mechanisms to ensure create performance;
- Add more graphs, and ability to change dates and parameters when drawing them;
- Investigate and validate all differences that other tools or available metrics may return;_

**Additional notes regarding submission from OP:**

No additional notes were added.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/a3mc/Casper-Metrics | 210c662


# Install & Usage Testing Procedure and Findings

Reviewer was able to install and run the project by following [installation instructions](https://github.com/a3mc/Casper-Metrics/blob/master/docs/INSTALLATION.md) which are served under the project documentation. Also, project has usage examples and easy to use. 

## Overall Impression of usage testing

Installation and execution documentation is well prepared, easy to understand and provides sufficient intructions. Reviewer was able to build and run the project by following the documentation. Reviewer thinks that usage testing meets acceptance criteria requirements and it also run without any errors.  

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# End-to-End & Unit Testing

E2E test results are documented under the [reports folder](https://github.com/a3mc/Casper-Metrics/tree/master/e2e/Reports) and Unit tests are written and can be found under [tests folder](https://github.com/a3mc/Casper-Metrics/tree/master/src/__tests__).

Reviever observed that e2e tests were detailed and well documented and controls such as integer control, requirements control, timestamp validation control, era validation control, confirmation control, and filter control were added.
Also, unit tests for each module were written with positive and negative paths.


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS
End-to-end tests | PASS
# Documentation

### Code Documentation

Codes are generally well documented and commented. Low-level code documentation is good enough to meet CRDAO code revview standarts and allow auto-generation of the documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The reviewer notes that the project provides comprehensive usage instructions with examples, along with installation, build, and test instructions, and that the materials are organized clearly.

Project documentation could be found in the [docs folder](https://github.com/a3mc/Casper-Metrics/tree/master/docs) of project.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings documentation is detailed and well prepared so this review should pass.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project can be quickly set up using the documentation which can be found in Github repository of the project which also has usage instructions. Also, project is already live and can be tested/used by visiting [website of the project](https://caspermetrics.io). 

# Final Conclusion

Project is well structured and documented in detail along with usage and intallation instructions. Low-level code documentation is well enough. Project meets the requirements stated in milestone acceptance criteria. Also, Project has well enough e2e tests and unit tests. As project documentation is well structured, code level documentation is sufficient enough and accptance criteria requirements are met, reviever thinks that this submission should pass.

# Recommendation

Recommendation | PASS
------------ | -------------
