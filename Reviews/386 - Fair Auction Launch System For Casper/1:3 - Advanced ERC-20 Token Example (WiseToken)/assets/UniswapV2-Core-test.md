```
UniswapV2-Core (main) $ make test
# Test ERC20
cd ./erc20/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20 --target wasm32-unknown-unknown
warning: unused imports: `BlockTime`, `ContractHash`
 --> erc20/src/erc20.rs:8:49
  |
8 |     system::mint::Error as MintError, ApiError, BlockTime, ContractHash, ContractPackageHash, Key,
  |                                                 ^^^^^^^^^  ^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused import: `hex::encode`
  --> erc20/src/erc20.rs:13:5
   |
13 | use hex::encode;
   |     ^^^^^^^^^^^

warning: unused imports: `hash_message`, `keccak256`
  --> erc20/src/erc20.rs:14:17
   |
14 | use renvm_sig::{hash_message, keccak256};
   |                 ^^^^^^^^^^^^  ^^^^^^^^^

warning: `erc20` (lib) generated 3 warnings
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20-token.wasm 2>/dev/null | true
cargo build --release -p erc20-proxy --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/erc20-proxy-token.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm erc20-tests/wasm
cargo test -p erc20-tests
   Compiling proc-macro2 v1.0.43
   Compiling unicode-ident v1.0.3
   Compiling quote v1.0.21
   Compiling syn v1.0.99
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.129
   Compiling serde_derive v1.0.143
   Compiling typenum v1.15.0
   Compiling serde v1.0.143
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.3
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling ppv-lite86 v0.2.16
   Compiling radium v0.3.0
   Compiling byteorder v1.4.3
   Compiling remove_dir_all v0.5.3
   Compiling fastrand v1.8.0
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.83
   Compiling opaque-debug v0.3.0
   Compiling hashbrown v0.12.3
   Compiling schemars v0.8.5
   Compiling bit-vec v0.6.3
   Compiling fnv v1.0.7
   Compiling once_cell v1.13.0
   Compiling itoa v1.0.3
   Compiling cpufeatures v0.2.2
   Compiling ryu v1.0.11
   Compiling quick-error v1.2.3
   Compiling bitflags v1.3.2
   Compiling lazy_static v1.4.0
   Compiling dyn-clone v1.0.9
   Compiling quick-error v2.0.1
   Compiling regex-syntax v0.6.27
   Compiling static_assertions v1.1.0
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.0
   Compiling pkg-config v0.3.25
   Compiling cc v1.0.73
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling either v1.7.0
   Compiling anyhow v1.0.61
   Compiling wee_alloc v0.4.5
   Compiling memory_units v0.4.0
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling cfg-if v0.1.10
   Compiling pin-project-lite v0.2.9
   Compiling iana-time-zone v0.1.42
   Compiling downcast-rs v1.2.0
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling tracing-core v0.1.29
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling indexmap v1.9.1
   Compiling num-iter v0.1.43
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.3
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
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling rand v0.8.5
   Compiling ff v0.8.0
   Compiling blake2 v0.9.2
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
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling thiserror v1.0.32
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
   Compiling casper-execution-engine v2.0.0
   Compiling contract-utils v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/utils/contract-utils)
   Compiling casper-engine-test-support v2.2.0
   Compiling test-env v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/utils/test-env)
   Compiling erc20-tests v0.1.0 (/workspace/CasperLabs-UniswapV2-Core/erc20/erc20-tests)
    Finished test [unoptimized + debuginfo] target(s) in 1m 12s
     Running unittests (target/debug/deps/erc20_tests-210c2cacc1639236)

running 10 tests
test erc20_tests::test_erc20_mint ... ok
test erc20_tests::test_deploy ... ok
test erc20_tests::test_erc20_approve ... ok
test erc20_tests::test_erc20_burn ... ok
test erc20_tests::test_erc20_transfer_with_same_sender_and_recipient ... ok
test erc20_tests::test_erc20_transfer_from_too_much - should panic ... ok
test erc20_tests::test_erc20_increase_allowance ... ok
test erc20_tests::test_erc20_transfer ... ok
test erc20_tests::test_erc20_transfer_from ... ok
test erc20_tests::test_erc20_decrease_allowance ... ok

test result: ok. 10 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 6.02s

   Doc-tests erc20-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
# Test WCSPR
cd ./wcspr/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
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
    Finished release [optimized] target(s) in 0.04s
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
    Finished release [optimized] target(s) in 0.04s
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
    Finished release [optimized] target(s) in 0.04s
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
warning: unused import: `system`
  --> invalid-purse-proxy/src/main.rs:12:38
   |
12 |     contract_api::{account, runtime, system},
   |                                      ^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `invalid-purse-proxy` (bin "invalid-purse-proxy") generated 1 warning
    Finished release [optimized] target(s) in 0.04s
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
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests (target/debug/deps/wcspr_tests-82dc7f50f2424493)

running 14 tests
test wcspr_tests::test_wcspr_deploy ... ok
test wcspr_tests::test_wcspr_deposit_more_than_u256_limit - should panic ... ok
test wcspr_tests::test_wcspr_withdraw_no_deposit - should panic ... ok
test wcspr_tests::test_wcspr_approve ... ok
test wcspr_tests::test_wcspr_deposit_invalid_access_rights_purse - should panic ... ok
test wcspr_tests::test_wcspr_transfer_from_too_much - should panic ... ok
test wcspr_tests::test_wcspr_transfer_too_much - should panic ... ok
test wcspr_tests::test_wcspr_deposit ... ok
test wcspr_tests::test_wcspr_deposit_too_much - should panic ... ok
test wcspr_tests::test_wcspr_withdraw_more_than_u256_limit - should panic ... ok
test wcspr_tests::test_wcspr_withdraw_too_much - should panic ... ok
test wcspr_tests::test_wcspr_withdraw ... ok
test wcspr_tests::test_wcspr_decrease_allowance ... ok
test wcspr_tests::test_wcspr_increase_allowance ... ok

test result: ok. 14 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.76s

   Doc-tests wcspr-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
# Test Factory
cd ./factory/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cargo build --release -p factory --target wasm32-unknown-unknown
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/factory.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../flashswapper/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../pair/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../wcspr/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../erc20/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
cargo test -p factory-tests
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
warning: unused import: `std::collections::BTreeMap`
 --> factory-tests/src/factory_tests.rs:1:5
  |
1 | use std::collections::BTreeMap;
  |     ^^^^^^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default
help: consider adding a `#[cfg(test)]` to the containing module
 --> factory-tests/src/lib.rs:2:1
  |
