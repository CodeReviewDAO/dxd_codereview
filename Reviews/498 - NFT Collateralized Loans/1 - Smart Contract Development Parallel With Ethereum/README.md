Grant Proposal | [NFT Collateralized Loans](https://portal.devxdao.com/public-proposals/498)
------------ | -------------
Milestone | 1
Milestone Title | Smart Contract Development Parallel With Ethereum
OP | CaptainBernardo
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**


Deliverables
Some of this grant will go to pay for common RnD between both the Casper and Solana versions.
NFT Locker Contract
Contains NFT locking
Contains loan logic 
Contains defaulting logic
NFT Locker Factory
Deploys the locker contracts
We will add support for extended CEP47 -> ERC1155 via gap analysis
Documentation & Tests

**Acceptance criteria:**

Users can put up an NFT for collateral
Counter parties can make loans
Users can make payments
Counter parties can automatically get the NFT if a default occurs

CRDAO: Verification for this will be as a suite of unit tests for each contract.

**Additional notes regarding submission from OP:**

Completed per criteria

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-LiquidNFT | eb03989

# Install & Usage Testing Procedure and Findings

The reviewer followed the instructions on the README of the project to set it up, deploy to the Testnet, and test its functionality by running the end-to-end tests. The procedure was carried out on Ubuntu 20.04.

At the first attempts of following the instructions, the reviewer encountered a number of issues/errors, mostly at the documentation level, causing the project to be not buildable/deployable/usable, which would normally result in a review with a FAIL recommendation. The reviewer provided the OP with the feedback coming out of these attempts. The OP fixed & improved the project and its documentation based on the feedback, and informed the reviewer that the project is now ready to be reviewed. The review presented here covers the latest version of the project which includes all of those fixes and the improvements.

Since the OP did not provide an application with a UI which utilizes the smart contracts in the project, and the acceptance criteria of the milestone specifically instructs the CRDAO to do the verifications based on unit tests, the usage testing part of this review focuses on the unit and the end-to-end tests.

Reviewer first installed the prerequisites by following the instructions on the main README, and then built and deployed the smart contracts by following the instructions on the README under the `Contracts` directory. Afterwards, the reviewer ran all unit tests again by following the instructions under the `Contracts` directory. Lastly, the reviewer ran the end-to-end tests by using the scripts provided under the `JsClients` directory.

Below are the test-run logs from the latest CI job as of this review was written. The rest of the logs can be found under the [assets](assets) directory.

```
make test-liquid-factory && make test-liquid-helper && make test-liquid-locker
make[1]: Entering directory '/home/circleci/project'
make build-contract-liquid-factory && make copy-wasm-file-liquid-factory && make test-only-liquid-factory
make[2]: Entering directory '/home/circleci/project'
cargo build --release -p liquid-factory -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
warning: unnecessary parentheses around method argument
   --> Contracts/liquid-locker/liquid-locker-crate/src/liquid_locker.rs:216:21
    |
216 |                     (prepay_amount
    |                     ^
217 |                         .checked_div(epoch_payback)
218 |                         .unwrap_or_revert_with(Error::LiquidLockerDivision0)),
    |                                                                             ^
    |
    = note: `#[warn(unused_parens)]` on by default
help: remove these parentheses
    |
216 ~                     prepay_amount
217 |                         .checked_div(epoch_payback)
218 ~                         .unwrap_or_revert_with(Error::LiquidLockerDivision0),
    |

warning: `liquid-locker-crate` (lib) generated 1 warning
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/home/circleci/project'
make[2]: Entering directory '/home/circleci/project'
cp target/wasm32-unknown-unknown/release/liquid-factory.wasm Contracts/liquid-factory/liquid-factory-tests/wasm
cp target/wasm32-unknown-unknown/release/erc20-token.wasm Contracts/liquid-factory/liquid-factory-tests/wasm
cp target/wasm32-unknown-unknown/release/cep47-token.wasm Contracts/liquid-factory/liquid-factory-tests/wasm
make[2]: Leaving directory '/home/circleci/project'
make[2]: Entering directory '/home/circleci/project'
cargo test -p liquid-factory-tests
 Downloading crates ...
  Downloaded casper-engine-test-support v2.1.0
  Downloaded casper-execution-engine v1.5.0
   Compiling proc-macro2 v1.0.43
   Compiling unicode-ident v1.0.4
   Compiling quote v1.0.21
   Compiling syn v1.0.99
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.132
   Compiling serde_derive v1.0.144
   Compiling typenum v1.15.0
   Compiling serde v1.0.144
   Compiling cfg-if v1.0.0
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.85
   Compiling fastrand v1.8.0
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling remove_dir_all v0.5.3
   Compiling ryu v1.0.11
   Compiling cpufeatures v0.2.5
   Compiling schemars v0.8.5
   Compiling bit-vec v0.6.3
   Compiling itoa v1.0.3
   Compiling bitflags v1.3.2
   Compiling once_cell v1.14.0
   Compiling hashbrown v0.12.3
   Compiling fnv v1.0.7
   Compiling quick-error v1.2.3
   Compiling regex-syntax v0.6.27
   Compiling static_assertions v1.1.0
   Compiling dyn-clone v1.0.9
   Compiling lazy_static v1.4.0
   Compiling quick-error v2.0.1
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.0
   Compiling cc v1.0.73
   Compiling pkg-config v0.3.25
   Compiling thiserror v1.0.35
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling either v1.8.0
   Compiling anyhow v1.0.65
   Compiling wee_alloc v0.4.5
   Compiling memory_units v0.4.0
   Compiling pin-project-lite v0.2.9
   Compiling cfg-if v0.1.10
   Compiling match_cfg v0.1.0
   Compiling downcast-rs v1.2.0
   Compiling memory_units v0.3.0
   Compiling iana-time-zone v0.1.48
   Compiling linked-hash-map v0.5.6
   Compiling tracing-core v0.1.29
   Compiling bit-set v0.5.3
   Compiling itertools v0.10.4
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling rand_chacha v0.2.2
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling indexmap v1.9.1
   Compiling num-iter v0.1.43
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling lmdb-sys v0.8.0
   Compiling getrandom v0.2.7
   Compiling tempfile v3.3.0
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.44
   Compiling hostname v0.3.1
   Compiling rand_core v0.6.4
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling wasmi-validation v0.3.0
   Compiling rand v0.8.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling chrono v0.4.22
   Compiling proptest v1.0.0
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.2
   Compiling schemars_derive v0.8.5
   Compiling datasize_derive v0.2.10
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.23
   Compiling thiserror-impl v1.0.35
   Compiling tracing-attributes v0.1.22
   Compiling casper_types_derive v0.1.0
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling tracing v0.1.36
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.7
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling uint v0.9.3
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casper-execution-engine v1.5.0
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-engine-test-support v2.1.0
   Compiling test-env v0.1.0 (/home/circleci/project/Contracts/utils/test-env)
   Compiling liquid-factory-tests v0.2.1 (/home/circleci/project/Contracts/liquid-factory/liquid-factory-tests)
warning: unused import: `BlockTime`
 --> Contracts/liquid-factory/liquid-factory-tests/src/liquid_factory_tests.rs:3:56
  |
3 | use casper_types::{account::AccountHash, runtime_args, BlockTime, Key, RuntimeArgs, U256};
  |                                                        ^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default
help: consider adding a `#[cfg(test)]` to the containing module
 --> Contracts/liquid-factory/liquid-factory-tests/src/lib.rs:2:1
  |
2 | pub mod liquid_factory_tests;
  | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `self`
 --> Contracts/liquid-factory/liquid-factory-tests/src/liquid_factory_instance.rs:1:17
  |
1 | use std::time::{self, SystemTime};
  |                 ^^^^

warning: unused variable: `env`
   --> Contracts/liquid-factory/liquid-factory-tests/src/liquid_factory_tests.rs:301:9
    |
301 |         env,
    |         ^^^ help: if this is intentional, prefix it with an underscore: `_env`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `lockers_contract_address`
   --> Contracts/liquid-factory/liquid-factory-tests/src/liquid_factory_tests.rs:306:9
    |
306 |         lockers_contract_address,
    |         ^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_lockers_contract_address`

warning: `liquid-factory-tests` (lib test) generated 4 warnings
    Finished test [unoptimized + debuginfo] target(s) in 59.19s
     Running unittests src/lib.rs (target/debug/deps/liquid_factory_tests-549f99a6eb4f8f92)

running 9 tests
test liquid_factory_tests::test_update_master ... ok
test liquid_factory_tests::test_revoke_master ... ok
test liquid_factory_tests::test_create_empty_locker ... ok
test liquid_factory_tests::test_donate_to_locker ... ok
test liquid_factory_tests::test_create_liquid_locker ... ok
test liquid_factory_panic_tests::should_not_be_able_to_contribute_after_contribution_phase_end - should panic ... ok
test liquid_factory_tests::test_contribute_to_locker ... ok
test liquid_factory_flow_test::should_be_able_to_liquadate_locker_as_owner_didnt_do_payment_for_days ... ok
test liquid_factory_tests::test_payback_to_locker ... ok

test result: ok. 9 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 17.33s

   Doc-tests liquid-factory-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/home/circleci/project'
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
make build-contract-liquid-helper && make copy-wasm-file-liquid-helper && make test-only-liquid-helper
make[2]: Entering directory '/home/circleci/project'
cargo build --release -p liquid-helper -p liquid-helper-proxy --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/home/circleci/project'
make[2]: Entering directory '/home/circleci/project'
cp target/wasm32-unknown-unknown/release/liquid-helper.wasm Contracts/liquid-helper/liquid-helper-tests/wasm
cp target/wasm32-unknown-unknown/release/liquid-helper-proxy.wasm Contracts/liquid-helper/liquid-helper-tests/wasm
make[2]: Leaving directory '/home/circleci/project'
make[2]: Entering directory '/home/circleci/project'
cargo test -p liquid-helper-tests
 Downloading crates ...
  Downloaded casperlabs-test-env v0.1.0
   Compiling casperlabs-test-env v0.1.0
   Compiling liquid-helper-tests v0.2.1 (/home/circleci/project/Contracts/liquid-helper/liquid-helper-tests)
    Finished test [unoptimized + debuginfo] target(s) in 7.39s
     Running unittests src/lib.rs (target/debug/deps/liquid_helper_tests-d544d4c8b874091c)

running 15 tests
test liquid_helper_tests::test_deploy ... ok
test liquid_helper_tests::liquidate_to ... ok
test liquid_helper_tests::ownerless_locker ... ok
test liquid_helper_tests::floor_not_reached ... ok
test liquid_helper_tests::not_single_provider ... ok
test liquid_helper_tests::time_since ... ok
test liquid_helper_tests::starting_timestamp ... ok
test liquid_helper_tests::reached_total ... ok
test liquid_helper_tests::payment_time_not_set ... ok
test liquid_helper_tests::below_floor_asked ... ok
test liquid_helper_tests::missed_deadline ... ok
test liquid_helper_tests::missed_activate ... ok
test liquid_helper_tests::contribution_phase ... ok
test liquid_helper_tests::payback_timestamp ... ok
test liquid_helper_tests::get_tokens ... ok

test result: ok. 15 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 4.06s

   Doc-tests liquid-helper-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/home/circleci/project'
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
make build-contract-liquid-locker && make copy-wasm-file-liquid-locker && make test-only-liquid-locker
make[2]: Entering directory '/home/circleci/project'
cargo build --release -p liquid-locker -p liquid-locker-proxy -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
warning: unnecessary parentheses around method argument
   --> Contracts/liquid-locker/liquid-locker-crate/src/liquid_locker.rs:216:21
    |
216 |                     (prepay_amount
    |                     ^
217 |                         .checked_div(epoch_payback)
218 |                         .unwrap_or_revert_with(Error::LiquidLockerDivision0)),
    |                                                                             ^
    |
    = note: `#[warn(unused_parens)]` on by default
help: remove these parentheses
    |
216 ~                     prepay_amount
217 |                         .checked_div(epoch_payback)
218 ~                         .unwrap_or_revert_with(Error::LiquidLockerDivision0),
    |

warning: `liquid-locker-crate` (lib) generated 1 warning
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/home/circleci/project'
make[2]: Entering directory '/home/circleci/project'
cp target/wasm32-unknown-unknown/release/liquid-locker.wasm Contracts/liquid-locker/liquid-locker-tests/wasm
cp target/wasm32-unknown-unknown/release/liquid-locker-proxy.wasm Contracts/liquid-locker/liquid-locker-tests/wasm
cp target/wasm32-unknown-unknown/release/cep47-token.wasm Contracts/liquid-locker/liquid-locker-tests/wasm
cp target/wasm32-unknown-unknown/release/erc20-token.wasm Contracts/liquid-locker/liquid-locker-tests/wasm
make[2]: Leaving directory '/home/circleci/project'
make[2]: Entering directory '/home/circleci/project'
cargo test -p liquid-locker-tests
   Compiling liquid-locker-tests v0.1.0 (/home/circleci/project/Contracts/liquid-locker/liquid-locker-tests)
    Finished test [unoptimized + debuginfo] target(s) in 4.70s
     Running unittests src/lib.rs (target/debug/deps/liquid_locker_tests-82874e0502716f7c)

running 16 tests
test liquid_locker_tests::test_deploy ... ok
test liquid_locker_tests::test_contribution_phase ... ok
test liquid_locker_tests::test_calculate_epoch ... ok
test liquid_locker_tests::test_intialize ... ok
test liquid_locker_tests::test_donate_funds ... ok
test liquid_locker_tests::test_increase_payment_rate ... ok
test liquid_locker_tests::test_decrease_payment_time ... ok
test liquid_locker_tests::test_rescue_locker ... ok
test liquid_locker_tests::test_disable_locker ... ok
test liquid_locker_tests::test_claim_interest_public ... ok
test liquid_locker_tests::test_liquidate_locker ... ok
test liquid_locker_tests::test_refund_due_disabled ... ok
test liquid_locker_tests::test_enable_locker ... ok
test liquid_locker_tests::test_claim_interest_single ... ok
test liquid_locker_tests::test_pay_back_funds ... ok
test liquid_locker_tests::test_refund_due_single ... ok

test result: ok. 16 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 15.11s

   Doc-tests liquid-locker-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/home/circleci/project'
make[1]: Leaving directory '/home/circleci/project'
```

## Overall Impression of usage testing

It was observed that the project builds and passes the automated tests successfully after the fixes and improvements by the OP, and the documentation provides sufficient installation/execution instructions. However, the reviewer thinks that the documentation still has room for improvement towards more explanations about the command parameters, better gas amount values on the sample commands, as well as more explanations covering the entirety of the project as it is a complex one which may be hard to understand.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has sufficient tests covering both the positive and the negative paths. Moreover, there are end-to-end tests which build and deploy the contracts on the TestNet, and make calls to them. The reviewer observed that all of the tests successfully pass.

The reviewer also observed that the project has CI facilities in place, automatically building and testing the smart contracts on every new commit. Taking the complexity of the project into account, the reviewer also suggests adding a CI action to the repository that runs the end-to-end tests by using NCTL.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Most critical functions have been observed to have standard comments to provide the code-level documentation, but the reviewer recommends that much more code-level documentation to be added before the final milestone to improve the maintainability of such a complex project.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Project Documentation was observed to be acceptable with usage documentation and examples. However, the reviewer thinks that it would be very useful to have documentation at the architecture level, documenting the "Why?"s and reasoning of the project's design decisions, as well as some less-technical documentation, explaining the project's nature and use cases.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are at an acceptable state, with room for further improvements. The code-level documentation is acceptable for this first milestone, but needs to be improved before the final milestone.

The reviewer communicated the shortcomings of the documentation, along with further points of possible improvements which may not fall in the scope of this review, with the OP. OP acknowledged the feedback, and showed interest in working on further improvements.

# Open Source Practices

## Licenses

The Project is correctly released under the Apache-2.0 license.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repository. The project has a contribution policy. However, the repository doesn't have a description or the relevant tags, hindering its discoverability. Moreover, the contribution policy can be improved by referring to more proper communication channels.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, and has extensive tests.

# Final Conclusion

The project is generally in a very good shape in terms of open-source guidelines. Moreover, the project has extensive tests, and a sufficient level of documentation. The project also successfully builds and passes the automated tests, providing the promised functionality. However, the project documentation can be improved further based on the notes in the relevant sections of this review.

The reviewer also recommends the following points to be fixed/improved as soon as possible:
* A CI action that runs end-to-end tests by using NCTL should be added to the code repository.
* A CI action that runs static analysis on the code-base should be added to the code repository.
* Instructions to generate code-level documentation should be added to the documentation.
* Proper actions/config should be added to the repository to generate and publish code-level documentation upon every new commit.
* The sample commands need to be optimized and fixed to have proper gas amount values, and extensive explanations for each parameter, explaining not only "how" but also "why".
* The JS scripts for teh end-to-end tests need to be improved to have better error & exception handling, with verbose feedback to the user.
* The project documentation should be improved by adding documentation for the high-level design and architecture.

Thus, in the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
