Grant Proposal | [135 - CasperHolders - Next features](https://portal.devxdao.com/public-proposals/135)
------------ | -------------
Milestone | 1-4
Milestone Title(s) | 1 - Casper Open Data</br>2 - Operation history & Staking rewards Overview</br> 3 - Ledger Integration</br>4 - Code Review
OP | Killian 
Reviewer | Michael Steuer <michael@make.software>

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
https://github.com/casperholders/casperdata | c536924
https://github.com/casperholders/casperholdersfront | 2edf769
https://github.com/casperholders/casperholdersapi | 06cc883
https://github.com/casperholders/casperholderscore | 63fb143

# Install & Usage Testing Procedure and Findings

The project and milestones are spread out across 4 different GitHub repositories, each of which need to be set up. While 
there is technically nothing wrong with that, it makes this submission rather complex, and risky for OP, because a problem in
1 repository, can result in a failure of all 4. Much like with Pull Requests, it is recommended to have more concisely 
defined deliverables in future milestones.

As a first step, Reviewer checked out each of the 4 repositories (at the revisions listed above) and will attempt to use the
set up instructions for each to get them up and running.

### `casperdata`
Reviewer successfully cloned repository. 

The "How to build" section provides for simple "local dev" set up instructions, but
prefaces these simple commands with "Make sure to setup your database & config correctly before that". While it's not entirely
clear what the OP means by this (especially considering that the project comprises 3 more repositories, each of which could be
or contain the database), they did include a section later in the README that provides for "Technical information & Database config". 
Reviewer will attempt to use that information in order to set up the required database. Reviewer recommends that the set up
instructions are improved to:
* clearly outline the prerequisites
* present the steps-to-be-performed in chronological order

Using the "example to run a local postgres db" line provided, Reviewer was able to spin up a local Postgres db docker image.
Subsequently the Reviewer tried the provided "How to build" commands and noticed that the project successfully started,
executed its database migrations and started fetching blocks from a Casper Node RPC endpoint. The process of retrieving, parsing
and inserting blocks into the database is expected to take a bit of time. After some time the process of retrieving new blocks froze. 
Reviewer reached out to OP and was advised to restart the process. After restarting the process, the process appeared to resume, but after some
time froze again. Reviewer restarted the process many times, and even tried synching against other Casper Nodes than the one
suggested by OP. In addition, the process once failed entirely and self-exited with "Code 1".
Reviewer has been in touch with OP throughout these issues, and OP
is not certain what caused these issues. After about a full working day of trying, Reviewer concluded that in its current state the project
is not ready for primetime, and does not meet the acceptance criteria. 

Reviewer recommends the following remedial steps to OP before resubmitting the milestone:
1. Investigate the underlying cause. It appears that synching always works well initially, but eventually some resource limit is reached and the process
   simply halts
2. Attemp to catch / detect the circumstances underlying the freezing issue, and address them in code so that the synching process is more fault tolerant
3. Improve the logging so that it's easier to interpret what is going on, and what the process is hanging on
4. Consider making the process multi-core for faster processing and better fault tolerant
5. Consider using a process manager such as PM2, which can monitor for failed processes, parallelize processes, and allow for better monitoring during
process execution
   
## Overall Impression of usage testing

### `casperdata`
While the database was populated, Reviewer installed a Postgres client (Navicat for Postgress - trial) in order
to review the persisted data. While the milestone definition and related acceptance criteria do not explicitly promise 
completeness of the data, it is implied in the use case of the project. Reviewer found that the data stored is NOT complete, 
and therefore not universally useful for third parties who may need to access additional properties of the data entities. For example,
`Blocks` are persisted without a reference to which (validator) account proposed them, their parentHash, or their state root hash. 

Testing was ceased due to the FAIL conditions outlines above. Once the FAIL conditions are addressed, the project can be submitted for re-testing.


Requirement | Finding
------------ | -------------
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

### `casperdata`

Unit testing was not reviewed due to the FAIL conditions outlines above.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | to be tested in a future submission
Unit Tests - At least one negative path test | to be tested in a future submission
Unit Tests - Additional path tests | to be tested in a future submission

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
Example Documented | to be tested in a future submission

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

Even though sparing no effort on attempting to get the project working properly, and interacting directly with OP in order
to address the underlying issues so that a FAIL would not have to result, unfortunately Reviewer has no other choice but to
conclude the project is not ready for final code review and recommends that the submission is FAILED and returns to the OP.

# Final Conclusion

Even though sparing no effort on attempting to get the project working properly, and interacting directly with OP in order
to address the underlying issues so that a FAIL would not have to result, unfortunately Reviewer has no other choice but to
conclude the project is not ready for final code review and recommends that the submission is FAILED and returns to the OP.

# Recommendation

Recommendation | FAIL
------------ | -------------
