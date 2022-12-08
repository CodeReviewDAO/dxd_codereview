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
After downloading the repository (https://gitlab.memri.io/memri/plugins/telegram/), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Telegram_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Telegram_Install.MD)

### Usage


## Zero-shot Plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/zero-shot-plugin), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Zeroshot_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Zeroshot_Install.MD)

### Usage


## Gmail OAuth Plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/gmail_oauth), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Gmail_OAuth_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Gmail_OAuth_Install.MD)

### Usage


## Language Identification Plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/language-identification), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Language_Identification_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Language_Identification_Install.MD)
### Usage


## Twitter Topic Model Plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/twitter-topic-model), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Twitter_Topic_Model_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Twitter_Topic_Model_Install.MD)

### Usage


## Overall Impression of usage testing


Requirement | Finding
------------ | -------------
Project builds without errors |  
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | 

# Unit / Automated Testing

## Telegram Plugin 

## Zero-shot Plugin

## Gmail OAuth Plugin

## Language Identification Plugin

## Twitter Topic Model Plugin


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | 
Unit Tests - At least one negative path test | 
Unit Tests - Additional path tests | 

# Documentation

### Code Documentation

Requirement | Finding
------------ | -------------
Code Documented | 

### Project Documentation

## Telegram Plugin 

## Zero-shot Plugin

## Gmail OAuth Plugin

## Language Identification Plugin

## Twitter Topic Model Plugin

Requirement | Finding
------------ | -------------
Usage Documented | 

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
The repository doesn't contain a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.  It is recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Zero-shot Plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Gmail OAuth Plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Language Identification Plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Twitter Topic Model Plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

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
