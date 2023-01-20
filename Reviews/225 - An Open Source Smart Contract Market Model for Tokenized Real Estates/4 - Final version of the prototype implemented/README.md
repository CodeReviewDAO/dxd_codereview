Grant Proposal | [225 - An Open Source Smart Contract Market Model for Tokenized Real Estates](https://portal.devxdao.com/public-proposals/225)
------------ | -------------
Milestone | 4
Milestone Title | Final version of the prototype implemented
OP | Vincent Peikert 
Reviewer | Furkan Ahmet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The model is intensively challenged and refined with key stakeholders of the market model (e.g., banks, real estate companies, different investor classes). For this task we will work together with existing clients of ours in Switzerland (in particular with those who showed interest in using the results of this project).
Legal stress test on the overall system and processes developed, in order to ensure compliance with financial regulatory legislation and KYC/AML related matters. For this task will work together with specialized law firms providing tokenization stress testing frameworks.
Elements of digital on-boarding solutions, which follow global regulatory standards in compliance with FATF, FINMA, FCA, CySEC, MAS for data protection, KYB/KYC and AML/CTF etc. incorporated.

**Acceptance criteria:**

The model is intensively challenged and refined with key stakeholders of the market model (e.g., banks, real estate companies, different investor classes). For this task we will work together with existing clients of ours in Switzerland (in particular with those who showed interest in using the results of this project).
Legal stress test on the overall system and processes developed, in order to ensure compliance with financial regulatory legislation and KYC/AML related matters. For this task will work together with specialized law firms providing tokenization stress testing frameworks.
Elements of digital on-boarding solutions, which follow global regulatory standards in compliance with FATF, FINMA, FCA, CySEC, MAS for data protection, KYB/KYC and AML/CTF etc. incorporated.

**Additional notes regarding submission from OP:**

https://github.com/NoumenaDigital/devxdao-m3/commit/1baa595f2b7ae90aefe164a4a3c85a6e2c5a4b47

OP Milestone Submission Notes
With the above linked GitHub repository we submit Milestone 4.

Since Milestone 4 contains some documentation with regards to the legal considerations of a Tokenized Real Estate Marketplace and only 2 minor corrections to the code, it has been submitted within the repository of Milestone 3. 

The Markdown file (milestone4-legalConsiderations.md) and the PDF (Milestone 4 - Legal Considerations) provide a comprehensive analysis of the legal considerations to be considered when creating a Tokenized Real Estate Market Place.

The Code changes restrict the platform from whitelisting investor accounts, since this should only be possible by the bank.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/NoumenaDigital/devxdao-m3 | effd42f

# Install & Usage Testing Procedure and Findings

Following the instructions in the [README](https://github.com/NoumenaDigital/devxdao-m3) of the project, the reviewer was able to successfully build the project along with it's dependencies, and run the tests for this milestone on Ubuntu 20.04.

[Build Logs](assets/buildlog.md)

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions. The project functionality meets/exceeds the acceptance criteria and operates without errors. Usage instructions and provided demos are sufficient and clear.

Requirement | Finding
------------ | -------------
The project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has sufficient amount of tests, covering both positive and negative paths. All tests run successfully. GitHub Actions is active.

[Test Logs](assets/testlog.md)
[Actions](https://github.com/NoumenaDigital/devxdao-m3/actions/runs/3854781550/jobs/6569137528)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code has good amount of low-level documentation but it can be improved by adding more details.

Requirement | Finding
------------ | -------------
Low-level function documentation | PASS with Notes

### Project Documentation

The project has sufficient documentation coverage for usage with examples, along with the installation, build and test instructions. README of the project has links to demos for the project.

Files regarding Milestone #4 can be found under [doc](https://github.com/NoumenaDigital/devxdao-m3/tree/master/doc/m4Documentation) folder.

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS

# Open Source Practices

## Licenses

The project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open-source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. The project also has CONTRIBUTING and SECURITY policies.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project published publicly on GitHub. Project documentation is sufficient enough as general. Unit test coverage is good enough, and all test run successfully.

# Final Conclusion

The project meets the milestone acceptance criteria. Install and usage instructions are sufficient. Tests run successfully.

Thus, in the reviewer's opinion, this submission should PASS.

# Recommendation

Recommendation | PASS
------------ | -------------

