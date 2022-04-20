Grant Proposal | [295 - Casper Scala SDK](https://portal.devxdao.com/public-proposals/295)
------------ | -------------
Milestone | 3
Milestone Title | Scala version of Casper Domain Objects
OP | Mustapha Chad ABAHMANE <elmabahma@gmail.com>
Reviewers | Muhammet Kara & Mateusz Gorski

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Scala version of CLType primitives
- Scala version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects

**Acceptance criteria:**

- Scala version of CLType primitives
- Scala version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects 
- Unit test full coverage

**Additional notes regarding submission from OP:**

For this millestone :
- We have implemented the CLType and CLValue primitives.
- We have implemented Byte serialization standards for CLTypes, CLValue primitives  and Deploy related objects according to : https://caspernetwork.readthedocs.io/en/latest/implementation/serialization-standard.html?highlight=serialization#serialization-standard
- We have have added unit tests for Byte serialization
- We have added more tests for the whole SDK.
- Enhanced the documentation

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/casper-scala-sdk | 070423e1afaf58fb347b873831de63c076b97106

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/caspercommunityio/casper-scala-sdk, reviewer was able to successfully build the source code and run the tests for this milestone on Ubuntu 20.04. The reviewer was also able to install the published maven package of the project (`io.caspercommunity:casper-scala-sdk_3:1.2.1`) as a dependency on a newly created project, and run queries against a node on the Casper Network and get valid responses.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, the project functionality meets/exceeds the acceptance criteria and operates without errors.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has a total number of 212 tests, covering both positive and negative paths. The tests are configured to run automatically by means of automated actions on the repository. Although there are some tests still existing just as a stub, and marked as TODO, the implemented tests are already in very good state, in the reviewer's opinion. The reviewer praises the OP for the extensive coverage of the tests on the project.

[Tests Run](test-run.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The reviewer has observed that the critical functions of the code-base has an acceptable level of code-level documentation by means of standard inline comments which allow auto-generation of the documentation. It was also observed that the project has an already generated copy of this documentation published and publicly reachable and navigatable. However, the reviewer thinks that the code-level documentation on the newly implemented (sicne the previous review) sections of the code-base could be improved with more comprehensive/explanatory comments.

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

The project as committed to GitHub and both the unit tests and the manual tests pass. However, the reviewers would like to point out the following shortcomings in terms of the programming language's best practices. It is highly recommended to fix these points to make sure the project is production-ready.

### Error handling

#### Throwing exceptions.

##### files:
* `RPCCommand.scala`
* `RPCService.scala`
* `HttpRPCService.scala`
* `Crypto.scala`
* `AccountHashDeserializer.scala`
* `CLPublicKeyDeserializer.scala`
* `CLTypeDeserialiser.scala`
* `CLValueDeSerializer.scala`
* `DeployExecutableDeserializer.scala`
* `HashDeserializer.scala`
* `RPCResultDeserializer.scala`
* `SignatureDeserializer.scala`
* `URefDeserializer.scala`
* `JsonConverter.scala`

Throwing an exception is a side-effect and this violates the functional programming paradigm.

Scala does not have a concept of *checked exception*, unlike Java, so using them in Scala code has not only much worse UX but it's more dangerous as `scalac` (Scala compiler) does not provide the safety net that Java does.

Throwing exceptions is not the preferable way of signaling errors in Scala code. Code should return `Try` or `Either` or signal errors via other error Monads. 

In order to incorporate SDK into Scala code, callers will have to use `try { ... } catch { ... } ` blocks which is not only not "idiomatic Scala" but, most importantly, it pushes the responsibility of being aware of the errors to the caller: just from the type definition of a method, caller is not able to recognize which errors it has to handle so he/she has to read the code it's calling all the way down to define how to handle the exceptions. If he/she doesn't do it, it's risking runtime failures due to unhandled exceptions that will bring down the whole app.

Examples of exceptions being thrown that need changing to error types:
1. Methods are throwing exceptions when peers node is not available.
2. In method `send` (`HttpRPCService.scala:56`), `val response = post(...)` might throw an exception but it's not being caught (not part of `try { ... } catch { ...}` clause).
3. In `HttpRPCService.scala:send`, `JsonConverter.toJson` might throw an exception but it is not being handled.
4. Continuing on the above, all JSON manipulation methods can throw exceptions - `JsonConverter.fromJson`, `JsonConverter.toJson`.

**Strong Suggestion:**  Refactor the code to use error-carrying types (like `Try`, `Either`, Error monads or special enums to distinguish various error cases).

**Severity:** HIGH

### Blocking calls

Even though there is a `sendAsync` variant implemented, it's never used. All methods in `CasperSdk` use `send` and are blocking. This may or may not impact the overall performance of the host project.

**Severity:** MEDIUM

### Usage of `Future.apply { ... }`

**file:** `HttpRPCService.scala`

`Future.apply` forks and runs the closure immediately on the call-side. This may lead to unexpected results rather than `IO`-like libraries that describe the computation and leave the execution for later.


**severity:** LOW. `callAsync` is not used.

### Non-standard implementation of JSON (de)serialization.

Authors of Casper SDK chose to use Jackson as JSON (de)serialization library. It uses reflection which means it will fail in runtime rather than compile-time. Note that `fastparse-jackson` throws exceptions as well - which are not handled in the code.

**Severity:** MEDIUM.

**Suggestion:** Usage of native Scala libraries for JSON manipulation: circe, jsoniter-scala.

### Implementation of `Id` Monad.

For the purpose of returning `T` from API methods, the SDK authors implemented an `IdInstance` for `Monad`. Such instance of Monad is not "lawfull" - i.e. does not satisfy Monad laws.

**Severity:** LOW.

**Suggestion:** User proper `Monad` instance and _higher-kinded types_ in SDK API (`def foo[T](): F[T]`).

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. The SDK is well-documented and has extensive automated tests.

However, the reviewers think that there is some room for improvement regarding the code-level documentation of the newly implemented parts of the code-base. Moreover, the reviewers highly suggest that the shortcomings pointed out under the Coding Standards section shall be taken care of to make sure the project is ready for prime time.

Thus, in the reviewers' opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
