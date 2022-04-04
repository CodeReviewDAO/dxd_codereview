Grant Proposal | [135 - CasperHolders - Next features](https://portal.devxdao.com/public-proposals/135)
------------ | -------------
Milestone | 1-4
Milestone Title(s) | 1 - Casper Open Data</br>2 - Operation history & Staking rewards Overview</br> 3 - Ledger Integration</br>4 - Code Review 2
OP | Killian 
Reviewer | David Tai david.tai@rengo.capital

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

### Milestone 1

Release a software to scan the Casper Blockchain from the start and that keep the data in sync with the blockchain.
Automate the release of open data gathered by the software.

Additional feature : Allow all validators on casper holders to delegate on them. Same for undelegating.

### Milestone 2

User ability to see operations history (Transfer / Delegation / Smart contract call etc...)
User ability to see staking rewards and projections in the future.

### Milestone 3

Add the ability to use Ledger for transfer operations.

### Milestone 4

I will have to do a code review with the DAO or anybody else but I don't know how much does it cost and how long does it takes.

**Acceptance criteria:**

### Milestone 1

* Release the software on github
* Provide a way to download open data gathered by the software on Github or a website.
* User can delegate / undelegate on any validator.

### Milestone 2

* A user can see his staking rewards overview and projections in the future.
* A user can see past operations list and detail.

### Milestone 3

Users should be able to use ledger for transfer operations.

### Milestone 4

Full disclosure of the code review with issues created on the github repo and timeline to remediate the potentials issues.

**Additional notes regarding submission from OP:**

Let me add a little bit of context for this review :

#### Milestone 1 :

Release a software to scan the Casper Blockchain from the start and that keep the data in sync with the blockchain.

Automate the release of open data gathered by the software.

Done on this repo : https://github.com/casperholders/casperdata

SQL Backups are available here : https://backup.casperholders.io/ & https://backup.testnet.casperholders.io/

Since Casper reverted the mixed case with 1.4.4 I'll need to wipe and re-parse the testnet & mainnet soon so those backup won't match.

Additional feature : Allow all validators on casper holders to delegate on them. Same for undelegating.

Done on this repo : https://github.com/casperholders/casperholdersfront & https://github.com/casperholders/casperholdersapi

The website retrieve validators informations from the API if the API is down the website fallback to onchain data.


#### Milestone 2 : Operation history & Staking rewards Overview

User ability to see operations history (Transfer / Delegation / Smart contract call etc...)

User ability to see staking rewards and projections in the future.

Done on this repo : https://github.com/casperholders/casperholdersfront & use data from Casper Data. The blockchain data created with casper data are available through an api that isn't developped. It use postgrest (not postgres) it's a piece of software that expo rest endpoint for a given postgres database. So no need to develop or test it.

#### Milestone 3 : Ledger integration

Done on this repo : https://github.com/casperholders/casperholdersfront


#### Milestone 4 : Code review (No review to do this milestone was here before we had a code review process on DxD)

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/casperholders/casperdata | 047d7f5
https://github.com/casperholders/casperholdersfront | 0dced34
https://github.com/casperholders/casperholdersapi | 1b0aa66
https://github.com/casperholders/casperholderscore | e5a7871

# Install & Usage Testing Procedure and Findings

I will quote the first review:

"The project and milestones are spread out across 4 different GitHub repositories, each of which need to be set up. While 
there is technically nothing wrong with that, it makes this submission rather complex, and risky for OP, because a problem in
1 repository, can result in a failure of all 4. Much like with Pull Requests, it is recommended to have more concisely 
defined deliverables in future milestones.

As a first step, Reviewer checked out each of the 4 repositories (at the revisions listed above) and will attempt to use the
set up instructions for each to get them up and running."

### `casperdata`

Reviewer was able to clone, build, and run using minikube by following the instuctions.

During the manually testing process where in the reviewer attempted over two weeks to fully synchronize testnet, the reviewer ran into several issues with several updates to the readme.md and the codebase:

1. node 17 seems to have higher memory usage in practice- OP Fixed with note in "Node Version" section "We're only supporting the Node 16 LTS version for now"
2. Garbage collection and out of memory issues - OP addressed with adjusting defaults in `.env` and fixing bugs in the the various parsers files.  There are still ongoing but less major issues.
3. Timeout cascades where the volume of timeouts handled by the node.js block http handing, causing more timeouts - adjustments to `.env` constants.
4. The postgres schema does not include all data from querying the blockchain - the schema is documented and additions can be requested using the existing Contributing.md.

### `casperholdersfront`

Reviewer was able to build and run automated testing.  Reviewer was also able to open and use the features of the website.  This website is already in production as part of the mobile app.  The reviewer encounted an error with openssl on Ubuntu 20.04 when running with node 17 but this is an issue present in other projects using cryptography libraries (including the user's own).  This is an ecosystem issue reviewer so will assume the ecosystem resolves this or posts work arounds.

### `casperholdersapi`

Reviewer was able to build and run unit test.

### `casperholderscore`

Reviewer was able to build and run unit test.

## Overall Impression of usage testing

### `casperdata`

Testing took approximately ~10 days to perform the full synchronization of testnet.  Test net was fully synchronized after  bugs were found and fixed.  

### `casperholdersfront`

The reviewer was able to test the website and the mobile app manually and run the automated testing.

### `casperholdersapi`

The reviewer was able to test this part by using the website.  It is also possible to test this in production.

### `casperholderscore`

This code is built into the website and tested at the same time as the website

Requirement | Finding
------------ | -------------
Project builds without errors | PASS (on npm 16 only due to some issues with 17's openssl updates)
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

### `casperdata`

The unit tests cover block and deploy parsing processes.  Tests are detailed and complete.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

### `casperholdersfront`

The tests for the website are remarkably complete and well organized, testing most major paths of interest.  Reviewer did not have to manually test much to confirm major flows work

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS (This is harder to quantify but inputs and ux state tests do test some error handling)
Unit Tests - Additional path tests | PASS

### `casperholdersapi`

Tests are sparse but the library just wraps casper node functions and is an in memory cache for casper node data that supports sorting (add JSON to in memory variable).  Additional testing would just be testing the casper node itself.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | N/A

### `casperholderscore`

The tests here are the detailed and hit most major features, test validate both pass and failure paths.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code is well-documented, where applicable

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

#### `casperdata`
The usage documentation, as explained above, can be improved with prerequisites and sequential installation steps (they are currently listed out 
of order).

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

Overall the project is well documented and the intention of the OP to make their project suitable and easy-to-understand
for public consumption/usage is very clear.

# Open Source Practices

## Licenses

Each of the repositories is released under the Apache License 2.0

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is fairly standard for a fullstack javascript application.

### `casperdata`

This project is structured like a typical javascript project.  Inline comments are sparse but the readme is detailed in how the project works.

### `casperholdersfront`

Documentation is pretty sparse, mostly on the component level, but it is sufficient for anyone versed in vue to understand the project without much difficulty as it follows a standard view structure.

### `casperholdersapi`

Swagger documentation can be generated from the inline comments, code here is relatively straight forward and adheres to common standards.

### `casperholderscore`

This project has full jsdoc support using inline comments.  This project is structured like a typical javascript project.

# Final Conclusion

This project took a very line time to thoroughly test.  OP and the reviewer had numerous discussions on how to improve the project which resulted in numerous changes and upgrades.  As a result, the review believes that the project is now in a state where it is reasonably functional and accomplish the description in each project's readme.

# Recommendation

Recommendation | PASS
------------ | -------------
