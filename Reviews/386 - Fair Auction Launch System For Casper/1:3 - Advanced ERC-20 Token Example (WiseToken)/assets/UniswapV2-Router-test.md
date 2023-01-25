```
UniswapV2-Router (main) $ make test
# Test Library
cd ./uniswap-v2-library/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cargo build --release -p uniswap-v2-library --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.15s
wasm-strip target/wasm32-unknown-unknown/release/uniswap-v2-library.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm uniswap-v2-library-tests/wasm
cargo test -p uniswap-v2-library-tests
warning: unused variable: `router_contract`
   --> uniswap-v2-library-tests/src/uniswap_v2_library_tests.rs:261:55
    |
261 |     let (env, owner, test_contract, _, factory, pair, router_contract) = deploy_library();
    |                                                       ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `router_contract`
   --> uniswap-v2-library-tests/src/uniswap_v2_library_tests.rs:321:55
    |
321 |     let (env, owner, test_contract, _, factory, pair, router_contract) = deploy_library();
    |                                                       ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`

warning: unused variable: `router_contract`
   --> uniswap-v2-library-tests/src/uniswap_v2_library_tests.rs:380:55
    |
380 |     let (env, owner, test_contract, _, factory, pair, router_contract) = deploy_library();
    |                                                       ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`

warning: `uniswap-v2-library-tests` (lib test) generated 3 warnings
    Finished test [unoptimized + debuginfo] target(s) in 0.08s
     Running unittests src/lib.rs (target/debug/deps/uniswap_v2_library_tests-52b6480b8abd9e00)

running 7 tests
test uniswap_v2_library_tests::test_uniswap_get_amount_out ... ok
test uniswap_v2_library_tests::test_uniswap_get_amount_in ... ok
test uniswap_v2_library_tests::test_library_deploy ... ok
test uniswap_v2_library_tests::quote ... ok
test uniswap_v2_library_tests::test_uniswap_get_amounts_in ... ok
test uniswap_v2_library_tests::test_uniswap_get_reserves ... ok
test uniswap_v2_library_tests::test_uniswap_get_amounts_out ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 22.67s

   Doc-tests uniswap-v2-library-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
# Test Router
cd ./uniswap-v2-router/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
cargo build --release -p uniswap-v2-router --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.06s
wasm-strip uniswap-v2-router/target/wasm32-unknown-unknown/release/uniswap-v2-router.wasm 2>/dev/null | true
cargo build --release -p purse-proxy --target wasm32-unknown-unknown
   Compiling syn v1.0.107
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling serde v1.0.151
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.17
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling sha2 v0.9.9
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling ff v0.8.0
   Compiling ed25519 v1.2.0
   Compiling blake2 v0.9.2
   Compiling group v0.8.0
   Compiling hmac v0.10.1
   Compiling rand_chacha v0.2.2
   Compiling uint v0.9.5
   Compiling rand v0.7.3
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.3
   Compiling serde_derive v1.0.151
   Compiling num-derive v0.3.3
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
   Compiling purse-proxy v0.1.0 (/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router/purse-proxy)
    Finished release [optimized] target(s) in 24.38s
wasm-strip target/wasm32-unknown-unknown/release/purse-proxy.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm uniswap-v2-router-tests/wasm
cargo test -p uniswap-v2-router-tests
   Compiling proc-macro2 v1.0.49
   Compiling unicode-ident v1.0.6
   Compiling quote v1.0.23
   Compiling syn v1.0.107
   Compiling libc v0.2.138
   Compiling autocfg v1.1.0
   Compiling cfg-if v1.0.0
   Compiling typenum v1.16.0
   Compiling version_check v0.9.4
   Compiling serde_derive v1.0.151
   Compiling serde v1.0.151
   Compiling getrandom v0.1.16
   Compiling subtle v2.4.1
   Compiling byteorder v1.4.3
   Compiling ppv-lite86 v0.2.17
   Compiling unicode-xid v0.2.4
   Compiling fnv v1.0.7
   Compiling crunchy v0.2.2
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling opaque-debug v0.3.0
   Compiling block-padding v0.2.1
   Compiling fastrand v1.8.0
   Compiling serde_json v1.0.91
   Compiling remove_dir_all v0.5.3
   Compiling bitflags v1.3.2
   Compiling hashbrown v0.12.3
   Compiling ryu v1.0.12
   Compiling bit-vec v0.6.3
   Compiling quick-error v1.2.3
   Compiling itoa v1.0.5
   Compiling once_cell v1.16.0
   Compiling cpufeatures v0.2.5
   Compiling schemars v0.8.5
   Compiling quick-error v2.0.1
   Compiling lazy_static v1.4.0
   Compiling regex-syntax v0.6.28
   Compiling static_assertions v1.1.0
   Compiling dyn-clone v1.0.10
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling cc v1.0.78
   Compiling base64 v0.13.1
   Compiling thiserror v1.0.38
   Compiling pkg-config v0.3.26
   Compiling ident_case v1.0.1
   Compiling strsim v0.9.3
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling anyhow v1.0.68
   Compiling wee_alloc v0.4.5
   Compiling byte-tools v0.3.1
   Compiling either v1.8.0
   Compiling subtle v1.0.0
   Compiling iana-time-zone v0.1.53
   Compiling pin-project-lite v0.2.9
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.4.0
   Compiling cfg-if v0.1.10
   Compiling memory_units v0.3.0
   Compiling downcast-rs v1.2.0
   Compiling tiny-keccak v2.0.2
   Compiling ahash v0.4.7
   Compiling opaque-debug v0.2.3
   Compiling linked-hash-map v0.5.6
   Compiling fake-simd v0.1.2
   Compiling derive_builder v0.9.0
   Compiling keccak v0.1.3
   Compiling filesize v0.2.0
   Compiling arrayref v0.3.6
   Compiling rustc-hex v2.1.0
   Compiling more-asserts v0.2.2
   Compiling cryptoxide v0.3.6
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.2
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.3
   Compiling tracing-core v0.1.30
   Compiling bitvec v0.18.5
   Compiling block-padding v0.1.5
   Compiling itertools v0.10.5
   Compiling hashbrown v0.9.1
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.8
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.45
   Compiling num_cpus v1.14.0
   Compiling hostname v0.3.1
   Compiling lmdb-sys v0.8.0
   Compiling generic-array v0.12.4
   Compiling rand_core v0.6.4
   Compiling rand_core v0.5.1
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling rand_chacha v0.2.2
   Compiling digest v0.8.1
   Compiling crypto-mac v0.7.0
   Compiling block-buffer v0.7.3
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling hmac v0.7.1
   Compiling sha2 v0.8.2
   Compiling rand v0.8.5
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling ff v0.8.0
   Compiling sha2 v0.9.9
   Compiling sha3 v0.9.1
   Compiling blake2 v0.9.2
   Compiling rand v0.7.3
   Compiling hmac-drbg v0.2.0
   Compiling ed25519 v1.2.0
   Compiling group v0.8.0
   Compiling num-complex v0.4.2
   Compiling chrono v0.4.23
   Compiling proptest v1.0.0
   Compiling libsecp256k1 v0.3.5
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling darling_core v0.10.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling borsh-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.3
   Compiling datasize_derive v0.2.11
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.38
   Compiling tracing-attributes v0.1.23
   Compiling casper_types_derive v0.1.0
   Compiling darling_macro v0.10.2
   Compiling datasize v0.2.11
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling darling v0.10.2
   Compiling derive_builder_core v0.9.0
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling tracing v0.1.37
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.8
   Compiling toml v0.5.10
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling casper-types v1.5.0
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casper-execution-engine v2.0.1
   Compiling casperlabs-contract-utils v0.1.4
   Compiling casper-engine-test-support v2.2.0
   Compiling casperlabs-test-env v0.2.0
   Compiling uniswap-v2-router-tests v0.1.0 (/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router/uniswap-v2-router-tests)
warning: unused import: `cryptoxide::ed25519`
 --> uniswap-v2-router-tests/src/uniswap_instance.rs:5:5
  |
5 | use cryptoxide::ed25519;
  |     ^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::hash_message`
 --> uniswap-v2-router-tests/src/uniswap_instance.rs:6:5
  |
