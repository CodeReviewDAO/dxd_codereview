cd contract && cargo build --release --target wasm32-unknown-unknown
warning: unused variable: `res`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:69:9
   |
69 |     let res = s.sign_ecdsa_recoverable(&msg, &key);
   |         ^^^ help: if this is intentional, prefix it with an underscore: `_res`
   |
   = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `r`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:71:9
   |
71 |     let r = hex::encode(&sig_bytes[..32]);
   |         ^ help: if this is intentional, prefix it with an underscore: `_r`

warning: unused variable: `s`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:72:9
   |
72 |     let s = hex::encode(&sig_bytes[32..64]);
   |         ^ help: if this is intentional, prefix it with an underscore: `_s`

warning: unused variable: `slice`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:77:9
   |
77 |     let slice = vec.as_slice();
   |         ^^^^^ help: if this is intentional, prefix it with an underscore: `_slice`

warning: `contract-utils` (lib) generated 4 warnings (run `cargo fix --lib -p contract-utils` to apply 4 suggestions)
    Finished release [optimized] target(s) in 0.05s
cd counter-call && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.04s
cd erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.04s
wasm-strip contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm 2>/dev/null | true
wasm-strip counter-call/target/wasm32-unknown-unknown/release/counter-call.wasm 2>/dev/null | true
mkdir -p tests/wasm
cp contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm tests/wasm
cp counter-call/target/wasm32-unknown-unknown/release/counter-call.wasm tests/wasm
cp erc20/target/wasm32-unknown-unknown/release/erc20_token.wasm tests/wasm/erc20.wasm
cd tests && cargo test
 Downloading crates ...
  Downloaded quick-error v1.2.3
  Downloaded bincode v1.3.3
  Downloaded quick-error v2.0.1
  Downloaded pin-project-lite v0.2.9
  Downloaded num-rational v0.2.4
  Downloaded either v1.8.1
  Downloaded strum_macros v0.24.3
  Downloaded bit-set v0.5.3
  Downloaded ctor v0.1.26
  Downloaded syn v0.15.44
  Downloaded thiserror-impl v1.0.40
  Downloaded unarray v0.1.4
  Downloaded thiserror v1.0.40
  Downloaded dyn-clone v1.0.11
  Downloaded num_cpus v1.15.0
  Downloaded downcast-rs v1.2.0
  Downloaded getrandom v0.2.9
  Downloaded toml v0.5.11
  Downloaded strum v0.24.1
  Downloaded filesize v0.2.0
  Downloaded unicode-xid v0.1.0
  Downloaded fastrand v1.9.0
  Downloaded rustversion v1.0.12
  Downloaded linked-hash-map v0.5.6
  Downloaded quote v0.6.13
  Downloaded io-lifetimes v1.0.10
  Downloaded wasmi-validation v0.4.1
  Downloaded rusty-fork v0.3.0
  Downloaded parity-wasm v0.42.2
  Downloaded rustix v0.37.19
  Downloaded match_cfg v0.1.0
  Downloaded wait-timeout v0.2.0
  Downloaded tracing-attributes v0.1.24
  Downloaded proc-macro2 v0.4.30
  Downloaded regex-syntax v0.7.1
  Downloaded libm v0.2.7
  Downloaded lazy_static v1.4.0
  Downloaded rand_pcg v0.3.1
  Downloaded uuid v0.8.2
  Downloaded regex v1.8.1
  Downloaded value-bag v1.0.0-alpha.9
  Downloaded rand_xorshift v0.3.0
  Downloaded num-bigint v0.2.6
  Downloaded anyhow v1.0.71
  Downloaded lmdb-rkv v0.14.0
  Downloaded tempfile v3.5.0
  Downloaded proptest-derive v0.3.0
  Downloaded proptest v1.1.0
  Downloaded hostname v0.3.1
  Downloaded regex-syntax v0.6.29
  Downloaded lmdb-rkv-sys v0.11.2
  Downloaded linux-raw-sys v0.3.7
  Downloaded bit-vec v0.6.3
  Downloaded casper-engine-test-support v5.0.0
  Downloaded memory_units v0.3.0
  Downloaded hex-buffer-serde v0.2.2
  Downloaded casper-wasm-utils v1.0.0
  Downloaded wasmi v0.9.1
  Downloaded casper-execution-engine v5.0.0
   Compiling proc-macro2 v1.0.58
   Compiling unicode-ident v1.0.8
   Compiling quote v1.0.27
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.144
   Compiling typenum v1.16.0
   Compiling serde v1.0.163
   Compiling cfg-if v1.0.0
   Compiling syn v1.0.109
   Compiling libm v0.2.7
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling ppv-lite86 v0.2.17
   Compiling funty v1.1.0
   Compiling io-lifetimes v1.0.10
   Compiling wyz v0.2.0
   Compiling byteorder v1.4.3
   Compiling radium v0.3.0
   Compiling cc v1.0.79
   Compiling block-padding v0.2.1
   Compiling rustix v0.37.19
   Compiling bitflags v1.3.2
   Compiling proc-macro2 v0.4.30
   Compiling opaque-debug v0.3.0
   Compiling rustversion v1.0.12
   Compiling bitvec v0.18.5
   Compiling linux-raw-sys v0.3.7
   Compiling generic-array v0.14.7
   Compiling crunchy v0.2.2
   Compiling unicode-xid v0.1.0
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling indexmap v1.9.3
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling once_cell v1.17.1
   Compiling syn v2.0.16
   Compiling fastrand v1.9.0
   Compiling serde_json v1.0.96
   Compiling cpufeatures v0.2.7
   Compiling hashbrown v0.12.3
   Compiling syn v0.15.44
   Compiling quote v0.6.13
   Compiling rand_chacha v0.2.2
   Compiling heck v0.4.1
   Compiling ryu v1.0.13
   Compiling itoa v1.0.6
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling getrandom v0.2.9
   Compiling signature v1.2.2
   Compiling wait-timeout v0.2.0
   Compiling sha2 v0.9.9
   Compiling hmac v0.10.1
   Compiling thiserror v1.0.40
   Compiling regex-syntax v0.7.1
   Compiling keccak v0.1.4
   Compiling quick-error v1.2.3
   Compiling bit-vec v0.6.3
   Compiling rand_core v0.6.4
   Compiling ff v0.8.0
   Compiling schemars v0.8.5
   Compiling group v0.8.0
   Compiling fnv v1.0.7
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling bit-set v0.5.3
   Compiling num-complex v0.4.3
   Compiling sha3 v0.9.1
   Compiling ed25519 v1.2.0
   Compiling rand v0.7.3
   Compiling crypto-mac v0.8.0
   Compiling unarray v0.1.4
   Compiling rand v0.8.5
   Compiling regex-syntax v0.6.29
   Compiling untrusted v0.7.1
   Compiling quick-error v2.0.1
   Compiling base64 v0.13.1
   Compiling static_assertions v1.1.0
   Compiling dyn-clone v1.0.11
   Compiling lazy_static v1.4.0
   Compiling derp v0.0.14
   Compiling blake2 v0.9.2
   Compiling rand_pcg v0.3.1
   Compiling num-bigint v0.2.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling pkg-config v0.3.27
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling humantime v2.1.0
   Compiling num-rational v0.2.4
   Compiling parity-wasm v0.42.2
   Compiling log v0.4.17
   Compiling regex v1.8.1
   Compiling anyhow v1.0.71
   Compiling wee_alloc v0.4.5
   Compiling either v1.8.1
   Compiling secp256k1-sys v0.8.1
   Compiling itertools v0.10.5
   Compiling tracing-core v0.1.31
   Compiling tempfile v3.5.0
   Compiling lmdb-rkv-sys v0.11.2
   Compiling cfg-if v0.1.10
   Compiling pem v0.8.3
   Compiling rusty-fork v0.3.0
   Compiling serde_derive_internals v0.25.0
   Compiling proptest v1.1.0
   Compiling wasmi-validation v0.4.1
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.4.0
   Compiling memory_units v0.3.0
   Compiling downcast-rs v1.2.0
   Compiling pin-project-lite v0.2.9
   Compiling hostname v0.3.1
   Compiling wasmi v0.9.1
   Compiling num_cpus v1.15.0
   Compiling tiny-keccak v2.0.2
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling lmdb-rkv v0.14.0
   Compiling datasize_derive v0.2.14
   Compiling schemars_derive v0.8.5
   Compiling strum_macros v0.24.3
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling serde_derive v1.0.163
   Compiling zeroize_derive v1.4.2
   Compiling thiserror-impl v1.0.40
   Compiling tracing-attributes v0.1.24
   Compiling proptest-derive v0.3.0
   Compiling datasize v0.2.14
   Compiling secp256k1 v0.27.0
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling strum v0.24.1
   Compiling tracing v0.1.37
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.9
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling toml v0.5.11
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling casper-wasm-utils v1.0.0
   Compiling num v0.4.0
   Compiling casper-types v3.0.0
   Compiling casper-hashing v2.0.0
   Compiling casper-contract v3.0.0
   Compiling contract-utils v0.1.0 (/workspace/bridge-casper-smart-contracts/utils/contract-utils)
