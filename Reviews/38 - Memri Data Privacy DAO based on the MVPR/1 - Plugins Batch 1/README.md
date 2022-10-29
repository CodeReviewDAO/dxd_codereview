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
https://gitlab.memri.io/memri/plugins/whatsapp-multi-device | 084b8a44a78da9c4f331bcba92d1192c47dcc9ad
https://gitlab.memri.io/memri/plugins/twitter | a56e041e8befdddd6aa241964e46ebb16ec1978e
https://gitlab.memri.io/memri/plugins/instagram | 7657837227fd603ed2a97aabfde131b8dad7d40e
https://gitlab.memri.io/memri/plugins/gmail | 795a5072cd9dd4d19ca2c8aa98ed96fd603196a4
https://gitlab.memri.io/memri/plugins/sentiment_plugin | 6f0e0ba6bc8c432196f7043db1d3a5c8657071d9


# Install & Usage Testing Procedure and Findings

There was some issue in the initial installation process of the Memri POD required to test the plugins as the reviewer used a Windows machine, but after troubleshooting, the reviewer was able to get a POD up and running on Docker to begin test on the plugins. However, the process of installing a Memri POD is not the main subject matter of this job, so reviewer takes it as a granted that the Memri POD is working.

## Whatsapp Plugin 

### Install 

