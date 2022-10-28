Grant Proposal | [372 - 1-2-3-4 - Riak v3.x Packaging Enhancement Project](https://portal.devxdao.com/public-proposals/372)
------------ | -------------
Milestone | 1-2-3-4
Milestone Title | Create FreeBSD, OSX, SUSE and Alpine Linux Packaging Tools for Riak KV, CS and Stanchion - Submission 2
OP | Bob The Marauder
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

**This is a repost of CRDAO Job #131 under new circumstances.**

CRDAO Job #131 failed due to a licensing semantic. Per vote #637 (https://portal.devxdao.com/app/proposal/637) on the DEVxDAO, this particular licensing semantic has been waived for this job and this job specifically. Therefore, this job is being reposted for re-consideration under the new standards. The existing review is fine in content and the review should not need to be rerun.


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
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS


# Unit / Automated Testing

Note that, since OP does not have permission to modify the main repo, they are not able to push their tests to it. The decision on this is on DEVxDAO on their terms, while it fails the requirements expected by CRDAO. No unit tests or explanations about manual testing is available in the pull request provided.

Previous review of this job failed due to a licensing semantic. Per vote #637 (https://portal.devxdao.com/app/proposal/637) on the DEVxDAO, this particular licensing semantic has been waived for this job and this job specifically. Therefore, this job is being reposted for re-consideration under the new standards. The existing review is fine in content and the review should not need to be rerun.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes


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

No documentation exists for packaging. A user needs to know how to work with packaging to work on them. However, a Makefile is present that defines the way how the packages could be generated which is deemed sufficient for these milestones.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

No documentation exists for packaging. A user needs to know how to work with packaging to work on them.


# Open Source Practices

## Licenses

Repository for Riak KV is missing a license. This has been discussed in detail with the developer but further action cannot be taken.

Previous review of this job failed due to a licensing semantic. Per vote #637 (https://portal.devxdao.com/app/proposal/637) on the DEVxDAO, this particular licensing semantic has been waived for this job and this job specifically. Therefore, this job is being reposted for re-consideration under the new standards. The existing review is fine in content and the review should not need to be rerun.

Riak CS and Stanchion are licensed under Apache License-2.0.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

## Contribution Policies

All of the repositories that the pull request made into, namely Riak KV, Riak CS and Stanchion are missing both the SECURITY and CONTRIBUTING policies. This issue also has been discussed in detail with the OP but it could not be resolved. This is because OP is providing an open source code to the main repository, which they do not maintain. This should be regarded when making a decision by DEVxDAO since the OP has no control over the main repository.

Previous review of this job failed due to a licensing semantic. Per vote #637 (https://portal.devxdao.com/app/proposal/637) on the DEVxDAO, this particular licensing semantic has been waived for this job and this job specifically. Therefore, this job is being reposted for re-consideration under the new standards. The existing review is fine in content and the review should not need to be rerun.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project. Overall sufficient work is done.


# Final Conclusion

Since this is an open source pull request made into another repo, whose license status is not clear, some aspects of this review are not completely compatible with the expectations of CRDAO. Since the OP has no direct influence on the main repository, they cannot modify some parts of it, namely change the license, provide extra unit tests, and etc. However, DEVxDAO waived some requirements for this grant:

> Previous review of this job failed due to a licensing semantic. Per vote #637 (https://portal.devxdao.com/app/proposal/637) on the DEVxDAO, this particular licensing semantic has been waived for this job and this job specifically. Therefore, this job is being reposted for re-consideration under the new standards. The existing review is fine in content and the review should not need to be rerun.

This decision is effective. The project meets the acceptance criteria. Because of these, reviewer suggests this milestone to PASS with Notes.


# Recommendation

Recommendation | PASS with Notes
------------ | -------------