warning: unused variable: `res`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:69:9
   |
69 |     let res = s.sign_ecdsa_recoverable(&msg, &key);
   |         ^^^ help: if this is intentional, prefix it with an underscore: `_res`
   |
   = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `r`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:71:9
   |
71 |     let r = hex::encode(&sig_bytes[..32]);
   |         ^ help: if this is intentional, prefix it with an underscore: `_r`

warning: unused variable: `s`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:72:9
   |
72 |     let s = hex::encode(&sig_bytes[32..64]);
   |         ^ help: if this is intentional, prefix it with an underscore: `_s`

warning: unused variable: `slice`
  --> /workspace/bridge-casper-smart-contracts/utils/contract-utils/src/keccak.rs:77:9
   |
77 |     let slice = vec.as_slice();
   |         ^^^^^ help: if this is intentional, prefix it with an underscore: `_slice`

   Compiling casper-execution-engine v5.0.0
warning: `contract-utils` (lib) generated 4 warnings (run `cargo fix --lib -p contract-utils` to apply 4 suggestions)
   Compiling casper-engine-test-support v5.0.0
   Compiling test-env v0.1.0 (/workspace/bridge-casper-smart-contracts/utils/test-env)
   Compiling tests v1.0.0 (/workspace/bridge-casper-smart-contracts/tests)
