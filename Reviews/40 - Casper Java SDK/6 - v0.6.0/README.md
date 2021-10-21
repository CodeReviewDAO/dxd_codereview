Grant Proposal | [40 - Casper Java SDK](https://portal.devxdao.com/public-proposals/40)
------------ | -------------
Milestone | 6
Milestone Title | v0.6.0
OP | Carl Norburn <carl.norburn@gmail.com>
Reviewer | Muhammet Kara <muhammetk@gmail.com>

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
https://github.com/casper-network/casper-java-sdk | 1179598

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/casper-network/casper-java-sdk, the reviewer was able to successfully install the library as a dependency on a Java project from the common central package repository of the language. The reviewer was also able to successfully build the source code for this milestone by using the build script at the root of the repository.

## Overall Impression of usage testing

The reviewer was able to successfully test the usage of the library by leveraging the usage samples in the source code, including connecting to and querying a Casper node, and submitting transactions to the network. However, it was observed that the links to the usage examples on the project's README file were broken, and only 2 out of the listed 8 usage examples were actually implemented.

The reviewer could not test the following methods because they were not found in the code-base, rendering the project incomplete in terms of the promised functionality through the deliverables listed in the milestones:
- getRPCSchema
- getBlock - latest, by height, by hash
- getDeploy - by hash


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL
Can connect to a Casper node | PASS

# Unit / Automated Testing

Project contains 190 unit tests that can be executed from the console. Tests cover both positive and negative test paths. The reviewer has observed that all tests run successfully without errors. The code-base also has 3 integration tests which are outside of the scope of this review, and thus skipped.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code documentation covers most of the code base, and the provided build script produces the documentation in an easily navigatable HTML format. However it was seen that some of the classes and critical methods were missing the code-level documentation although they were well-named, hinting their purposes. The reviewer suggests improving the documentation even further by covering the remaining parts with short and explanatory comments.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

README.md has sufficient examples for the most basic use cases with minimal examples. The reviewer suggests improving the usage documentation with more details and implementing the rest of the listed examples on the README.md file.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

There are certain improvements recommended. However, in the opinion of this Reviewer none are of the severity that they would require a FAIL of this submission.

# Open Source Practices

## Licenses

The Project is released under the MIT License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. However, the project does not contain a CONTRIBUTING policy. It is hughly suggested that the OP should add a proper contribution policy to provide guidelines for teh potential contributors as it is crucial for the sustainability of an open-source project. However, this is not a reason to the fail the submission, in the reviewer's opinion.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass. However, the project is missing certain functionality, rendering it incomplete.

# Final Conclusion

The project does not provide the functionality described in the grant application and milestone acceptance criteria. Thus, in the reviewer's opinion, this submission should fail.

# Recommendation

Recommendation | FAIL
------------ | -------------
