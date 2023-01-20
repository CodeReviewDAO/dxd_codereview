```
muharremsalel@Muharrems-MBP sbp-dxd-m2 % make test
cd did_registry && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.27s
wasm-strip target/wasm32-unknown-unknown/release/did_registry.wasm 2>/dev/null | true
mkdir -p tests/wasm
cp target/wasm32-unknown-unknown/release/did_registry.wasm tests/wasm
cd tests && cargo test
  Downloaded ctor v0.1.26
  Downloaded rand_chacha v0.3.1
  Downloaded time v0.1.45
  Downloaded log v0.4.17
  Downloaded uuid v0.8.2
  Downloaded tracing-core v0.1.30
  Downloaded downcast-rs v1.2.0
  Downloaded lazy_static v1.4.0
  Downloaded linked-hash-map v0.5.6
  Downloaded quick-error v2.0.1
  Downloaded quick-error v1.2.3
  Downloaded wait-timeout v0.2.0
  Downloaded tracing-attributes v0.1.23
  Downloaded pkg-config v0.3.26
  Downloaded num-bigint v0.2.6
  Downloaded tracing v0.1.37
  Downloaded thiserror-impl v1.0.38
  Downloaded match_cfg v0.1.0
  Downloaded indexmap v1.9.2
  Downloaded itertools v0.10.5
  Downloaded iana-time-zone v0.1.53
  Downloaded bit-vec v0.6.3
  Downloaded thiserror v1.0.38
  Downloaded dyn-clone v1.0.10
  Downloaded core-foundation-sys v0.8.3
  Downloaded chrono v0.4.23
  Downloaded regex-syntax v0.6.28
  Downloaded wasmi v0.8.0
  Downloaded pwasm-utils v0.16.0
  Downloaded serde_derive_internals v0.25.0
  Downloaded rand_xorshift v0.3.0
  Downloaded casper_types_derive v0.1.0
  Downloaded datasize_derive v0.2.13
  Downloaded datasize v0.2.13
  Downloaded casper-engine-test-support v2.2.0
  Downloaded memory_units v0.3.0
  Downloaded remove_dir_all v0.5.3
  Downloaded bincode v1.3.3
  Downloaded anyhow v1.0.68
  Downloaded hostname v0.3.1
  Downloaded proptest v1.0.0
  Downloaded value-bag v1.0.0-alpha.9
  Downloaded tempfile v3.3.0
  Downloaded num_cpus v1.15.0
  Downloaded casperlabs-test-env v0.3.0
  Downloaded casper-hashing v1.4.3
  Downloaded hashbrown v0.12.3
  Downloaded schemars v0.8.5
  Downloaded getrandom v0.2.8
  Downloaded fnv v1.0.7
  Downloaded either v1.8.0
  Downloaded cc v1.0.78
  Downloaded casper-execution-engine v2.0.1
  Downloaded filesize v0.2.0
  Downloaded lmdb-sys v0.8.0
  Downloaded schemars_derive v0.8.5
  Downloaded pin-project-lite v0.2.9
  Downloaded rusty-fork v0.3.0
  Downloaded lmdb v0.8.0
  Downloaded fastrand v1.8.0
  Downloaded bit-set v0.5.3
  Downloaded num-rational v0.2.4
  Downloaded wasmi-validation v0.3.0
  Downloaded hex-buffer-serde v0.2.2
  Downloaded hex-buffer-serde v0.3.0
  Downloaded parity-wasm v0.41.0
  Downloaded 66 crates (2.7 MB) in 1.61s
   Compiling proc-macro2 v1.0.50
   Compiling quote v1.0.23
   Compiling unicode-ident v1.0.6
   Compiling syn v1.0.107
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.139
   Compiling typenum v1.16.0
   Compiling serde_derive v1.0.152
   Compiling serde v1.0.152
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling ppv-lite86 v0.2.17
   Compiling wyz v0.2.0
   Compiling byteorder v1.4.3
   Compiling fastrand v1.8.0
   Compiling opaque-debug v0.3.0
   Compiling remove_dir_all v0.5.3
   Compiling serde_json v1.0.91
   Compiling crunchy v0.2.2
   Compiling fnv v1.0.7
   Compiling bit-vec v0.6.3
   Compiling quick-error v1.2.3
   Compiling hashbrown v0.12.3
   Compiling ryu v1.0.12
   Compiling once_cell v1.17.0
   Compiling cpufeatures v0.2.5
   Compiling bitflags v1.3.2
   Compiling itoa v1.0.5
   Compiling schemars v0.8.5
   Compiling lazy_static v1.4.0
   Compiling regex-syntax v0.6.28
   Compiling static_assertions v1.1.0
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.10
   Compiling cc v1.0.78
   Compiling core-foundation-sys v0.8.3
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling pkg-config v0.3.26
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling thiserror v1.0.38
   Compiling either v1.8.0
   Compiling anyhow v1.0.68
   Compiling downcast-rs v1.2.0
   Compiling pin-project-lite v0.2.9
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling bit-set v0.5.3
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling indexmap v1.9.2
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling tracing-core v0.1.30
   Compiling rand_chacha v0.2.2
   Compiling itertools v0.10.5
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.8
   Compiling tempfile v3.3.0
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.45
   Compiling hostname v0.3.1
   Compiling num_cpus v1.15.0
   Compiling lmdb-sys v0.8.0
   Compiling iana-time-zone v0.1.53
   Compiling rand_core v0.6.4
   Compiling rusty-fork v0.3.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling group v0.8.0
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
   Compiling proptest v1.0.0
   Compiling chrono v0.4.23
   Compiling lmdb v0.8.0
   Compiling wasmi v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.3
   Compiling datasize_derive v0.2.13
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.38
   Compiling tracing-attributes v0.1.23
   Compiling casper_types_derive v0.1.0
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.13
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling tracing v0.1.37
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.8
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling common v0.1.0 (/Users/muharremsalel/Desktop/CRDao/sbp-dxd-m2/did_common)
   Compiling casper-execution-engine v2.0.1
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.3.0
   Compiling tests v0.1.0 (/Users/muharremsalel/Desktop/CRDao/sbp-dxd-m2/tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 08s
     Running unittests src/lib.rs (/Users/muharremsalel/Desktop/CRDao/sbp-dxd-m2/target/debug/deps/tests-087cf5a2b051a31e)

running 23 tests
test did_contract_tests::test_identity_get_owner_identity_not_changed ... ok
test did_contract_tests::test_deploy ... ok
test did_contract_tests::test_change_owner_by_non_owner_rejected - should panic ... ok
test did_contract_tests::test_add_delegate_by_non_owner_rejected - should panic ... ok
test did_contract_tests::test_revoke_delegate_by_non_owner_rejected - should panic ... ok
test did_contract_tests::test_revoke_attribute_by_owner_missing_identity - should panic ... ok
test did_contract_tests::test_revoke_attribute_by_non_owner_rejected - should panic ... ok
test did_contract_tests::test_change_owner_by_owner_successful ... ok
test did_contract_tests::test_add_delegate_by_owner_successful ... ok
test did_contract_tests::test_change_owner_and_try_to_change_by_previous_owner_rejected - should panic ... ok
test did_contract_tests::test_revoke_attribute_by_owner_missing_attribute - should panic ... ok
test did_contract_tests::test_revoke_attribute_by_owner_successful ... ok
test did_contract_tests::test_revoke_delegate_by_owner_missing_delegate - should panic ... ok
test did_contract_tests::test_add_delegate_for_existing_delegate_type_successful ... ok
test did_contract_tests::test_add_delegate_update_existing_delegate_successful ... ok
test did_contract_tests::test_add_delegate_for_existing_identity_successful ... ok
test did_contract_tests::test_revoke_delegate_by_owner_missing_identity - should panic ... ok
test did_contract_tests::test_set_attribute_by_non_owner_rejected - should panic ... ok
test did_contract_tests::test_set_attribute_by_owner_successful ... ok
test did_contract_tests::test_revoke_delegate_by_owner_missing_delegate_type - should panic ... ok
test did_contract_tests::test_revoke_delegate_by_owner_successful ... ok
test did_contract_tests::test_set_attribute_update_existing_attribute_successful ... ok
test did_contract_tests::test_set_attribute_for_existing_identity_successful ... ok

test result: ok. 23 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.11s

   Doc-tests tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```