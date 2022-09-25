```
$ make test-all
make test-liquid-factory && make test-liquid-helper && make test-liquid-locker
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make build-contract-liquid-factory && make copy-wasm-file-liquid-factory && make test-only-liquid-factory
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cargo build --release -p liquid-factory -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cp target/wasm32-unknown-unknown/release/liquid-factory.wasm liquid-factory/liquid-factory-tests/wasm
cp target/wasm32-unknown-unknown/release/erc20-token.wasm liquid-factory/liquid-factory-tests/wasm
cp target/wasm32-unknown-unknown/release/cep47-token.wasm liquid-factory/liquid-factory-tests/wasm
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cargo test -p liquid-factory-tests
  Downloaded casper-execution-engine v1.5.0
  Downloaded casper-engine-test-support v2.1.0
  Downloaded 2 crates (221.3 KB) in 0.27s
   Compiling proc-macro2 v1.0.43
   Compiling unicode-ident v1.0.3
   Compiling quote v1.0.21
   Compiling syn v1.0.99
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.132
   Compiling typenum v1.15.0
   Compiling serde_derive v1.0.144
   Compiling serde v1.0.144
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.3
   Compiling ppv-lite86 v0.2.16
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling byteorder v1.4.3
   Compiling fastrand v1.8.0
   Compiling serde_json v1.0.85
   Compiling opaque-debug v0.3.0
   Compiling remove_dir_all v0.5.3
   Compiling crunchy v0.2.2
   Compiling quick-error v1.2.3
   Compiling hashbrown v0.12.3
   Compiling schemars v0.8.5
   Compiling bit-vec v0.6.3
   Compiling cpufeatures v0.2.5
   Compiling ryu v1.0.11
   Compiling bitflags v1.3.2
   Compiling once_cell v1.14.0
   Compiling fnv v1.0.7
   Compiling itoa v1.0.3
   Compiling dyn-clone v1.0.9
   Compiling static_assertions v1.1.0
   Compiling quick-error v2.0.1
   Compiling regex-syntax v0.6.27
   Compiling lazy_static v1.4.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.0
   Compiling cc v1.0.73
   Compiling hex_fmt v0.3.0
   Compiling pkg-config v0.3.25
   Compiling log v0.4.17
   Compiling parity-wasm v0.41.0
   Compiling anyhow v1.0.64
   Compiling wee_alloc v0.4.5
   Compiling either v1.8.0
   Compiling memory_units v0.4.0
   Compiling memory_units v0.3.0
   Compiling iana-time-zone v0.1.47
   Compiling cfg-if v0.1.10
   Compiling downcast-rs v1.2.0
   Compiling pin-project-lite v0.2.9
   Compiling match_cfg v0.1.0
   Compiling linked-hash-map v0.5.6
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.3
   Compiling tracing-core v0.1.29
   Compiling itertools v0.10.3
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.7
   Compiling tempfile v3.3.0
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.44
   Compiling hostname v0.3.1
   Compiling rand_core v0.6.3
   Compiling rusty-fork v0.3.0
   Compiling lmdb-sys v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling ff v0.8.0
   Compiling rand v0.8.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling group v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling proptest v1.0.0
   Compiling chrono v0.4.22
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.2
   Compiling schemars_derive v0.8.5
   Compiling datasize_derive v0.2.10
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.23
   Compiling thiserror-impl v1.0.34
   Compiling tracing-attributes v0.1.22
   Compiling casper_types_derive v0.1.0
   Compiling datasize v0.2.10
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling thiserror v1.0.34
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling tracing v0.1.36
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.7
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
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-engine-test-support v2.1.0
   Compiling test-env v0.1.0 (/workspace/CasperLabs-LiquidNFT/Contracts/utils/test-env)
   Compiling liquid-factory-tests v0.2.1 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-factory/liquid-factory-tests)
    Finished test [unoptimized + debuginfo] target(s) in 55.73s
     Running unittests src/lib.rs (target/debug/deps/liquid_factory_tests-220b26130ee572dd)

running 12 tests
test liquid_factory_tests::test_update_master ... ok
test liquid_factory_tests::test_revoke_master ... ok
test liquid_factory_tests::test_create_empty_locker ... ok
test liquid_factory_tests::test_contribute_to_locker ... ok
test liquid_factory_tests::test_donate_to_locker ... ok
test liquid_factory_tests::test_create_liquid_locker ... ok
test liquid_factory_panic_tests::should_not_be_able_to_contribute_after_contribution_phase_end - should panic ... ok
test liquid_factory_flow_test::should_be_able_to_contribute_before_contribution_phase_end ... ok
test liquid_factory_flow_test::should_be_able_to_liquadate_locker_as_owner_didnt_do_payment_for_days ... ok
test liquid_factory_flow_test::should_return_back_nft_to_owner_as_floor_not_reached_in_contribution_phase ... ok
test liquid_factory_tests::test_payback_to_locker ... ok
test liquid_factory_flow_test::test_contract_flow ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 26.52s

   Doc-tests liquid-factory-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make build-contract-liquid-helper && make copy-wasm-file-liquid-helper && make test-only-liquid-helper
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cargo build --release -p liquid-helper -p liquid-helper-proxy --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cp target/wasm32-unknown-unknown/release/liquid-helper.wasm liquid-helper/liquid-helper-tests/wasm
cp target/wasm32-unknown-unknown/release/liquid-helper-proxy.wasm liquid-helper/liquid-helper-tests/wasm
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cargo test -p liquid-helper-tests
  Downloaded casperlabs-test-env v0.1.0
  Downloaded 1 crate (3.6 KB) in 0.55s
   Compiling casperlabs-test-env v0.1.0
   Compiling liquid-helper-tests v0.2.1 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-helper/liquid-helper-tests)
    Finished test [unoptimized + debuginfo] target(s) in 7.41s
     Running unittests src/lib.rs (target/debug/deps/liquid_helper_tests-40080fd342242fae)

running 15 tests
test liquid_helper_tests::missed_deadline ... ok
test liquid_helper_tests::not_single_provider ... ok
test liquid_helper_tests::test_deploy ... ok
test liquid_helper_tests::ownerless_locker ... ok
test liquid_helper_tests::get_tokens ... ok
test liquid_helper_tests::missed_activate ... ok
test liquid_helper_tests::time_since ... ok
test liquid_helper_tests::liquidate_to ... ok
test liquid_helper_tests::starting_timestamp ... ok
test liquid_helper_tests::payback_timestamp ... ok
test liquid_helper_tests::reached_total ... ok
test liquid_helper_tests::floor_not_reached ... ok
test liquid_helper_tests::contribution_phase ... ok
test liquid_helper_tests::payment_time_not_set ... ok
test liquid_helper_tests::below_floor_asked ... ok

test result: ok. 15 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 4.40s

   Doc-tests liquid-helper-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make build-contract-liquid-locker && make copy-wasm-file-liquid-locker && make test-only-liquid-locker
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cargo build --release -p liquid-locker -p liquid-locker-proxy -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cp target/wasm32-unknown-unknown/release/liquid-locker.wasm liquid-locker/liquid-locker-tests/wasm
cp target/wasm32-unknown-unknown/release/liquid-locker-proxy.wasm liquid-locker/liquid-locker-tests/wasm
cp target/wasm32-unknown-unknown/release/cep47-token.wasm liquid-locker/liquid-locker-tests/wasm
cp target/wasm32-unknown-unknown/release/erc20-token.wasm liquid-locker/liquid-locker-tests/wasm
make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[2]: Entering directory '/workspace/CasperLabs-LiquidNFT/Contracts'
cargo test -p liquid-locker-tests
   Compiling liquid-locker-tests v0.1.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker-tests)
    Finished test [unoptimized + debuginfo] target(s) in 4.41s
     Running unittests src/lib.rs (target/debug/deps/liquid_locker_tests-9387e45962dbba39)

running 16 tests
test liquid_locker_tests::test_deploy ... ok
test liquid_locker_tests::test_calculate_epoch ... ok
test liquid_locker_tests::test_contribution_phase ... ok
test liquid_locker_tests::test_intialize ... ok
test liquid_locker_tests::test_decrease_payment_time ... ok
test liquid_locker_tests::test_increase_payment_rate ... ok
test liquid_locker_tests::test_donate_funds ... ok
test liquid_locker_tests::test_disable_locker ... ok
test liquid_locker_tests::test_claim_interest_public ... ok
test liquid_locker_tests::test_liquidate_locker ... ok
test liquid_locker_tests::test_rescue_locker ... ok
test liquid_locker_tests::test_refund_due_disabled ... ok
test liquid_locker_tests::test_enable_locker ... ok
test liquid_locker_tests::test_claim_interest_single ... ok
test liquid_locker_tests::test_pay_back_funds ... ok
test liquid_locker_tests::test_refund_due_single ... ok

test result: ok. 16 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 16.69s

   Doc-tests liquid-locker-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT/Contracts'
```
