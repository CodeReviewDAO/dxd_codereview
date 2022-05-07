Grant Proposal | [513 - On-Chain MVPR)](https://portal.devxdao.com/public-proposals/513)
------------ | -------------
Milestone | 1
Milestone Title | Reputation Token
OP | Michael Steuer
Reviewer | Yunusemre Şentürk <se.yunusemre@gmail.com>

# Milestone Details
This is the first milestone of grant.
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

A reputation token contract built on the Casper network
A JavaScript client that can install the reputation token, interact with all its interfaces, and facilitate E2E testing
Documentation associated with the above

**Acceptance criteria:**

Token can be installed on the Casper Network
Reputation can be minted and transferred to specific accounts
JS Client enables installation, usage and testing of the contract

**Additional notes regarding submission from OP:**

Reputation Token contract and associated Javascript client are complete. Tester can review current state of the repository, or choose to look specifically at the "Milestone 1" milestone inside the repository.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/dao-contracts/tree/milestone-1 | 9ae7ae4


# Install & Usage Testing Procedure and Findings

The reviewer observed that, by following the instructions in the README of https://github.com/make-software/dao-contracts/tree/milestone-1 was enough to successfully build the source code on an Ubuntu 20.04 server using `cargo 1.54.0-nightly (44456677b 2021-06-12)` and `rustc 1.55.0-nightly (a85f584ae 2021-06-16)`. 

However, there should have been a small information about rust language is prerequested in the README.md eventhough it is obvious that the repository is based on rust language. 

The reviewer thinks that the preparing an axample JS client is a good idea to fast the testing procedure up, therefore, having the client README.md files' link in the main README.md file would have been better aproach. 

Here is build output : 
```bash
yunusem@ubuntu-20-04-crdao-513-1-onchainMVPR:~/new/dao-contracts$ make build-contracts
cargo build --release --target wasm32-unknown-unknown -p casper-dao-contracts
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /home/yunusem/new/dao-contracts/contracts/Cargo.toml
workspace: /home/yunusem/new/dao-contracts/Cargo.toml
   Compiling proc-macro2 v1.0.36
   Compiling version_check v0.9.4
   Compiling autocfg v1.0.1
   Compiling typenum v1.15.0
   Compiling unicode-xid v0.2.2
   Compiling syn v1.0.86
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling serde_derive v1.0.134
   Compiling serde v1.0.134
   Compiling crunchy v0.2.2
   Compiling cfg-if v1.0.0
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.76
   Compiling itoa v1.0.1
   Compiling static_assertions v1.1.0
   Compiling wee_alloc v0.4.5
   Compiling hex v0.4.3
   Compiling rand_core v0.6.3
   Compiling ryu v1.0.9
   Compiling bitflags v1.3.2
   Compiling memory_units v0.4.0
   Compiling cfg-if v0.1.10
   Compiling base64 v0.13.0
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling lazy_static v1.4.0
   Compiling generic-array v0.14.5
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.0
   Compiling num-iter v0.1.42
   Compiling bitvec v0.18.5
   Compiling rand_chacha v0.2.2
   Compiling rand v0.8.4
   Compiling ff v0.8.0
   Compiling rand v0.7.3
   Compiling quote v1.0.15
   Compiling group v0.8.0
   Compiling uint v0.9.1
   Compiling num-complex v0.4.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling synstructure v0.12.6
   Compiling num-derive v0.3.3
   Compiling casper-dao-macros v0.1.0 (/home/yunusem/new/dao-contracts/macros)
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling zeroize_derive v1.3.1
   Compiling ed25519 v1.2.0
   Compiling zeroize v1.5.0
   Compiling serde_bytes v0.11.5
   Compiling num v0.4.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.0
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling casper-types v1.4.6
   Compiling casper-contract v1.4.3
   Compiling casper-dao-utils v0.1.0 (/home/yunusem/new/dao-contracts/utils)
   Compiling casper-dao-contracts v0.1.0 (/home/yunusem/new/dao-contracts/contracts)
    Finished release [optimized] target(s) in 4m 48s
wasm-strip target/wasm32-unknown-unknown/release/reputation_contract.wasm 2>/dev/null | true
```

The reviewer finds client/README.md file is missleading about installation, instead, the reviewer used `npm install [path/to/client/folder]` command.

Here is client [install output](assets/client-install-output)

## Overall Impression of usage testing

It was observed that the README.md file is missing some small guidence information.

Requirement | Finding
------------ | -------------
Documentation provides sufficient installation/execution instructions | PASS with Notes 
Project builds without errors | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

It was observed that the project builds and passes the automated tests successfully. Here is the `make test` [output](assets/make-test-output).

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

It was observed that the code documentation was acceptable for this stage of the project. 

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project documentation seem to be not well documented regarding usage and examples, however, the reviewer thinks that it is enough to test the first acceptance criteria.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS with notes

## Overall Conclusion on Documentation

A little bit more example and usage documentation is required. `make docs` is not good enough for remote reviewing.

# Open Source Practices

## Licenses

The project contains a `LICENCE` file in source tree.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains no CONTRIBUTING nor SECURITY policy that links to a Code of Conduct policy.
Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, but it is a bit shame that simple installation 
procedure have been made complicated by providing less instruction.

# Final Conclusion

The reviewer recommends that this submission should pass code review, with the warning of the OSS contribution best practices, and suggests the OP to act on that.

# Recommendation

Recommendation | PASS with notes.
------------ | -------------
