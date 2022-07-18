Grant Proposal | [513 - On-Chain MVPR](https://portal.devxdao.com/public-proposals/513)
------------ | -------------
Milestone | 2
Milestone Title | Variable Repository
OP | Michael Steuer
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

This is a Key/Value store contract that supports writes from white listed contracts only, its contents are variables that influence voting, bidding, and other contracts.

**Acceptance criteria:**

- Configurations can be set from specific accounts
- JS Client enables installation, usage and testing of the contract

**Additional notes regarding submission from OP:**

Please find the release notes for Milestone 2 and 4 here: https://github.com/make-software/dao-contracts/releases/tag/milestone-2-4

Release Notes:

This release contains the following smart contracts:
- Variable Repository - keeps track of system parameters,
- Variable Repository Voter - allows voting on system parameters,
- Admin Contract - central contract, that enables the upgrade of the whole system,
- KYC NFT - keeps track of accounts that passed the KYC process,
- KYC Voter - allows performing a KYC process and mints KYC NFT,
- VA NFT - keeps track of accounts that are VAs.
- Onboarding Voter - allows to onboard new VAs and mints VA NFT.

Notes for the DEVxDAO:
- This code fully realizes milestone #2: Variable Repository.
- This code fully realizes milestone #4: KYC Contract.
- It contains a large part of the voting code required for milestone #5: Voting Contract. A full code will be the subject of the next release.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/dao-contracts/tree/milestone-2-4 | 7c24f46


# Install & Usage Testing Procedure and Findings

Reviewer used an Ubuntu 20.04.2 LTS local machine and a GitHub Codespaces cloud machine with Ubuntu 20.04.4 LTS installed for this review.

README provides installation instructions. However, the prerequisites are not mentioned there. It is understood from the repository that it needs `rust` and relevant `cargo` packages to be installed, however these are not listed in the README. Reviewer installed these using the official Rust method listed on their [website](https://www.rust-lang.org/tools/install):

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
(_Log:_ [`rust` installation](assets/rustup.md))

After that, running `make build-contracts` did not work and resulted in an error:

```sh
@ggurbet ➜ /workspaces/dao-contracts (7c24f46) $ make build-contracts
make: *** No rule to make target 'build-contracts'.  Stop.
```

Upon inspecting the `Makefile`, reviewer found out the correct target name has since been changed to `build-dao-contracts`. This needs to be updated in the README.

After that, issuing the `make` command with the correct target, reviewer run into other error messages:

```sh
@ggurbet ➜ /workspaces/dao-contracts (7c24f46 ✗) $ make build-dao-contracts
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
error[E0463]: can't find crate for `core`
  |
  = note: the `wasm32-unknown-unknown` target may not be installed
  = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

error: aborting due to previous error

For more information about this error, try `rustc --explain E0463`.
error: could not compile `rand_core`

To learn more, run the command again with --verbose.
error[E0463]: can't find crate for `core`
  |
  = note: the `wasm32-unknown-unknown` target may not be installed
  = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

error: aborting due to previous error

For more information about this error, try `rustc --explain E0463`.
error: build failed
make: *** [Makefile:14: build-dao-contracts] Error 101
```

Using `rustc --explain E0463` to get more information about the error:

~~~sh
A plugin/crate was declared but cannot be found.

Erroneous code example:

```
#![feature(plugin)]
#![plugin(cookie_monster)] // error: can't find crate for `cookie_monster`
extern crate cake_is_a_lie; // error: can't find crate for `cake_is_a_lie`
```

You need to link your code to the relevant crate in order to be able to use it
(through Cargo or the `-L` option of rustc example). Plugins are crates as
well, and you link to them the same way.

## Common causes

- The crate is not present at all. If using Cargo, add it to `[dependencies]`
  in Cargo.toml.
- The crate is present, but under a different name. If using Cargo, look for
  `package = ` under `[dependencies]` in Cargo.toml.

## Common causes for missing `std` or `core`

- You are cross-compiling for a target which doesn't have `std` prepackaged.
  Consider one of the following:
  + Adding a pre-compiled version of std with `rustup target add`
  + Building std from source with `cargo build -Z build-std`
  + Using `#![no_std]` at the crate root, so you won't need `std` in the first
    place.
- You are developing the compiler itself and haven't built libstd from source.
  You can usually build it with `x.py build library/std`. More information
  about x.py is available in the [rustc-dev-guide].

[rustc-dev-guide]: https://rustc-dev-guide.rust-lang.org/building/how-to-build-and-run.html#building-the-compiler
~~~

Reviewer followed the instructions given alongside the error messages:

```sh
@ggurbet ➜ /workspaces/dao-contracts (7c24f46 ✗) $ rustup target add wasm32-unknown-unknown
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
 13.4 MiB /  13.4 MiB (100 %)  11.6 MiB/s in  1s ETA:  0s
```

```sh
@ggurbet ➜ /workspaces/dao-contracts (7c24f46 ✗) $ cargo build -Zbuild-std
  Downloaded linked-hash-map v0.5.3
  Downloaded ctor v0.1.21
  Downloaded tracing-attributes v0.1.18
  Downloaded pkg-config v0.3.24
  Downloaded downcast-rs v1.2.0
  Downloaded anyhow v1.0.53
  Downloaded bit-set v0.5.2
  Downloaded bincode v1.3.3
  Downloaded rusty-fork v0.3.0
  Downloaded tracing v0.1.29
  Downloaded itertools v0.10.3
  Downloaded hex-buffer-serde v0.3.0
  Downloaded schemars_derive v0.8.5
  Downloaded wasmi v0.8.0
  Downloaded tracing-core v0.1.21
  Downloaded schemars v0.8.5
  Downloaded parity-wasm v0.41.0
  Downloaded thiserror-impl v1.0.30
  Downloaded rand_xorshift v0.3.0
  Downloaded num-bigint v0.2.6
  Downloaded fastrand v1.7.0
  Downloaded quick-error v1.2.3
  Downloaded cc v1.0.72
  Downloaded tempfile v3.3.0
  Downloaded regex-syntax v0.6.25
  Downloaded wasmi-validation v0.3.0
  Downloaded pwasm-utils v0.16.0
  Downloaded remove_dir_all v0.5.3
  Downloaded rand_chacha v0.3.1
  Downloaded thiserror v1.0.30
  Downloaded wait-timeout v0.2.0
  Downloaded value-bag v1.0.0-alpha.8
  Downloaded hex-buffer-serde v0.2.2
  Downloaded casper-execution-engine v1.4.4
  Downloaded datasize v0.2.10
  Downloaded proptest v1.0.0
  Downloaded serde_derive_internals v0.25.0
  Downloaded lmdb v0.8.0
  Downloaded casper-engine-test-support v2.0.3
  Downloaded chrono v0.4.19
  Downloaded uuid v0.8.2
  Downloaded pin-project-lite v0.2.8
  Downloaded quick-error v2.0.1
  Downloaded either v1.6.1
  Downloaded bit-vec v0.6.3
  Downloaded fnv v1.0.7
  Downloaded casper-hashing v1.4.3
  Downloaded datasize_derive v0.2.10
  Downloaded getrandom v0.2.4
  Downloaded hashbrown v0.11.2
  Downloaded log v0.4.14
  Downloaded time v0.1.43
  Downloaded num-rational v0.2.4
  Downloaded lmdb-sys v0.8.0
  Downloaded once_cell v1.9.0
  Downloaded match_cfg v0.1.0
  Downloaded indexmap v1.8.0
  Downloaded hostname v0.3.1
  Downloaded dyn-clone v1.0.4
  Downloaded memory_units v0.3.0
  Downloaded 60 crates (2.6 MB) in 0.47s
error: -Zbuild-std requires --target
```

Notice the error message at the end.

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | PASS / FAIL / PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes

# Unit / Automated Testing

_Summarize the result of the unit testing / automated testing / integration testing provided in the Milestone. Feel free to include automated test output, either as text, image or other artifact. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS / FAIL / PASS with Notes
Unit Tests - At least one negative path test | PASS / FAIL / PASS with Notes
Unit Tests - Additional path tests | PASS / FAIL / PASS with Notes

# Documentation

### Code Documentation

Code is well documented. Critical functionality is properly explained and lots of additional comments exist.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project documentation is done via Rustdoc. All critical functionality of the code is documented. There are examples inside the documentation about how to use different aspects of the code. There was one warning while generating the documentation, which needs developer attention.

[*Documentation build logs*](assets/docs.md)

![](assets/docs.png)

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

Code documentation is sufficient. General documentation is sufficient and includes usage examples.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project does not contain CONTRIBUTING and SECURITY policies. These need to be included before the final milestone. Pull requests and Issues are enabled on the repository and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

_Provide any general observations about the project you want to add to your review. These can be subjective in nature as well, and do not contribute to your recommendation to pass or fail the submission._

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
