| Grant Proposal  | [581 - XPRIZE DECENTRALIZED COMMUNITY](https://portal.devxdao.com/public-proposals/581) |
|-----------------|-----------------------------------------------------------------------------------------|
| Milestone       | All Code Milestones                                                                     |
| Milestone Title | All Code Milestones                                                                     |
| OP              | Jim Mainard, CTO  XPRIZE FOUNDATION <Jim.Mainard@xprize.org>                            |
| Reviewers       | Karol Marter <karol@casper.network><br>Michael Steuer <michael@make.services>           |

# Milestone Details

## Details & Acceptance Criteria

### Milestone 5 

#### Details of what will be delivered in milestones: 

![img.png](img.png)
![img_1.png](img_1.png)
![img_2.png](img_2.png)
![img_3.png](img_3.png)
![img_4.png](img_4.png)
![img_5.png](img_5.png)
![img_6.png](img_6.png)


#### Acceptance criteria:

Web 3 NFT community incentivization system is launched and starts minting NFTs  for activities that advance the formation, structure, and governance of PROJECT FUTURE’s new venture engagement

### Additional notes regarding submission from OP:

OP has provided a detailed document outlining all milestone deliveries [here](https://streaklinks.com/B0_WrxJnp6HgI1ypTwI5vxiW/https%3A%2F%2Framprate.docsend.com%2Fview%2Fxuqnudiqekujvx6m)

Reviewer notes that this grant is of a unique nature, both in terms of the grant agreement, which is multi-party, as well as in terms
of the agreed upon Acceptance Criteria - several deliverables are based on proprietary systems of which the underlying
codebase cannot be reviewed, and correct functioning has to be deduced from provided screenshots and/or emperical testing to
the extent possible.

From a code review perspective, the Reviewer will only focus on the provided open-source repositories.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

_SparkEngine_: builds on top of the core open-source matrix platform, serving as a communication 
broker between the Vatom App client and external Spark Plugin servers. It ensures secure communication, 
authorizes plugin providers, and prevents user credentials from being sent to external systems. 
The Spark Engine extends Vatom's data model for community-specific post types, enforces business and 
community policies, enables Web3 behaviors natively in communities, and supports custom Sparks 
(Sparks are plug-ins built using SparkSDK running on Spark Engine). Spark Engine is available at:

https://github.com/VatomInc/spark-engine

_SparkSDK_: Base SDK that provides key capabilities for developers to build custom extensions to Vatom Connect (Community)

https://github.com/VatomInc/spark-sdk

_Plug-in written for XPRIZE_: This plugin builds on top of SparkSDK to deliver XPRIZE
Visioneering specific functionality related to Sketch Scoring and Voting:

https://github.com/VatomInc/spark-xprize-plugin

| Repository                                      | Revision Reviewed |
|-------------------------------------------------|-------------------|
| https://github.com/VatomInc/spark-engine        | 640a91d           |
| https://github.com/VatomInc/spark-sdk           |                   |
| https://github.com/VatomInc/spark-xprize-plugin |                   |




# Install & Usage Testing Procedure and Findings

## Spark Engine
The documentation for the Spark Engine repository is VERY minimal. In fact, the README is still titled "REPLACEME". 
The set-up instructions are very minimal and not well explained. For example:

```
Copy and edit config:
cp .env.template .env
```

It does not explain what to edit, what each of the environment variables mean, and how to properly set up the environment. The 
Reviewer or user is left to guess. 

Then, when the project is ran in "Local" mode, at first an error occurs:

```
Error: Cannot find module 'source-map-support/register'
```

Reviewer was able to mitigate this error by executing:

``` 
yarn add source-map-support
```

Subsequently the application ran without errors, but with several warnings that the OP should address. Once the application runs,
there are no instructions on how to use or test the application. Without such documentation, it is impossible for this Reviewer
to test if the application functions properly. Also no Unit Tests appear to be provided.

## Spark SDK

The documentation for the Spark SDK was non-existent. Only an empty README file was provided. Reviewer did inspect the `package.json`
file in order to discover available command, and tried the `yarn` command, followed by the `yarn build` command. The package appears
to build successfully without errors or warnings, but there is no documented ability to use, test or run it. Also no Unit Tests appear
to be provided.


## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

| Requirement                                                                        | Finding                       |
|------------------------------------------------------------------------------------|-------------------------------|
| Project builds without errors                                                      | PASS / FAIL / PASS with Notes |
| Documentation provides sufficient installation/execution instructions              | PASS / FAIL / PASS with Notes |
| Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes |

# Unit / Automated Testing

_Summarize the result of the unit testing / automated testing / integration testing provided in the Milestone. Feel free to include
automated test output, either as text, image or other artifact. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

| Requirement                                  | Finding                       |
|----------------------------------------------|-------------------------------|
| Unit Tests - At least one positive path test | PASS / FAIL / PASS with Notes |
| Unit Tests - At least one negative path test | PASS / FAIL / PASS with Notes |
| Unit Tests - Additional path tests           | PASS / FAIL / PASS with Notes |

# Documentation

### Code Documentation

_Summarize the code level documentation you encountered. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

| Requirement     | Finding                       |
|-----------------|-------------------------------|
| Code Documented | PASS / FAIL / PASS with Notes |

### Project Documentation

_Summarize the project level documentation you encountered. This covers the information provided in the README for the project, 
as well any exampled provided. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

| Requirement        | Finding                       |
|--------------------|-------------------------------|
| Usage Documented   | PASS / FAIL / PASS with Notes |
| Example Documented | PASS / FAIL / PASS with Notes |

## Overall Conclusion on Documentation

_Summarize your review of the documentation in this project, including code, usage and examples_

# Open Source Practices

## Licenses

_List which Open Source license is used and note anything that's non-standard. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

| Requirement                               | Finding                       |
|-------------------------------------------|-------------------------------|
| OSI-approved open source software license | PASS / FAIL / PASS with Notes |

## Contribution Policies

_Confirm that the project contains a `CONTRIBUTING` and `SECURITY` policy, and optionally an associated `Code of Conduct` policy. Confirm
that Pull Requests and Issues are enabled on the repository and that generally the Project is set up for public participation. 
Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

| Requirement                     | Finding                       |
|---------------------------------|-------------------------------|
| OSS contribution best practices | PASS / FAIL / PASS with Notes |

# Coding Standards

## General Observations

_Provide any general observations about the project you want to add to your review. These can be subjective in nature as well, and do not
contribute to your recommendation to pass or fail the submission._

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

| Recommendation | PASS / FAIL / PASS with Notes |
|----------------|-------------------------------|
