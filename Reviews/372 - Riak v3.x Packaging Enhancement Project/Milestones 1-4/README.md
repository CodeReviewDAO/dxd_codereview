Grant Proposal | [372 - 1-2-3-4 - Riak v3.x Packaging Enhancement Project](https://portal.devxdao.com/public-proposals/372)
------------ | -------------
Milestone | 1
Milestone Title | Create FreeBSD, OSX, SUSE and Alpine Linux Packaging Tools for Riak KV, CS and Stanchion
OP | Bob The Marauder
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Updates to the code base that allow packages for Riak KV, Riak CS and Stanchion version 3 to be built that work on a modern version of FreeBSD.

**Acceptance criteria:**

* Most recent Riak KV version 3 package at that time builds successfully on FreeBSD, OSX, SUSE and Alpine Linux
* Most recent Riak CS version 3 package at that time builds successfully on FreeBSD, OSX, SUSE and Alpine Linux.
* Most recent Stanchion version 3 package at that time builds successfully on FreeBSD, OSX, SUSE and Alpine Linux.
* PR filed against Riak KV version 3 on Github to include FreeBSD, OSX, SUSE and Alpine Linux packaging tools.
* PR filed against Riak CS version 3 on Github to include FreeBSD, OSX, SUSE and Alpine Linux packaging tools.
* PR filed against Stanchion version 3 on Github to include FreeBSD, OSX, SUSE and Alpine Linux packaging tools.
* FreeBSD, OSX, SUSE and Alpine Linux packages publicly available from https://files.tiot.jp for Riak KV, Riak CS and Stanchion version 3.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/TI-Tokyo/riak_kv | 58b3fc2
https://github.com/TI-Tokyo/riak_cs | aa1c442
https://github.com/TI-Tokyo/stanchion | 438383f


# Install & Usage Testing Procedure and Findings

The installation of packages is not strictly mentioned in a doc and the user is expected to know how to make it themselves. The process is easy, however someone not familiar with software packaging would struggle to find their way.

## Overall Impression of usage testing

Packages are created successfully after running the relevant makefile for each operating system and their corresponding packaging system. OP also provides the packages on the https://files.tiot.jp website they mentioned at the time of the submission of the pull request.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | PASS


# Unit / Automated Testing

No unit tests or explanations about manual testing is available.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL


# Documentation

### Code Documentation

*This part of the review considers the pull requests made upon the main repo provided by the developer for FreeBSD, OSX, SUSE and Alpine operating systems.*

Code documentation is satisfying. All critical methods have been commented. There are also examples for usage inside the code as comments.

However, there are some extra code that is commented out and there are some irrelevant comments inside the code. Reviewer suggests removing these before pushing to production in future PRs.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

*This part of the review considers the pull requests made upon the main repo provided by the developer for FreeBSD, OSX, SUSE and Alpine operating systems.*

No documentation exists for packaging. A user needs to know how to work with packaging to work on them.

Requirement | Finding
------------ | -------------
Usage Documented | FAIL
Example Documented | FAIL

## Overall Conclusion on Documentation

No documentation exists for packaging. A user needs to know how to work with packaging to work on them.


# Open Source Practices

## Licenses

Repository for Riak KV is missing a license. This has been discussed in detail with the developer but further action cannot be taken. Since the nature of the review for a pull request, it has been deemed that this needs additional attention from OP. In its current state, the license requirement fails.

Riak CS and Stanchion are licensed under Apache License-2.0.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

## Contribution Policies

All of the repositories that the pull request made into, namely Riak KV, Riak CS and Stanchion are missing both the SECURITY and CONTRIBUTING policies. This issue also has been discussed in detail with the OP but it could not be resolved.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL


# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project. Overall sufficient work is done.


# Final Conclusion

Project does what it is supposed to do. However, most other aspects needed for this review are missing. There is no specific documentation, there are missing licenses, there is no mention of tests, and finally no work on contribution and security policies exist. Because of these shortcomings, reviewer suggests this project to FAIL.


# Recommendation

Recommendation | FAIL
------------ | -------------
