Grant Proposal | [392 - Casper Dart SDK](https://portal.devxdao.com/public-proposals/392)
------------ | -------------
Milestone | 1
Milestone Title | Alpha
OP | cdolaz
Reviewer | Kien Nguyen

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Scaffolding of Dart SDK project, public on GitHub, and able to connect to a Casper Node and execute and return response for at least 1 method

**Acceptance criteria:**

- Dart SDK project is available on public GitHub repository
- When instantiated, can connect to a Casper node
- When connected, it can make at least 1 method call and return a response

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/cdolaz/casper_dart_sdk | a49ced1

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/cdolaz/casper_dart_sdk, reviewer was
able to successfully build the source code for this milestone.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

``` sh
casper_dart_sdk git:(main) ✗ dart run build_runner build 
[INFO] Generating build script completed, took 165ms
[INFO] Reading cached asset graph completed, took 27ms
[INFO] Checking for updates since last build completed, took 280ms
[INFO] Running build completed, took 9ms
[INFO] Caching finalized dependency graph completed, took 16ms
[INFO] Succeeded after 29ms with 0 outputs (0 actions)
```

Reviewer found an error while trying to use the SDK in a Flutter web app and reported it to the OP. The OP solved the problem quickly. The SDK is now available in all supported platforms (Web, Android, iOS).

```
http://127.0.0.1:9101?uri=http://127.0.0.1:58201/RVA_FCUz-GM=/
flutter: getPeers
flutter: 18.163.249.168:35000
flutter: 95.216.67.162:35000
flutter: 89.58.25.11:35000
flutter: 65.21.235.219:35000
flutter: 65.21.227.181:35000
flutter: 162.55.6.177:35000
flutter: 88.99.89.209:35000
flutter: 65.108.7.50:35000
flutter: 65.108.42.61:35000
flutter: 94.130.33.181:35000
```


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Reviewer can find unit test for all main and helper functions. The test coverage is good for both positive and negative paths.

[Test Logs](assets/test.json)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Reviewer found that all key functions of the project have low-level code documentation that can be used to automatically generate documentation.

Requirement | Finding
------------ | -------------
Low level function documentation | PASS

### Project Documentation

The README file provides minimum but sufficient documentation on how to build the project and some usages.

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS


# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. The project also has CONTRIBUTING and SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS 
------------ | -------------
