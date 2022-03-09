
Grant Proposal | [56 - ERC-1337 Native Implementation](https://portal.devxdao.com/public-proposals/56)
------------ | -------------
Milestone | 1 & 2
Milestone Title | Contract implementation & Subscription Signing Implementation
OP | CaptainBernardo
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the first and the second milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The following functional contract calls will be functional:

- isSubscriptionActive
- getSubscriptionHash
- isSubscriptionReady
- cancelSubscription
- executeSubscription

Furthermore, a test suite will be created to demonstrate these calls are functional. These points will be delivered approximately 7 weeks after grant acceptance.

The following functional contract calls will be functional:

- getSubscriptionSigner

Furthermore, a test suite will be created to demonstrate these calls are functional. These points will be delivered approximately 2 weeks after the previous milestone's completion. This milestone is subject to some uncertainty, as it directly relies upon some Casper signing semantics not changing. Casper semantics have changed in recent memory, so it is possible some extra work may be required.

**Acceptance criteria:**

- Subscription calls are functional
- Test suite quantitatively proves the functionality
- Code is delivered in native RUST

- Subscription call is functional
- Any signing standard work that needs to be completed to support this is done (May require extra work to implement if Casper's standards change somehow)

**Additional notes regarding submission from OP:**
Tests and documentation are completed that demonstrate all functionality. 

What is being submitted is the closest we could approximate EIP-1337.  There were several limitations on the port.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/casper-eip-1337 | 93854d5 & df37046

# Install & Usage Testing Procedure and Findings

The reviewer followed the instructions on the README of the project to set it up, deploy to the Testnet, and test its functionality. The procedure was carried out on Ubuntu 20.04.

It was seen that the link to the documentation at the `Install the rust environment and casper client` step was broken. Reviewer was able to find the resource by himself by navigating through the official Casper documentation to install the prerequisites.

Reviewer then attempted to build the project by issuing the commands given on the README, but encountered a failure at the `make build-contract` step:

```bash
$ make build-contract
cargo build --release -p casper-contract-eip-1337 --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/casper-contract-eip-1337/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/subscription_hash_signer/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
error: failed to download `uint v0.9.3`

Caused by:
  unable to get packages from source

Caused by:
  failed to parse manifest at `/workspace/.cargo/registry/src/github.com-1ecc6299db9ec823/uint-0.9.3/Cargo.toml`

Caused by:
  feature `edition2021` is required

  consider adding `cargo-features = ["edition2021"]` to the manifest
make: *** [Makefile:5: build-contract] Error 101
```

Due to the failure at the build step, the reviewer was not able to continue with the rest of the instructions. Nonetheless, after some research, it was revealed that the error was due to a recent upgrade on one of the reviewed project's dependencies, which is not in the OP's control. Then the OP acted on the newly found information, and quickly fixed the error on the project, allowing the reviewer to continue with the rest of the review.

After the fixes by the OP, the reviewer was able to successfully build the [smart contract(s)](assets/build.md) and the [signer utility](assets/build-signer-utility.md), and observed that all of the automated [tests pass](assets/test.md).

Then the reviewer deployed an ERC20 contract on the Testnet to be able to use for testing, and deployed and tested the project by following the given instructions, after a number of improvements by the OP on the instructions based on the reviewer's further feedback.

* Deploy the contract: https://testnet.cspr.live/deploy/7a6d68ccb376b7cc3921a8d840c9c65dd5f4b94b09dfa2d0c2977abb3c729fae
* Approve spending: https://testnet.cspr.live/deploy/b3ef92f04f9933adb6495147dcd56901f053ecdb650b756b99e3004a0a129678
* Approve again to raise the spending limit: https://testnet.cspr.live/deploy/b015a2389bed7d825a914f089eb877b1c95b1d8696af3e49c9176fe34311811d
* Create the subscription hash: https://testnet.cspr.live/deploy/a193748f6620dcb7d480eb081357feae932016b1b5c03da06ba12b3639c89964
* Execute the subscription payment: https://testnet.cspr.live/deploy/43adfdf904b53670adc1f3049597e53710019d314715563e2e50c36226375ef1
* Cancel the subscription: https://testnet.cspr.live/deploy/f818d5230434a1dde896f74dc436568bbf37fb056d3555081a0e9e9fb29dc9ff
* Payment attempt after cancellation (fails as expected): https://testnet.cspr.live/deploy/41ee6e744d4864df1a8c5ff27ab9bfc7c11b15d39b19c9fb503c750dd40b1f0f


## Overall Impression of usage testing

It was observed that the project builds and passes the automated tests successfully after the quick fixes by the OP, and the documentation provides sufficient installation/execution instructions. However, the reviewer thinks that the documentation still has room for improvement towards further simplicity, clear explanations and sampel commands.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has sufficient tests covering both the positive and the negative paths. The reviewer observed that all of the tests successfully pass.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

All critical functions have been observed to have standard comments to provide the code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project Documentation was observed to be acceptable with usage documentation and examples. However, the reviewer thinks that more examples and use cases would be highly beneficial for the users of the project.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are at an acceptable state, with room for further improvements. The code-level documentation is sufficient.

The reviewer communicated the shortcomings of the documentation, along with further points of possible improvements which may not fall in the scope of this review, with the OP. OP acknowledged the feedback, and showed interest in working on further improvements.

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution policy. However, the project lacks a security policy, and the repository doesn't have the relevant tags, hindering its discoverability.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and has extensive tests.

# Final Conclusion

The project is generally in a very good shape in terms of open-source guidelines. Moreover, the project has extensive tests, and a sufficient level of documentation. The project also successfully builds and passes both the manual and the automated tests, providing the promised functionality. However, the project documentation can be improved further based on the notes in teh relevant sections of this review.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------