warning: unused import: `std::collections::BTreeMap`
  --> src/integration_tests.rs:15:9
   |
15 |     use std::collections::BTreeMap;
   |         ^^^^^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused imports: `CLTyped`, `URef`, `account::AccountHash`
  --> src/integration_tests.rs:23:9
   |
23 |         account::AccountHash,
   |         ^^^^^^^^^^^^^^^^^^^^
24 |         bytesrepr::{FromBytes, ToBytes},
25 |         CLTyped, ContractPackageHash, Key, URef, BLAKE2B_DIGEST_LENGTH, U256,
   |         ^^^^^^^                            ^^^^

warning: unused import: `test_env::TestEnv`
  --> src/integration_tests.rs:27:9
   |
27 |     use test_env::TestEnv;
   |         ^^^^^^^^^^^^^^^^^

warning: use of deprecated static `casper_engine_test_support::DEFAULT_RUN_GENESIS_REQUEST`: prefer `PRODUCTION_RUN_GENESIS_REQUEST` as it uses cost tables matching those used in Casper Mainnet
  --> src/integration_tests.rs:11:9
   |
11 |         DEFAULT_RUN_GENESIS_REQUEST, PRODUCTION_RUN_GENESIS_REQUEST,
   |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(deprecated)]` on by default

warning: use of deprecated static `casper_engine_test_support::DEFAULT_RUN_GENESIS_REQUEST`: prefer `PRODUCTION_RUN_GENESIS_REQUEST` as it uses cost tables matching those used in Casper Mainnet
   --> src/integration_tests.rs:941:30
    |
941 |         builder.run_genesis(&DEFAULT_RUN_GENESIS_REQUEST).commit();
    |                              ^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `FromBytes`
  --> src/integration_tests.rs:24:21
   |
24 |         bytesrepr::{FromBytes, ToBytes},
   |                     ^^^^^^^^^

warning: unused variable: `erc20_contract_package_hash_string`
   --> src/integration_tests.rs:555:13
    |
555 |         let erc20_contract_package_hash_string = erc20_contract_package_hash.to_formatted_string();
    |             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_erc20_contract_package_hash_string`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `bridge_pool_contract_package_hash_string`
   --> src/integration_tests.rs:556:13
    |
556 |         let bridge_pool_contract_package_hash_string =
    |             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_bridge_pool_contract_package_hash_string`

warning: unused variable: `erc20_contract_package_hash_string`
   --> src/integration_tests.rs:665:13
    |
665 |         let erc20_contract_package_hash_string = erc20_contract_package_hash.to_formatted_string();
    |             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_erc20_contract_package_hash_string`

