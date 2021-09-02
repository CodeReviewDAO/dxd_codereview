Grant Proposal | [60 - Financial crime prevention and risk intelligence on-chain tool](https://portal.devxdao.com/public-proposals/60)
------------ | -------------
Milestone | 1
Milestone Title | Efficient-query the casper blockchain
OP | Aberto
Reviewer | Michael Steuer <michael@make.software>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- A conversion layer to transform the Casper Blockchain to an efficiently "queryable" format (SQL or no-SQL format to be decided during the project)
- An API to efficiently query the transformed Casper blockchain. This lays the foundation for the  "trace the coin¨" feature

**Acceptance criteria:**

- Have a working GraphQL API to successfully query all transactions from/to a given wallet to easily run the API

**Additional notes regarding submission from OP:**

The repository was made public just now. There you can find the java code implementing the Casper Crawler, and the REST and GraphQL APIs. (as a side note, we do use a self-made rudimentary version of a java-casper-sdk with just the necessary methods for our purpose. That said, another member of the team already submitted a grant proposal to fully develop the casper-java-sdk and make it available to the community in the coming weeks, like the java community could easily have access to the Casper Network through a proper SDK).

We do believe the README.md should be complete enough to describe how to run in development mode, compile the java project, build the docker images (either in jvm or native mode) and run all necessary containers (elastic search, ori and kibana) in a docker-compose file.

Please let us know if you have any question/feedback. We are happy to address those in a call.

**REST API**
- Swagger-ui: http://localhost:8080/q/swagger-ui/
- Swagger file: http://localhost:8080/swagger

**GraphQL API**
- GraphQL-ui: http://localhost:8080/q/graphql-ui/
- Schema: http://localhost:8080/graphql/schema.graphql

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/syntifi/ori | fbf2ee8

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/syntifi/ori, reviewer was
able to successfully build and run that project. Two initial things to note with the initial instructions about running
the docker image:
- Using the "Copy" command on GitHub.com, pasting it and executing it results in an error ('docker: invalid reference format.'). To address this, the command had to be reformatted to 1 line
- The instructions don't mention that you first have to create a docket network with the name `elastic`

Upon first attempt to compile the project with `./mvnw compile quarkus:dev` as per the instructions, compilation failed with:

```bash
[INFO] ------------------------------------------------------------------------
[INFO] BUILD FAILURE
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  13.948 s
[INFO] Finished at: 2021-09-01T14:26:58-07:00
[INFO] ------------------------------------------------------------------------
[ERROR] Failed to execute goal on project ori: Could not resolve dependencies for project com.syntifi.ori:ori:jar:0.1.0: Could not find artifact com.syntifi.casper:casper-sdk:jar:0.1.2 in central (https://repo.maven.apache.org/maven2) -> [Help 1]
[ERROR] 
[ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
[ERROR] Re-run Maven using the -X switch to enable full debug logging.
[ERROR] 
[ERROR] For more information about the errors and possible solutions, please read the following articles:
[ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/DependencyResolutionException
```

Reviewer then reviewed the `pom.xml` file and found a commented-out command hint titled `INSTALLING FROM A FILE`, edited it
to point to a version of `casper-sdk-0.1.2.jar` that appeared to be included in the project inside `/src/main/resources` and tried
installing the Casper Java SDK.

Once that succeeded, Reviewer tried to compile the project again. This time the compilation succeeded. 

It should be noted that the documentation on how to get the project running, based on the above experience, 
is significantly deficient. It required significant time, effort, trial and error on behalf of the Reviewer to 
get the project to even compile. The standard expectations is that following the provided instructions should be a fool-proof
way to get a project to compile and run.

Once the application was compiled and running, finally, Reviewer was able to smoke-test the Dev UI successfully and 
interact with and review the various components of the system.

In order to test the acceptance criteria (Have a working GraphQL API to successfully query all transactions from/to a given wallet to easily run the API), Reviewer
first had to figure out how to populate the underlying database. Using instructions here: https://github.com/syntifi/ori/blob/main/src/main/java/com/syntifi/ori/task/README.md 
Reviewer was able to start a crawler process.

Subsequently testing the REST API here: http://localhost:8080/q/swagger-ui/#/, Reviewer was able to confirm that the crawler had indeed
retrieved blockchain data and populated its database. The Swagger API UI provides for easy testing of the API endpoints. 

Reviewer was able to test each API endpoint and each of their verbs. The documentation
was minimal for each end point, in the sense that it did not explain the use of each API endpoint, or provide the correct input format
for each parameter. For example, the end-points requiring a date (for example `/score/{account}` or `/traceCoin/forward/{account}` all failed with 
unhandled exception output in the API response, relating to unparseable date input when dates were provided. A human-readable error and/or an example input format
would remedy this issue). Moreover, unhandled exceptions should not be returned in API responses. Similarly, it was not clear what account format the `{account}` input
expected. The same account format (`account-hash-2be16861369304884b4d0755d321a05e7cca5911c28ccbe17f9976b8c727e34c`) that resulted in valid output for the `/transaction/account/{account}` endpoint,
resulted in `Not Found` errors when providing the same input to `/score/{account}`, `/traceCoin/forward/{account}`, and `/traceCoin/back/{account}`. Better documentation is needed.

After testing the REST API, Reviewer started testing the GraphQL API via the GraphQL UI. Reviewer confirmed that the documented
queries worked correctly. The following queries were successfully tried:

```graphQL
{
  casperTransfers(blockHash:"aad5c77f3e9707e5557e1dd703b63baeb8cadeb7d4add0435e647a85878cd556") {
    id
    to
    from
    amount
    gas
    source
    deployHash
    target
  }
  
}
```

```graphQL
{
  casperBlockByHash(blockHash: "aad5c77f3e9707e5557e1dd703b63baeb8cadeb7d4add0435e647a85878cd556") {
    hash
    header {
      timeStamp
      bodyHash
      accumulatedSeed
      protocolVersion
      parentHash
      stateRootHash
    }
    body {
      proposer
    }
    proofs {
      signature
      publicKey
    }
  }
  
}
```

```graphQL
{
  casperBlockByHeight(blockHeight: 1) {
    hash
    header {
      timeStamp
      bodyHash
      accumulatedSeed
      protocolVersion
      parentHash
      stateRootHash
    }
    body {
      proposer
    }
    proofs {
      signature
      publicKey
    }
  }
  
}
```

```graphQL
{
  casperNodes {
    address
    nodeId
  }  
}
```

```graphQL
{
  transactions (from:"account-hash-2be16861369304884b4d0755d321a05e7cca5911c28ccbe17f9976b8c727e34c") {
    hash
    from
    to
    amount
    blockHash
    timeStamp
  }
}
```

```graphQL
{
  transaction(
    hash: "7cafb799f5890ef49c3500a83c66ff9b1ee37215b6ce07971aaa0acacd758dfa"
  ) {
    hash
    amount
    blockHash
  }
}
```

## Overall Impression of usage testing

While the Acceptance Criteria of "Have a working GraphQL API to successfully query all transactions from/to a given wallet to easily run the API" is minimally
met, and the project provides additional functionality in a REST API and includes helpful testing/configuration UIs, the project falls severely
short in providing the necessary documentation required to properly set up and run the project, or to properly use the provided APIs. Those APIs where for the usage
parameters were correctly inferred by Reviewer and thus tested, operated correctly. However several others, Reviewer was never able to test. Since the untestable 
APIs were part of the REST API and thus outside of the Acceptance Criteria for this milestone, the "API Endpoints work without error" will "PASS with notes". Reviewer 
recommends addressing the identified deficiencies before a next milestone submission.

Requirement | Finding
------------ | -------------
Project builds and runs without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL
API Endpoints work without error | PASS with notes

# Unit / Automated Testing

Project contains 24 unit tests that can be executed from the console. Tests cover both positive and negative test paths.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code in the project is essentially comment/documentation free, other than in the AMLRules.java class

Requirement | Finding
------------ | -------------
Low level function documentation | FAIL

### Project Documentation

As identified above, the project does NOT contain sufficient documentation describing the prerequisites and steps to set up, compile and run the project

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | FAIL

### API Documentation

While some auto-generated API documentation is included, as identified above the lack of endpoint usage descriptions and/or input parameter format examples
has resulted in this Reviewer being unable to test certain API endpoint. As such, this requirement is not met.

Requirement | Finding
------------ | -------------
API documentation | FAIL

## Overall Conclusion on Documentation

Given the number of FAILs above, the overall conclusion has to be that this project falls short of the expected level of documentation.

# Open Source Practices

## Licenses

The Project is released under the MIT License

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

Code is generally well-structured and very readable. The project as committed to GitHub cannot be run without finding the hidden workaround
of installing the Casper SDK Jar from file.

# Final Conclusion

The project appears to provide the functionality described in the grant application and milestone acceptance criteria. Some of the functionality
could not be tested due to a lack of clear documentation (specifically the "Trace the coin" functionality).

The deliverable falls short in the following areas:
* Documentation

For a project of this magnitude, in both scope and cost, strict adherence to the minimal standards should be enforced, and therefore, it is this Reviewer's 
opinion that this milestone submission should fail, until the identified shortcomings are addressed. I do believe these are easily addressed, and I look forward
to reviewing the milestone again in the near future to re-assess my recommendation.

# Recommendation

Recommendation | FAIL
------------ | -------------

