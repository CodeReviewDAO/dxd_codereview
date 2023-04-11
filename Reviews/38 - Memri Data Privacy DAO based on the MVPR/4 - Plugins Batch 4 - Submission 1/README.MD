Grant Proposal | [38 - Memri Data Privacy DAO based on the MVPR](https://portal.devxdao.com/public-proposals/38)
------------ | -------------
Milestone | 4
Milestone Title | Plugins Batch 4 - Submission 1
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

RSS importer
repo https://gitlab.memri.io/memri/plugins/rss-importer
video https://drive.google.com/file/d/1Q4jyaDohW720eG_HfpiiJQ4a7SVH7vW8/view?usp=share_link

Summarization plugin
repo https://gitlab.memri.io/memri/plugins/summarization-plugin
video https://drive.google.com/file/d/1vkdotRaP9X0qAvs6XvsmisQ1aiWhHw1p/view?usp=share_link

Google Calendar Importer
repo https://gitlab.memri.io/memri/plugins/google-calendar/-/tree/v0.1
video  https://drive.google.com/file/d/1bBmrp5p2BwQNnUX1z1ntpcGbgIBmn8Oi/view?usp=share_link

Google Photos Importer
repo https://gitlab.memri.io/experiments/google-photos/-/tree/v0.1
video https://www.loom.com/share/28b9eb1c4283466287e498140cc3b9bb

Mastodon Importer
repo https://gitlab.memri.io/memri/plugins/mastodon
video https://www.loom.com/share/320d4cddd8b541719dba1d1e19680170

## Milestone Submission 

The following milestone assets/artifacts were submitted for review: 

Repository | Revision Reviewed
------------ | -------------
https://gitlab.memri.io/memri/plugins/rss-importer | 754a0f5c3b36fd9815aaa8519349658dce649aa6
https://gitlab.memri.io/memri/plugins/summarization-plugin | e098ad2b19e11497550a9d09b0e4777382d44461
https://gitlab.memri.io/memri/plugins/google-calendar/-/tree/v0.1 | e59b4f1ff8635de50dbdfdc1c2efffca6cfa9902
https://gitlab.memri.io/experiments/google-photos/-/tree/v0.1| f95e11fa236456d35684b754d3ed9f1c2497171f
https://gitlab.memri.io/memri/plugins/mastodon | 2576f0063368011510d071c9889f0d7b67385a23


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
To test the plugin, the reviewer followed along and performed the same steps as in the video here: (https://www.loom.com/share/473300a2332f406fb441635df3ac6a3e)

In doing so, the reviewer was able to recreate the same results and confirm the plugin works as intended.

Accessing Swagger UI:
![alt text](https://github.com/hoopav/dxd_codereview/blob/99367de375c3bf63192c7013c93f482f62794d63/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/speech-to-text_webservice.PNG)

Testing Endpoint: 
![alt text](https://github.com/hoopav/dxd_codereview/blob/99367de375c3bf63192c7013c93f482f62794d63/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/speech-to-text_webservice2.PNG)


## Optical Character Recognition plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/ocr), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [ocr_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/ec6515944863ab1cd0f509bc232f8305dfb6c387/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/ocr_install.MD)

### Usage
To test the plugin, the reviewer followed along and performed the same steps as in the video here: (https://www.loom.com/share/3788bd6b50b0422cb462567f89ebc899)

In doing so, the reviewer was able to recreate the same results and confirm the plugin works as intended.

Results:
![alt text](https://github.com/hoopav/dxd_codereview/blob/41c382c8eee44982e6b4731b297efd61a9b86c57/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/ocr_success.PNG)


## Image Tagging plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/image-tagging), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [image_tagging_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/b9c072df48fac54e4de9c478ab6cb2b9bdf58a11/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/image_tagging_install.MD)

### Usage
To test the plugin, the reviewer followed along and performed the same steps as in the video here: (https://drive.google.com/file/d/1UAFk3wsa2NdZAh6SuBEcDDaaGfsuEV1Q/view?usp=share_link)

In doing so, the reviewer was able to recreate the same results and confirm the plugin works as intended.

Accessing Swagger UI:
![alt text](https://github.com/hoopav/dxd_codereview/blob/99367de375c3bf63192c7013c93f482f62794d63/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/image_tagging_swaggerUI.PNG)

Testing Image tagging:
![alt text](https://github.com/hoopav/dxd_codereview/blob/main/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/image_tagging_success.PNG)


## Language translation plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/language-translation), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [language_translation_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/2ce30c60dbd157b92f3c3ff9bb7bca8a50995740/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/language_translation_install.MD)
### Usage
To test the plugin, the reviewer followed along and performed the same steps as in the video here: (https://drive.google.com/file/d/1HGz6jgn6E5puYKqw76Emd7KhKKNwTYF5/view?usp=share_link)

In doing so, the reviewer was able to recreate the same results and confirm the plugin works as intended.

## Semantic search plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/semantic-search), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [semantic_search_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/8de533031367a79c8457419da7c7aa49cbd67267/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/semantic_search_install.MD)

### Usage
To test the plugin, the reviewer followed along and performed the same steps as in the video here: (https://drive.google.com/file/d/1GNtot4vma2cVV17D7wOTbhO1cHmLjieh/view?usp=share_link)

In doing so, the reviewer was able to recreate the same results and confirm the plugin works as intended.

Accessing Swagger UI:
![alt text](https://github.com/hoopav/dxd_codereview/blob/21130b3f50756fc6e34e7a1a3006e6737aba303f/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/semantic_swaggerUI.PNG)

Testing plugin with demo:
![alt text](https://github.com/hoopav/dxd_codereview/blob/21130b3f50756fc6e34e7a1a3006e6737aba303f/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/semantic_demoSuccess.PNG)


## Overall Impression of usage testing

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

## Speech to Text
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [speech-to-text_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/b007ff798957b38771b2b5cb23de8a436340cc03/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/speech-to-text_unittest_pass.MD)

## Optical Character Recognition plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [ocr_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/d8f584b1f3ceeeef40378962d061a5d71bad1736/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/ocr_unittest_pass.MD)

## Image Tagging plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [image_tagging_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/d8f584b1f3ceeeef40378962d061a5d71bad1736/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/image_tagging_unittest_pass.MD)

## Language translation plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. The provided unit test failed to pass. However, the Reviewer notes that it appears to be due to an incorrect import statement that is an easy fix. Despite this, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [language_translation_unittest_fail.MD](https://github.com/hoopav/dxd_codereview/blob/d8f584b1f3ceeeef40378962d061a5d71bad1736/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/language_translation_unittest_fail.MD)

## Semantic search plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [semantic_search_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/d8f584b1f3ceeeef40378962d061a5d71bad1736/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/3%20-%20Plugins%20Batch%203%20-%20Submission%201/assets/semantic_search_unittest_pass.MD)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
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
The repository doesn't contain a CONTRIBUTING or a SECURITY  policy. The repository also lacks relevant tags, hindering its discoverability.  It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

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
