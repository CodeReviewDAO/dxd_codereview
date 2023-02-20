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
After downloading the repository (https://gitlab.memri.io/memri/plugins/telegram/), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Telegram_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Telegram_Install.MD)

### Usage
In order to use the plugin, Telegram API keys had to be obtained. As referenced in the README, the user followed the steps located at (https://core.telegram.org/api/obtaining_api_id) and obtained the necessary keys.

Following that, the user ran the following commands:

```
export TELEGRAM_APP_KEY=$key
export TELEGRAM_APP_SECRET="$secretkey"
run_plugin --metadata "metadata.json" --pod_full_address https://dev.pod.memri.io
```

$key and $secretkey here are placeholders for the actual Telegram API keys. When the reviewer ran the commands, the necessary keys were inputted. Note that the last command is different from the README. Due to the reviewer not being able to run a proper Memri POD due to using a Windows machine, the dev pod was used instead by providing the full address.

The plugin properly generated a QR code to login to the reviewer's Telegram account, as shown below:
![alt text](https://github.com/hoopav/dxd_codereview/blob/45982d869341c0e5f7a8c0963ff053b13721d676/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/telegram_QR.PNG)

Following that, on logging into the datastream explorer, the reviewer confirmed that Telegram account information and messages were added.

![alt_text](https://github.com/hoopav/dxd_codereview/blob/45982d869341c0e5f7a8c0963ff053b13721d676/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/telegram_success.PNG)

## Optical Character Recognition plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/zero-shot-plugin), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .[cli]`

See [Zeroshot_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Zeroshot_Install.MD)

### Usage

To test the plugin, the reviewer followed along and performed the same steps as in the video here: (https://www.loom.com/share/527d14f9d78a4a68ad4a270a30d6099f)

In doing so, the reviewer was able to recreate the same results and confirm the plugin works as intended.

## Image Tagging plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/gmail_oauth), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Gmail_OAuth_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Gmail_OAuth_Install.MD)

### Usage
The reviewer followed the steps to obtain credentials for the Gmail plugin as detailed in the README and was able to successfully obtain the requisite OAuth client ID credentials as a JSON file, as well as set the GMAIL_CLIENT_SECRET_FILE environment variable to the path of the JSON file.

Following that, the reviewer ran the command:

```
run_plugin --metadata "metadata.json" --pod_full_address https://dev.pod.memri.io
```

The reviewer was then able to successfully connect and authenticate with the plugin.

![alt text](https://github.com/hoopav/dxd_codereview/blob/62c8525fadfba1844558cfde5f012ffc565c6b34/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/gmail_success.PNG)

![alt text](https://github.com/hoopav/dxd_codereview/blob/62c8525fadfba1844558cfde5f012ffc565c6b34/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/gmail_success2.PNG)


## Language translation plugin

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/language-identification), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Language_Identification_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Language_Identification_Install.MD)
### Usage

Following the usage instructions (substituting http://0.0.0.0:8008 with the Windows equivalent address) the reviewer was able to spin up the HTTP webserver and then test the plugin by identifying sample languages as seen below:

![alt text](https://github.com/hoopav/dxd_codereview/blob/041e70bc2191aa3fc4f72eb79c8b3ed7d5863600/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/language_identification_success.PNG)

![alt text](https://github.com/hoopav/dxd_codereview/blob/041e70bc2191aa3fc4f72eb79c8b3ed7d5863600/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/language_identification_success2.PNG)

The plugin seems to work as intended for the most part, but obscure languages and romanized sentences of languages with their own characters seem to not register properly. (i.e. the romanized Japanese sentences and the Hmong sentence). However, the reviewer notes that this is due to FastText's model that the plugin is using. In terms of the plugin's strict functionality of being able to handle an inputted text and identifying the language, it works as intended.

## Semantic search plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/twitter-topic-model), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [Twitter_Topic_Model_Install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/fd81ef6ad5644e8262d5f2a0180c48c1d1437ca5/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/Twitter_Topic_Model_Install.MD)

### Usage
Following the usage instructions (substituting http://0.0.0.0:8008 with the Windows equivalent address) the reviewer was able to spin up the HTTP webserver.

![alt text](https://github.com/hoopav/dxd_codereview/blob/b75032369e2a8e9217cd53760afa37d365fe26de/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/2%20-%20Plugins%20Batch%202%20-%20Submission%202/assets/twitter_topic_model_success.PNG)

Then, following the instructions in the video here: (https://www.loom.com/share/138dcbb4c1074364b0bf085bc1678232) the reviewer was able to replicate the results of the test data as well as for the reviewer's own tweets. 

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
