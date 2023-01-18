```
$ make test
cargo build --release -p wcspr --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-token.wasm 2>/dev/null | true
cargo build --release -p test --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-complex v0.4.2
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling test v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract)
    Finished release [optimized] target(s) in 18.94s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-test.wasm 2>/dev/null | true
cargo build --release -p test2 --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
   Compiling test2 v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2)
    Finished release [optimized] target(s) in 2.02s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-test2.wasm 2>/dev/null | true
cargo build --release -p purse-proxy --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
   Compiling purse-proxy v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/wcspr/purse-proxy)
    Finished release [optimized] target(s) in 1.00s
wasm-strip target/wasm32-unknown-unknown/release/purse-proxy.wasm 2>/dev/null | true
cargo build --release -p invalid-purse-proxy --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
   Compiling invalid-purse-proxy v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/wcspr/invalid-purse-proxy)
warning: unused import: `system`
  --> invalid-purse-proxy/src/main.rs:12:38
   |
12 |     contract_api::{account, runtime, system},
   |                                      ^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `invalid-purse-proxy` (bin "invalid-purse-proxy") generated 1 warning
    Finished release [optimized] target(s) in 0.96s
wasm-strip target/wasm32-unknown-unknown/release/invalid-purse-proxy.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm wcspr-tests/wasm
# cp test-contract/target/wasm32-unknown-unknown/release/*.wasm wcspr-tests/wasm
cargo test -p wcspr-tests
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
  Downloaded ctor v0.1.23
  Downloaded num_cpus v1.13.1
  Downloaded cc v1.0.73
  Downloaded time v0.1.44
  Downloaded pkg-config v0.3.25
  Downloaded either v1.7.0
  Downloaded regex-syntax v0.6.27
  Downloaded tracing-core v0.1.29
  Downloaded dyn-clone v1.0.9
  Downloaded tracing-attributes v0.1.22
  Downloaded iana-time-zone v0.1.42
  Downloaded casper-execution-engine v2.0.0
  Downloaded once_cell v1.13.0
  Downloaded itertools v0.10.3
  Downloaded datasize_derive v0.2.10
  Downloaded datasize v0.2.10
  Downloaded indexmap v1.9.1
  Downloaded getrandom v0.2.7
  Downloaded chrono v0.4.21
  Downloaded anyhow v1.0.61
  Downloaded tracing v0.1.36
  Downloaded 21 crates (1.3 MB) in 0.73s
   Compiling proc-macro2 v1.0.43
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.3
   Compiling syn v1.0.99
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.129
   Compiling serde_derive v1.0.143
   Compiling typenum v1.15.0
   Compiling serde v1.0.143
   Compiling cfg-if v1.0.0
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.3
   Compiling ppv-lite86 v0.2.16
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling fastrand v1.8.0
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.83
   Compiling remove_dir_all v0.5.3
   Compiling bit-vec v0.6.3
   Compiling quick-error v1.2.3
   Compiling fnv v1.0.7
   Compiling schemars v0.8.5
   Compiling hashbrown v0.12.3
   Compiling once_cell v1.13.0
   Compiling cpufeatures v0.2.2
   Compiling ryu v1.0.11
   Compiling bitflags v1.3.2
   Compiling itoa v1.0.3
   Compiling dyn-clone v1.0.9
   Compiling lazy_static v1.4.0
   Compiling regex-syntax v0.6.27
   Compiling quick-error v2.0.1
   Compiling static_assertions v1.1.0
   Compiling cc v1.0.73
   Compiling base64 v0.13.0
   Compiling hex_fmt v0.3.0
   Compiling pkg-config v0.3.25
   Compiling base16 v0.2.1
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling anyhow v1.0.61
   Compiling either v1.7.0
   Compiling wee_alloc v0.4.5
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling downcast-rs v1.2.0
   Compiling cfg-if v0.1.10
   Compiling iana-time-zone v0.1.42
   Compiling memory_units v0.4.0
   Compiling pin-project-lite v0.2.9
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling rand_chacha v0.2.2
   Compiling bit-set v0.5.3
   Compiling bitvec v0.18.5
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling tracing-core v0.1.29
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling indexmap v1.9.1
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling itertools v0.10.3
   Compiling rand v0.7.3
   Compiling getrandom v0.2.7
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.44
   Compiling hostname v0.3.1
   Compiling num_cpus v1.13.1
   Compiling wasmi-validation v0.3.0
   Compiling lmdb-sys v0.8.0
   Compiling rand_core v0.6.3
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling rand v0.8.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ff v0.8.0
   Compiling ed25519 v1.2.0
   Compiling group v0.8.0
   Compiling num-complex v0.4.2
   Compiling chrono v0.4.21
   Compiling proptest v1.0.0
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.2
   Compiling datasize_derive v0.2.10
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.23
   Compiling thiserror-impl v1.0.32
   Compiling tracing-attributes v0.1.22
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling thiserror v1.0.32
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling tracing v0.1.36
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.7
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling pwasm-utils v0.16.0
   Compiling uint v0.9.3
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casper-execution-engine v2.0.0
   Compiling contract-utils v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/utils/contract-utils)
   Compiling casper-engine-test-support v2.2.0
   Compiling test-env v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/utils/test-env)
   Compiling wcspr-tests v0.2.1 (/workspace/CasperLabs-UniswapV2-Core/wcspr/wcspr-tests)
warning: unused variable: `owner`
  --> wcspr-tests/src/wcspr_tests.rs:55:32
   |
55 |     let (env, token, proxy, _, owner) = deploy();
   |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`
   |
   = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `owner`
  --> wcspr-tests/src/wcspr_tests.rs:81:32
   |
