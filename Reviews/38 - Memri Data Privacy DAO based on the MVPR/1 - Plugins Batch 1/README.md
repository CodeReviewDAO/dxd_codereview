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

'''pip install -e .'''

There was an issue in the installation being caused by requiring "pycrytpo" for the plugin. However, removal of the requirement in the setup.py file allowed a successful install.

### Usage

The Reviewer followed the instructions in the README to run the plugin within docker and was able to successfully import messages and connect with Whatsapp.

## Twitter Plugin

### Install

After downloading the repository (https://gitlab.memri.io/memri/plugins/twitter), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

'''pip install -e .'''

### Usage

The Reviewer followed the instructions in the README to run the plugin within docker and was able to successfully login to the Twitter API via oauth. Afterwards, the Reviewer was able to import data for the User account, Followers and following accounts, and user timeline tweets.

## Instagram Plugin

### Install 

After downloading the repository (https://gitlab.memri.io/memri/plugins/instagram), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

'''pip install -e .'''

### Usage

The Reviewer followed the instructions in the README to run the plugin within docker and was able to successfully login to an Instagram account and import Instagram post data.

## Gmail Plugin

### Install 

After downloading the repository (https://gitlab.memri.io/memri/plugins/gmail), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

'''pip install -e .'''

### Usage

The Reviewer followed the instructions in the README to run the plugin within docker and was able to successfully import messages and connect with Whatsapp.

## Sentiment Plugin

### Install

After downloading the repository (https://gitlab.memri.io/memri/plugins/sentiment_plugin), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

'''pip install -e .'''

### Usage

The Reviewer followed the instructions in the README to run the plugin within docker and was able to successfully import messages and connect with Whatsapp.

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors |  PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

## Whatsapp Plugin 

The tests run successfully. See [whatsapp_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/16636690b0d1a9bdc0481fc32249d825ad156705/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/whatsapp_testresults.MD)

## Twitter Plugin

The tests run successfully. See [twitter_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/16636690b0d1a9bdc0481fc32249d825ad156705/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/twitter_testresults.MD)

## Instagram Plugin

The tests run successfully. See [instagram_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/16636690b0d1a9bdc0481fc32249d825ad156705/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/instagram_testresults.MD)

## Gmail Plugin

The tests run successfully. See [gmail_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/16636690b0d1a9bdc0481fc32249d825ad156705/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/gmail_testresults.MD)

## Sentiment Plugin

The tests run successfully. See [sentiment_testresults.MD](https://github.com/hoopav/dxd_codereview/blob/16636690b0d1a9bdc0481fc32249d825ad156705/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/1%20-%20Plugins%20Batch%201/assets/sentiment_testresults.MD)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS 
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation

Overall, for each plugin, the code is clear and readable enough to follow even for someone new to the project. Where context is needed for memory addresses, flags, or potentially confusing areas, proper documentation has been added to make clear what is being done.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Overall, the project level documentation for each plugin is sufficient to inform the utility as well as usage process, but it is a bit terse. 

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
