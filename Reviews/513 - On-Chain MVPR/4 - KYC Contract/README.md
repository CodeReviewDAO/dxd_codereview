Grant Proposal | [513 - On-Chain MVPR](https://portal.devxdao.com/public-proposals/513)
------------ | -------------
Milestone | 4
Milestone Title | Variable Repository
OP | Michael Steuer
Reviewer | Ömer ÇAKMAK <farukomercakmak@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- A KYC contract built on the Casper network
- A JavaScript client that can install the KYC token, interact with all its interfaces, and facilitate E2E testing
- Documentation associated with the above

**Acceptance criteria:**

- KYC contract can be installed on the Casper Network
- KYC results can be captured and matched against unique VA identifiers
- JS Client enables installation, usage and testing of the contract

**Additional notes regarding submission from OP:**

Please find the release notes for milestones #2 and #4 here: https://github.com/make-software/dao-contracts/releases/tag/milestone-2-4

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

Reviewer used the Ubuntu 20.04 local machine for this review.

The README provides installation instructions, but no prerequisites are specified. From the terminal output we see that `rust` and revelant `cargo` packages need to be loaded. Reviewer installed them using the steps on the official [Rust page](https://www.rust-lang.org/tools/install):

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Note: Rust install logs [here](assets/install_rust.log)

No build was done when the `make build-contracts` command was run. Then the reviewer checked the updated README file and decided to use the `make build-all` command mentioned there.

Then the `build-all` command was run, but the error was received:
```
foc@foc:~/dao-contracts$ make build-all
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
info: syncing channel updates for 'nightly-2021-06-17-x86_64-unknown-linux-gnu'
info: latest update on 2021-06-17, rust version 1.55.0-nightly (a85f584ae 2021-06-16)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
info: installing component 'rust-std'
info: installing component 'rustc'
info: installing component 'rustfmt'
error[E0463]: can't find crate for `core`
  |
  = note: the `wasm32-unknown-unknown` target may not be installed
  = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

error: aborting due to previous error

For more information about this error, try `rustc --explain E0463`.
error: could not compile `subtle`

To learn more, run the command again with --verbose.
error: build failed
make: *** [Makefile:14: build-dao-contracts] Error 101
```
The steps shown in the error output were run:
```
foc@foc:~/dao-contracts$ rustup target add wasm32-unknown-unknown
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
 13.4 MiB /  13.4 MiB (100 %)  13.0 MiB/s in  1s ETA:  0s
```

After that, run `make build-all` again:
```
foc@foc:~/dao-contracts$ make build-all
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc20
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc721
```

## Overall Impression of usage testing

_Summarize your impression following detailed usage testing and provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Project builds without errors | PASS / FAIL / PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes

# Unit / Automated Testing

All of the test steps specified in this step worked successfully.

You can access the unit tests log [here](assets/test.log).

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS 
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation

Reviewer found the code to be well documented. All critical functionality has explanatory comments.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Documentation was built successfully. But it gave a few warnings. It might be good to fix them.

```
foc@foc:~/dao-contracts$ make docs >> docs.log
  Downloaded bit-set v0.5.2
  Downloaded getrandom v0.2.4
  Downloaded log v0.4.14
  Downloaded fnv v1.0.7
  Downloaded either v1.6.1
....
warning: `casper-dao-contracts` (lib doc) generated 6 warnings
    Finished dev [unoptimized + debuginfo] target(s) in 54.31s
     Opening /home/foc/dao-contracts/target/doc/casper_dao_contracts/index.html
```
You can access documentation build logs [here](assets/docs.log).

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS

## Overall Conclusion on Documentation

A little more sample and usage information is needed.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project does not contain CONTRIBUTING and SECURITY policies.  Pull requests and Issues are enabled. This is sufficient as it is not the final milestone.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

The readability of the code is sufficient. In general the source code is well written. Best practices used.

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
