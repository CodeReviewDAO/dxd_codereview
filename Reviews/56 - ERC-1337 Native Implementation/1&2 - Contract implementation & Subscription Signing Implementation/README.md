
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
https://github.com/Rengo-Labs/casper-eip-1337 | 180f2cb

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

Due to the failure at the build step, the reviewer was ot able to continue with the rest of the instructions.

## Overall Impression of usage testing

It was observed that the project fails to build, making it impossible to continue using. However, documentation provides sufficient installation/execution instructions. The project functionality could not be checked.

Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | N/A

# Unit / Automated Testing

The project has extensive tests covering both the positive and the negative paths. However, the reviewer was not ale to run the tests to see their results due to the error encountered at the build step.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A

# Documentation

### Code Documentation

All critical functions have been observed to have standard comments to provide the code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project Documentation was observed to be extensive with sufficient usage documentation and examples.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient, as well as the code-level documentation.

# Open Source Practices

## Licenses

The Project is correctly released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution and a security policy. However, the project lacks a security policy, and the repository doesn't have the relevant tags, hindering its discoverability.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, has extensive tests.

# Final Conclusion

The is generally in a very good shape in terms of open-source guidelines. Moreover, the project has extensive tests, and a sufficient level of documentation. However, the project fails to build by following the given instructions, making it unusable.

Thus, in the reviewers opinion, this submission should fail.

# Recommendation

Recommendation | FAIL
------------ | -------------

