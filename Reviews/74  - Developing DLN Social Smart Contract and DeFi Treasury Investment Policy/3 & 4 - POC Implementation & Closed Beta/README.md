Grant Proposal | [74 - Developing DLN Social Smart Contract and DeFi Treasury Investment Policy](https://portal.devxdao.com/public-proposals/74)
------------ | -------------
Milestone | 3 & 4 
Milestone Title | POC Implementation & Closed Beta
OP | Dr. Adel
Reviewer | David Tai <dtaipublic@gmail.com>

# Milestone Details

3. Specific to organizations who have signed LOIs:	Dhosa Chandaneswar Bratyajana Samity, Afghanistan Women Council, HELP SL
To map the internal workflow into a usable system	
To help onboarding	
For each selected entity, an acceptance test will be completed

OP Milestone Submission URL
https://www.unlock-bc.com/81513/blockchain-alphafin-implements-project-for-micro-financing-in-india/

OP Milestone Submission Notes
The implementation for the customization required by DCBS (https://dcbs.in/), including:
Login capabilities
Help options
Bengali language translation
Contact customization
Linking proposal

4. To deploy to their users
Scale up the frontend and add CDN network, load balancers

Based on the success of the previous POC users
Create the material required for the onboarding including local translations
Execute on getting the proposals, funding and payment
complete the repayment and distribution of rewards

## Details & Acceptance Criteria

3. Fully functional POC accepted by the partner

4. A full report per each partner POC will be generated 
Successful users

**Details of what will be delivered in milestone:**

The reviewer asked the OP and discussed what exactly the testing procedure for milestone 3 was and discovered that the reviewer had material for both milestones 3 & 4.

Materials included:
- POC sign off
- DLN Manual
- DLN POC & Production Website
- DLN Press Release
- Video Walkthrough/Tutorial
- Evidence of User Testing
- dlndao.org/start repository

Thus it was decided to do both milestone 3 and 4 together with the sign off of the DxD Program Management office when OP pointed out that the production front-end code had been merged into the POC main repository for milestone 4.

**Acceptance criteria:**

Acceptance criteria are the partner sign offs, the DLN tutorial material, and code base.  The scope of the CRDAO only includes the codebase.

**Additional notes regarding submission from OP:**

The reviewer has attached relevant materials for the code review (manual & video walkthrough) and a signed attestation that a third-party entity (DCBS) was able to use the platform and that it met their expectations.

## Milestone Submission

The following milestone assets/artifacts were submitted for review in addition to the materials attached:

Repository | Revision Reviewed
------------ | -------------
https://github.com/dlndao/start/ | 7700b2e

# Install & Usage Testing Procedure and Findings

The installation process is standard for a React + Typescript + node.js application.  The only remarkable thing about the installation process was that `nvm` was required to get it to work becasue it is specifically targeted at version 14 LTS.

This to be expected as the latest node.js LTS that is supported in the targetted runtime is 14 and more modern runtimes would cause backwards comaptibility issues.

The code was completely documented on a function level though there's no overall technical documentation and the function level documentation is rather spartan and could be expanded upon.

For testing, the reviewer deployed a local version, manually reviewed the AWS deployment artifacts and checked if they were typical, and reviewed the deployed instance to replicate the flows described in the video and manual.  The local version built but could not deploy without the AWS environment. 

```
Module not found: Can't resolve './aws-exports' in '/mnt/b/projects/start/src'
```

While its pretty simple to deploy a node.js AWS service and AWS amplify backend service, the documentation was lacking.  However, the AWS deployment artifacts were unremarkable and followed standard AWS conventions so will pass with notes asking for explicit AWS deployment instructions.

The production deployment had features that worked as expected with the casper signer and verified on chain.

## Overall Impression of usage testing

Usage testing involved running through manual testing scripts.  The reviewer did not find any functional issues with the testing scripts.  The reviewer does note that there are some english text sill visible with the Bengali translation.  The reviewer does not have the expertise to judge whether or not having mixed English and Bengali text is considered sufficient translation in that particular region.

Requirement | Finding
------------ | -------------
Project builds and runs without errors | PASS with notes (include AWS deploy docs)
Documentation provides sufficient installation/execution instructions | PASS with notes (include AWS deploy docs, works in AWS but not locally)
Bengali Translation is present | PASS with notes (are some English words expected?)

# Unit / Automated Testing

The was only manual testing as this was a website.  I am fine to pass this as with the current manually testing scripts as opposed to automated testing since this is a thin UI that talks with unit tested smart contracts.

Requirement | Finding
------------ | -------------
Unit Tests | N/A

# Documentation

### Code Documentation

Code documentation is sparse but exists on every function.

Requirement | Finding
------------ | -------------
React/Typescript Documentation | PASS

### Project Documentation

README.md instructions work for compilation locally and when ran in an AWS environment.  There is no real documentation around the AWS deployment but this has been discussed with the OP and it will be submitted with milestone 5.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with notes (submit more detailed AWS documents with milestone 5)

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The project is MIT licensed.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project 

# Final Conclusion

The project should pass in its current state but not pass milestone 5 unless notes are addressed.

# Recommendation

Recommendation | PASS with notes
------------ | -------------