warning: unused variable: `bridge_pool_contract_package_hash_string`
   --> src/integration_tests.rs:666:13
    |
666 |         let bridge_pool_contract_package_hash_string =
    |             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_bridge_pool_contract_package_hash_string`

warning: unused variable: `erc20_contract_package_hash_string`
    --> src/integration_tests.rs:1028:13
     |
1028 |         let erc20_contract_package_hash_string = erc20_contract_package_hash.to_formatted_string();
     |             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_erc20_contract_package_hash_string`

warning: unused variable: `bridge_pool_contract_package_hash_string`
    --> src/integration_tests.rs:1029:13
     |
1029 |         let bridge_pool_contract_package_hash_string =
     |             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_bridge_pool_contract_package_hash_string`

warning: variable does not need to be mutable
    --> src/integration_tests.rs:1372:13
     |
1372 |         let mut signature_vec: Vec<u8> = signature;
     |             ----^^^^^^^^^^^^^
     |             |
     |             help: remove this `mut`
     |
     = note: `#[warn(unused_mut)]` on by default

warning: constant `COUNTER_CALL_WASM` is never used
  --> src/integration_tests.rs:31:11
   |
31 |     const COUNTER_CALL_WASM: &str = "counter-call.wasm"; // The session code that calls the contract
   |           ^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: constant `CONTRACT_KEY` is never used
  --> src/integration_tests.rs:37:11
   |
37 |     const CONTRACT_KEY: &str = "bridge_pool"; // Named key referencing this contract
   |           ^^^^^^^^^^^^

warning: constant `LIQUIDITY_KEY` is never used
  --> src/integration_tests.rs:38:11
   |
38 |     const LIQUIDITY_KEY: &str = "liquidity"; // Named key referencing the count value
   |           ^^^^^^^^^^^^^

warning: constant `CONTRACT_VERSION_KEY` is never used
  --> src/integration_tests.rs:39:11
   |
39 |     const CONTRACT_VERSION_KEY: &str = "version"; // Automatically incremented version in a contract package
   |           ^^^^^^^^^^^^^^^^^^^^

warning: `tests` (bin "integration-tests" test) generated 17 warnings (run `cargo fix --bin "integration-tests" --tests` to apply 10 suggestions)
    Finished test [unoptimized + debuginfo] target(s) in 1m 25s
     Running unittests src/integration_tests.rs (target/debug/deps/integration_tests-28761e1b19258f14)

running 8 tests
test tests::should_be_able_to_install_and_add_signer ... ok
test tests::should_be_able_to_install_and_allow_target ... ok
test tests::should_be_able_to_install_and_add_liquidity ... ok
test tests::should_be_able_to_install_add_and_remove_signer ... ok
test tests::should_be_able_to_install_and_get_liquidity ... ok
test tests::should_be_able_to_install_and_add_liquidity_and_remove_liquidity ... ok
test tests::should_be_able_to_install_and_add_liquidity_and_swap ... ok
test tests::should_be_able_to_install_and_add_liquidity_and_withdraw_signed ... FAILED

failures:

