Grant Proposal | [295 - Casper Scala SDK](https://portal.devxdao.com/public-proposals/295)
------------ | -------------
Milestone | 4
Milestone Title | Final release of Scala SDK
OP | Mustapha Chad ABAHMANE <elmabahma@gmail.com>
Reviewers | Muhammet Kara & Mateusz Gorski

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- ED25519/SECP256K1 key pairs  Wrappers
- PutDeploy RPC call implemented
- Refactoring Scala SDK calls to return Casper Domaine Specific Objects
- Scala SDK  published as a package via Maven and SBT

**Acceptance criteria:**

- ED25519/SECP256K1 key pairs  Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects
- Scala SDK  available as a package via Maven and SBT
- Unit tests

**Additional notes regarding submission from OP:**

Final milestone with following :
- PuDeploy RPC call implemented
- Casper Keys wrappers and key management via CLPublicKey and KeyPair objects
- full test coverage for casper key management  and Putdeploy RPC call
- Scala SDK is  available in remote repositories for Maven and SBT

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/casper-scala-sdk | [e3f26fa094f8c85f881d56f8e709dfc5cae2e801](https://github.com/caspercommunityio/casper-scala-sdk/commit/e3f26fa094f8c85f881d56f8e709dfc5cae2e801)

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/caspercommunityio/casper-scala-sdk, reviewer was able to successfully build the source code and run the tests for this milestone on Ubuntu 20.04. The reviewer was also able to install the published maven package of the project as a dependency on a newly created project, and run queries against a node on the Casper Network and get valid responses.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, the project functionality meets/exceeds the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total number of 212 tests, covering both positive and negative paths. The tests are configured to run automatically by means of automated actions on the repository. Although the implemented tests are already in very good state, in the reviewer's opinion, **the remaining test stubs marked as TODO should also be implemented for full coverage**, as this is the final milestone of the project.

[Tests Run](test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with Notes
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

The reviewer has observed that the critical functions of the code-base has an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation. It was also observed that the project has an already generated copy of this documentation published and publicly reachable and navigatable. However, the reviewer thinks that **the code-level documentation certain sections of the code-base could be improved with more comprehensive/explanatory comments.**

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Reviewer has observed that the project has detailed documentation for usage with examples, along with the installation, build and test instructions.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository, and the project contains a CONTRIBUTING and a SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

The project as committed to GitHub and both the unit tests and the manual tests pass. However, the reviewers have identified a number of shortcomings and common practice violations specific to the programming language of the project, which would render the project not useful in a production environment. **Reviewers think that these issues must be resolved, for this project to be usable in a production environment.** GitHub issues to provide an easy way to track these points have been created by the reviewers.

* [Swallowing errors and mapping them to None variant.](https://github.com/caspercommunityio/casper-scala-sdk/issues/3)
* [JSON (un)marshalling operations should not return null but instead propagate the failure to the caller.](https://github.com/caspercommunityio/casper-scala-sdk/issues/4)
* [Don't call .get on Option.](https://github.com/caspercommunityio/casper-scala-sdk/issues/8)
* [Don't call .get on Try type.](https://github.com/caspercommunityio/casper-scala-sdk/issues/9)
* [Side-effecting parameterless methods should have parentheses.](https://github.com/caspercommunityio/casper-scala-sdk/issues/2)
* [Simplify the Try to None mapping in HexUtils.scala](https://github.com/caspercommunityio/casper-scala-sdk/issues/5)
* [Remove all print(ln) from the code.](https://github.com/caspercommunityio/casper-scala-sdk/issues/6)
* [Replace Option.apply with Option.](https://github.com/caspercommunityio/casper-scala-sdk/issues/7)
* [Don't report JSON (un)marshalling as RPC no data.](https://github.com/caspercommunityio/casper-scala-sdk/issues/10)

# Final Conclusion

The project mostly provides the functionality described in the grant application and milestone acceptance criteria. The SDK is well-documented and has extensive automated tests except a few test stubs missing implementation.

However, the reviewers think that there is some room for improvement regarding the code-level documentation of certain parts of the code-base. Moreover, the reviewers think that there are a number of issues in the code-base, violating common practices of the language, which makes the project unusable in a production environment.

Thus, in the reviewers' opinion, this submission should fail.

# Recommendation

Recommendation | FAIL
------------ | -------------
