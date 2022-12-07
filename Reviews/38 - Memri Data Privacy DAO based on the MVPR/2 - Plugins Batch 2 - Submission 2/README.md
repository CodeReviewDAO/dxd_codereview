Grant Proposal | [38 - Memri Data Privacy DAO based on the MVPR](https://portal.devxdao.com/public-proposals/38)
------------ | -------------
Milestone | 2
Milestone Title | Plugins Batch 2 - Submission 2
OP | Memri
Reviewer | HouPha Vang

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

5 plugins for the Memri POD.

**Acceptance criteria:**

Each plugin must adhere to the following acceptance criteria: https://gitlab.memri.io/memri/docs.memri.io/-/wikis/Acceptance-criteria-for-plugins. 
To test install the Memri POD and run the plugin.

**Additional notes regarding submission from OP:**

Please find a the list of plugins that have been completed under this milestone and their specific repositories below:

telegram
- repository: https://gitlab.memri.io/memri/plugins/telegram
- video: https://www.loom.com/share/c2fa02fc71304a74aa7b43688a68e460

zero shot
- repository: https://gitlab.memri.io/memri/plugins/zero-shot-plugin
- video: https://www.loom.com/share/527d14f9d78a4a68ad4a270a30d6099f
  
gmail oauth
- repository: https://gitlab.memri.io/memri/plugins/gmail_oauth
- video: https://www.loom.com/share/709cf2cfd744431b859fed46f3a095f7

language identification:
- repository: https://gitlab.memri.io/memri/plugins/language-identification
- video: https://www.loom.com/share/c881a50f8db54a839784334eebe33578
  
twitter-topic-model:
- repository: https://gitlab.memri.io/memri/twitter-topic-model
- video: https://www.loom.com/share/138dcbb4c1074364b0bf085bc1678232

You can reach us on discord: https://discord.gg/kRTcDtGUmr
Or in the CRDAO Telegram group (@allbeingsthriving)

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://gitlab.memri.io/memri/plugins/telegram | 995fa5003ba280e11d9e8c68e4f9c053fb8ad532
https://gitlab.memri.io/memri/plugins/zero-shot-plugin | c7b9796cb4bedf74c5a1e23c2361986ea4c06ef1
https://gitlab.memri.io/memri/plugins/gmail_oauth | e720cc4b0530d1ad3297c4ccd1ba758390b73b54
https://gitlab.memri.io/memri/plugins/language-identification | 39f7b0c78781ca59782c05ea5cc004cbb259d536
https://gitlab.memri.io/memri/twitter-topic-model | 011d130396e7468890fffedb74700f6158392bf7


# Install & Usage Testing Procedure and Findings

## Telegram Plugin 

### Install 

### Usage


## Zero-shot Plugin

### Install

### Usage


## Gmail OAuth Plugin

### Install 

### Usage


## Language Identification Plugin

### Install 

### Usage


## Twitter Topic Model Plugin

### Install

### Usage


## Overall Impression of usage testing

Overall, the plugins build and operate without errors when not on a Windows machine. However, the Reviewer suggests adding a note on the plugins that issues may arise when attempting to utilize the plugins on a Windows operating system.  Otherwise, the documentation provides sufficient installation/execution instructions and project functionality meets acceptance criteria.

Requirement | Finding
------------ | -------------
Project builds without errors |  PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

## Telegram Plugin 

## Zero-shot Plugin

## Gmail OAuth Plugin

## Language Identification Plugin

## Twitter Topic Model Plugin


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

## Telegram Plugin 

## Zero-shot Plugin

## Gmail OAuth Plugin

## Language Identification Plugin

## Twitter Topic Model Plugin

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

# Final Conclusion

The project meets the functional requirements and the Reviewer was able to confirm that the plugins designed for the current milestone run as expected. However, the Reviewer faced a lot of issues in trying to install the plugins and the Memri POD on a Windows machine. It could be due to a lack of familiarity with the project on the Reviewer's behalf, but this may be something that could be looked into. In addition, the Reviewer suggests revisiting the Memri POD quickstart guide (https://docs.memri.io/overview/quickStart/) to ensure it is up to date. 

The reviewer also suggests adding in the missing policies and adding tags to each repository to improve discoverability.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