---- tests::should_be_able_to_install_and_add_liquidity_and_withdraw_signed stdout ----
erc20_contract_hash "contract-af425c8c851e4eb341f504454ba886b886e1fac8961f20e7c74b6d6b929614b0"
erc20_contract_package_hash.to_formatted_string() is contract-package-b712ba79119a19b1880814eba5aaaaa01ec295d880a263ee69a9aebf01828b93
bridge_pool_contract_package_hash.to_formatted_string() is contract-package-b1dbb5177b641878f3b5577c38bd0c795076c5d4063161d24f16fc1a383b7e22
bridge_pool_contract_hash.to_formatted_string() is contract-a6d06b4e9a3ee12867dc7fdb6b79e60a36628dc7d70d7b20811847f57f1c3ea7
signature is 5eaca1dd5f48b005862df653d943343b84ff1cfbdc5205ab0aeb0d1cb75064627ffe2f7a3d1e72290e8d3584a0b3624e1dd49df11fa3c2d83e15cbb28f86bd3b00
amount is 1
erc20_contract_package_hash_string is contract-package-b712ba79119a19b1880814eba5aaaaa01ec295d880a263ee69a9aebf01828b93
signer_string is cc29f0f5005edfe3755b3f52f98e01785b47703f
thread 'tests::should_be_able_to_install_and_add_liquidity_and_withdraw_signed' panicked at 'Expected successful execution result, but instead got: Failure {
    error: Exec(
        Interpreter(
            "trap: Trap { kind: Unreachable }",
        ),
    ),
    transfers: [],
    cost: Gas(
        5045067480,
    ),
    execution_journal: ExecutionJournal(
        [
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Hash(8aaf51097e8ef647f598f0c31b2ced495cdafd6e8e8202f539a59344682a8193),
                Identity,
            ),
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Hash(ee6d1cbd6af09faacbc97e71d326dc2ab4a24ec783aebdb07a15d3c848a01302),
                Identity,
            ),
            (
                Key::Hash(a61edb38669f2e5c65447708989f34939145988f5f4b5c8ed3d6399c0a6450ee),
                Identity,
            ),
            (
                Key::Hash(ee6d1cbd6af09faacbc97e71d326dc2ab4a24ec783aebdb07a15d3c848a01302),
                Identity,
            ),
            (
                Key::Balance(d124a145ff53378cfff7970ca163b2acee77570c6c6852fc717de5067c325db6),
                Identity,
            ),
            (
                Key::Balance(eb40a2b1455716c2f4f75e47ee8efb459390b61c6c7db9fdb24fc5c9fd76d147),
                Identity,
            ),
            (
                Key::Balance(d124a145ff53378cfff7970ca163b2acee77570c6c6852fc717de5067c325db6),
                Write(
                    CLValue(
                        CLValue {
                            cl_type: U512,
                            bytes: Bytes(
                                [
                                    8,
                                    0,
                                    64,
                                    205,
                                    101,
                                    142,
                                    58,
                                    99,
                                    1,
                                ],
                            ),
                        },
                    ),
                ),
            ),
            (
                Key::Balance(eb40a2b1455716c2f4f75e47ee8efb459390b61c6c7db9fdb24fc5c9fd76d147),
                AddUInt512(
                    1500000000000,
                ),
            ),
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Hash(8aaf51097e8ef647f598f0c31b2ced495cdafd6e8e8202f539a59344682a8193),
                Identity,
            ),
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Balance(eb40a2b1455716c2f4f75e47ee8efb459390b61c6c7db9fdb24fc5c9fd76d147),
                Identity,
            ),
            (
                Key::Hash(2b0bafe7e494bda805d8805708f197df592080aa091f8c3ea48d5124086d38d1),
                Identity,
            ),
            (
                Key::Hash(ee6d1cbd6af09faacbc97e71d326dc2ab4a24ec783aebdb07a15d3c848a01302),
                Identity,
            ),
            (
                Key::Hash(a61edb38669f2e5c65447708989f34939145988f5f4b5c8ed3d6399c0a6450ee),
                Identity,
            ),
            (
                Key::Hash(ee6d1cbd6af09faacbc97e71d326dc2ab4a24ec783aebdb07a15d3c848a01302),
                Identity,
            ),
            (
                Key::Balance(eb40a2b1455716c2f4f75e47ee8efb459390b61c6c7db9fdb24fc5c9fd76d147),
                Identity,
            ),
            (
                Key::Balance(3742e6011967754e97d28b35be8d915159db7b05370f802e79c9d4507f075e04),
                Identity,
            ),
            (
                Key::Balance(eb40a2b1455716c2f4f75e47ee8efb459390b61c6c7db9fdb24fc5c9fd76d147),
                Write(
                    CLValue(
                        CLValue {
                            cl_type: U512,
                            bytes: Bytes(
                                [
                                    0,
                                ],
                            ),
                        },
                    ),
                ),
            ),
            (
                Key::Balance(3742e6011967754e97d28b35be8d915159db7b05370f802e79c9d4507f075e04),
                AddUInt512(
                    1500000000000,
                ),
            ),
        ],
    ),
}', /workspace/.cargo/registry/src/github.com-1ecc6299db9ec823/casper-engine-test-support-5.0.0/src/wasm_test_builder.rs:842:13
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace


failures:
    tests::should_be_able_to_install_and_add_liquidity_and_withdraw_signed

test result: FAILED. 7 passed; 1 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.69s

error: test failed, to rerun pass `--bin integration-tests`
make: *** [Makefile:20: test] Error 101
