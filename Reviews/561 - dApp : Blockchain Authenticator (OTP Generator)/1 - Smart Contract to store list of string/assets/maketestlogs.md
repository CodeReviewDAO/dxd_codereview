# Output of the "make test" command

```sh


cd contract && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.04s
wasm-strip contract/target/wasm32-unknown-unknown/release/contract.wasm 2>/dev/null | true
mkdir -p tests/wasm
cp contract/target/wasm32-unknown-unknown/release/contract.wasm tests/wasm
cd tests && cargo test
 Downloading crates ...
  Downloaded schemars v0.8.5
  Downloaded tracing-core v0.1.26
  Downloaded match_cfg v0.1.0
  Downloaded bincode v1.3.3
  Downloaded wait-timeout v0.2.0
  Downloaded hostname v0.3.1
  Downloaded dyn-clone v1.0.5
  Downloaded hex-buffer-serde v0.2.2
  Downloaded indexmap v1.8.1
  Downloaded pin-project-lite v0.2.8
  Downloaded time v0.1.43
  Downloaded value-bag v1.0.0-alpha.8
  Downloaded fastrand v1.7.0
  Downloaded quick-error v2.0.1
  Downloaded quick-error v1.2.3
  Downloaded tracing-attributes v0.1.20
  Downloaded uuid v0.8.2
  Downloaded either v1.6.1
  Downloaded memory_units v0.3.0
  Downloaded serde_derive_internals v0.25.0
  Downloaded wasmi v0.8.0
  Downloaded proptest v1.0.0
  Downloaded num-rational v0.2.4
  Downloaded regex-syntax v0.6.25
  Downloaded lmdb-sys v0.8.0
  Downloaded lmdb v0.8.0
  Downloaded getrandom v0.2.6
  Downloaded chrono v0.4.19
  Downloaded cc v1.0.73
  Downloaded tempfile v3.3.0
  Downloaded itertools v0.10.3
  Downloaded pkg-config v0.3.25
  Downloaded downcast-rs v1.2.0
  Downloaded casper-hashing v1.4.3
  Downloaded bit-vec v0.6.3
  Downloaded tracing v0.1.34
  Downloaded thiserror-impl v1.0.30
  Downloaded schemars_derive v0.8.5
  Downloaded rusty-fork v0.3.0
  Downloaded rand_xorshift v0.3.0
  Downloaded pwasm-utils v0.16.0
  Downloaded parity-wasm v0.41.0
  Downloaded once_cell v1.10.0
  Downloaded num-bigint v0.2.6
  Downloaded log v0.4.16
  Downloaded linked-hash-map v0.5.4
  Downloaded hex-buffer-serde v0.3.0
  Downloaded hashbrown v0.11.2
  Downloaded ctor v0.1.22
  Downloaded remove_dir_all v0.5.3
  Downloaded rand_chacha v0.3.1
  Downloaded lazy_static v1.4.0
  Downloaded fnv v1.0.7
  Downloaded anyhow v1.0.56
  Downloaded bit-set v0.5.2
  Downloaded thiserror v1.0.30
  Downloaded datasize_derive v0.2.10
  Downloaded datasize v0.2.10
  Downloaded wasmi-validation v0.3.0
  Downloaded casper-engine-test-support v2.1.0
  Downloaded casper-execution-engine v1.5.0
   Compiling proc-macro2 v1.0.37
   Compiling unicode-xid v0.2.2
   Compiling syn v1.0.91
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.124
   Compiling serde_derive v1.0.136
   Compiling typenum v1.15.0
   Compiling serde v1.0.136
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling funty v1.1.0
   Compiling ppv-lite86 v0.2.16
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.79
   Compiling opaque-debug v0.3.0
   Compiling fastrand v1.7.0
   Compiling remove_dir_all v0.5.3
   Compiling crunchy v0.2.2
   Compiling lazy_static v1.4.0
   Compiling ryu v1.0.9
   Compiling itoa v1.0.1
   Compiling fnv v1.0.7
   Compiling cpufeatures v0.2.2
   Compiling bit-vec v0.6.3
   Compiling hashbrown v0.11.2
   Compiling quick-error v1.2.3
   Compiling bitflags v1.3.2
   Compiling schemars v0.8.5
   Compiling dyn-clone v1.0.5
   Compiling regex-syntax v0.6.25
   Compiling static_assertions v1.1.0
   Compiling quick-error v2.0.1
   Compiling pkg-config v0.3.25
   Compiling cc v1.0.73
   Compiling hex_fmt v0.3.0
   Compiling log v0.4.16
   Compiling base64 v0.13.0
   Compiling parity-wasm v0.41.0
   Compiling once_cell v1.10.0
   Compiling base16 v0.2.1
   Compiling anyhow v1.0.56
   Compiling either v1.6.1
   Compiling downcast-rs v1.2.0
   Compiling memory_units v0.3.0
   Compiling match_cfg v0.1.0
   Compiling pin-project-lite v0.2.8
   Compiling linked-hash-map v0.5.4
   Compiling tracing-core v0.1.26
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling generic-array v0.14.5
   Compiling value-bag v1.0.0-alpha.8
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.42
   Compiling num-rational v0.4.0
   Compiling indexmap v1.8.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.2
   Compiling itertools v0.10.3
   Compiling rand v0.7.3
   Compiling quote v1.0.18
   Compiling getrandom v0.2.6
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.43
   Compiling hostname v0.3.1
   Compiling wasmi-validation v0.3.0
   Compiling rand_core v0.6.3
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling lmdb-sys v0.8.0
   Compiling num-complex v0.4.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling rand v0.8.5
   Compiling ff v0.8.0
   Compiling signature v1.2.2
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling chrono v0.4.19
   Compiling hmac v0.10.1
   Compiling ed25519 v1.2.0
   Compiling group v0.8.0
   Compiling proptest v1.0.0
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.2
   Compiling schemars_derive v0.8.5
   Compiling datasize_derive v0.2.10
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.22
   Compiling thiserror-impl v1.0.30
   Compiling tracing-attributes v0.1.20
   Compiling datasize v0.2.10
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling thiserror v1.0.30
   Compiling tracing v0.1.34
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.5
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
   Compiling casper-execution-engine v1.5.0
   Compiling casper-engine-test-support v2.1.0
   Compiling tests v0.1.0 (/workspace/blockchain-authenticator-contract/tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 12s
     Running unittests (target/debug/deps/integration_tests-5924344271c8fdee)

running 9 tests
test tests::should_create_named_keys ... ok
test tests::should_add_non_existing_element ... ok
test tests::should_panic_missing_parameters - should panic ... ok
test tests::should_add_multiple_elements ... ok
test tests::should_del_element ... ok
test tests::should_update_existing_element ... ok
test tests::should_not_del_element_non_existing_element ... ok
test tests::should_remove_all_elements ... ok
test tests::should_del_multiple_elements ... ok

test result: ok. 9 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.57s

```
