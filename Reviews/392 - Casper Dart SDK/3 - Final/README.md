Grant Proposal | [392 - Casper Dart SDK](https://portal.devxdao.com/public-proposals/392)
------------ | -------------
Milestone | 3
Milestone Title | Final Version 
OP | cdolaz
Reviewer | Kien Nguyen

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The Dart SDK is feature complete and fully tested, and has detailed code documentation, appropriate unit test coverage and available as a Dart package via pub.dev

**Acceptance criteria:**

- the Dart SDK is feature complete, including the alpha and beta milestones, and discretionary convenience methods and types
- all unit tests pass
- all methods have detailed Documentation
- the Dart SDK is available as a Dart package via pub.dev

**Additional notes regarding submission from OP:**

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/cdolaz/casper_dart_sdk | fa4dc0e

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/cdolaz/casper_dart_sdk, reviewer was
able to successfully build the source code for this milestone.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

Reviewer also found that the sdk was published at pub.dev
https://pub.dev/packages/casper_dart_sdk

``` sh
casper_dart_sdk git:(main) ✗ dart run build_runner build
[INFO] Generating build script completed, took 559ms
[INFO] Precompiling build script... completed, took 4.8s
[INFO] Building new asset graph completed, took 511ms
[INFO] Checking for unexpected pre-existing outputs. completed, took 4.0s
[INFO] Running build completed, took 8.5s
[INFO] Caching finalized dependency graph completed, took 41ms
[INFO] Succeeded after 8.6s with 56 outputs (130 actions)
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

The README file provides documentation on how to build the project. The usage was added at (https://github.com/cdolaz/casper_dart_sdk/blob/main/doc/usage.md)

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

Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass. The package was also published at pub.dev.


# Final Conclusion

The project provides the functionality described in the grant application, milestone acceptance criteria and also the sdk standard.

# Recommendation

Recommendation | PASS 
------------ | -------------
