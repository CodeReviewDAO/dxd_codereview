
Grant Proposal | [329 - 2 - Apache Camel Casper connector](https://portal.devxdao.com/public-proposals/329)
------------ | -------------
Milestone | 2
Milestone Title | Apache Camel Casper connector
OP | Chad | 
Reviewer | Alexandre Carvalho <adcarvalho@gmail.com>

# Milestone Details
This is the second milestone of grant. 
The review will cover the second milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Implementing CasperConsumer : Subscribe to the Casper Event Stream Server  to consume messages from the endpoint 
- Implementing CasperConsumer Operations :  block_added,  deploy_processed, block_finalized etc.
- Unit testing  CasperConsumer 
- Publishing camel-casper component to Maven repositories and  https://camel.apache.org/components/next/

**Acceptance criteria:**

- CasperConsumer fully implemented and documented 
- All CapserConsumer operations fully implemented and tested 
- Unit tests passes 
- Fully implemented , tested and documented camel-casper component, available in GitHub , published into Maven repositories

**Additional notes regarding submission from OP:**

In this milestone:
- Camel-casper consumer component is implemented
- Camel-casper consumer is tested on all the SSE events: 
   DEPLOY_PROCESSED,
   DEPLOY_ACCEPTED,
   DEPLOY_EXPIRED,
   BLOCK_ADDED,
   FINALITY_SIGNATURE,
   FAULT,
   STEP;

using a embeded SSE server runing on localhost.  This is due to the difficulty to use testnet or mainnet nodes to run those unit tests.

Unit tests on the consumer component uses mock data classes generated to inject Json payload into the SSE server. 
No SDK (a part C# one) had implemented these classes. 

- Documentation for consumer was added
- Snapshot version is available in maven repos under version 3.14.1-SNAPSHOT.
- Next step : ask Apache to add the component to the official list : https://camel.apache.org/components/2.x/index.html

During the 3-months maintenance period, the OP will:

- Start the procedure to add the Camel Casper component to the list of official components: https://camel.apache.org/components/3.14.x/index.html

Procedure: https://camel.apache.org/community/contributing/


- Update the component according to the next updates of the Java SDK used (in particular for compatibility with version 1.4 of the Casper node)

- Update the component to release the 3.15.x versions only supporting JDK 11 and higher

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/camel-casper | [d1e4c8b](https://github.com/caspercommunityio/camel-casper/tree/d1e4c8be5f5a0e11605120d0f81891475b4dab06)

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/caspercommunityio/camel-casper, reviewer was able to successfully build the source code for this milestone, and all tests have successfully passed.

Build Results can be found here: [329_2_Build.md](resources/329_2_Build.md)

## Overall Impression of usage testing

By following the provided instructions on the repository, the reviewer was able to compile and successfully run the tests.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes 

The Java SDK used in this project was developed for the casper node spec v1.3. That means two RPC requests (query_global_state and info_get_validator_changes) are unavailable. The OP implemented code to support those and it would require a minimal change during the maintenance period, as soon as the SDK provides them. For this reason the reviewer considers the acceptance criteria met, therefore the 'Pass with Notes' above.

# Unit / Automated Testing

Project contains 50 unit tests that can be executed from the console. The reviewer has observed that all tests run successfully without errors. With the generated coverage report, it was observed a sustainable level of test coverage (> 80%) for critical pieces of the software.

Test Results can be found here: [329_2_TestResults.md](resources/329_2_Test_Results.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS 
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation

The reviewer has observed that the project has sufficient code-level documentation with summaries and comments specially on critical classes and methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Reviewer has observed that the project has detailed documentation for usage with examples, along with the installation, build and test instructions. 

Requirement | Finding
------------ | -------------
  Usage Documented | PASS
  Example Documented | PASS


## Overall Conclusion on Documentation

Based on the reviewer's findings, this should pass. In addition, javadoc runs succesfully and the generation output evidence can be found here: [329_2_Javadoc_Results.md](resources/329_2_Javadoc_Results.md)

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution and a security policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. Although this project took measures to provide full 1.4 spec compatibility, since no Java SDK supports 1.4 spec it will be needed for the method call to be updated/included during maintenance when the SDK provides them.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------