Grant Proposal | [372 - 1 - Riak v3.x Packaging Enhancement Project](https://portal.devxdao.com/public-proposals/372)
------------ | -------------
Milestone | 1
Milestone Title | Create FreeBSD Packaging Tools for Riak KV, CS and Stanchion
OP | Bob The Marauder
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Updates to the code base that allow packages for Riak KV, Riak CS and Stanchion version 3 to be built that work on a modern version of FreeBSD.

**Acceptance criteria:**

* Most recent Riak KV version 3 package at that time builds successfully on FreeBSD.
* Most recent Riak CS version 3 package at that time builds successfully on FreeBSD.
* Most recent Stanchion version 3 package at that time builds successfully on FreeBSD.
* PR filed against Riak KV version 3 on Github to include FreeBSD packaging tools.
* PR filed against Riak CS version 3 on Github to include FreeBSD packaging tools.
* PR filed against Stanchion version 3 on Github to include FreeBSD packaging tools.
* FreeBSD packages publicly available from https://files.tiot.jp for Riak KV, Riak CS and Stanchion version 3.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/TI-Tokyo/riak_kv | 58b3fc2
https://github.com/TI-Tokyo/riak_cs | aa1c442
https://github.com/TI-Tokyo/stanchion | 438383f


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

_Summarize the code level documentation you encountered. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

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

_List which Open Source license is used and note anything that's non-standard. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS / FAIL / PASS with Notes

## Contribution Policies

_Confirm that the project contains a `CONTRIBUTING` and `SECURITY` policy, and optionally an associated `Code of Conduct` policy. Confirm
that Pull Requests and Issues are enabled on the repository and that generally the Project is set up for public participation. 
Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS / FAIL / PASS with Notes

# Coding Standards

## General Observations

_Provide any general observations about the project you want to add to your review. These can be subjective in nature as well, and do not
contribute to your recommendation to pass or fail the submission._

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
