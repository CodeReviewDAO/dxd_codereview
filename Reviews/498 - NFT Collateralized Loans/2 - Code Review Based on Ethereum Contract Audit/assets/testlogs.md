make all
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT'
make build-contract-liquid-factory && make build-contract-liquid-locker
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cargo build --release -p liquid-factory -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Updating crates.io index
   Compiling proc-macro2 v1.0.51
   Compiling unicode-ident v1.0.8
   Compiling quote v1.0.23
   Compiling syn v1.0.109
   Compiling typenum v1.16.0
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling cfg-if v1.0.0
   Compiling getrandom v0.1.16
   Compiling subtle v2.4.1
   Compiling serde_derive v1.0.152
   Compiling serde v1.0.152
   Compiling unicode-xid v0.2.4
   Compiling byteorder v1.4.3
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling crunchy v0.2.2
   Compiling block-padding v0.2.1
   Compiling ppv-lite86 v0.2.17
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.94
   Compiling rand_core v0.6.4
   Compiling itoa v1.0.6
   Compiling hex v0.4.3
   Compiling static_assertions v1.1.0
   Compiling ryu v1.0.13
   Compiling wee_alloc v0.4.5
   Compiling base16 v0.2.1
   Compiling memory_units v0.4.0
   Compiling bitflags v1.3.2
   Compiling cfg-if v0.1.10
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling fnv v1.0.7
   Compiling strsim v0.9.3
   Compiling ident_case v1.0.1
   Compiling subtle v1.0.0
   Compiling byte-tools v0.3.1
   Compiling opaque-debug v0.2.3
   Compiling fake-simd v0.1.2
   Compiling tiny-keccak v2.0.2
   Compiling ahash v0.4.7
   Compiling thiserror v1.0.39
   Compiling derive_builder v0.9.0
   Compiling keccak v0.1.3
   Compiling arrayref v0.3.6
   Compiling cryptoxide v0.3.6
   Compiling rustc-hex v2.1.0
   Compiling rand v0.8.5
   Compiling generic-array v0.14.6
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling bitvec v0.18.5
   Compiling block-padding v0.1.5
   Compiling hashbrown v0.9.1
   Compiling rand_core v0.5.1
   Compiling uint v0.9.5
   Compiling rand_chacha v0.2.2
   Compiling rand v0.7.3
   Compiling generic-array v0.12.4
   Compiling digest v0.8.1
   Compiling crypto-mac v0.7.0
   Compiling block-buffer v0.7.3
   Compiling hmac v0.7.1
   Compiling sha2 v0.8.2
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling hmac-drbg v0.2.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling sha3 v0.9.1
   Compiling libsecp256k1 v0.3.5
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.3
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
   Compiling darling_core v0.10.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling borsh-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.3
   Compiling num-derive v0.3.3
   Compiling casper_types_derive v0.1.0
   Compiling thiserror-impl v1.0.39
   Compiling darling_macro v0.10.2
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling darling v0.10.2
   Compiling derive_builder_core v0.9.0
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.9
   Compiling toml v0.5.11
   Compiling casper-types v1.5.0
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.1.4
   Compiling common v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/common)
   Compiling liquid-base-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/crates/liquid-base-crate)
   Compiling liquid-transfer-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/crates/liquid-transfer-crate)
   Compiling casperlabs-erc20 v0.3.0
   Compiling casperlabs-cep47 v0.2.1
   Compiling liquid-helper-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/crates/liquid-helper-crate)
   Compiling liquid-locker-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker-crate)
   Compiling liquid-factory-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-factory/liquid-factory-crate)
   Compiling cep47 v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/mock-cep47)
   Compiling liquid-factory v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-factory/liquid-factory)
   Compiling erc20 v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/mock-erc20)
    Finished release [optimized] target(s) in 52.28s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cargo build --release -p liquid-locker -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
   Compiling liquid-locker v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker)
    Finished release [optimized] target(s) in 4.11s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make test-liquid-factory
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT'
make build-contract-liquid-factory && make copy-wasm-file-liquid-factory && make test-only-liquid-factory
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cargo build --release -p liquid-factory -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cp target/wasm32-unknown-unknown/release/liquid-factory.wasm Contracts/liquid-factory/liquid-factory-tests/wasm
cp target/wasm32-unknown-unknown/release/erc20-token.wasm Contracts/liquid-factory/liquid-factory-tests/wasm
cp target/wasm32-unknown-unknown/release/cep47-token.wasm Contracts/liquid-factory/liquid-factory-tests/wasm
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cargo test -p liquid-factory-tests
 Downloading crates ...
  Downloaded io-lifetimes v1.0.6
   Compiling proc-macro2 v1.0.51
   Compiling unicode-ident v1.0.8
   Compiling quote v1.0.23
   Compiling syn v1.0.109
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.139
   Compiling serde_derive v1.0.152
   Compiling typenum v1.16.0
   Compiling serde v1.0.152
   Compiling cfg-if v1.0.0
   Compiling libm v0.2.6
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling ppv-lite86 v0.2.17
   Compiling wyz v0.2.0
   Compiling io-lifetimes v1.0.6
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling byteorder v1.4.3
   Compiling bitflags v1.3.2
   Compiling rustix v0.36.9
   Compiling linux-raw-sys v0.1.4
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.94
   Compiling fastrand v1.9.0
   Compiling cpufeatures v0.2.5
   Compiling hashbrown v0.12.3
   Compiling bit-vec v0.6.3
   Compiling ryu v1.0.13
   Compiling schemars v0.8.5
   Compiling itoa v1.0.6
   Compiling fnv v1.0.7
   Compiling quick-error v1.2.3
   Compiling once_cell v1.17.1
   Compiling regex-syntax v0.6.28
   Compiling lazy_static v1.4.0
   Compiling static_assertions v1.1.0
   Compiling dyn-clone v1.0.11
   Compiling unarray v0.1.4
   Compiling quick-error v2.0.1
   Compiling base64 v0.13.1
   Compiling pkg-config v0.3.26
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling cc v1.0.79
   Compiling thiserror v1.0.39
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling wee_alloc v0.4.5
   Compiling anyhow v1.0.69
   Compiling either v1.8.1
   Compiling pin-project-lite v0.2.9
   Compiling memory_units v0.3.0
   Compiling memory_units v0.4.0
   Compiling iana-time-zone v0.1.53
   Compiling cfg-if v0.1.10
   Compiling match_cfg v0.1.0
   Compiling downcast-rs v1.2.0
   Compiling linked-hash-map v0.5.6
   Compiling rand_chacha v0.2.2
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.2
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.3
   Compiling bitvec v0.18.5
   Compiling tracing-core v0.1.30
   Compiling itertools v0.10.5
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling lmdb-sys v0.8.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling ff v0.8.0
   Compiling num-complex v0.4.3
   Compiling group v0.8.0
   Compiling getrandom v0.2.8
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.45
   Compiling hostname v0.3.1
   Compiling rand_core v0.6.4
   Compiling chrono v0.4.23
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling rand v0.8.5
   Compiling wasmi v0.8.0
   Compiling tempfile v3.4.0
   Compiling rusty-fork v0.3.0
   Compiling lmdb v0.8.0
   Compiling proptest v1.1.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.3
   Compiling datasize_derive v0.2.13
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.39
   Compiling tracing-attributes v0.1.23
   Compiling casper_types_derive v0.1.0
   Compiling datasize v0.2.13
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling tracing v0.1.37
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.9
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling pwasm-utils v0.16.0
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-execution-engine v1.5.0
   Compiling casper-engine-test-support v2.1.0
   Compiling test-env v0.1.0 (/workspace/CasperLabs-LiquidNFT/Contracts/utils/test-env)
   Compiling liquid-factory-tests v0.2.1 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-factory/liquid-factory-tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 18s
     Running unittests src/lib.rs (target/debug/deps/liquid_factory_tests-d3f92c4e429da554)

running 12 tests
test liquid_factory_tests::test_update_master ... ok
test liquid_factory_tests::test_revoke_master ... ok
test liquid_factory_tests::test_create_liquid_locker ... ok
test liquid_factory_tests::test_deploy ... ok
test liquid_factory_panic_tests::should_not_be_able_to_contribute_after_contribution_phase_end - should panic ... ok
test liquid_factory_flow_test::should_be_able_to_contribute_before_contribution_phase_end ... ok
test liquid_factory_tests::test_contribute_to_locker ... ok
test liquid_factory_flow_test::should_be_able_to_liquadate_locker_as_owner_didnt_do_payment_for_days ... ok
test liquid_factory_tests::test_donate_to_locker ... ok
test liquid_factory_flow_test::should_return_back_nft_to_owner_as_floor_not_reached_in_contribution_phase ... ok
test liquid_factory_tests::test_payback_to_locker ... ok
test liquid_factory_flow_test::test_contract_flow ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 40.35s

   Doc-tests liquid-factory-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
