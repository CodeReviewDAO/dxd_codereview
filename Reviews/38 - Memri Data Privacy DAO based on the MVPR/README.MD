Grant Proposal | [38 - Memri Data Privacy DAO based on the MVPR](https://portal.devxdao.com/public-proposals/38)
------------ | -------------
Milestone | 5
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
https://gitlab.memri.io/memri/plugins/rss-importer | 77c6587da90c1f142b9e6f9f154b61056416dd2a
https://gitlab.memri.io/memri/plugins/summarization-plugin | 2a59397b230781e75be45acd6ede505223561aea
https://gitlab.memri.io/memri/plugins/google-calendar/-/tree/v0.1 | b262a6ea6c99e81a1aa34ddbb8169774fdc995d2
https://gitlab.memri.io/memri/plugins/google-photos/-/tree/v0.2 | 0b16a3ed86ba5c2803324589e5b69fc5983744b3
https://gitlab.memri.io/memri/plugins/mastodon | c35d2a8fd8f77127031119baa857692ffcc589c6


# Install & Usage Testing Procedure and Findings

## General Notes
It is presumed that the user of the plugins is familiar with the process of setting up a Memri POD as well as examining data in the Memri Datastream Explorer at https://data.memri.io/. 

Here, the reviewer used https://dev.pod.memri.io as the pod to test the following plugins.

## RSS importer

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/rss-importer), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [rss-importer_install_1.MD for install output](https://github.com/hoopav/dxd_codereview/blob/8fd7732ed555a7872c8f50cfdcef61853b0c0273/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss-importer_install_1.md)

The plugin installed successfully. However, when the reviewer tried to install scraping using the instructions provided in the README, the installation failed.

See [rss-importer_install_2.MD for install output](https://github.com/hoopav/dxd_codereview/blob/960aa6ceffa2e51db455079f224adf2ccb0afe1b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss-importer_install_2.md)

The reviewer had to search for an answer, and the instructions on the plugin README were incorrect. 
After trying and failing to install scraping according to the instructions, reviewer installed 
the referenced Postlight parser on a global level using the command:

`yarn add @postlight/parser`

### Usage
To test the plugin, the reviewer attempted to follow along and performed the same steps as in the referenced video, but the video restricted access and the reviewer could not confirm the steps.  

Instead, the reviewer followed the README instructions and attempted to run the plugin accordingly.

Rather than the suggested command:
`run_plugin --metadata "metadata.json"`

The reviewer ran the plugin with:
`run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"`

This was to use a working pod instead of attempting to handle potential cross OS compatibility issues in setting up a pod.

The output from running the plugin is recorded in rss-importer_run.MD and the results of importing 
data to the pod can be seen in rss_pod_results.PNG

The reviewer was not able to test "Run with scraping" in the instructions due to a failure to install the Postlight API as instructed.

The reviewer was not able to test the Plugin Endpoints as instructed using 
`http://0.0.0.0:8010/docs`

However, the reviewer was able to test the Plugin Endpoints using 
`http://localhost:8080/docs`

#### Get Feeds
![alt text](https://github.com/hoopav/dxd_codereview/blob/960aa6ceffa2e51db455079f224adf2ccb0afe1b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss_get_feeds.PNG)

#### Add Feed
![alt text](https://github.com/hoopav/dxd_codereview/blob/960aa6ceffa2e51db455079f224adf2ccb0afe1b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss_add_feed.PNG)
![alt text](https://github.com/hoopav/dxd_codereview/blob/960aa6ceffa2e51db455079f224adf2ccb0afe1b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss_added_feed.PNG)

#### Deactivate Feed
![alt text](https://github.com/hoopav/dxd_codereview/blob/960aa6ceffa2e51db455079f224adf2ccb0afe1b/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss_deactivate_feed.PNG)

## Summarization plugin

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/summarization-plugin), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

`pip install -e .`

See [summarization_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/summarization_install.md)

### Usage
To test the plugin, the reviewer attempted to follow along and performed the same steps as in the referenced video, but the video restricted access and the reviewer could not confirm the steps.  

Instead, the reviewer followed the README instructions and attempted to run the plugin accordingly.

Rather than the suggested command:
`run_plugin --metadata "metadata.json"`

The reviewer ran the plugin with:
`run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"`

See [summarization_run.MD for command output](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/summarization_run.md)

Results:
The reviewer was not able to test the Web API endpoints as instructed using 
`http://0.0.0.0:8008/docs`

However, the reviewer was able to test the endpoints using 
`http://localhost:8080/docs`

#### Web API 
![alt_text](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/summarization_webapi.PNG)

The Web API appears to work as intended. However, due to the failure to perform scraping with the RSS plugin, the reviewer could not properly test the output for summarize as there was no data to summarize.


## Google Calendar Importer

### Install 
After downloading the repository (https://gitlab.memri.io/memri/plugins/google-calendar/-/tree/v0.1), the reviewer followed the installation process in the README.

First, the reviewer created a google cloud project and enabled the API.

Then the reviewer created and loaded credentials for the API as instructed using:
```
    export GOOGLE_CLIENT_ID="..."
    export GOOGLE_CLIENT_SECRET="..."
    export PROJECT_ID="..."
```

while replacing "..." with the reviewer's credentials.

Following that, the reviewer created a virtual environment and activated the virtual environment with:
`python -m venv env`

and

`"env\Scripts\activate"`

The first command is different from the one listed in the README instructions due to the reviewer having
python3 installed as the default python, thus allowing 'python' over 'python3'. The second is different
because the reviewer is testing on a Windows machine, and the command is the equivalent of the one listed
in the README.

Next, the reviewer installed all dependencies with:

`pip install -r requirements.txt'

Again, changing 'pip3' to 'pip' because python3 is the reviewer's default python.

### Usage
To test the plugin, the reviewer ran the plugin with:
`run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"`

using the hosted pod to test.

The command output is in [g_calendar_run.md.](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/g_calendar_run.md)

The Oauth authentication flow worked successfully, as seen below.
![alt_text](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/g_calendar_successOauth.PNG)

The reviewer's google calendar was successfully imported, as seen below.
![alt_text](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/g_calendar_successImport1.PNG)
![alt_text](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/g_calendar_successImport2.PNG)

## Google Photos Importer

### Install 
When the reviewer began testing, the repository listed on the job lead to a 404 page, and the 
Google Photos Importer plugin repository at https://gitlab.memri.io/memri/plugins/google-photos 
was empty. As a result, the reviewer could not install or test this plugin. 

Through discussion with the developer, the issue was resolved and the listed url 
allowed access to the repository for the reviewer to test the plugin. In addition, the repository
for the latest build of the plugin was provided. (https://gitlab.memri.io/memri/plugins/google-photos/-/tree/v0.2)

After downloading the repository, the reviewer followed the installation process in the README.

First, the reviewer created a google cloud project and enabled the API.

Then the reviewer created and loaded credentials for the API as instructed using:
```
    export GOOGLE_CLIENT_ID="..."
    export GOOGLE_CLIENT_SECRET="..."
    export PROJECT_ID="..."
```

while replacing "..." with the reviewer's credentials.

Following that, the reviewer created a virtual environment and activated the virtual environment with:
`python -m venv env`

and

`"env\Scripts\activate"`

The first command is different from the one listed in the README instructions due to the reviewer having
python3 installed as the default python, thus allowing 'python' over 'python3'. The second is different
because the reviewer is testing on a Windows machine, and the command is the equivalent of the one listed
in the README.

### Usage
To test the plugin, the reviewer ran the plugin with:
`run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"`

using the hosted pod to test.

However, this resulted in errors, as seen in [gphotos_run_output.MD.](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/gphotos_run_output.MD)

After some analysis, it turned out this was because the README instructions did not instruct to install
the plugin after setting up the google cloud application and virtual environment.

To make the plugin work, the reviewer installed the plugin with:

`pip install -e .`

Following that, the reviewer was able to successfully run the program with:
`run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json`

The output for the run can be seen in [gphotos_import_run.MD.](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/gphotos_import_run.MD)

The Oauth authhorization was successful, as seen below.
![alt_text](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/g_photo_successOauth.PNG)

In addition, the photo import was successful. The reviewer used an account with a single photo,
and that photo's entry can be seen reflected in the pod data viewer below.
![alt_text](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/g_photo_successImport.PNG)



## Mastodon Importer

### Install
After downloading the repository (https://gitlab.memri.io/memri/plugins/mastodon), the reviewer followed the installation process in the README by opening a terminal in the downloaded repository and running the command: 

```
    pip install -e .[dev]
    pre-commit install
```

See [mastodon_install.MD for install output](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/mastodon_install.MD)

Following that, the reviewer setup the required Twitter credentials according to the README
instructions. 

However, on using 

`twitter-oauth --pod dev`

as instructed, the reviewer met with a Traceback error stating a module 'twitter_v2' was not found.

At first, the reviewer believed this to be the newest version of Twitter's python API and updated
accordingly. However, the error persisted.

After a bit of research, the reviewer determined that the error was due to not having installed 
Memri's twitter-v2 plugin located here: (https://gitlab.memri.io/memri/plugins/twitter-v2)

On review of the video to help with installation and running of the plugin (https://www.loom.com/share/320d4cddd8b541719dba1d1e19680170) the reviewer realized that 
the README for the plugin is completely incorrect. The current README appears to be for 
the twitter-v2 plugin referenced above and has not been changed to reflect the proper plugin.

### Usage
To test the plugin, the reviewer followed along with the steps in the video (https://www.loom.com/share/320d4cddd8b541719dba1d1e19680170).

After the initial hurdle of the incorrect README in the repository, the reviewer was 
able to recreate the same results and confirm the plugin works as intended.



## Overall Impression of usage testing

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS with Notes

# Unit / Automated Testing

## RSS importer
There is positive path testing and negative path testing with sample dummy data. See [rss-importer_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/rss-importer_unittest_pass.MD)

## Summarization plugin
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [summarization_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/summarization_unittest_pass.MD)

## Google Calendar Importer
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [google_calendar_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/google_calendar_unittest_pass.MD)

## Google Photos Importer
There is positive path testing with sample dummy data, but no negative path testing with malformed data as might be expected from this sort of plugin. However, as the core functionality works with the data that Reviewer imported in the usability testing, Reviewer suggests PASS with Notes. See [google_photos_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/google_photos_unittest_pass.MD)

## Mastodon Importer
There is positive path testing and negative path testing with sample dummy data. See [mastodon_unittest_pass.MD](https://github.com/hoopav/dxd_codereview/blob/536510883ba0790888c5a19ee3032be7f5122620/Reviews/38%20-%20Memri%20Data%20Privacy%20DAO%20based%20on%20the%20MVPR/4%20-%20Plugins%20Batch%204%20-%20Submission%201/assets/mastodon_unittest_pass.MD)

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

The exception is the Mastodon plugin, but as it appears from the video that a corrected README exists, 
it should be a simple fix.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes

## Overall Conclusion on Documentation

The reviewer concludes that the project has sufficient and comprehensive general documentation.

# Open Source Practices

## Licenses

The required license for these plugins is the Memri Privacy Preserving License. This license is present in the repositories of each plugin except the Google Calendar plugin, which is currently the Mozilla Public License Version 2.0. Although the Memri Privacy Preserving License is a Mozilla Public License, this should be fixed to be in compliance with Memri's policies.

Requirement | Finding
------------ | -------------
Memri Privacy Preserving License | PASS with Notes

## Contribution Policies

Issues are enabled for all the plugin repositories, but Pull requests are not.

## RSS importer
The repository doesn't contain a CONTRIBUTING or a SECURITY  policy. The repository also lacks relevant tags, hindering its discoverability.  It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Summarization plugin
The repository doesn't contain a CONTRIBUTING or a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Google Calendar Importer
The repository doesn't contain a CONTRIBUTING or a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Google Photos Importer
The repository doesn't contain a CONTRIBUTING or a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

## Mastodon Importer
The repository doesn't contain a CONTRIBUTING or a SECURITY policy. The repository also lacks relevant tags, hindering its discoverability. It is recommended to add a CONTRIBUTING policy so that future contributors may know how to contribute to the plugin. It is also recommended to add a SECURITY policy so that users who discover vulnerabilities know the proper procedure to report the issue, as well as if the plugin is being supported.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations
The Code is generally well-structured and readable, and documentation is added where context is necessary. 

The README instructions for the plugins are clear enough to follow and when everything is properly setup, it is a simple process to use the plugins. 

# Final Conclusion

The project meets the functional requirements and the reviewer was able to confirm that the plugins designed for the current milestone run as expected. The reviewer suggests adding in the missing policies and adding tags to each repository to improve discoverability, as well as more unit testing in general due to the nature of the plugins by testing the checks for malformed data. The reviewer also suggests 
updating the Mastodon README to match what was shown in the video.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------