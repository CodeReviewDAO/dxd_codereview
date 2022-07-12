Grant Proposal | [57 - Infrastructure and development framework for self-sovereign identity app developers](https://portal.devxdao.com/public-proposals/57)
------------ | -------------
Milestone | 3
Milestone Title | Infrastructure and development framework for self-sovereign identity app developers
OP | sg/Credentia
Reviewer | David Tai

# Milestone Details
The review will cover the 3nd milestone criteria set forth below.

## Details & Acceptance Criteria

Develop a smart contract based system that allows to anchor Verifiable Credentials on the layer 1 protocol. Develop a publicly discoverable revocation registry.

**Details of what will be delivered in milestone:**

- VC timestamping service published on Github
- Revocation service deployed, tested and published on Github

**Acceptance criteria:**

This milestone consists of two main applications:

1. Demo Casper SSI Framework application: https://github.com/credentia-network/casper-ssi-demo

2. Verifiable Credentials registry (Casper-based timestamping service, revocation service): https://github.com/credentia-network/VCRegistry

The goal of demo application is to provide comprehensive showcase of the Casper SSI Framework in a form of demo web application.

Features include:
- Creation and management of DIDs
- Sign in in with Casper Signer
- Issuance of Verifiable Credentials (based on preset templates)
- Wallet for Verifiable Credentials for end user (diaply and management)
- Revocation of Verifiable Credentials by the issuer
- Requesting selective data from the end users by the Verifier
- Accepting and sharing Verifiable Credentials
- Viewing Credential data

DemoVCRegistry is a reference implementation of the VC registry contract that can be a backbone for decentralized document management system based on w3c VC specification. The contract implements registration of VCs, revoking and also a Verifiable Presentation request/response flow.

**Additional notes regarding submission from OP:**

https://github.com/credentia-network/

Documentation for VC SDK, smart contracts and demo application can be found here: https://github.com/credentia-network/Docs

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/credentia-network/casper-ssi-demo | 16c9145

# Install & Usage Testing Procedure and Findings

The reviewer followed the instructions on the README of the project to build and run the project, and run the example application and go through all the flows.  Documentation is detailed with many images of each flow.

The reviewer was able to run the example application following the instructions.  The reviewer ran into a few issues with the example application, namely that the reviewer didn't read the documentation very well and the error catching on the example does not validate DIDs.

After getting this issue resolved, the reviewer was able to view and execute the issuing process, the holder approval process, and the verification by the issuer process.  The website is relatively simple and easy to use.

The React/Typescript code is built idiomatically and is very readable for someone with experience in React/Typescript even without inline comments.  The project was constructed using a standard react-scripts template.

## Overall Impression of usage testing

Review was able to follow the instructions to verify behavior.  A video of the process is attached. 

**As this milestone was completed in Q4 before the CRDAO but not submitted until late Q1 and the new review system was in place, the reviewer feels that certain exceptions are necessary for this particular project.**  The reviewer feels comfortable in passing this.  Previous requirement to upgrade to 1.4.5 for the smart contracts were performed.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The website does not have unit tests as it is an example site.  However, manual testing instructions are clear and concise and easy to test (5-10 minutes) with some familiarity.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A

# Documentation

### Code Documentation

Code-level documentation does not exist.  However everything is done idiomatically so its very simple to understand what is doing what and where all the components are located in.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project is well documented with clear and concise instructions.  Images and other visual aids are provided.  A large body of documetnation exists for the entire project and is located in its own repository.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS


## Overall Conclusion on Documentation

In the reviewer's opinion, despite missing inline documentation, the project is easily understandable and conforms to conventions common in the open source space for a Typescript/React project.

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository.  Reviewer submitted issues that the OP responded to quickly to in the past.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is well-structured and readable. The project has been committed to GitHub.  React components have been abstracted well and broken up into reuseable primitives.  The purpose of this project is to serve as an example/starter for DID applications and this repository seems sufficient to fulfill that role.

# Final Conclusion

This example application is functional, simple, and had some well documented high level documentation.  Taken together wholistically with the rest of the code base which is also well documented, reviewer recommends a pass.

# Recommendation

Recommendation | PASS
------------ | -------------