After downloading the repository (https://gitlab.memri.io/memri/plugins/whatsapp-multi-device), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

There was an issue in the installation being caused by requiring "pycrytpo" for the plugin. However, removal of the requirement in the setup.py file allowed a successful install.

### Usage

The Reviewer followed the instructions in the README to run the plugin within the frontend app and was able to successfully import messages and connect with Whatsapp.

![alt text](https://github.com/hoopav/dxd_codereview/blob/2e1377a57631587cd5fa7741aa081051b72ce3b3/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/whatsapp_import_success1.PNG)

![alt text](https://github.com/hoopav/dxd_codereview/blob/2e1377a57631587cd5fa7741aa081051b72ce3b3/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/whatsapp_import_success2.PNG)

![alt text](https://github.com/hoopav/dxd_codereview/blob/2e1377a57631587cd5fa7741aa081051b72ce3b3/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/whatsapp_import_success3.PNG)

## Twitter Plugin

### Install

After downloading the repository (https://gitlab.memri.io/memri/plugins/twitter), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

### Usage

The Reviewer followed the instructions in the README to run the plugin within the frontend app and was able to successfully login to the Twitter API via oauth. Afterwards, the Reviewer was able to import data for the User account, Followers and following accounts, and user timeline tweets. However, it is noted that the date of the posts seem to be off by a month.

![alt text](https://github.com/hoopav/dxd_codereview/blob/34c2286216688d23d3609b2adf369be8eab7ba40/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/twitter_import_success1.PNG)

![alt text](https://github.com/hoopav/dxd_codereview/blob/34c2286216688d23d3609b2adf369be8eab7ba40/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/twitter_import_success2.PNG)

![alt text](https://github.com/hoopav/dxd_codereview/blob/34c2286216688d23d3609b2adf369be8eab7ba40/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/twitter_import_success3.PNG)

## Instagram Plugin

### Install 

After downloading the repository (https://gitlab.memri.io/memri/plugins/instagram), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

### Usage

The Reviewer followed the instructions in the README to run the plugin within docker and was able to successfully login to an Instagram account and import Instagram post data.


## Gmail Plugin

### Install 

After downloading the repository (https://gitlab.memri.io/memri/plugins/gmail), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

### Usage

The Reviewer followed the instructions in the README to create an App Password for a Gmail account, and then successfully connected and imported data. Note: the path in the README for the credentials is erroneously listed as Instagram when it should be gmail_importer.

However, in attempting to run the steps again on another day, Reviewer was unable to reproduce the results and instead was met with an error message. See [here](https://github.com/hoopav/dxd_codereview/blob/ebff13a78375c4e730be9aaeed7fcb8fd7f879d2/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/gmail_error.MD).

The Reviewer notes that Gmail recently had an update however, so the Reviewer suggests Pass with a note to review the api and see if there are any material changes and refactors that must be performed.

## Sentiment Plugin

### Install

After downloading the repository (https://gitlab.memri.io/memri/plugins/sentiment_plugin), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

### Usage

The Reviewer followed the instructions in the README to run the plugin after starting a Pod in docker. The Reviewer had data to make predictions on from running the Whatsapp plugin, and after running the plugin, was able to confirm that labels with the sentiment of the message have been added to the data in the Pod.

## Overall Impression of usage testing

Overall, the plugins build and operate without errors when not on a Windows machine. However, the Reviewer suggests adding a note on the plugins that issues may arise when attempting to utilize the plugins on a Windows operating system.  Otherwise, the documentation provides sufficient installation/execution instructions and project functionality meets acceptance criteria.

Requirement | Finding
------------ | -------------
Project builds without errors |  PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

## Whatsapp Plugin 

There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, since this is an early milestone and the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [whatsapp_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/60f8cda5d05074c728442596576e427d336a426b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/whatsapp_testresults.MD)

## Twitter Plugin

There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, since this is an early milestone and the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [twitter_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/60f8cda5d05074c728442596576e427d336a426b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/twitter_testresults.MD)

## Instagram Plugin

There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, since this is an early milestone and the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [instagram_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/60f8cda5d05074c728442596576e427d336a426b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/instagram_testresults.MD)

## Gmail Plugin

There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, since this is an early milestone and the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [gmail_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/60f8cda5d05074c728442596576e427d336a426b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/gmail_testresults.MD)

## Sentiment Plugin

There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, since this is an early milestone and the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [sentiment_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/60f8cda5d05074c728442596576e427d336a426b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/sentiment_testresults.MD)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

Overall, for each plugin, the code is clear and readable enough to follow even for someone new to the project. Where context is needed for memory addresses, flags, or potentially confusing areas, proper documentation has been added to make clear what is being done.

However, there may be insufficient code-level comments to auto-generate documentation as not every function has been commented. To the uninitiated user, or to a user that is overwhelmed, it could be a source of confusion. Reviewer suggests revisiting the code-level comments and adding in descriptions for every function as well as formatting for autogeneration of documentation as a user convenience. However, Reviewer does not believe this is enough to justify failure at this early stage and so suggests PASS with Notes.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Overall, the project level documentation for each plugin is sufficient to inform the utility as well as usage process, but it is a bit terse in simply stating the general function of the plugins. More information about each plugin and its potential uses could be included in an "About" section for each plugin. In addition, a unified or standardized template for each plugin's README might be beneficial. Although each plugin's README covers roughly the same topics, the formatting is mostly different between each plugin's README.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes

## Overall Conclusion on Documentation

The reviewer concludes that the project has sufficient and comprehensive general documentation.

# Open Source Practices

## Licenses

The required license for these plugins is the Memri Privacy Preserving License. This license is present in the repositories of each plugin.

Requirement | Finding
------------ | -------------
Memri Privacy Preserving License | PASS

## Contribution Policies

Pull requests and Issues are enabled for all the plugin repositories. 

### Whatsapp Plugin 

The repository doesn't contain a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.

### Twitter Plugin

The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.

### Instagram Plugin

The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.

### Gmail Plugin

The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.

### Sentiment Plugin

The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct 

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

The Code is generally well-structured and readable, and documentation is added where context is necessary. 

The README instructions for the plugins are clear enough to follow and when everything is properly setup, it is a simple process to use the plugins. However, it may be good to include that Windows is not currently supported and make it clear that there may be many installation obstacles to get a proper Memri POD up and running, if not in the plugins then on the https://docs.memri.io/overview/quickStart/

# Final Conclusion

The project meets the functional requirements and the Reviewer was able to confirm that the plugins designed for the current milestone run as expected. However, the Reviewer faced a lot of issues in trying to install the plugins and the Memri POD on a Windows machine. It could be due to a lack of familiarity with the project on the Reviewer's behalf, but this may be something that could be looked into. In addition, the Reviewer suggests revisiting the Memri POD quickstart guide (https://docs.memri.io/overview/quickStart/) to ensure it is up to date. 

The reviewer also suggests adding in the missing policies and adding tags to each repository to improve discoverability.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
