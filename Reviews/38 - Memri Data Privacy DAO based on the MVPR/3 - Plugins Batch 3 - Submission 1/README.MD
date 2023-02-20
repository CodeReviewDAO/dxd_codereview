Grant Proposal | [38 - Memri Data Privacy DAO based on the MVPR](https://portal.devxdao.com/public-proposals/38)
------------ | -------------
Milestone | 3
Milestone Title | Plugins Batch 3 - Submission 1
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

- Speech to Text
repository: https://gitlab.memri.io/memri/plugins/speech-to-text
video: https://www.loom.com/share/473300a2332f406fb441635df3ac6a3e
- Optical Character Recognition plugin
repository: https://gitlab.memri.io/memri/plugins/ocr
video: https://www.loom.com/share/3788bd6b50b0422cb462567f89ebc899
- Image Tagging plugin
repository: https://gitlab.memri.io/memri/plugins/image-tagging
video: https://drive.google.com/file/d/1UAFk3wsa2NdZAh6SuBEcDDaaGfsuEV1Q/view?usp=share_link
- Language translation plugin
repository: https://gitlab.memri.io/memri/plugins/language-translation
video:https://drive.google.com/file/d/1HGz6jgn6E5puYKqw76Emd7KhKKNwTYF5/view?usp=share_link
- Semantic search plugin
repository: https://gitlab.memri.io/memri/plugins/semantic-search
video: https://drive.google.com/file/d/1GNtot4vma2cVV17D7wOTbhO1cHmLjieh/view?usp=share_link

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://gitlab.memri.io/memri/plugins/speech-to-text | 754a0f5c3b36fd9815aaa8519349658dce649aa6
https://gitlab.memri.io/memri/plugins/ocr | e098ad2b19e11497550a9d09b0e4777382d44461
https://gitlab.memri.io/memri/plugins/image-tagging | e59b4f1ff8635de50dbdfdc1c2efffca6cfa9902
https://gitlab.memri.io/memri/plugins/language-translation | f95e11fa236456d35684b754d3ed9f1c2497171f
https://gitlab.memri.io/memri/plugins/semantic-search | 2576f0063368011510d071c9889f0d7b67385a23


# Install & Usage Testing Procedure and Findings

## General Notes
It is presumed that the user of the plugins is familiar with the process of setting up a Memri POD as well as examining data in the Memri Datastream Explorer at https://data.memri.io/. 

Here, the reviewer used https://dev.pod.memri.io as the pod to test the following plugins.

## Speech to Text

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/speech-to-text), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Speech-to-text_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/ed071a29758ed037f239c655f841037fb74a7266/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/Speech-to-text_install.MD)

### Usage


## Optical Character Recognition plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/ocr), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [ocr_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/ec6515944863ab1cd0f509bc232f8305dfb6c387/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/ocr_install.MD)

### Usage



## Image Tagging plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/image-tagging), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [image_tagging_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/b9c072df48fac54e4de9c478ab6cb2b9bdf58a11/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/image_tagging_install.MD)

### Usage


## Language translation plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/language-translation), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [language_translation_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/2ce30c60dbd157b92f3c3ff9bb7bca8a50995740/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/language_translation_install.MD)
### Usage


## Semantic search plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/semantic-search), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [semantic_search_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/8de533031367a79c8457419da7c7aa49cbd67267/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/semantic_search_install.MD)

### Usage


## Overall Impression of usage testing

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

## Speech to Text
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [Telegram_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/915a70b7aebfacf894713a13db88e6f8c14950f1/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Telegram_unittest_pass.MD)

## Optical Character Recognition plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [Zeroshot_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/f11b7f6db2b9d13990cc7d08a5c525e08ffd8b46/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Zeroshot_unittest_pass.MD)

## Image Tagging plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [GmailOauth_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/f11b7f6db2b9d13990cc7d08a5c525e08ffd8b46/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/GmailOauth_unittest_pass.MD)

## Language translation plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [LanguageIdentification_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/f11b7f6db2b9d13990cc7d08a5c525e08ffd8b46/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/LanguageIdentification_unittest_pass.MD)

## Semantic search plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [TwitterTopicModel_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/f11b7f6db2b9d13990cc7d08a5c525e08ffd8b46/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/TwitterTopicModel_unittest_pass.MD)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

Overall, for each plugin, the code is clear and readable enough to follow even for someone new to the project. Where context is needed for memory addresses, flags, uncommon imports/utilities, or potentially confusing areas, proper documentation has been added to make clear what is being done.

However, there may be insufficient code-level comments to auto-generate documentation as not every function has been commented. To the uninitiated user, or to a user that is overwhelmed, it could be a source of confusion. Reviewer suggests revisiting the code-level comments and adding in descriptions for every function as well as formatting for autogeneration of documentation as a user convenience.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Overall, the project level documentation for each plugin is sufficient to inform the utility as well as usage process. It is clear, readable, and provides both enough description for how the plugin is to be used, as well as what the plugin is used for. There is clear consistency between each plugin's README as well, providing for uniformity and ease of use as a result of the uniformity.

Requirement | Finding
------------ | -------------
Usage Documented | PASS

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

## Speech to Text
The repository doesn't contain a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability.  It is recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Optical Character Recognition plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Image Tagging plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Language translation plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Semantic search plugin
The repository doesn't contain a CONTRIBUTING and a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations
The Code is generally well-structured and readable, and documentation is added where context is necessary. 

The README instructions for the plugins are clear enough to follow and when everything is properly setup, it is a simple process to use the plugins. 

# Final Conclusion

The project meets the functional requirements and the reviewer was able to confirm that the plugins designed for the current milestone run as expected. The reviewer suggests adding in the missing policies and adding tags to each repository to improve discoverability, as well as more unit testing in general due to the nature of the plugins by testing the checks  for malformed data.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
