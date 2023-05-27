```bash
gitpod /workspace/casper_staking/staking_contract ((v0.3.1)) $ make test
cd staking_contract && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cd ../erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
warning: unused import: `alloc::string::String`
 --> erc20/src/error.rs:2:5
  |
2 | use alloc::string::String;
  |     ^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: missing documentation for a function
   --> erc20/src/entry_points.rs:145:1
    |
145 | pub fn mint() -> EntryPoint {
    | ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    |
note: the lint level is defined here
   --> erc20/src/lib.rs:13:9
    |
13  | #![warn(missing_docs)]
    |         ^^^^^^^^^^^^

warning: missing documentation for a variant
  --> erc20/src/error.rs:28:5
   |
28 |     UserAllowance(u16),
   |     ^^^^^^^^^^^^^

warning: `casper-erc20` (lib) generated 3 warnings (run `cargo fix --lib -p casper-erc20` to apply 1 suggestion)
warning: unused import: `core::panic::PanicInfo`
  --> erc20-token/src/main.rs:10:5
   |
10 | use core::panic::PanicInfo;
   |     ^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `erc20-token` (bin "erc20_token") generated 1 warning (run `cargo fix --bin "erc20_token"` to apply 1 suggestion)
    Finished release [optimized] target(s) in 0.04s
wasm-strip ../erc20/erc20-token/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cp staking_contract/target/wasm32-unknown-unknown/release/*.wasm staking_contract_tests/wasm
cp ../erc20/target/wasm32-unknown-unknown/release/erc20_token.wasm staking_contract_tests/wasm/erc20.wasm
cd staking_contract_tests && cargo test
  Downloaded hostname v0.3.1
  Downloaded downcast-rs v1.2.0
  Downloaded bit-vec v0.6.3
  Downloaded chrono v0.4.19
  Downloaded proc-macro2 v1.0.40
  Downloaded proptest v1.0.0
  Downloaded serde_derive v1.0.138
  Downloaded serde_json v1.0.82
  Downloaded unicode-ident v1.0.1
  Downloaded num_cpus v1.13.1
  Downloaded match_cfg v0.1.0
  Downloaded remove_dir_all v0.5.3
  Downloaded rand_xorshift v0.3.0
  Downloaded wait-timeout v0.2.0
  Downloaded rand_chacha v0.3.1
  Downloaded tempfile v3.3.0
  Downloaded syn v1.0.98
  Downloaded schemars_derive v0.8.5
  Downloaded wasmi v0.8.0
  Downloaded filesize v0.2.0
  Downloaded quick-error v1.2.3
  Downloaded tracing-attributes v0.1.22
  Downloaded uuid v0.8.2
  Downloaded value-bag v1.0.0-alpha.9
  Downloaded time v0.1.44
  Downloaded tracing-core v0.1.28
  Downloaded ryu v1.0.10
  Downloaded wasmi-validation v0.3.0
  Downloaded libc v0.2.126
  Downloaded linked-hash-map v0.5.6
  Downloaded num-rational v0.2.4
  Downloaded num-bigint v0.2.6
  Downloaded memory_units v0.3.0
  Downloaded lmdb-sys v0.8.0
  Downloaded thiserror v1.0.31
  Downloaded parity-wasm v0.41.0
  Downloaded itoa v1.0.2
  Downloaded indexmap v1.9.1
  Downloaded hashbrown v0.12.1
  Downloaded fastrand v1.7.0
  Downloaded getrandom v0.2.7
  Downloaded generic-array v0.14.5
  Downloaded hex-buffer-serde v0.3.0
  Downloaded datasize v0.2.10
  Downloaded casper-engine-test-support v2.2.0
  Downloaded bincode v1.3.3
  Downloaded serde v1.0.138
  Downloaded regex-syntax v0.6.27
  Downloaded tracing v0.1.35
  Downloaded casper-hashing v1.4.3
  Downloaded rusty-fork v0.3.0
  Downloaded hex-buffer-serde v0.2.2
  Downloaded itertools v0.10.3
  Downloaded either v1.7.0
  Downloaded datasize_derive v0.2.10
  Downloaded ctor v0.1.22
  Downloaded bit-set v0.5.2
  Downloaded anyhow v1.0.58
  Downloaded pwasm-utils v0.16.0
  Downloaded lmdb v0.8.0
  Downloaded lazy_static v1.4.0
  Downloaded cc v1.0.73
  Downloaded quick-error v2.0.1
  Downloaded thiserror-impl v1.0.31
  Downloaded serde_derive_internals v0.25.0
  Downloaded serde_bytes v0.11.6
  Downloaded schemars v0.8.5
  Downloaded quote v1.0.20
  Downloaded pkg-config v0.3.25
  Downloaded pin-project-lite v0.2.9
  Downloaded fnv v1.0.7
  Downloaded dyn-clone v1.0.6
  Downloaded casper-execution-engine v2.0.0
  Downloaded 73 crates (3.9 MB) in 0.65s
   Compiling proc-macro2 v1.0.40
   Compiling quote v1.0.20
   Compiling unicode-ident v1.0.1
   Compiling syn v1.0.98
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.126
   Compiling serde_derive v1.0.138
   Compiling typenum v1.15.0
   Compiling serde v1.0.138
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.3
   Compiling ppv-lite86 v0.2.16
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling fastrand v1.7.0
   Compiling serde_json v1.0.82
   Compiling crunchy v0.2.2
   Compiling remove_dir_all v0.5.3
   Compiling rand_chacha v0.2.2
   Compiling ryu v1.0.10
   Compiling bitvec v0.18.5
   Compiling cpufeatures v0.2.2
   Compiling bitflags v1.3.2
   Compiling hashbrown v0.12.1
   Compiling fnv v1.0.7
   Compiling schemars v0.8.5
   Compiling generic-array v0.14.5
   Compiling once_cell v1.13.0
   Compiling itoa v1.0.2
   Compiling quick-error v1.2.3
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.1
   Compiling num-rational v0.4.1
   Compiling bit-vec v0.6.3
   Compiling rand v0.7.3
   Compiling static_assertions v1.1.0
   Compiling lazy_static v1.4.0
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.6
   Compiling getrandom v0.2.7
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling bit-set v0.5.2
   Compiling regex-syntax v0.6.27
   Compiling num-bigint v0.2.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling rand_core v0.6.3
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.0
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling base16 v0.2.1
   Compiling pkg-config v0.3.25
   Compiling cc v1.0.73
   Compiling num-rational v0.2.4
   Compiling log v0.4.17
   Compiling rand v0.8.5
   Compiling parity-wasm v0.41.0
   Compiling either v1.7.0
   Compiling wee_alloc v0.4.5
   Compiling anyhow v1.0.58
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling itertools v0.10.3
   Compiling time v0.1.44
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling blake2 v0.9.2
   Compiling tracing-core v0.1.28
   Compiling downcast-rs v1.2.0
   Compiling ff v0.8.0
   Compiling num-complex v0.4.2
   Compiling memory_units v0.3.0
   Compiling group v0.8.0
   Compiling pin-project-lite v0.2.9
   Compiling memory_units v0.4.0
   Compiling match_cfg v0.1.0
   Compiling cfg-if v0.1.10
   Compiling num_cpus v1.13.1
   Compiling hostname v0.3.1
   Compiling linked-hash-map v0.5.6
   Compiling chrono v0.4.19
   Compiling filesize v0.2.0
   Compiling wasmi-validation v0.3.0
   Compiling proptest v1.0.0
   Compiling lmdb-sys v0.8.0
   Compiling wasmi v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling lmdb v0.8.0
   Compiling zeroize_derive v1.3.2
   Compiling schemars_derive v0.8.5
   Compiling datasize_derive v0.2.10
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.22
   Compiling thiserror-impl v1.0.31
   Compiling tracing-attributes v0.1.22
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling tracing v0.1.35
   Compiling thiserror v1.0.31
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.6
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.3
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casper-execution-engine v2.0.0
   Compiling contract-utils v0.1.0 (/workspace/casper_staking/staking_contract/utils/contract-utils)
   Compiling casper-engine-test-support v2.2.0
   Compiling test-env v0.1.0 (/workspace/casper_staking/staking_contract/utils/test-env)
   Compiling staking_contract_tests v0.1.0 (/workspace/casper_staking/staking_contract/staking_contract_tests)
warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:211:9
    |
211 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:346:9
    |
346 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:499:9
    |
499 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:648:9
    |
648 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:780:9
    |
780 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: constant `ADDRESS` is never used
  --> src/staking_contract_tests.rs:15:7
   |
15 | const ADDRESS: &str = "9e7283533626d0c7d43fa9ca745af20d8dac7fc3bfe03cdfe50d523a2a0f498d";
   |       ^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: `staking_contract_tests` (lib test) generated 6 warnings (run `cargo fix --lib -p staking_contract_tests --tests` to apply 5 suggestions)
    Finished test [unoptimized + debuginfo] target(s) in 1m 07s
     Running unittests src/lib.rs (target/debug/deps/staking_contract_tests-3339c36f060eeb27)

running 6 tests
test staking_contract_tests::test_approve_and_stake ... ok
test staking_contract_tests::test_approve_and_stake_and_staker_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_amount_staked ... ok
test staking_contract_tests::test_approve_and_stake_and_get_current_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_withdraw ... ok
test staking_contract_tests::test_approve_and_stake_and_add_reward ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.47s

   Doc-tests staking_contract_tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```