Grant Proposal | [38 - Memri Data Privacy DAO based on the MVPR](https://portal.devxdao.com/public-proposals/38)
------------ | -------------
Milestone | 1
Milestone Title | Plugins Batch 1
OP | Memri
Reviewer | HouPha Vang

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

5 high quality plugins for the Memri POD including full CI/CD testing that either import data from an external resource ("importer") or analyze existing data and create new links and entities based on that information ("indexer").

**Acceptance criteria:**

Each plugin must adhere to the following acceptance criteria:
https://gitlab.memri.io/memri/docs.memri.io/-/wikis/Acceptance-criteria-for-plugins

To test install the Memri POD and run the plugin.

**Additional notes regarding submission from OP:**

N.B. Following proposal #631 the milestones for #38 have changed. This first milestone covers the first 5 plugins for Memri as specified in #631. I noticed the milestones in the system have not yet been updated following approval of #631. This first milestone grant portion should be 100K EUR (not 160K EUR).

This milestone covers 5 plugins that can be tested within the Memri pod. These plugins are:

### Importers
Whatsapp
https://gitlab.memri.io/memri/plugins/whatsapp-multi-device

Twitter
https://gitlab.memri.io/memri/plugins/twitter

Instagram
https://gitlab.memri.io/memri/plugins/instagram

gmail imap
https://gitlab.memri.io/memri/plugins/gmail

### Indexers
Sentiment analysis
https://gitlab.memri.io/memri/plugins/sentiment_plugin

In order to verify the function of these plugins you will need to do the following:
1. Install Memri POD (the flutter front-end is optional): https://docs.memri.io/overview/quickStart/ 
2. Install the plugin(s): https://docs.memri.io/component-architectures/pod/Plugins/
3. Inspect the pod using the pod explorer: https://docs.memri.io/guides/Inspect-your-pod/

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://gitlab.memri.io/memri/plugins | 1111aaaa


# Install & Usage Testing Procedure and Findings

General Notes
As suggested, I went to the documentation at https://docs.memri.io/overview/quickStart/ to begin the installation process. There was an immediate obstacle in following the instructions as the links to obtain the “Pod” and the “Flutter front-end” resulted in 404 pages.
Although I managed to find the Pod and the Flutter front-end at the gitlab repository listed in the job, it would be good to fix the broken links or remove them completely as it can confuse a user during initial set up.


##Installation
###Setting up Pod
####Hosted
####Using Docker
####Local build
###Setting up flutter front-end

### Connecting front-end and Pod


###Documentation

### Build


## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | PASS / FAIL / PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes

# Unit / Automated Testing

_Summarize the result of the unit testing / automated testing / integration testing provided in the Milestone. Feel free to include
automated test output, either as text, image or other artifact. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS / FAIL / PASS with Notes
Unit Tests - At least one negative path test | PASS / FAIL / PASS with Notes
Unit Tests - Additional path tests | PASS / FAIL / PASS with Notes

# Documentation

### Code Documentation

_Summarize the code level documentation you encountered. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Code Documented | PASS / FAIL / PASS with Notes

### Project Documentation

_Summarize the project level documentation you encountered. This covers the information provided in the README for the project, 
as well any exampled provided. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Usage Documented | PASS / FAIL / PASS with Notes
Example Documented | PASS / FAIL / PASS with Notes

## Overall Conclusion on Documentation

_Summarize your review of the documentation in this project, including code, usage and examples_

# Open Source Practices

## Licenses

_List which Open Source license is used and note anything that's non-standard. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS / FAIL / PASS with Notes

## Contribution Policies

_Confirm that the project contains a `CONTRIBUTING` and `SECURITY` policy, and optionally an associated `Code of Conduct` policy. Confirm
that Pull Requests and Issues are enabled on the repository and that generally the Project is set up for public participation. 
Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS / FAIL / PASS with Notes

# Coding Standards

## General Observations

_Provide any general observations about the project you want to add to your review. These can be subjective in nature as well, and do not
contribute to your recommendation to pass or fail the submission._

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
