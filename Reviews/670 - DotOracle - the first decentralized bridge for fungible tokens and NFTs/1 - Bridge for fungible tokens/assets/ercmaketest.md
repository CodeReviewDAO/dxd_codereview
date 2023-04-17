cargo build --release --target wasm32-unknown-unknown  -p erc20-token  -p erc20-test  -p erc20-test-call
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20_token.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc20_test.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc20_test_call.wasm 2>/dev/null | true;
cargo test
 Downloading crates ...
  Downloaded fnv v1.0.7
  Downloaded anyhow v1.0.43
  Downloaded cc v1.0.70
  Downloaded downcast-rs v1.2.0
  Downloaded wasmi-validation v0.3.0
  Downloaded ctor v0.1.21
  Downloaded value-bag v1.0.0-alpha.7
  Downloaded tempfile v3.2.0
  Downloaded num-iter v0.1.42
  Downloaded rand_xorshift v0.3.0
  Downloaded hostname v0.3.1
  Downloaded match_cfg v0.1.0
  Downloaded bit-set v0.5.2
  Downloaded remove_dir_all v0.5.3
  Downloaded wait-timeout v0.2.0
  Downloaded quick-error v2.0.1
  Downloaded num v0.4.0
  Downloaded lazy_static v1.4.0
  Downloaded rand_chacha v0.3.1
  Downloaded linked-hash-map v0.5.4
  Downloaded pin-project-lite v0.2.7
  Downloaded memory_units v0.3.0
  Downloaded pkg-config v0.3.19
  Downloaded num-rational v0.2.4
  Downloaded num-bigint v0.2.6
  Downloaded rusty-fork v0.3.0
  Downloaded time v0.1.43
  Downloaded getrandom v0.2.3
  Downloaded tracing-attributes v0.1.15
  Downloaded hex-buffer-serde v0.2.2
  Downloaded bit-vec v0.6.3
  Downloaded either v1.6.1
  Downloaded quick-error v1.2.3
  Downloaded log v0.4.14
  Downloaded uuid v0.8.2
  Downloaded bincode v1.3.3
  Downloaded num-complex v0.4.0
  Downloaded tracing-core v0.1.19
  Downloaded tracing v0.1.26
  Downloaded parity-wasm v0.41.0
  Downloaded num-bigint v0.4.2
  Downloaded itertools v0.10.1
  Downloaded pwasm-utils v0.16.0
  Downloaded wasmi v0.8.0
  Downloaded lmdb-sys v0.8.0
  Downloaded lmdb v0.8.0
  Downloaded proptest v1.0.0
  Downloaded chrono v0.4.19
  Downloaded casper-engine-test-support v1.3.2
  Downloaded casper-execution-engine v1.3.2
   Compiling proc-macro2 v1.0.29
   Compiling unicode-xid v0.2.0
   Compiling syn v1.0.76
   Compiling libc v0.2.101
   Compiling autocfg v1.0.0
   Compiling version_check v0.9.3
   Compiling serde v1.0.105
   Compiling typenum v1.14.0
   Compiling cfg-if v1.0.0
   Compiling getrandom v0.1.14
   Compiling cfg-if v0.1.10
   Compiling subtle v2.4.1
   Compiling ppv-lite86 v0.2.10
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling bitflags v1.2.1
   Compiling byteorder v1.4.3
   Compiling ryu v1.0.3
   Compiling regex-syntax v0.6.25
   Compiling crunchy v0.2.2
   Compiling lazy_static v1.4.0
   Compiling serde_json v1.0.67
   Compiling remove_dir_all v0.5.3
   Compiling tinyvec_macros v0.1.0
   Compiling opaque-debug v0.3.0
   Compiling itoa v0.4.5
   Compiling schemars v0.8.3
   Compiling quick-error v1.2.3
   Compiling memchr v2.4.1
   Compiling hashbrown v0.11.2
   Compiling matches v0.1.9
   Compiling cpufeatures v0.2.1
   Compiling bit-vec v0.6.3
   Compiling fnv v1.0.7
   Compiling percent-encoding v2.1.0
   Compiling unicode-bidi v0.3.6
   Compiling dyn-clone v1.0.4
   Compiling quick-error v2.0.1
   Compiling static_assertions v1.1.0
   Compiling pulldown-cmark v0.8.0
   Compiling once_cell v1.8.0
   Compiling base64 v0.13.0
   Compiling hex_fmt v0.3.0
   Compiling wee_alloc v0.4.5
   Compiling base16 v0.2.1
   Compiling memory_units v0.4.0
   Compiling semver-parser v0.9.0
   Compiling pkg-config v0.3.19
   Compiling cc v1.0.70
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.14
   Compiling anyhow v1.0.43
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling pin-project-lite v0.2.7
   Compiling either v1.6.1
   Compiling downcast-rs v1.2.0
   Compiling linked-hash-map v0.5.4
   Compiling tracing-core v0.1.19
   Compiling tinyvec v1.3.1
   Compiling bitvec v0.18.5
   Compiling generic-array v0.14.4
   Compiling unicase v2.6.0
   Compiling value-bag v1.0.0-alpha.7
   Compiling form_urlencoded v1.0.1
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling num-bigint v0.4.2
   Compiling num-rational v0.4.0
   Compiling indexmap v1.7.0
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling num-iter v0.1.42
   Compiling bit-set v0.5.2
   Compiling itertools v0.10.1
   Compiling unicode-normalization v0.1.19
   Compiling quote v1.0.9
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.3
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.43
   Compiling hostname v0.3.1
   Compiling regex v1.5.4
   Compiling rand_core v0.5.1
   Compiling rand_core v0.6.3
   Compiling num-complex v0.4.0
   Compiling idna v0.2.3
   Compiling lmdb-sys v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling chrono v0.4.19
   Compiling group v0.8.0
   Compiling rand v0.8.4
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.8
   Compiling rand v0.7.3
   Compiling blake2 v0.9.2
   Compiling url v2.2.2
   Compiling tempfile v3.2.0
   Compiling rusty-fork v0.3.0
   Compiling proptest v1.0.0
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.3
   Compiling serde_derive_internals v0.25.0
   Compiling serde_derive v1.0.105
   Compiling zeroize_derive v1.1.0
   Compiling thiserror-impl v1.0.29
   Compiling schemars_derive v0.8.3
   Compiling datasize_derive v0.2.9
   Compiling displaydoc v0.1.7
   Compiling num-derive v0.3.0
   Compiling ctor v0.1.21
   Compiling tracing-attributes v0.1.15
   Compiling zeroize v1.4.1
   Compiling datasize v0.2.9
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.0
   Compiling ecdsa v0.10.2
   Compiling tracing v0.1.26
   Compiling k256 v0.7.3
   Compiling thiserror v1.0.29
   Compiling hex v0.4.3
   Compiling ed25519 v1.2.0
   Compiling serde_bytes v0.11.5
   Compiling toml v0.5.8
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling ed25519-dalek v1.0.1
   Compiling uint v0.9.1
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling version-sync v0.9.2
   Compiling casper-types v1.3.2
   Compiling casper-contract v1.3.2
   Compiling casper-execution-engine v1.3.2
   Compiling casper-erc20 v0.2.1 (/workspace/casper-erc20/erc20)
   Compiling casper-engine-test-support v1.3.2
   Compiling erc20-tests v0.1.0 (/workspace/casper-erc20/example/erc20-tests)
   Compiling tests v0.1.0 (/workspace/casper-erc20/testing/tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 46s
     Running unittests (target/debug/deps/casper_erc20-3638f9bd3b20ee2c)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests (target/debug/deps/erc20_tests-fcbc3f23939637b7)

running 6 tests
test tests::should_install ... ok
test tests::should_transfer ... ok
test tests::should_transfer_full_amount ... ok
test tests::should_not_transfer_with_insufficient_balance - should panic ... ok
test tests::should_transfer_from ... ok
test tests::should_not_transfer_from_more_than_approved - should panic ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.81s

     Running unittests (target/debug/deps/tests-55ca2fdb07855644)

running 22 tests
test lib_integration_tests::should_not_store_balances_or_allowances_under_account_after_install ... ok
test lib_integration_tests::should_have_queryable_properties ... ok
test lib_integration_tests::should_not_transfer_from_without_enough_allowance ... ok
test lib_integration_tests::should_have_correct_balance_after_own_transfer ... ok
test lib_integration_tests::should_approve_funds_account_to_contract ... ok
test lib_integration_tests::should_approve_funds_account_to_account ... ok
test lib_integration_tests::should_not_transfer_more_than_owned_balance ... ok
test lib_integration_tests::should_approve_funds_contract_to_account ... ok
test lib_integration_tests::should_transfer_from_account_by_contract ... ok
test lib_integration_tests::should_transfer_from_from_account_to_account ... ok
test lib_integration_tests::should_approve_funds_contract_to_contract ... ok
test lib_integration_tests::should_have_correct_balance_after_own_transfer_from ... ok
test lib_integration_tests::should_transfer_account_to_contract ... ok
test lib_integration_tests::should_transfer_account_to_account ... ok
test lib_integration_tests::should_transfer_contract_to_contract ... ok
test lib_integration_tests::should_transfer_full_owned_amount ... ok
test lib_integration_tests::should_transfer_contract_to_account ... ok
test lib_integration_tests::test_should_not_mint_above_limits ... ok
test lib_integration_tests::should_verify_zero_amount_transfer_is_noop ... ok
test lib_integration_tests::test_should_not_burn_above_balance ... ok
test lib_integration_tests::should_verify_zero_amount_transfer_from_is_noop ... ok
test lib_integration_tests::test_mint_and_burn_tokens ... ok

test result: ok. 22 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 12.83s

   Doc-tests casper-erc20

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