2 | pub mod factory_tests;
  | ^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `ContractPackageHash`
 --> factory-tests/src/factory_tests.rs:4:41
  |
4 |     account::AccountHash, runtime_args, ContractPackageHash, Key, RuntimeArgs, U256,
  |                                         ^^^^^^^^^^^^^^^^^^^
  |
help: consider adding a `#[cfg(test)]` to the containing module
 --> factory-tests/src/lib.rs:2:1
  |
2 | pub mod factory_tests;
  | ^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `std::collections::BTreeMap`
 --> factory-tests/src/factory_instance.rs:1:5
  |
1 | use std::collections::BTreeMap;
  |     ^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: unused imports: `CLTyped`, `ContractPackageHash`, `U256`
 --> factory-tests/src/factory_instance.rs:8:61
  |
8 |     account::AccountHash, bytesrepr::ToBytes, runtime_args, CLTyped, ContractPackageHash, Key,
  |                                                             ^^^^^^^  ^^^^^^^^^^^^^^^^^^^
9 |     RuntimeArgs, U256,
  |                  ^^^^

warning: `factory-tests` (lib test) generated 4 warnings
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests (target/debug/deps/factory_tests-4c5d57042d9748b4)

running 7 tests
test factory_tests::test_calling_construction - should panic ... ok
test factory_tests::test_factory_deploy ... ok
test factory_tests::test_factory_set_white_list_with_non_owner - should panic ... ok
test factory_tests::test_factory_set_fee_to ... ok
test factory_tests::test_factory_set_fee_to_setter ... ok
test factory_tests::test_factory_set_white_list ... ok
test factory_tests::test_factory_create_pair ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.58s

   Doc-tests factory-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
# Test Flashswapper
cd ./flashswapper/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cargo build --release -p flashswapper --target wasm32-unknown-unknown
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/flashswapper-token.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm flashswapper-tests/wasm
cargo test -p flashswapper-tests
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests (target/debug/deps/flashswapper_tests-c4cacba29e659e05)

running 2 tests
test flash_swapper_tests::test_flash_swapper_deploy ... ok
test flash_swapper_tests::test_calling_construction - should panic ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.93s

   Doc-tests flashswapper-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
# Test Pair
cd ./pair/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p pair --target wasm32-unknown-unknown
warning: unused import: `BlockTime`
  --> pair/src/pair.rs:13:29
   |
13 |     runtime_args, ApiError, BlockTime, ContractPackageHash, Key, RuntimeArgs, URef, U128, U256,
   |                             ^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::hash_message`
  --> pair/src/pair.rs:17:5
   |
17 | use renvm_sig::hash_message;
   |     ^^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `renvm_sig::keccak256`
  --> pair/src/pair.rs:18:5
   |
18 | use renvm_sig::keccak256;
   |     ^^^^^^^^^^^^^^^^^^^^

warning: value assigned to `liquidity` is never read
   --> pair/src/pair.rs:932:17
    |
932 |         let mut liquidity: U256 = 0.into();
    |                 ^^^^^^^^^
    |
    = note: `#[warn(unused_assignments)]` on by default
    = help: maybe it is overwritten before being read?

warning: `pair` (lib) generated 4 warnings
warning: unused import: `hex::encode`
  --> pair/bin/pair_token.rs:18:5
   |
18 | use hex::encode;
   |     ^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::keccak256`
  --> pair/bin/pair_token.rs:20:5
   |
20 | use renvm_sig::keccak256;
   |     ^^^^^^^^^^^^^^^^^^^^

warning: `pair` (bin "pair-token") generated 2 warnings
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/pair-token.wasm 2>/dev/null | true
cargo build --release -p test --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/pair-test.wasm 2>/dev/null | true
cargo build --release -p test2 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/pair-test2.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm pair-tests/wasm
cargo test -p pair-tests
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests (target/debug/deps/pair_tests-4668cd4577f5973b)

running 15 tests
test pair_tests::test_pair_transfer_too_much - should panic ... ok
test pair_tests::test_calling_construction - should panic ... ok
test pair_tests::test_pair_deploy ... ok
test pair_tests::test_pair_approve ... ok
test pair_tests::test_pair_set_treasury_fee_percent ... ok
test pair_tests::test_pair_transfer_with_same_sender_and_recipient ... ok
test pair_tests::test_pair_transfer ... ok
test pair_tests::test_pair_transfer_from_too_much - should panic ... ok
test pair_tests::test_pair_transfer_from ... ok
test pair_tests::test_pair_initialize ... ok
test pair_tests::test_pair_sync ... ok
test pair_tests::test_pair_mint ... ok
test pair_tests::test_pair_skim ... ok
test pair_tests::test_pair_swap ... ok
test pair_tests::test_pair_burn ... ok

test result: ok. 15 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 32.20s

   Doc-tests pair-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
```

