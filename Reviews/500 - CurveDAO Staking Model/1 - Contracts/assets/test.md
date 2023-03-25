```
$ make test-curve-token-v3
make build-contract-curve-token-v3 && make copy-wasm-file-curve-token-v3 && make test-only-curve-token-v3
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p curve-erc20 -p curve-rewards -p curve-token-v3 -p test-session-code --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.10s
wasm-strip target/wasm32-unknown-unknown/release/curve-token-v3.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-token-v3.wasm ./curve-token-v3/curve-token-v3-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./curve-token-v3/curve-token-v3-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./curve-token-v3/curve-token-v3-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-rewards.wasm ./curve-token-v3/curve-token-v3-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p curve-token-v3-tests
  Downloaded casper-execution-engine v1.5.0
  Downloaded filesize v0.2.0
  Downloaded casperlabs-test-env v0.3.0
  Downloaded casper-engine-test-support v2.2.0
  Downloaded 4 crates (236.1 KB) in 0.32s
   Compiling proc-macro2 v1.0.50
   Compiling quote v1.0.23
   Compiling unicode-ident v1.0.6
   Compiling syn v1.0.107
   Compiling libc v0.2.139
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling cfg-if v1.0.0
   Compiling typenum v1.16.0
   Compiling serde_derive v1.0.152
   Compiling serde v1.0.152
   Compiling subtle v2.4.1
   Compiling getrandom v0.1.16
   Compiling crunchy v0.2.2
   Compiling fnv v1.0.7
   Compiling unicode-xid v0.2.4
   Compiling ppv-lite86 v0.2.17
   Compiling wyz v0.2.0
   Compiling block-padding v0.2.1
   Compiling opaque-debug v0.3.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling byteorder v1.4.3
   Compiling cpufeatures v0.2.5
   Compiling serde_json v1.0.91
   Compiling fastrand v1.8.0
   Compiling remove_dir_all v0.5.3
   Compiling quick-error v1.2.3
   Compiling bit-vec v0.6.3
   Compiling bitflags v1.3.2
   Compiling itoa v1.0.5
   Compiling hashbrown v0.12.3
   Compiling schemars v0.8.5
   Compiling ryu v1.0.12
   Compiling once_cell v1.17.0
   Compiling static_assertions v1.1.0
   Compiling dyn-clone v1.0.10
   Compiling quick-error v2.0.1
   Compiling regex-syntax v0.6.28
   Compiling lazy_static v1.4.0
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling thiserror v1.0.38
   Compiling pkg-config v0.3.26
   Compiling wee_alloc v0.4.5
   Compiling cc v1.0.78
   Compiling ident_case v1.0.1
   Compiling log v0.4.17
   Compiling parity-wasm v0.41.0
   Compiling strsim v0.9.3
   Compiling memory_units v0.4.0
   Compiling cfg-if v0.1.10
   Compiling either v1.8.1
   Compiling anyhow v1.0.68
   Compiling pin-project-lite v0.2.9
   Compiling match_cfg v0.1.0
   Compiling downcast-rs v1.2.0
   Compiling memory_units v0.3.0
   Compiling iana-time-zone v0.1.53
   Compiling tiny-keccak v2.0.2
   Compiling linked-hash-map v0.5.6
   Compiling derive_builder v0.9.0
   Compiling ahash v0.4.7
   Compiling keccak v0.1.3
   Compiling base64 v0.12.3
   Compiling arrayref v0.3.6
   Compiling filesize v0.2.0
   Compiling rustc-hex v2.1.0
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling bit-set v0.5.3
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.2
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling tracing-core v0.1.30
   Compiling bitvec v0.18.5
   Compiling itertools v0.10.5
   Compiling hashbrown v0.9.1
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.8
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.45
   Compiling hostname v0.3.1
   Compiling num_cpus v1.15.0
   Compiling lmdb-sys v0.8.0
   Compiling rand_core v0.5.1
   Compiling rand_core v0.6.4
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.2.2
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling ff v0.8.0
   Compiling rand v0.7.3
   Compiling num-complex v0.4.3
   Compiling group v0.8.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling rand v0.8.5
   Compiling signature v1.2.2
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling libsecp256k1-core v0.2.2
   Compiling hmac v0.8.1
   Compiling sha3 v0.9.1
   Compiling hmac v0.10.1
   Compiling chrono v0.4.23
   Compiling ed25519 v1.2.0
   Compiling hmac-drbg v0.3.0
   Compiling proptest v1.0.0
   Compiling libsecp256k1-gen-ecmult v0.2.1
   Compiling libsecp256k1-gen-genmult v0.2.1
   Compiling libsecp256k1 v0.5.0
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling darling_core v0.10.2
   Compiling borsh-derive-internal v0.8.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.3
   Compiling datasize_derive v0.2.13
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling thiserror-impl v1.0.38
   Compiling ctor v0.1.26
   Compiling tracing-attributes v0.1.23
   Compiling casper_types_derive v0.1.0
   Compiling darling_macro v0.10.2
   Compiling datasize v0.2.13
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling darling v0.10.2
   Compiling ecdsa v0.10.2
   Compiling derive_builder_core v0.9.0
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling tracing v0.1.37
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.8
   Compiling toml v0.5.11
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling casper-types v1.5.0
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)
   Compiling casper-contract v1.4.4
   Compiling casper-hashing v1.4.3
   Compiling casper-execution-engine v2.0.1
   Compiling casper-execution-engine v1.5.0
   Compiling casperlabs-contract-utils v0.2.2
   Compiling curve-casper-erc20 v0.1.0
   Compiling common v0.2.0 (/workspace/CasperLabs-Curve-DAO/common)
   Compiling crv20 v0.1.0
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.3.0
   Compiling curve-token-v3-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/curve-token-v3/curve-token-v3-tests)
    Finished test [unoptimized + debuginfo] target(s) in 2m 29s
     Running unittests src/lib.rs (target/debug/deps/curve_token_v3_tests-bc96b943260a2f70)

running 10 tests
test curve_token_v3_tests::deployment ... ok
test curve_token_v3_tests::burn_from ... ok
test curve_token_v3_tests::mint ... ok
test curve_token_v3_tests::transfer ... ok
test curve_token_v3_tests::set_minter ... ok
test curve_token_v3_tests::test_set_name ... ok
test curve_token_v3_tests::decimals ... ok
test curve_token_v3_tests::transfer_from ... ok
test curve_token_v3_tests::increase_allowance ... ok
test curve_token_v3_tests::decrease_allowance ... ok

test result: ok. 10 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 33.20s

   Doc-tests curve-token-v3-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

########################################################################################################

$ make test-curve-erc20
make build-contract-curve-erc20 && make copy-wasm-file-curve-erc20 && make test-only-curve-erc20
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p curve-erc20 --target wasm32-unknown-unknown
   Compiling syn v1.0.107
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling serde v1.0.152
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.17
   Compiling hex v0.4.3
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling sha2 v0.9.9
   Compiling signature v1.2.2
   Compiling ff v0.8.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling ed25519 v1.2.0
   Compiling hmac v0.10.1
   Compiling group v0.8.0
   Compiling blake2 v0.9.2
   Compiling rand_chacha v0.2.2
   Compiling uint v0.9.5
   Compiling rand v0.7.3
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.3
   Compiling serde_derive v1.0.152
   Compiling num-derive v0.3.3
   Compiling casper_types_derive v0.1.0
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_json v1.0.91
   Compiling serde_bytes v0.11.8
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling curve-casper-erc20 v0.1.0
   Compiling casperlabs-contract-utils v0.2.2
   Compiling crv20 v0.1.0
   Compiling curve-erc20 v0.1.0 (/workspace/CasperLabs-Curve-DAO/curve-erc20/curve-erc20)
    Finished release [optimized] target(s) in 33.94s
wasm-strip target/wasm32-unknown-unknown/release/curve-erc20.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./curve-erc20/curve-erc20-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p curve-erc20-tests
   Compiling syn v1.0.107
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling crunchy v0.2.2
   Compiling block-buffer v0.9.0
   Compiling sha2 v0.9.9
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling hmac v0.10.1
   Compiling group v0.8.0
   Compiling ed25519 v1.2.0
   Compiling blake2 v0.9.2
   Compiling rand v0.7.3
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling serde_derive v1.0.152
   Compiling zeroize_derive v1.3.3
   Compiling datasize_derive v0.2.13
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.38
   Compiling tracing-attributes v0.1.23
   Compiling casper_types_derive v0.1.0
   Compiling value-bag v1.0.0-alpha.9
   Compiling datasize v0.2.13
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling thiserror v1.0.38
   Compiling tracing v0.1.37
   Compiling serde v1.0.152
   Compiling hex v0.4.3
   Compiling num-rational v0.4.1
   Compiling indexmap v1.9.2
   Compiling serde_json v1.0.91
   Compiling serde_bytes v0.11.8
   Compiling log v0.4.17
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling schemars v0.8.5
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling casper-hashing v1.4.3
   Compiling casperlabs-contract-utils v0.2.2
   Compiling curve-casper-erc20 v0.1.0
   Compiling casper-execution-engine v2.0.1
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.3.0
   Compiling curve-erc20-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/curve-erc20/curve-erc20-tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 19s
     Running unittests src/lib.rs (target/debug/deps/curve_erc20_tests-6e71f80411db9311)

running 8 tests
test curve_erc20_tests::test_deploy ... ok
test curve_erc20_tests::test_erc20_transfer_account_zero_address_check - should panic ... ok
test curve_erc20_tests::test_erc20_transfer ... ok
test curve_erc20_tests::test_set_name_symbol ... ok
test curve_erc20_tests::test_erc20_mint_burn ... ok
test curve_erc20_tests::test_erc20_approve_transfer_from ... ok
test curve_erc20_tests::test_erc20_approve_transfer_from_zero_address_check - should panic ... ok
test curve_erc20_tests::test_erc20_increase_decrease_allowance ... ok

test result: ok. 8 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 10.70s

   Doc-tests curve-erc20-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

######################################################################################################

$ make test-erc20-crv
make build-contract-erc20-crv && make copy-wasm-file-erc20-crv && make test-only-erc20-crv
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p erc20-crv-session-code -p erc20-crv --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.10s
wasm-strip target/wasm32-unknown-unknown/release/erc20-crv.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//erc20-crv-session-code.wasm ./erc20-crv/erc20-crv-tests/wasm
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./erc20-crv/erc20-crv-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./erc20-crv/erc20-crv-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p erc20-crv-tests
  Downloaded casperlabs-test-env v0.1.2
  Downloaded 1 crate (3.7 KB) in 0.23s
   Compiling base64 v0.13.1
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling casper-hashing v1.4.3
   Compiling casperlabs-contract-utils v0.2.2
   Compiling curve-casper-erc20 v0.1.0
   Compiling common v0.2.0 (/workspace/CasperLabs-Curve-DAO/common)
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-execution-engine v2.0.1
   Compiling casper-execution-engine v1.5.0
   Compiling crv20 v0.1.0
   Compiling erc20-crv v0.1.0 (/workspace/CasperLabs-Curve-DAO/erc20-crv/erc20-crv)
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.1.2
   Compiling erc20-crv-tests v0.2.0 (/workspace/CasperLabs-Curve-DAO/erc20-crv/erc20-crv-tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 11s
     Running unittests src/lib.rs (target/debug/deps/erc20_crv_tests-8a6dc65b6bc8388f)

running 16 tests
test erc20_crv_tests::test_start_epoch_time_write ... ok
test erc20_crv_tests::test_update_mining_parameters ... ok
test erc20_crv_tests::set_and_remove_admin ... ok
test erc20_crv_tests::test_mintable_in_timeframe ... ok
test erc20_crv_tests::test_future_epoch_time_write ... ok
test erc20_crv_tests::test_transfer ... ok
test erc20_crv_tests::test_set_minter ... ok
test erc20_crv_tests::test_total_supply ... ok
test erc20_crv_tests::test_deploy ... ok
test erc20_crv_tests::test_available_supply ... ok
test erc20_crv_tests::test_increase_allowance ... ok
test erc20_crv_tests::test_mint ... ok
test erc20_crv_tests::test_transfer_from ... ok
test erc20_crv_tests::burn ... ok
test erc20_crv_tests::test_decrease_allowance ... ok
test erc20_crv_tests::test_allowance ... ok

test result: ok. 16 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 36.27s

   Doc-tests erc20-crv-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

########################################################################################################

$ make test-fee-distributor
make build-contract-fee-distributor && make copy-wasm-file-fee-distributor && make test-only-fee-distributor
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p curve-erc20 -p fee-distributor-session-code -p voting-escrow -p fee-distributor -p erc20-crv --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.10s
wasm-strip target/wasm32-unknown-unknown/release/fee-distributor.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//fee-distributor-session-code.wasm ./fee-distributor/fee-distributor-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./fee-distributor/fee-distributor-tests/wasm
cp ./target/wasm32-unknown-unknown/release//fee-distributor.wasm ./fee-distributor/fee-distributor-tests/wasm
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./fee-distributor/fee-distributor-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./fee-distributor/fee-distributor-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./fee-distributor/fee-distributor-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p fee-distributor-tests 
   Compiling fee-distributor-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/fee-distributor/fee-distributor-crate)
   Compiling fee-distributor-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/fee-distributor/fee-distributor-tests)
    Finished test [unoptimized + debuginfo] target(s) in 5.63s
     Running unittests src/lib.rs (target/debug/deps/fee_distributor_tests-2e4297a65bc022e4)

running 12 tests
test fee_distributor_tests::test_checkpoint_token ... ok
test fee_distributor_tests::test_burn ... ok
test fee_distributor_tests::test_apply_admin ... ok
test fee_distributor_tests::test_deploy ... ok
test fee_distributor_tests::test_toggle_allow_checkpoint_token ... ok
test fee_distributor_tests::test_ve_for_at ... ok
test fee_distributor_tests::test_commit_admin ... ok
test fee_distributor_tests::test_kill_me ... ok
test fee_distributor_tests::test_recover_balance ... ok
test fee_distributor_tests::test_checkpoint_total_supply ... ok
test fee_distributor_tests::test_claim ... ok
test fee_distributor_tests::test_claim_many ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 56.23s

   Doc-tests fee-distributor-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

##########################################################################################################################

$ make test-gauge-controller
make build-contract-gauge-controller && make copy-wasm-file-gauge-controller && make test-only-gauge-controller
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p minter -p test-session-code -p erc20-crv -p liquidity-gauge-v3 -p gauge-controller-session-code -p curve-erc20 -p voting-escrow -p gauge-controller --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.50s
wasm-strip target/wasm32-unknown-unknown/release/gauge-controller-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//gauge-controller-token.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//minter-token.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-v3.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//gauge-controller-session-code.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./gauge-controller/gauge-controller-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./gauge-controller/gauge-controller-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p gauge-controller-tests ownership_and_deploy_test_cases -- --test-threads=1
   Compiling base64 v0.13.1
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling common v0.2.0 (/workspace/CasperLabs-Curve-DAO/common)
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-execution-engine v2.0.1
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.1.2
   Compiling gauge-controller-tests v0.2.1 (/workspace/CasperLabs-Curve-DAO/gauge-controller/gauge-controller-tests)
    Finished test [unoptimized + debuginfo] target(s) in 57.01s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 3 tests
test gauge_controller_tests::ownership_and_deploy_test_cases::test_deploy ... ok
test gauge_controller_tests::ownership_and_deploy_test_cases::test_gauge_controller_apply_transfer_ownership ... ok
test gauge_controller_tests::ownership_and_deploy_test_cases::test_gauge_controller_commit_transfer_ownership ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 42 filtered out; finished in 32.55s

cargo test -p gauge-controller-tests checkpoint_function_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.17s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 5 tests
test gauge_controller_tests::checkpoint_function_test_cases::test_gauge_controller_change_type_weight ... ok
test gauge_controller_tests::checkpoint_function_test_cases::test_gauge_controller_checkpoint ... ok
test gauge_controller_tests::checkpoint_function_test_cases::test_gauge_controller_checkpoint_by_user ... ok
test gauge_controller_tests::checkpoint_function_test_cases::test_gauge_controller_checkpoint_gauge ... ok
test gauge_controller_tests::checkpoint_function_test_cases::test_gauge_controller_checkpoint_gauge_by_user ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 40 filtered out; finished in 58.02s

cargo test -p gauge-controller-tests vote_function_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 45 filtered out; finished in 0.00s

cargo test -p gauge-controller-tests gauge_types_and_add_type_functions_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 5 tests
test gauge_controller_tests::gauge_types_and_add_type_functions_test_cases::test_gauge_controller_add_type ... ok
test gauge_controller_tests::gauge_types_and_add_type_functions_test_cases::test_gauge_controller_gauge_types ... ok
test gauge_controller_tests::gauge_types_and_add_type_functions_test_cases::test_gauge_controller_gauge_types_by_user ... ok
test gauge_controller_tests::gauge_types_and_add_type_functions_test_cases::test_gauge_controller_gauge_types_by_user_multiple_times ... ok
test gauge_controller_tests::gauge_types_and_add_type_functions_test_cases::test_gauge_controller_gauge_types_multiple_times ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 40 filtered out; finished in 59.09s

cargo test -p gauge-controller-tests get_gauge_and_sum_per_type_weight_test_cases  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 5 tests
test gauge_controller_tests::get_gauge_and_sum_per_type_weight_test_cases::test_gauge_controller_get_gauge_weight ... ok
test gauge_controller_tests::get_gauge_and_sum_per_type_weight_test_cases::test_gauge_controller_get_gauge_weight_multiple_users ... ok
test gauge_controller_tests::get_gauge_and_sum_per_type_weight_test_cases::test_gauge_controller_get_weights_sum_per_type ... ok
test gauge_controller_tests::get_gauge_and_sum_per_type_weight_test_cases::test_gauge_controller_get_weights_sum_per_type_by_user ... ok
test gauge_controller_tests::get_gauge_and_sum_per_type_weight_test_cases::test_gauge_controller_get_weights_sum_per_type_multiple_times ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 40 filtered out; finished in 71.36s

cargo test -p gauge-controller-tests add_gauge_function_test_cases  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 2 tests
test gauge_controller_tests::add_gauge_function_test_cases::test_gauge_controller_add_gauge ... ok
test gauge_controller_tests::add_gauge_function_test_cases::test_gauge_controller_add_gauge_multiple_time ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 43 filtered out; finished in 23.01s

cargo test -p gauge-controller-tests panic_test_cases_1  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.11s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 6 tests
test gauge_controller_tests::panic_test_cases_1::test_gauge_controller_add_gauge_by_user - should panic ... ok
test gauge_controller_tests::panic_test_cases_1::test_gauge_controller_add_gauge_multiple_time_by_user - should panic ... ok
test gauge_controller_tests::panic_test_cases_1::test_gauge_controller_apply_transfer_ownership_by_user - should panic ... ok
test gauge_controller_tests::panic_test_cases_1::test_gauge_controller_change_gauge_weight_without_adding_gauge - should panic ... ok
test gauge_controller_tests::panic_test_cases_1::test_gauge_controller_gauge_types_without_adding_gauge_types - should panic ... ok
test gauge_controller_tests::panic_test_cases_1::test_gauge_controller_vote_for_gauge_weights_by_user - should panic ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 39 filtered out; finished in 66.86s

cargo test -p gauge-controller-tests panic_test_cases_2  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 6 tests
test gauge_controller_tests::panic_test_cases_2::test_deploy_with_address_zero - should panic ... ok
test gauge_controller_tests::panic_test_cases_2::test_gauge_controller_apply_transfer_ownership_without_commiting_transfer_ownership - should panic ... ok
test gauge_controller_tests::panic_test_cases_2::test_gauge_controller_change_gauge_weight_by_user - should panic ... ok
test gauge_controller_tests::panic_test_cases_2::test_gauge_controller_change_gauge_weight_without_adding_type - should panic ... ok
test gauge_controller_tests::panic_test_cases_2::test_gauge_controller_change_type_weight_by_user - should panic ... ok
test gauge_controller_tests::panic_test_cases_2::test_gauge_controller_commit_transfer_ownership_by_user - should panic ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 39 filtered out; finished in 56.12s

cargo test -p gauge-controller-tests change_gauge_test_cases  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.11s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 2 tests
test gauge_controller_tests::change_gauge_test_cases::test_gauge_controller_change_gauge_weight ... ok
test gauge_controller_tests::change_gauge_test_cases::test_gauge_controller_change_gauge_weight_multiple_time ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 43 filtered out; finished in 24.98s

cargo test -p gauge-controller-tests gauge_relative_weight_test_cases  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 5 tests
test gauge_controller_tests::gauge_relative_weight_test_cases::test_gauge_controller_gauge_relative_weight ... ok
test gauge_controller_tests::gauge_relative_weight_test_cases::test_gauge_controller_gauge_relative_weight_by_user ... ok
test gauge_controller_tests::gauge_relative_weight_test_cases::test_gauge_controller_gauge_relative_weight_without_adding_gauge ... ok
test gauge_controller_tests::gauge_relative_weight_test_cases::test_gauge_controller_gauge_relative_weight_write ... ok
test gauge_controller_tests::gauge_relative_weight_test_cases::test_gauge_controller_gauge_relative_weight_write_by_user ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 40 filtered out; finished in 68.03s

cargo test -p gauge-controller-tests get_type_and_total_weight_test_cases  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.11s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 3 tests
test gauge_controller_tests::get_type_and_total_weight_test_cases::test_gauge_controller_get_total_weight ... ok
test gauge_controller_tests::get_type_and_total_weight_test_cases::test_gauge_controller_get_total_weight_by_user ... ok
test gauge_controller_tests::get_type_and_total_weight_test_cases::test_gauge_controller_get_type_weight ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 42 filtered out; finished in 41.12s

cargo test -p gauge-controller-tests vote_functions_and_effect_with_period_test_cases  -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/gauge_controller_tests-aedad2d2300dcc57)

running 3 tests
test gauge_controller_tests::vote_functions_and_effect_with_period_test_cases::test_effect_on_following_period ... ok
test gauge_controller_tests::vote_functions_and_effect_with_period_test_cases::test_gauge_controller_vote_for_gauge_weights ... ok
test gauge_controller_tests::vote_functions_and_effect_with_period_test_cases::test_gauge_controller_vote_for_gauge_weights_multiple_time ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 42 filtered out; finished in 49.01s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

##################################################################################################################

$ make test-gauge-proxy
make build-contract-gauge-proxy && make copy-wasm-file-gauge-proxy && make test-only-gauge-proxy
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p gauge-proxy --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.17s
wasm-strip target/wasm32-unknown-unknown/release/gauge-proxy.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//gauge-proxy.wasm ./gauge-proxy/gauge-proxy-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p gauge-proxy-tests
   Compiling gauge-proxy-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/gauge-proxy/gauge-proxy-crate)
   Compiling gauge-proxy-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/gauge-proxy/gauge-proxy-tests)
    Finished test [unoptimized + debuginfo] target(s) in 6.70s
     Running unittests src/lib.rs (target/debug/deps/gauge_proxy_tests-8ebf097c52a971b6)

running 3 tests
test gauge_proxy_tests::test_deploy ... ok
test gauge_proxy_tests::test_commit_set_admins ... ok
test gauge_proxy_tests::test_accept_set_admins ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.55s

   Doc-tests gauge-proxy-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

###########################################################################################################

$ make test-liquidity-gauge-reward
make build-contract-liquidity-gauge-reward && make copy-wasm-file-liquidity-gauge-reward && make test-only-liquidity-gauge-reward
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p liquidity-gauge-reward-session-code -p test-session-code -p curve-rewards -p erc20-crv -p curve-erc20 -p voting-escrow -p gauge-controller  -p minter -p liquidity-gauge-reward --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.12s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-reward.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//gauge-controller-token.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-reward-session-code.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//minter-token.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-reward.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-rewards.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./liquidity-gauge-reward/liquidity-gauge-reward-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p liquidity-gauge-reward-tests deploy_checkpoints_and_claimable_tokens_and_reward_test_cases -- --test-threads=1
   Compiling liquidity-gauge-reward-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward/liquidity-gauge-reward-crate)
   Compiling liquidity-gauge-reward-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward/liquidity-gauge-reward-tests)
    Finished test [unoptimized + debuginfo] target(s) in 7.55s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_tests-d9a8c9b0b69ebd37)

running 6 tests
test liquidity_gauge_reward_tests::deploy_checkpoints_and_claimable_tokens_and_reward_test_cases::test_claim_rewards ... ok
test liquidity_gauge_reward_tests::deploy_checkpoints_and_claimable_tokens_and_reward_test_cases::test_claimable_reward ... ok
test liquidity_gauge_reward_tests::deploy_checkpoints_and_claimable_tokens_and_reward_test_cases::test_claimable_tokens ... ok
test liquidity_gauge_reward_tests::deploy_checkpoints_and_claimable_tokens_and_reward_test_cases::test_deploy ... ok
test liquidity_gauge_reward_tests::deploy_checkpoints_and_claimable_tokens_and_reward_test_cases::test_integrate_checkpoint ... ok
test liquidity_gauge_reward_tests::deploy_checkpoints_and_claimable_tokens_and_reward_test_cases::test_user_checkpoint ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 9 filtered out; finished in 71.26s

cargo test -p liquidity-gauge-reward-tests deposit_withdraw_kill_me_and_approve_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.15s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_tests-d9a8c9b0b69ebd37)

running 4 tests
test liquidity_gauge_reward_tests::deposit_withdraw_kill_me_and_approve_test_cases::test_deposit ... ok
test liquidity_gauge_reward_tests::deposit_withdraw_kill_me_and_approve_test_cases::test_kill_me ... ok
test liquidity_gauge_reward_tests::deposit_withdraw_kill_me_and_approve_test_cases::test_set_approve_deposit ... ok
test liquidity_gauge_reward_tests::deposit_withdraw_kill_me_and_approve_test_cases::test_withdraw ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 11 filtered out; finished in 54.58s

cargo test -p liquidity-gauge-reward-tests ownership_and_toggle_external_rewards_claim_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.14s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_tests-d9a8c9b0b69ebd37)

running 3 tests
test liquidity_gauge_reward_tests::ownership_and_toggle_external_rewards_claim_test_cases::test_apply_transfer_ownership ... ok
test liquidity_gauge_reward_tests::ownership_and_toggle_external_rewards_claim_test_cases::test_commit_transfer_ownership ... ok
test liquidity_gauge_reward_tests::ownership_and_toggle_external_rewards_claim_test_cases::test_toggle_external_rewards_claim ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 12 filtered out; finished in 34.24s

cargo test -p liquidity-gauge-reward-tests panic_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_tests-d9a8c9b0b69ebd37)

running 2 tests
test liquidity_gauge_reward_tests::panic_test_cases::test_apply_transfer_ownership_panic - should panic ... ok
test liquidity_gauge_reward_tests::panic_test_cases::test_withdraw_panic - should panic ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 13 filtered out; finished in 21.55s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

############################################################################################################################

$ make test-liquidity-gauge-reward-wrapper
make build-contract-liquidity-gauge-reward-wrapper && make copy-wasm-file-liquidity-gauge-reward-wrapper && make test-only-liquidity-gauge-reward-wrapper
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p erc20-crv -p curve-erc20 -p test-session-code -p minter -p voting-escrow -p gauge-controller -p liquidity-gauge-reward -p liquidity-gauge-reward-wrapper -p liquidity-gauge-reward-wrapper-session-code -p curve-rewards --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.14s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-reward-wrapper.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-reward-wrapper.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-reward-wrapper-session-code.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//minter-token.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-reward.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-rewards.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//gauge-controller-token.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p liquidity-gauge-reward-wrapper-tests panic_test_cases -- --test-threads=1
   Compiling liquidity-gauge-reward-wrapper-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-crate)
   Compiling liquidity-gauge-reward-wrapper-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-tests)
    Finished test [unoptimized + debuginfo] target(s) in 7.57s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_wrapper_tests-bec54f94a4dbb473)

running 5 tests
test liquidity_gauge_reward_wrapper_tests::panic_test_cases::test_apply_transfer_ownership_panic - should panic ... ok
test liquidity_gauge_reward_wrapper_tests::panic_test_cases::test_decrease_allowance_panic - should panic ... ok
test liquidity_gauge_reward_wrapper_tests::panic_test_cases::test_transfer_from_panic - should panic ... ok
test liquidity_gauge_reward_wrapper_tests::panic_test_cases::test_transfer_panic - should panic ... ok
test liquidity_gauge_reward_wrapper_tests::panic_test_cases::test_withdraw_panic - should panic ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 17 filtered out; finished in 108.35s

cargo test -p liquidity-gauge-reward-wrapper-tests allowance_and_approve_functions_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.45s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_wrapper_tests-bec54f94a4dbb473)

running 4 tests
test liquidity_gauge_reward_wrapper_tests::allowance_and_approve_functions_test_cases::test_allowance ... ok
test liquidity_gauge_reward_wrapper_tests::allowance_and_approve_functions_test_cases::test_approve ... ok
test liquidity_gauge_reward_wrapper_tests::allowance_and_approve_functions_test_cases::test_decrease_allowance ... ok
test liquidity_gauge_reward_wrapper_tests::allowance_and_approve_functions_test_cases::test_increase_allowance ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 18 filtered out; finished in 80.18s

cargo test -p liquidity-gauge-reward-wrapper-tests ownership_and_kill_functions_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.35s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_wrapper_tests-bec54f94a4dbb473)

running 3 tests
test liquidity_gauge_reward_wrapper_tests::ownership_and_kill_functions_test_cases::test_apply_transfer_ownership ... ok
test liquidity_gauge_reward_wrapper_tests::ownership_and_kill_functions_test_cases::test_commit_transfer_ownership ... ok
test liquidity_gauge_reward_wrapper_tests::ownership_and_kill_functions_test_cases::test_kill_me ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 19 filtered out; finished in 51.24s

cargo test -p liquidity-gauge-reward-wrapper-tests deposit_withdraw_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_wrapper_tests-bec54f94a4dbb473)

running 3 tests
test liquidity_gauge_reward_wrapper_tests::deposit_withdraw_test_cases::test_deposit ... ok
test liquidity_gauge_reward_wrapper_tests::deposit_withdraw_test_cases::test_set_approve_deposit ... ok
test liquidity_gauge_reward_wrapper_tests::deposit_withdraw_test_cases::test_withdraw ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 19 filtered out; finished in 78.45s

cargo test -p liquidity-gauge-reward-wrapper-tests transfer_and_transfer_from_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_wrapper_tests-bec54f94a4dbb473)

running 2 tests
test liquidity_gauge_reward_wrapper_tests::transfer_and_transfer_from_test_cases::test_transfer ... ok
test liquidity_gauge_reward_wrapper_tests::transfer_and_transfer_from_test_cases::test_transfer_from ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 20 filtered out; finished in 75.39s

cargo test -p liquidity-gauge-reward-wrapper-tests checkpoint_deploy_and_claim_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.14s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_reward_wrapper_tests-bec54f94a4dbb473)

running 5 tests
test liquidity_gauge_reward_wrapper_tests::checkpoint_deploy_and_claim_test_cases::test_claim_tokens ... ok
test liquidity_gauge_reward_wrapper_tests::checkpoint_deploy_and_claim_test_cases::test_claimable_reward ... ok
test liquidity_gauge_reward_wrapper_tests::checkpoint_deploy_and_claim_test_cases::test_claimable_tokens ... ok
test liquidity_gauge_reward_wrapper_tests::checkpoint_deploy_and_claim_test_cases::test_deploy ... ok
test liquidity_gauge_reward_wrapper_tests::checkpoint_deploy_and_claim_test_cases::test_user_checkpoint ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 17 filtered out; finished in 150.38s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

#######################################################################################################################

$ make test-liquidity-gauge-wrapper
make build-contract-liquidity-gauge-wrapper && make copy-wasm-file-liquidity-gauge-wrapper && make test-only-liquidity-gauge-wrapper
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p erc20-crv -p curve-erc20 -p test-session-code -p minter -p liquidity-gauge-v3 -p voting-escrow -p gauge-controller -p liquidity-gauge-wrapper-session-code -p liquidity-gauge-wrapper --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.52s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-wrapper.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-wrapper.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-wrapper-session-code.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//minter-token.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-v3.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//gauge-controller-token.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p liquidity-gauge-wrapper-tests panic_test_cases -- --test-threads=1
   Compiling liquidity-gauge-wrapper-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-wrapper/liquidity-gauge-wrapper-crate)
   Compiling liquidity-gauge-wrapper-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-wrapper/liquidity-gauge-wrapper-tests)
    Finished test [unoptimized + debuginfo] target(s) in 9.66s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 5 tests
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_apply_transfer_ownership - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_decrease_allowance - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_transfer - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_transfer_from - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_withdraw - should panic ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 16 filtered out; finished in 207.23s

cargo test -p liquidity-gauge-wrapper-tests allowance_and_approve_functions_test_cases_1 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.33s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 2 tests
test liquidity_gauge_wrapper_tests::allowance_and_approve_functions_test_cases_1::test_allowance ... ok
test liquidity_gauge_wrapper_tests::allowance_and_approve_functions_test_cases_1::test_approve ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 19 filtered out; finished in 325.50s

cargo test -p liquidity-gauge-wrapper-tests allowance_and_approve_functions_test_cases_2 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.38s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 2 tests
test liquidity_gauge_wrapper_tests::allowance_and_approve_functions_test_cases_2::test_decrease_allowance ... ok
test liquidity_gauge_wrapper_tests::allowance_and_approve_functions_test_cases_2::test_increase_allowance ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 19 filtered out; finished in 26.54s

cargo test -p liquidity-gauge-wrapper-tests ownership_and_kill_functions_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 3 tests
test liquidity_gauge_wrapper_tests::ownership_and_kill_functions_test_cases::test_apply_transfer_ownership ... ok
test liquidity_gauge_wrapper_tests::ownership_and_kill_functions_test_cases::test_commit_transfer_ownership ... ok
test liquidity_gauge_wrapper_tests::ownership_and_kill_functions_test_cases::test_kill_me ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 18 filtered out; finished in 41.11s

cargo test -p liquidity-gauge-wrapper-tests test_deposit -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 1 test
test liquidity_gauge_wrapper_tests::test_deposit ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 20 filtered out; finished in 305.40s

cargo test -p liquidity-gauge-wrapper-tests panic_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.36s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 5 tests
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_apply_transfer_ownership - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_decrease_allowance - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_transfer - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_transfer_from - should panic ... ok
test liquidity_gauge_wrapper_tests::panic_test_cases::test_panic_withdraw - should panic ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 16 filtered out; finished in 215.19s

# Intense memory test cases below (Require 32gb + RAM)
# cargo test -p liquidity-gauge-wrapper-tests test_withdraw -- --test-threads=1
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

##################################################################################################################################

$ cargo test -p liquidity-gauge-wrapper-tests test_withdraw -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.41s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_wrapper_tests-3e994078fb6738fe)

running 1 test
test liquidity_gauge_wrapper_tests::test_withdraw ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 20 filtered out; finished in 631.27s

#####################################################################################################################################

$ make test-minter
make build-contract-minter && make copy-wasm-file-minter && make test-only-minter
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p curve-erc20 -p erc20-crv -p erc20-crv-session-code -p liquidity-gauge-v3 -p liquidity-gauge-reward -p voting-escrow -p gauge-controller -p minter --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.57s
wasm-strip target/wasm32-unknown-unknown/release/minter-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//minter-token.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//gauge-controller-token.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-reward.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//liquidity-gauge-v3.wasm ./minter/minter-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-rewards.wasm ./minter/minter-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p minter-tests
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-execution-engine v2.0.1
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.1.2
   Compiling minter-tests v0.2.1 (/workspace/CasperLabs-Curve-DAO/minter/minter-tests)
    Finished test [unoptimized + debuginfo] target(s) in 54.02s
     Running unittests src/lib.rs (target/debug/deps/minter_tests-e0af022758c0f920)

running 6 tests
test minter_tests::test_deploy ... ok
test minter_tests::test_minter_toggle_approve_mint ... ok
test minter_tests::test_minter_mint has been running for over 60 seconds
test minter_tests::test_minter_mint_for has been running for over 60 seconds
test minter_tests::test_minter_mint_many has been running for over 60 seconds
test minter_tests::test_minter_mint_with_deposit has been running for over 60 seconds
test minter_tests::test_minter_mint ... ok
test minter_tests::test_minter_mint_many ... ok
test minter_tests::test_minter_mint_for ... ok
test minter_tests::test_minter_mint_with_deposit ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 391.55s

   Doc-tests minter-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

####################################################################################################

$ make test-reward-only-gauge
make build-contract-reward-only-gauge && make copy-wasm-file-reward-only-gauge && make test-only-reward-only-gauge
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p curve-erc20 -p erc20-crv -p curve-rewards -p reward-only-gauge -p reward-only-gauge-session-code --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.32s
wasm-strip target/wasm32-unknown-unknown/release/reward-only-gauge.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//erc20-crv.wasm ./reward-only-gauge/reward-only-gauge-tests/wasm
cp ./target/wasm32-unknown-unknown/release//reward-only-gauge-token.wasm ./reward-only-gauge/reward-only-gauge-tests/wasm
cp ./target/wasm32-unknown-unknown/release//reward-only-gauge-session-code.wasm ./reward-only-gauge/reward-only-gauge-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-rewards.wasm ./reward-only-gauge/reward-only-gauge-tests/wasm
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./reward-only-gauge/reward-only-gauge-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./reward-only-gauge/reward-only-gauge-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p reward-only-gauge-tests deploy_and_reward_contract_test_cases -- --test-threads=1
   Compiling reward-only-gauge-tests v0.2.1 (/workspace/CasperLabs-Curve-DAO/reward-only-gauge/reward-only-gauge-tests)
    Finished test [unoptimized + debuginfo] target(s) in 9.15s
     Running unittests src/lib.rs (target/debug/deps/reward_only_gauge_tests-0c6a237c6820def4)

running 2 tests
test reward_only_gauge_tests::deploy_and_reward_contract_test_cases::test_deploy ... ok
test reward_only_gauge_tests::deploy_and_reward_contract_test_cases::test_reward_contract ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 16 filtered out; finished in 7.90s

cargo test -p reward-only-gauge-tests ownership_and_set_reward_receiver_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.15s
     Running unittests src/lib.rs (target/debug/deps/reward_only_gauge_tests-0c6a237c6820def4)

running 3 tests
test reward_only_gauge_tests::ownership_and_set_reward_receiver_test_cases::test_accept_transfer_ownership ... ok
test reward_only_gauge_tests::ownership_and_set_reward_receiver_test_cases::test_commit_transfer_ownership ... ok
test reward_only_gauge_tests::ownership_and_set_reward_receiver_test_cases::test_set_rewards_receiver ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 15 filtered out; finished in 12.65s

cargo test -p reward-only-gauge-tests approve_and_allowances_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/reward_only_gauge_tests-0c6a237c6820def4)

running 3 tests
test reward_only_gauge_tests::approve_and_allowances_test_cases::test_approve ... ok
test reward_only_gauge_tests::approve_and_allowances_test_cases::test_decrease_allowance ... ok
test reward_only_gauge_tests::approve_and_allowances_test_cases::test_increase_allowance ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 15 filtered out; finished in 12.69s

cargo test -p reward-only-gauge-tests test_cases_related_to_rewards -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/reward_only_gauge_tests-0c6a237c6820def4)

running 6 tests
test reward_only_gauge_tests::test_cases_related_to_rewards::test_claim_rewards ... ok
test reward_only_gauge_tests::test_cases_related_to_rewards::test_claimable_reward ... ok
test reward_only_gauge_tests::test_cases_related_to_rewards::test_claimable_reward_write ... ok
test reward_only_gauge_tests::test_cases_related_to_rewards::test_claimed_reward ... ok
test reward_only_gauge_tests::test_cases_related_to_rewards::test_last_claim ... ok
test reward_only_gauge_tests::test_cases_related_to_rewards::test_set_rewards ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 12 filtered out; finished in 56.72s

cargo test -p reward-only-gauge-tests deposit_and_withdraw_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.28s
     Running unittests src/lib.rs (target/debug/deps/reward_only_gauge_tests-0c6a237c6820def4)

running 2 tests
test reward_only_gauge_tests::deposit_and_withdraw_test_cases::test_deposit ... ok
test reward_only_gauge_tests::deposit_and_withdraw_test_cases::test_withdraw ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 16 filtered out; finished in 10.17s

cargo test -p reward-only-gauge-tests transfer_and_transfer_from_test_cases -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/reward_only_gauge_tests-0c6a237c6820def4)

running 2 tests
test reward_only_gauge_tests::transfer_and_transfer_from_test_cases::test_transfer ... ok
test reward_only_gauge_tests::transfer_and_transfer_from_test_cases::test_transfer_from ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 16 filtered out; finished in 10.40s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

#####################################################################################################

$ make test-vesting-escrow
make build-contract-vesting-escrow && make copy-wasm-file-vesting-escrow && make test-only-vesting-escrow
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p vesting-escrow-session-code  -p curve-erc20 -p vesting-escrow --target wasm32-unknown-unknown
^[[D    Finished release [optimized] target(s) in 0.47s
wasm-strip target/wasm32-unknown-unknown/release/vesting-escrow.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./vesting-escrow/vesting-escrow-tests/wasm
cp ./target/wasm32-unknown-unknown/release//vesting-escrow-token.wasm ./vesting-escrow/vesting-escrow-tests/wasm
cp ./target/wasm32-unknown-unknown/release//vesting-escrow-session-code.wasm ./vesting-escrow/vesting-escrow-tests/wasm
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./vesting-escrow/vesting-escrow-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p vesting-escrow-tests
   Compiling vesting-escrow-tests v0.2.1 (/workspace/CasperLabs-Curve-DAO/vesting-escrow/vesting-escrow-tests)
    Finished test [unoptimized + debuginfo] target(s) in 10.21s
     Running unittests src/lib.rs (target/debug/deps/vesting_escrow_tests-463c41477e1a96e3)

running 18 tests
test vesting_escrow_tests::test_vesting_escrow_deploy ... ok
test vesting_escrow_tests::test_vesting_escrow_toggle_disable_when_disabled - should panic ... ok
test vesting_escrow_tests::test_vesting_escrow_commit_transfer_ownership ... ok
test vesting_escrow_tests::test_vesting_escrow_disable_fund_admins ... ok
test vesting_escrow_tests::test_vesting_escrow_toggle_disable_by_user - should panic ... ok
test vesting_escrow_tests::test_vesting_escrow_disable_can_disable ... ok
test vesting_escrow_tests::test_vesting_escrow_toggle_disable_after_toggle_disable ... ok
test vesting_escrow_tests::test_vesting_escrow_toggle_disable ... ok
test vesting_escrow_tests::test_vesting_escrow_apply_transfer_ownership ... ok
test vesting_escrow_tests::test_vesting_escrow_add_tokens_by_user - should panic ... ok
test vesting_escrow_tests::test_vesting_escrow_fund ... ok
test vesting_escrow_tests::test_vesting_escrow_fund_by_user - should panic ... ok
test vesting_escrow_tests::test_vesting_escrow_add_tokens ... ok
test vesting_escrow_tests::test_vesting_escrow_locked_supply ... ok
test vesting_escrow_tests::test_vesting_escrow_locked_of ... ok
test vesting_escrow_tests::test_vesting_escrow_balance_of ... ok
test vesting_escrow_tests::test_vesting_escrow_vested_supply ... ok
test vesting_escrow_tests::test_vesting_escrow_vested_of ... ok

test result: ok. 18 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 32.40s

   Doc-tests vesting-escrow-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

######################################################################################################

$ make test-vesting-escrow-factory
make build-contract-vesting-escrow-factory && make copy-wasm-file-vesting-escrow-factory && make test-only-vesting-escrow-factory
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p vesting-escrow-simple -p curve-erc20 -p vesting-escrow-factory -p vesting-escrow-factory-session-code --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.30s
wasm-strip target/wasm32-unknown-unknown/release/vesting-escrow-factory.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./vesting-escrow-factory/vesting-escrow-factory-tests/wasm
cp ./target/wasm32-unknown-unknown/release//vesting-escrow-factory-token.wasm ./vesting-escrow-factory/vesting-escrow-factory-tests/wasm
cp ./target/wasm32-unknown-unknown/release//vesting-escrow-factory-session-code.wasm ./vesting-escrow-factory/vesting-escrow-factory-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p vesting-escrow-factory-tests
   Compiling vesting-escrow-factory-tests v0.2.1 (/workspace/CasperLabs-Curve-DAO/vesting-escrow-factory/vesting-escrow-factory-tests)
    Finished test [unoptimized + debuginfo] target(s) in 7.19s
     Running unittests src/lib.rs (target/debug/deps/vesting_escrow_factory_tests-c98f4d0a73fa1f80)

running 4 tests
test vesting_escrow_factory_tests::test_deploy ... ok
test vesting_escrow_factory_tests::test_commit_transfer_ownership ... ok
test vesting_escrow_factory_tests::test_accept_transfer_ownership ... ok
test vesting_escrow_factory_tests::test_deploy_vesting_contract ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 5.99s

   Doc-tests vesting-escrow-factory-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

#################################################################################################

$ make test-voting-escrow
make build-contract-voting-escrow && make copy-wasm-file-voting-escrow && make test-only-voting-escrow
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p erc20-crv -p voting-escrow --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.28s
wasm-strip target/wasm32-unknown-unknown/release/vesting_escrow_simple.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./voting-escrow/voting-escrow-tests/wasm
cp ./target/wasm32-unknown-unknown/release//voting-escrow.wasm ./voting-escrow/voting-escrow-tests/wasm
cp ./target/wasm32-unknown-unknown/release//*.wasm ./voting-escrow/voting-escrow-tests/wasm
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p voting-escrow-tests
   Compiling casperlabs-test-env v0.3.0
   Compiling voting-escrow-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/voting-escrow/voting-escrow-crate)
   Compiling voting-escrow-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/voting-escrow/voting-escrow-tests)
    Finished test [unoptimized + debuginfo] target(s) in 12.58s
     Running unittests src/lib.rs (target/debug/deps/voting_escrow_tests-d52f889d0d12b409)

running 17 tests
test voting_escrow_tests::test_commit_transfer_ownership ... ok
test voting_escrow_tests::test_change_controller ... ok
test voting_escrow_tests::test_deploy ... ok
test voting_escrow_tests::test_checkpoint ... ok
test voting_escrow_tests::test_apply_transfer_ownership has been running for over 60 seconds
test voting_escrow_tests::test_balance_of has been running for over 60 seconds
test voting_escrow_tests::test_balance_of_at has been running for over 60 seconds
test voting_escrow_tests::test_create_lock has been running for over 60 seconds
test voting_escrow_tests::test_deposit_for has been running for over 60 seconds
test voting_escrow_tests::test_get_last_user_slope has been running for over 60 seconds
test voting_escrow_tests::test_increase_amount has been running for over 60 seconds
test voting_escrow_tests::test_increase_unlock_time has been running for over 60 seconds
test voting_escrow_tests::test_locked_end has been running for over 60 seconds
test voting_escrow_tests::test_total_supply has been running for over 60 seconds
test voting_escrow_tests::test_total_supply_at has been running for over 60 seconds
test voting_escrow_tests::test_user_point_history_ts has been running for over 60 seconds
test voting_escrow_tests::test_apply_transfer_ownership ... ok
test voting_escrow_tests::test_get_last_user_slope ... ok
test voting_escrow_tests::test_locked_end ... ok
test voting_escrow_tests::test_create_lock ... ok
test voting_escrow_tests::test_user_point_history_ts ... ok
test voting_escrow_tests::test_balance_of ... ok
test voting_escrow_tests::test_balance_of_at ... ok
test voting_escrow_tests::test_increase_unlock_time ... ok
test voting_escrow_tests::test_total_supply_at ... ok
test voting_escrow_tests::test_increase_amount ... ok
test voting_escrow_tests::test_deposit_for ... ok
test voting_escrow_tests::test_withdraw ... ok
test voting_escrow_tests::test_total_supply ... ok

test result: ok. 17 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 81.72s

   Doc-tests voting-escrow-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

###################################################################################################

$ make test-ownable
make build-contract-ownable && make copy-wasm-file-ownable && make test-only-ownable
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p ownable --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.28s
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//ownable.wasm ./ownable/ownable-tests/wasm/
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./ownable/ownable-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p ownable-tests 
   Compiling ownable-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/ownable/ownable-tests)
    Finished test [unoptimized + debuginfo] target(s) in 8.91s
     Running unittests src/lib.rs (target/debug/deps/ownable_tests-737632b5e64f32f1)

running 4 tests
test ownable_tests::test_deploy ... ok
test ownable_tests::renounce_ownership ... ok
test ownable_tests::transfer_ownership ... ok
test ownable_tests::is_owner ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.89s

   Doc-tests ownable-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

##############################################################################################

$ make test-i-reward-distribution-recipient
make build-i-reward-distribution-recipient && make copy-wasm-file-i-reward-distribution-recipient && make test-only-i-reward-distribution-recipient
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p i-reward-distribution-recipient --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.37s
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//i-reward-distribution-recipient.wasm ./i-reward-distribution-recipient/i-reward-distribution-recipient-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p i-reward-distribution-recipient-tests
   Compiling i-reward-distribution-recipient-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/i-reward-distribution-recipient/i-reward-distribution-recipient-tests)
    Finished test [unoptimized + debuginfo] target(s) in 9.44s
     Running unittests src/lib.rs (target/debug/deps/i_reward_distribution_recipient_tests-df53f2f7ca0f15da)

running 2 tests
test i_reward_distribution_recipient_tests::test_deploy ... ok
test i_reward_distribution_recipient_tests::test_set_reward_distribution ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.90s

   Doc-tests i-reward-distribution-recipient-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

##########################################################################################

$ make test-lp-token-wrapper
make build-contract-curve-erc20 && make build-lp-token-wrapper && make copy-wasm-file-lp-token-wrapper && make test-only-lp-token-wrapper
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p curve-erc20 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.30s
wasm-strip target/wasm32-unknown-unknown/release/curve-erc20.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release  -p test-session-code -p lp-token-wrapper --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.18s
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./lp-token-wrapper/lp-token-wrapper-tests/wasm/
cp ./target/wasm32-unknown-unknown/release//lp-token-wrapper.wasm ./lp-token-wrapper/lp-token-wrapper-tests/wasm/
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./lp-token-wrapper/lp-token-wrapper-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p lp-token-wrapper-tests
   Compiling lp-token-wrapper-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/lp-token-wrapper/lp-token-wrapper-tests)
    Finished test [unoptimized + debuginfo] target(s) in 9.11s
     Running unittests src/lib.rs (target/debug/deps/lp_token_wrapper_tests-50d4ee5dd962b2f7)

running 6 tests
test lp_token_wrapper_tests::test_deploy ... ok
test lp_token_wrapper_tests::withdraw_panic - should panic ... ok
test lp_token_wrapper_tests::total_supply ... ok
test lp_token_wrapper_tests::balance_of ... ok
test lp_token_wrapper_tests::stake ... ok
test lp_token_wrapper_tests::withdraw ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 8.20s

   Doc-tests lp-token-wrapper-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

#################################################################################################

$ make test-curve-rewards
make build-curve-rewards && make copy-wasm-file-curve-rewards && make test-only-curve-rewards
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p curve-erc20 -p test-session-code -p curve-rewards --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.31s
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release//curve-erc20.wasm ./curve-rewards/curve-rewards-tests/wasm/
cp ./target/wasm32-unknown-unknown/release//curve-rewards.wasm ./curve-rewards/curve-rewards-tests/wasm/
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./curve-rewards/curve-rewards-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p curve-rewards-tests 
   Compiling curve-rewards-tests v0.1.0 (/workspace/CasperLabs-Curve-DAO/curve-rewards/curve-rewards-tests)
    Finished test [unoptimized + debuginfo] target(s) in 10.21s
     Running unittests src/lib.rs (target/debug/deps/curve_rewards_tests-8bbdffbcb8e117c9)

running 11 tests
test curve_rewards_tests::test_deploy ... ok
test curve_rewards_tests::last_time_reward_applicable ... ok
test curve_rewards_tests::withdraw_panic - should panic ... ok
test curve_rewards_tests::exit_panic - should panic ... ok
test curve_rewards_tests::stake ... ok
test curve_rewards_tests::reward_per_token ... ok
test curve_rewards_tests::exit ... ok
test curve_rewards_tests::get_reward ... ok
test curve_rewards_tests::earned ... ok
test curve_rewards_tests::withdraw ... ok
test curve_rewards_tests::notify_reward_amount ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 17.73s

   Doc-tests curve-rewards-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

##############################################################################################

$ make test-liquidity-gauge-v3
make build-contract-liquidity-gauge-v3 && make copy-wasm-file-liquidity-gauge-v3 && make test-only-liquidity-gauge-v3
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo build --release -p test-session-code -p liquidity-gauge-v3-session-code -p liquidity-gauge-v3 -p curve-erc20 -p minter -p voting-escrow -p gauge-controller -p erc20-crv  --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.27s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-v3.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cp ./target/wasm32-unknown-unknown/release/liquidity-gauge-v3.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release/curve-erc20.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release/erc20-crv.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release/gauge-controller-token.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release/minter-token.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release/voting-escrow.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release/liquidity_gauge_v3_session_code.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
cp ./target/wasm32-unknown-unknown/release//test-session-code.wasm ./liquidity-gauge-v3/liquidity-gauge-v3-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'
make[1]: Entering directory '/workspace/CasperLabs-Curve-DAO'
cargo test -p liquidity-gauge-v3-tests t1 -- --test-threads=1
   Compiling liquidity-gauge-v3-tests v0.2.1 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-v3/liquidity-gauge-v3-tests)
    Finished test [unoptimized + debuginfo] target(s) in 7.69s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 6 tests
test liquidity_gauge_v3_tests::t10::test_claimable_tokens ... ok
test liquidity_gauge_v3_tests::t11::test_user_checkpoint ... ok
test liquidity_gauge_v3_tests::t12::test_accept_transfer_ownership ... ok
test liquidity_gauge_v3_tests::t12::test_set_killed ... ok
test liquidity_gauge_v3_tests::t1::test_commit_transfer_ownership ... ok
test liquidity_gauge_v3_tests::t1::test_deploy ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 17 filtered out; finished in 349.53s

cargo test -p liquidity-gauge-v3-tests t2 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.40s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 4 tests
test liquidity_gauge_v3_tests::t2::test_approve ... ok
test liquidity_gauge_v3_tests::t2::test_decimals ... ok
test liquidity_gauge_v3_tests::t2::test_decrease_allowance ... ok
test liquidity_gauge_v3_tests::t2::test_increase_allowance ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 19 filtered out; finished in 40.15s

cargo test -p liquidity-gauge-v3-tests t3 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 4 tests
test liquidity_gauge_v3_tests::t3::test_claimed_reward ... ok
test liquidity_gauge_v3_tests::t3::test_integrate_checkpoint ... ok
test liquidity_gauge_v3_tests::t3::test_last_claim ... ok
test liquidity_gauge_v3_tests::t3::test_reward_contract ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 19 filtered out; finished in 39.74s

cargo test -p liquidity-gauge-v3-tests t4 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 2 tests
test liquidity_gauge_v3_tests::t4::test_claimable_reward ... ok
test liquidity_gauge_v3_tests::t4::test_claimable_reward_write ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 21 filtered out; finished in 20.11s

cargo test -p liquidity-gauge-v3-tests t5 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 3 tests
test liquidity_gauge_v3_tests::t5::test_claim_rewards ... ok
test liquidity_gauge_v3_tests::t5::test_set_rewards ... ok
test liquidity_gauge_v3_tests::t5::test_set_rewards_receiver ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 20 filtered out; finished in 31.51s

cargo test -p liquidity-gauge-v3-tests t6 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.11s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 1 test
test liquidity_gauge_v3_tests::t6::test_deposit ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 22 filtered out; finished in 139.49s

cargo test -p liquidity-gauge-v3-tests t7 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.34s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 1 test
test liquidity_gauge_v3_tests::t7::test_withdraw ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 22 filtered out; finished in 311.32s

cargo test -p liquidity-gauge-v3-tests t10 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.44s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 1 test
test liquidity_gauge_v3_tests::t10::test_claimable_tokens ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 22 filtered out; finished in 156.08s

cargo test -p liquidity-gauge-v3-tests t11 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.56s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 1 test
test liquidity_gauge_v3_tests::t11::test_user_checkpoint ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 22 filtered out; finished in 141.73s

cargo test -p liquidity-gauge-v3-tests t12 -- --test-threads=1
    Finished test [unoptimized + debuginfo] target(s) in 0.39s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 2 tests
test liquidity_gauge_v3_tests::t12::test_accept_transfer_ownership ... ok
test liquidity_gauge_v3_tests::t12::test_set_killed ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 21 filtered out; finished in 20.38s

# Intense memory test cases below (Require 32gb + RAM)
# cargo test -p liquidity-gauge-v3-tests t8
# cargo test -p liquidity-gauge-v3-tests t9
make[1]: Leaving directory '/workspace/CasperLabs-Curve-DAO'

########################################################################################################

$ cargo test -p liquidity-gauge-v3-tests t8
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/liquidity_gauge_v3_tests-edaeae9a8a587287)

running 1 test
test liquidity_gauge_v3_tests::t8::test_transfer has been running for over 60 seconds
test liquidity_gauge_v3_tests::t8::test_transfer ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 22 filtered out; finished in 419.96s

##########################################################################################################
```
