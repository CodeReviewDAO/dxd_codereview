Grant Proposal | [346 - Blockcerts on Casper (with Verifiable Credentials and Open Badges capability)](https://portal.devxdao.com/public-proposals/346)
------------ | -------------
Milestone | 1
Milestone Title | Enable Issuing Casper Blockcerts (Open Badges)
OP | Zan McNaught
Reviewer | Yunusemre Şentürk <se.yunusemre@gmail.com>

# Milestone Details
This is the first milestone of grant.
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

– Set up either Casper JS SDK or REST API

– Generate or obtain a list of major nodes with high uptime

– Point Casper JS SDK or REST API to major nodes and check functionality

– Fork https://github.com/blockchain-certificates/cert-tools

– Add OP's previously proprietary backwards-compatible upgrades

– Enable instantiation of Casper-compatible Blockcerts (Open Badges version)

– Fork https://github.com/blockchain-certificates/cert-issuer 

– Enable signed transactions in order to issue Casper Blockcerts (Open Badges version)

**Acceptance criteria:**

A user will be able to instantiate and issue a batch of Casper Blockcerts (Open Badges). When issued, that batch’s hash will be written to the Casper blockchain. With a properly configured validator (Milestone #3), this hash will be usable for validating Casper Blockcerts.

**Additional notes regarding submission from OP:**

– BE SURE TO ONLY REVIEW THE "v2" BRANCH!!! The "master" branch is part of a future milestone. 

– Reviewers can follow the "Casper-specific Instructions" in the README and ignore the rest (which applies to Bitcoin and Ethereum issuing).

– When you issue a Casper Blockcert, you can find its transaction ID (txid) in the logs.

– If you get a signature error, just try again a couple times or change the Casper RPC Node IP Address.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/amazanzan/casper-cert-issuer/tree/v2 | 1991yye


# Install & Usage Testing Procedure and Findings

The reviewer observed that, following the instructions in the README of https://github.com/amazanzan/casper-cert-issuer/tree/v2, it was not possible to succesfully install the issuer.
The reviewer used following trials in order to compansate encountered errors : 
 
 1 - Used `macOS Monterey (12.2.1)` as host: problems with directly called subprocesses in setup.py does not work
 
 2 - Used a digital ocean droplet `debian 9` as host: prepared, compiled and installed fresh python3.9, after running setup.py the following error occured : `/usr/local/lib/python3.9/distutils/dist.py:261: UserWarning: Unknown distribution option: 'long_description_content_type'`
 
 3 - Used a gitpod instance to make sure nothing is wrong with build environment, so `ubuntu2004 LTS` as host: after running setup.py this error occured : `FileNotFoundError: [Errno 2] No such file or directory: 'requirements.txt'`

## Overall Impression of usage testing

It was observed that the documentation provides insufficient installation instructions.

Requirement | Finding
------------ | -------------
Documentation provides sufficient installation/execution instructions | FAIL
Project builds without errors | no-data
Project functionality meets/exceeds acceptance criteria and operates without error | no-data

# Unit / Automated Testing

no-data

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | no-data
Unit Tests - At least one negative path test | no-data
Unit Tests - Additional path tests | no-data

# Documentation

### Code Documentation

Code documentation was acceptable for this stage of the project.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project documentation seem to be well documented regarding usage and examples, however, no comperiable data obtained by the reviewer because of no-installation.

Requirement | Finding
------------ | -------------
Usage Documented | no-data
Example Documented | no-data

## Overall Conclusion on Documentation

No comperable data obtained by the reviewer.

# Open Source Practices

## Licenses

There is no `LICENCE` file in source tree, although the OP explains about licencing in README.md, there is no harm to put the MIT (as mentioned in README) licencing paperwork under one file to follow.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | FAIL

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, but it is a bit shame that simple installation 
procedure have been made complicated by providing less instruction.

# Final Conclusion

The reviewer recommends that this submission should fail code review, because it does not contain an OSI-approved open source license and
it failed to be installed on 3 different common platforms.

# Recommendation

Recommendation | FAIL
------------ | -------------
