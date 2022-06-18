Grant Proposal | [307 - 2:3 - Common blockchain security libraries for private key secure storage](https://portal.devxdao.com/public-proposals/307)
------------ | -------------
Milestone | 2 & 3
Milestone Title | Web library - Submission 1, React Native library - Submission 1
OP | Killian Hascoet <killianh@live.fr>
Reviewer | Gökhan Gurbetoğlu <ggurbet@gmail.com>


# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

### Milestone 2:

We will implement the architecture stated in milestone 1 deliverable with all methods, fully tested, released on github and npm.

### Milestone 3:

We will implement the architecture stated in milestone 1 deliverable with all methods, fully tested, released on github and npm.

**Acceptance criteria:**

### Milestone 2:

Release the source code on github & npm. Complies with the DoD (Proposal #196).

### Milestone 3:

Release the source code on github & npm. Complies with the DoD (Proposal #196).

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/CasperDash/casper-storage | c0ca883


# Install & Usage Testing Procedure and Findings

Following the instructions in the provided README, reviewer was able to successfully build the source code without errors for these milestones on a Pardus GNU/Linux 21.2 machine. All corresponding logs are listed below.

- [Build logs](assets/build.md)

## Overall Impression of usage testing

Documentation provides sufficient installation instructions. Reviewer easily set up the environment to build the project using these.

Reviewer was able to implement the critical methods of the library mentioned in the initial design document at https://github.com/CasperDash/casper-storage/blob/master/document/01-casper-storage-design.md using the provided code examples by the developer. Also, reviewer recommends developers to examine the tests which thoroughly cover all functionality with many use case scenarios that can help understand further functionality that is out of the scope of this review.

The critical methods meet the acceptance criteria for these milestones.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS


# Unit / Automated Testing

All automated unit tests PASS for these milestones. Testing is done via jest and contains automated tests that cover critical functionality. Reviewer successfully run all automated tests on a Pardus GNU/Linux 21.2 machine. Overall quality of tests are remarkably sufficient. Test output is below.

- [Unit tests output](assets/unit-tests.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS


# Documentation

### Code Documentation

Code documentation is very well prepared and is of high quality. All critical functionality of the code is commented. Many other helping comments and documentation are provided within the code and they are well prepared and detailed.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project has a very detailed documentation provided through TypeDoc. The generated documentation can be reached from the `/docs/` folder. There was two warnings while generating the documentation about the not included references which could be later added and does not affect the score of this assessment. The note about missing JavaScript core features file could also be on the local documentation instead of redirecting to the corresponding file on the GitHub repository.

The project also provides very detailed and well-prepared examples in its documentation. A developer would easily find their way implementing the source in their projects.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation is extensively detailed and has many additional parts that provide exceptional coverage of project's methods and usage.


# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING and SECURITY policies. Pull requests and Issues are enabled on the repository and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project. As a big bonus, developer added automated linting which increases the code quality. Overall exceptional work is done.


# Final Conclusion

Project provides the acceptance criteria for the milestones it cover. Unit tests are very well prepared and useful for both testing the library and for helping understand how different usage scenarios can be executed. Documentation is extensively detailed and has many additional parts that provide exceptional coverage of project's methods and usage. Coding practices used in the project are of skillful quality. Because of its sufficient deliverables, reviewers suggests the project to PASS.

# Recommendation

Recommendation | PASS
------------ | -------------
