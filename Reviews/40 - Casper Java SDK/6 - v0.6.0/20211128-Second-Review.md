Grant Proposal | [40 - Casper Java SDK](https://portal.devxdao.com/public-proposals/40)
------------ | -------------
Milestone | 6 (Resubmission)
Milestone Title | v0.6.0
OP | Carl Norburn <carl.norburn@gmail.com>
Reviewer | Muhammet Kara <muhammetk@gmail.com>
Date | 2021-11-28

# Introduction
This is the second submission of this milestone for code review. The first submission had failed due to not meeting the acceptance criteria. There were also some recommendations for improvement which were not necessarily causing a failure. OP has resubmitted the milestone for review again, asserting that the project has been amended to meet/exceed the acceptance criteria.

# Milestone Details
This is the final milestone of the grant, and the review will cover the entirety of the grant, including the deliverables of the previous milestones.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Optimised SDK with working unit and integration tests

**Deliverables of the previous milestones**

- Connect to the chain
- Basic queries:
- - getAccountBalance
- - getAccountHash*
- - getAccountInfo
- - getAccountMainPurseURef
- - getStateRootHash

- Connect to the chain with more advanced queries
- - getAuctionInfo
- - getNodePeers
- - getNodeStatus
- - getRPCSchema

- getBlock - latest, by height, by hash
- getDeploy - by hash
- general code tidy up
- documentation improvements

- setTransfer
- Post a transfer

- Deploy.toBytes
- Deploy.toJSON
- Deploy.fromBytes
- Deploy.fromJSON

**Acceptance criteria:**

- Client can connect to a node and issue queries.

- Client will be able to connect to a node & issue more complex queries.

- Client will be able to connect and query transfers on the chain.
- Optimisation on the code will have been started.

- Client will be able to connect to a node & submit a native transfer for processing.

- All Casper Labs types will have methods to serialize/de-serialize

- Optimised SDK with working unit and integration tests

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/casper-network/casper-java-sdk | 24da132

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/casper-network/casper-java-sdk, the reviewer was able to successfully install the library as a dependency on a Java project from the common central package repository of the language. The reviewer was also able to successfully build the source code for this milestone by using the build script at the root of the repository.

## Overall Impression of usage testing

The reviewer was able to successfully test the usage of the library by leveraging the usage samples in the source code, including connecting to and querying a Casper node, and submitting transactions to the network. It was observed that although the links to the usage examples on the project's README file were broken, and only 2 out of the listed 8 usage examples were actually implemented during the previous review, OP have improved the project by fixing the broken links and providing usage examples to cover all 8 cases.

The reviewer has observed that the following methods are now included in the repository, rendering the project complete in terms of the promised functionality through the deliverables listed in the milestones:
- getRPCSchema
- getBlock - latest, by height, by hash
- getDeploy - by hash


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Can connect to a Casper node | PASS

# Unit / Automated Testing

Project contains 190 unit tests that can be executed from the console whereas there were 190 unit tests in the previous submission. Tests cover both positive and negative test paths. The reviewer has observed that all tests run successfully without errors. The code-base also has 2 integration tests which are outside of the scope of this review, and thus skipped.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code documentation covers most of the code base, and the provided build script produces the documentation in an easily navigatable HTML format. The reviewer has also observed that the code-level documentation has been improved further by the OP since the previous submission, covering more classes and methods. The reviewer praises the OP for improving the documentation even further by following the reviewer's earlier recommendations.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

README.md had sufficient examples for the most basic use cases with minimal examples in the previous submission. The reviewer observed that the usage documentation has been improved with more details and implementing the rest of the listed examples on the README.md file. The reviewer again praises the OP for the great improvements in this regard compared to the previous submission.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

OP has greatly improved the documentation, following the recommendations on the previous review. The reviewer would like to thank the OP for his great job in this regard.

# Open Source Practices

## Licenses

The Project is released under the MIT License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. However, the project does not contain a CONTRIBUTING policy. The reviewer highly suggests that the OP should crown his nicely documented project by adding a proper contribution policy to provide guidelines for the potential contributors as it is crucial for the sustainability of an open-source project. However, this is not a reason to fail the whole submission, in the reviewer's opinion.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass. The project is also now functionally complete. It is also observed that the OP took the extra mile and provided more usage examples and code-level documentation even though those were not required. The reviewer would like to thank the OP for his hard work on this.

# Final Conclusion

The project now provides the functionality described in the grant application and milestone acceptance criteria. Thus, in the reviewer's opinion, this submission should pass.

# Recommendation

Recommendation | PASS
------------ | -------------