6 | use renvm_sig::hash_message;
  |     ^^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `renvm_sig::keccak256`
 --> uniswap-v2-router-tests/src/uniswap_instance.rs:7:5
  |
7 | use renvm_sig::keccak256;
  |     ^^^^^^^^^^^^^^^^^^^^

warning: unused variable: `router_contract`
   --> uniswap-v2-router-tests/src/uniswap_tests.rs:319:9
    |
319 |         router_contract,
    |         ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `router_contract`
   --> uniswap-v2-router-tests/src/uniswap_tests.rs:426:31
    |
426 |     let (env, uniswap, owner, router_contract, flash_swapper, _, token1, token2, _, _, factory) =
    |                               ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`

warning: unused variable: `router_contract`
   --> uniswap-v2-router-tests/src/uniswap_tests.rs:573:9
    |
573 |         router_contract,
    |         ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`

warning: unused variable: `router_contract`
   --> uniswap-v2-router-tests/src/uniswap_tests.rs:646:9
    |
646 |         router_contract,
    |         ^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_router_contract`

warning: `uniswap-v2-router-tests` (lib test) generated 7 warnings
    Finished test [unoptimized + debuginfo] target(s) in 1m 16s
     Running unittests src/lib.rs (target/debug/deps/uniswap_v2_router_tests-616bd6d1b262cb8c)

running 10 tests
test uniswap_tests::test_uniswap_deploy ... ok
test uniswap_tests::add_liquidity_cspr ... ok
test uniswap_tests::swap_exact_tokens_for_cspr ... ok
test uniswap_tests::swap_exact_cspr_for_tokens ... ok
test uniswap_tests::remove_liquidity ... ok
test uniswap_tests::add_liquidity ... ok
test uniswap_tests::swap_tokens_for_exact_tokens ... ok
test uniswap_tests::swap_exact_tokens_for_tokens ... ok
test uniswap_tests::swap_tokens_for_exact_cspr ... ok
test uniswap_tests::swap_cspr_for_exact_tokens ... ok

test result: ok. 10 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 41.15s

   Doc-tests uniswap-v2-router-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
```