81 |     let (env, token, proxy, _, owner) = deploy();
   |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `amount`
  --> wcspr-tests/src/wcspr_tests.rs:83:9
   |
83 |     let amount: U512 = 500.into();
   |         ^^^^^^ help: if this is intentional, prefix it with an underscore: `_amount`

warning: unused variable: `wcspr_package_hash_key`
  --> wcspr-tests/src/wcspr_tests.rs:85:9
   |
85 |     let wcspr_package_hash_key = Key::from(wcspr_package_hash);
   |         ^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_wcspr_package_hash_key`

warning: unused variable: `proxy`
   --> wcspr-tests/src/wcspr_tests.rs:113:22
    |
113 |     let (env, token, proxy, _, owner) = deploy();
    |                      ^^^^^ help: if this is intentional, prefix it with an underscore: `_proxy`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:113:32
    |
113 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:130:32
    |
130 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `proxy`
   --> wcspr-tests/src/wcspr_tests.rs:172:22
    |
172 |     let (env, token, proxy, _, owner) = deploy();
    |                      ^^^^^ help: if this is intentional, prefix it with an underscore: `_proxy`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:172:32
    |
172 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:190:32
    |
190 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:224:32
    |
224 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:258:32
    |
258 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `env`
   --> wcspr-tests/src/wcspr_tests.rs:403:10
    |
403 |     let (env, token, proxy, proxy2, owner) = deploy();
    |          ^^^ help: if this is intentional, prefix it with an underscore: `_env`

warning: unused variable: `token`
   --> wcspr-tests/src/wcspr_tests.rs:403:15
    |
403 |     let (env, token, proxy, proxy2, owner) = deploy();
    |               ^^^^^ help: if this is intentional, prefix it with an underscore: `_token`

warning: unused variable: `env`
   --> wcspr-tests/src/wcspr_tests.rs:419:10
    |
419 |     let (env, token, proxy, proxy2, owner) = deploy();
    |          ^^^ help: if this is intentional, prefix it with an underscore: `_env`

warning: unused variable: `token`
   --> wcspr-tests/src/wcspr_tests.rs:419:15
    |
419 |     let (env, token, proxy, proxy2, owner) = deploy();
    |               ^^^^^ help: if this is intentional, prefix it with an underscore: `_token`

warning: `wcspr-tests` (lib test) generated 16 warnings
    Finished test [unoptimized + debuginfo] target(s) in 1m 15s
     Running unittests (target/debug/deps/wcspr_tests-82dc7f50f2424493)

running 14 tests
test wcspr_tests::test_wcspr_deploy ... ok
test wcspr_tests::test_wcspr_deposit_invalid_access_rights_purse - should panic ... ok
test wcspr_tests::test_wcspr_transfer_from_too_much - should panic ... ok
test wcspr_tests::test_wcspr_deposit_more_than_u256_limit - should panic ... ok
test wcspr_tests::test_wcspr_deposit_too_much - should panic ... ok
test wcspr_tests::test_wcspr_approve ... ok
test wcspr_tests::test_wcspr_withdraw_no_deposit - should panic ... ok
test wcspr_tests::test_wcspr_transfer_too_much - should panic ... ok
test wcspr_tests::test_wcspr_deposit ... ok
test wcspr_tests::test_wcspr_withdraw ... ok
test wcspr_tests::test_wcspr_withdraw_too_much - should panic ... ok
test wcspr_tests::test_wcspr_withdraw_more_than_u256_limit - should panic ... ok
test wcspr_tests::test_wcspr_decrease_allowance ... ok
test wcspr_tests::test_wcspr_increase_allowance ... ok

test result: ok. 14 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.81s

   Doc-tests wcspr-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```

