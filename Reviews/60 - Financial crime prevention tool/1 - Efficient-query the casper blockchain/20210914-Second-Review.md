# Second Review

Grant Proposal | [60 - Financial crime prevention and risk intelligence on-chain tool](https://portal.devxdao.com/public-proposals/60)
------------ | -------------
Milestone | 1
Date | 9/14/2021

## Introduction
In response to the FAIL conditions in the original [Code Review](README.md) for this milestone, OP has requested a
Second Review of their milestone, after asserting that the FAIL conditions have been addressed in their milestone.

The following milestone assets/artifacts were submitted for second review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/syntifi/ori | b33bcf45d61574cf673ca575a70413355cfd4172
Comparison | https://github.com/syntifi/ori/compare/fbf2ee8...b33bcf45d61574cf673ca575a70413355cfd4172
Comparison Stats | 27 changed files with 965 additions and 79 deletions.

Reviewer is focusing this review solely on verifying that the FAIL conditions have been addressed.

## FAIL CONDITIONS 1 & 2

# | FAILED Condition
------------ | -------------
1 | Project builds and runs without errors
2 | Documentation provides sufficient installation/execution instructions

Both failed conditions are evaluated together in this second review, as they were closely tied. With sufficient installation
instructions, it would have been possible to correctly build and run the project without errors.

Reviewing the OPs changes, Reviewer notes that OP added the following sections and details to the README of the project:
* Dependencies
* Before build instructions
* Local jar dependencies (which addresses the failed dependency issue highlighted in the original review)
* Running unit-test (which addresses the remark in the original review: instructions don't mention that you first have to create a docket network with the name `elastic`)
* Build instructions (which includes a note that points out that "After building, the database is empty. Please follow the steps listed on After build instructions to populate the database." - 
  an issue that was pointed out in the original review)
* Running the application in dev mode
* Building and running Docker images
* After build instructions (which addresses issues pointed out in the original review)
* Features (which includes links to detailed API documentation for the REST API, the GraphQL API and Risk Metrics. The linked 
documentation certainly resolves another FAIL condition in the original review, "API Documentation").
  
> This reviewer would like to commend the OP with the quality and detail of the significantly improved project documentation.
> This is reviewer's opinion is now a quality example of what project documentation should look like.

After identifying the significantly improved documentation, reviewer confirmed that following the steps, the project builds
and run without errors. Thereby both original FAIL conditions have been addressed and should now pass.

### Second Review Results of FAIL Conditions 1 & 2

Requirement | Original Finding | New Finding
------------ | ------------- | -------------
Project builds and runs without errors | FAIL | PASS
Documentation provides sufficient installation/execution instructions | FAIL | PASS

## Other Notes of the Original Review

Reviewer was able to confirm that OP has addressed other notes from the original review as well. 

OP has added substantial low level function documenation to their codebase

Requirement | Original Finding | New Finding
------------ | ------------- | -------------
Low level function documentation | FAIL | PASS

As pointed out above, the new project documentation is exemplary and provides for easy to understand instructions to set up and run the project

Requirement | Original Finding | New Finding
------------ | ------------- | -------------
Sufficient Project Documentation | FAIL | PASS

OP now provides detailed API documentation for both the GraphQL and the REST API interfaces

Requirement | Original Finding | New Finding
------------ | ------------- | -------------
API documentation | FAIL | PASS

# Recommendation

Given that OP has mediated all FAIL conditions from the first review, it is this Reviewer's recommendation to PASS this code
review. I would like to compliment OP with the quality of the improvements made to the project.

Recommendation | PASS
------------ | -------------

