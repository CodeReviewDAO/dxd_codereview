

Grant Proposal | [153 - Uniswap Clone for Casper](https://portal.devxdao.com/public-proposals/153)
------------ | -------------
Milestone | 1
Milestone Title | Contract Port 4 Engineers + 2 QA Engineers
OP | Bernardo Herzer 
Reviewer | Robert Carbone <codereview@robertcarbone.com>

# Milestone Details
This is the first milestone of grant. 
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Modify existing ERC 20 Rust contract to be uniswap compliant 
UniswapV2Factory Smart Contract Port
UniswapV2Pair Smart Contract Port
Documentation, Verification, and Testing
Uniswap Router 2.0

**Acceptance criteria:**

We are able to deploy the uniswap contract and get it working with a compatible erc20.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/uniswap-v2-router-casper | YES
https://github.com/Rengo-Labs/uniswap-v2-core-casper | YES

# Install & Usage Testing Procedure and Findings

The furnished instructions we more than adaquate for this stage in the project and for the target audience(advanced users). 

## Overall Impression of usage testing

There was quite a good deal of code written for a Milestone named "Contract Port 4 Engineers + 2 QA Engineers" 
The Engineers involved clearly have a good handle on the technologies being implemented. 
The code is adaquatly laid out. Things are aligned, in no way messy, but have plenty of room for improved layout and added documention 
as the project continues. Exceedingly decent. 

Requirement | Finding
------------ | -------------
We are able to deploy the uniswap contract and get it working with a compatible erc20 | PASS

# Unit / Automated Testing

Working tests are not required for this review to pass the acceptance criteria. 
Despite this, the OP is well on their way to having adaquate tests.

There are Positive & Negative Test Cases. 
They are insufficent for the end of project,
but for the current state of the project they are sufficient. 


Requirement | Finding
------------ | -------------
Unit Tests - Sufficeint | PASS

# Documentation

The documentation for this project is excellent for this stage of the process.
They have a table of contents with links and type descriptions. 
They far are ahead of their milestones in this capacity.
Excellent. 

### Code Documentation

Next to the fantastic supporting documentation the inline documentation is exceedingly adaquate.
But again, for this stage of the process, this is more than sufficient.
The reviewer does urges the OP to include much more inline documentation in the source code. 
This would be very helpful for untrained newcomers whom actually want to read the soruce. 
That being said, it should also be noted that the OP has left plenty of space near each 
method to do so and very well may have intended to expand the documentation intime.
In all, a promising display.   

Requirement | Finding
------------ | -------------
Code Documented | PASS


### Project Documentation

Project Documentation was acceptable for this stage of the project. 

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

An impressive display for this stage. 

# Open Source Practices

## Licenses

The Project is released under the Apache License 2.0

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS


## Contribution Policies

The current state of the code is in private repositories. 
As this code is sensitive in nature at the moment, it is the opinion of this reviewer that this is 
appropriate, given the circumstances. If a malicious actor was to gain access to this code and set 
up a DEX, the reputation of the Casper Ecosystem could be affected. 

The OP has indicated that he is willing to show the 
repository to any individual that may ask. 
In light og the high-profile nature of the project, 
this seems reasonable and nessecary and this reveiwer 
urges other policing coleagues to consider this and 
waive the requirement. 


Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

Acceptable. 

## General Observations

# Final Conclusion

It has not been mentioned yet, but two other reviews have been done: 
 { Quantstamp's 1st Report, https://github.com/atomizable/dxd_codereview/blob/main/153%20-%20Uniswap%20Clone%20for%20Casper/Uniswap%20-%20Report.pdf }
,{ Maciej's Review, https://hackmd.io/@zie1ony/casper-uniswap-code-review }
From these we can clearly see the project being built and run.
The concerns raised by these two reviewers have been documented and it has been demonstrated that the
OP has addressed them all sufficiently, and again, for this first milestone of the project, more than sufficiently. 

Also note, regarding 'The QSP7 issue'
The OP has indicated that they are adding two new functions and these additions are currently 
in quality assurance phase at the momentt. 

Quantstamp will be issueing another report shortly. 
This should be addressed in future reviews by future reviewers. 

The reviewer has confirmed that the uniswap contract can be deployed within the same account. It shoud be noted that there 
is a limitation with the CLI with contracts deployed different to accounts. 
This seems to be due to a issue in the deployent namespace as contracts cannot easily be told thier own names. 
As this is an ecosystem problem that the team understands well,
it is the opinion of thie reviewer that the acceptance cirteria for a deploying a uniswap contract has been met. 
It has been demonstracted to the reviewer that they have it working with two erc20s. 

# Recommendation

Recommendation | PASS WITH NOTES
  ------------ | -------------











