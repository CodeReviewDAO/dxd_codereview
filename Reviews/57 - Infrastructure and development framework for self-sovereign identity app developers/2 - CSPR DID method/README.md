Grant Proposal | [57 - Infrastructure and development framework for self-sovereign identity app developers](https://portal.devxdao.com/public-proposals/57)
------------ | -------------
Milestone | 2
Milestone Title | Infrastructure and development framework for self-sovereign identity app developers
OP | sg/Credentia
Reviewer | David Tai

# Milestone Details
The review will cover the 2nd milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Develop an open source implementation of the `did:cspr` method. Method should support CRUD operation as did resolution into DID Document. Compatibility with the Universal Resolver open source project has to be implemented.

**Acceptance criteria:**

Functional deliverables:

1. DID Registry contract (Ref: https://github.com/uport-project/ethr-did-registry, https://github.com/ethereum/EIPs/issues/1056)
Delegates
Attributes
Revocation

2. DID Resolver (a driver for https://github.com/decentralized-identity/universal-resolver)
Verification method (“eth recovery” based) 

3. Basic DID SDK (ref: https://github.com/uport-project/ethr-did)
DID: Register operation. Offchain
DID: Update (Attributes, Delegates)
DID: Revoke

**Additional notes regarding submission from OP:**

Functional deliverables:
1. DID Registry contract (Ref: https://github.com/uport-project/ethr-did-registry, https://github.com/ethereum/EIPs/issues/1056) Delegates Attributes Revocation
2. DID Resolver (a driver for https://github.com/decentralized-identity/universal-resolver) Verification method (“eth recovery” based)
3. Basic DID SDK (ref: https://github.com/uport-project/ethr-did) DID: Register operation. Offchain DID: Update (Attributes, Delegates) DID: Revoke

https://github.com/credentia-network/

Milestone 2 submission includes:

1. DID smart contract for Casper Network
2. DID Resolver plugin
3. DID SDK (Veramo plugin)
4. Universal Resolver Driver for Casper DID method

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/credentia-network/VCRegistrytree/test1 | 5279d2c

# Install & Usage Testing Procedure and Findings

The reviewer followed the instructions on the README of the project to build the project, and run the automated tests, but it was observed that the README of the project lacks testing instructions but this has been communicated with the developer and is being addressed.  

The reviewer also documented an additional documentation repo that is linked from the README with deployment instructions:
https://github.com/credentia-network/Docs/blob/main/readme/casper-did-method-spec.md
https://github.com/credentia-network/Docs/blob/main/readme/smart-contract.md

Initially, the reviewer found the documentation out dated and not quite working.  The reviewer gave the OP feedback and it was corrected.  Unfortunately this project was completed a long time ago against the initial 1.1.1 version of Casper so it cannot be deployed to any of the test environments.  Thus, the reviewer requested automated testing against the 1.1.1 version of node using the v 1.1.1 version of the automated testing library instead of relying on scripts.

The reviewer then helped the OP develop the initial tests and provide examples of rust testing from the RengoLAbs/uniswap-for-casper repos.

The reviewer was eventually presented with integration tests representing the primary flows of:

1. Install Contract with Owner
2. Change the Owner of the Contract
3. Add/Revoke delegates
4. Add and Remove an attribute against an identity (account)
5. sendVPRequest
6. changeVPRequestStatus
7. changeVCRevocationFlag
8. issueDemoVC

These tests are able to pass against the 1.1.1 version of the node. 

[test](assets/test.md)

## Overall Impression of usage testing

Review was able to follow the instructions until deployment.  The project builds against v1.1.1.  However, this version is incompatible with v1.4.5 of the node and contracts will need to be updated.  

**As this milestone was completed in Q4 before the CRDAO but not submitted until late Q1 and the new review system was in place, the reviewer feels that certain exceptions are necessary for this particular project.**  The reviewer feels comfortable in passing this so long as upgrades are done to make it run on v1.4.5

Requirement | Finding
------------ | -------------
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | NA 

# Unit / Automated Testing

The reviewer observed that all of the tests successfully pass, but the project have **tests focusing only on the positive paths**. **The tests need to be improved to cover also the negative paths before the final milestone**.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

**The code-level documentation of the project has been observed to be extremely sparse** although which matches the reference implementation. Documentation is done as part of the protocol specification, rather than inline. In this regards, the actual documentation is very in depth.  **However, ideally the code-level documentation should be improved before the final milestone,** with comments for all code portions for the critical functionality.  This should be a relatively simple task of copying the specification documentation inline to each of the matching functions.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Project documentation is very detailed.  There is a full walkthrough from building to deployment and [usage of the application](https://github.com/credentia-network/Docs/blob/main/readme/smart-contract.md).  **However some links are currently broken due to refactoring of the repositories and must be fixed**.  **Testing instructions are also currently missing but uses the standard `make test`.**  These issues have been communicated to the OP who should resolve them before milestone 3.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are good and easy to understand and follow.  **However, there remain some glaring issues with broken links that should be fixed before milestone 3.**

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository.  Reviewer submitted issues that the OP responded to quickly.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and has successfully passing tests, focusing only on the positive paths.

# Final Conclusion

The reviewer has helped the OP to bring this grant to a point where the reviewer feels comfortable passing with a number of notes that need to be addressed in milestone 3, namely:

- Upgrade libraries to 1.4.3+
- Confirm documentation works for 1.4.3+
- Add a negative path for unit tests
- Add some minor project documentation omissions so the documentation is complete
- Inline project documentation

# Recommendation

Recommendation | PASS with Notes
------------ | -------------