```sh
$ make test
cargo build --release -p casper-contract-eip-1337 --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/casper-contract-eip-1337/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/subscription_hash_signer/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
warning: unused variable: `x`
   --> casper-contract-eip-1337/src/lib.rs:255:70
    |
255 | ...   let sig = Signature::ed25519(sig_bytes).unwrap_or_else(| x| runtime::revert(ApiError::User(ContractError::InvalidSignature as u16)));
    |                                                                ^ help: if this is intentional, prefix it with an underscore: `_x`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `x`
   --> casper-contract-eip-1337/src/lib.rs:307:70
    |
307 | ...   let sig = Signature::ed25519(sig_bytes).unwrap_or_else(| x| runtime::revert(ApiError::User(ContractError::InvalidSignature as u16)));
    |                                                                ^ help: if this is intentional, prefix it with an underscore: `_x`

warning: unused variable: `x`
   --> casper-contract-eip-1337/src/lib.rs:385:70
    |
385 | ...   let sig = Signature::ed25519(sig_bytes).unwrap_or_else(| x| runtime::revert(ApiError::User(ContractError::InvalidSignature as u16)));
    |                                                                ^ help: if this is intentional, prefix it with an underscore: `_x`

warning: unused variable: `transfer_from_result`
   --> casper-contract-eip-1337/src/lib.rs:408:25
    |
408 |                     let transfer_from_result: () = runtime::call_contract(
    |                         ^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_transfer_from_result`

warning: associated function is never used: `delete`
  --> casper-contract-eip-1337/src/hashes.rs:41:12
   |
41 |     pub fn delete(&self, account: AccountHash) {
   |            ^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: 5 warnings emitted

warning: constant is never used: `FROM`
 --> casper-contract-eip-1337/src/constants.rs:4:1
  |
4 | pub const FROM: &str= "from";
  | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(dead_code)]` on by default

warning: constant is never used: `GRACE_PERIOD_SECONDS`
  --> casper-contract-eip-1337/src/constants.rs:10:1
   |
10 | pub const GRACE_PERIOD_SECONDS: &str= "grace_period_seconds"; 
   | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `SUBSCRIPTION_HASH`
  --> casper-contract-eip-1337/src/constants.rs:12:1
   |
12 | pub const SUBSCRIPTION_HASH : &str="subscription_hash";
   | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `PUBLIC`
  --> casper-contract-eip-1337/src/constants.rs:14:1
   |
14 | pub const PUBLIC: &str= "public";
   | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `SIGNATURE`
  --> casper-contract-eip-1337/src/constants.rs:16:1
   |
16 | pub const SIGNATURE: &str= "signature";
   | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `NEXT_VALID_TIMESTAMP`
  --> casper-contract-eip-1337/src/constants.rs:20:1
   |
20 | pub const NEXT_VALID_TIMESTAMP: &str= "next_valid_timestamp"; 
   | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: 6 warnings emitted

    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/*.wasm
mkdir -p tests/wasm
cp target/wasm32-unknown-unknown/release/*.wasm tests/wasm
cp tests/erc-20-wasm/erc-20-e973bb5.wasm tests/wasm/erc-20.wasm
cargo test -p tests
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/casper-contract-eip-1337/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/subscription_hash_signer/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
  Downloaded bincode v1.3.3
  Downloaded hostname v0.3.1
  Downloaded chrono v0.4.19
  Downloaded num-complex v0.4.0
  Downloaded tracing-core v0.1.22
  Downloaded uuid v0.8.2
  Downloaded memory_units v0.3.0
  Downloaded either v1.6.1
  Downloaded num-bigint v0.2.6
  Downloaded tracing v0.1.31
  Downloaded value-bag v1.0.0-alpha.8
  Downloaded hex-buffer-serde v0.2.2
  Downloaded wasmi-validation v0.3.0
  Downloaded parity-wasm v0.41.0
  Downloaded lmdb-sys v0.8.0
  Downloaded wasmi v0.8.0
  Downloaded lmdb v0.8.0
  Downloaded casper-execution-engine v1.3.2
  Downloaded pwasm-utils v0.16.0
  Downloaded casper-engine-test-support v1.3.2
  Downloaded tracing-attributes v0.1.19
  Downloaded num-rational v0.2.4
  Downloaded num-iter v0.1.42
  Downloaded num v0.4.0
  Downloaded linked-hash-map v0.5.4
  Downloaded downcast-rs v1.2.0
  Downloaded match_cfg v0.1.0
  Downloaded ctor v0.1.21
  Downloaded anyhow v1.0.53
  Downloaded time v0.1.43
  Downloaded pin-project-lite v0.2.8
  Downloaded itertools v0.10.3
  Downloaded 32 crates (1.5 MB) in 0.34s
   Compiling log v0.4.14
   Compiling parity-wasm v0.41.0
   Compiling base64 v0.13.0
   Compiling anyhow v1.0.53
   Compiling either v1.6.1
   Compiling memory_units v0.3.0
   Compiling pin-project-lite v0.2.8
   Compiling match_cfg v0.1.0
   Compiling downcast-rs v1.2.0
   Compiling linked-hash-map v0.5.4
   Compiling generic-array v0.14.5
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.0
   Compiling indexmap v1.8.0
   Compiling unicase v2.6.0
   Compiling num-bigint v0.2.6
   Compiling value-bag v1.0.0-alpha.8
   Compiling num-iter v0.1.42
   Compiling num-rational v0.2.4
   Compiling serde_derive v1.0.136
   Compiling serde v1.0.136
   Compiling typenum v1.15.0
   Compiling getrandom v0.1.16
   Compiling bitvec v0.18.5
   Compiling tracing-core v0.1.22
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.79
   Compiling tinyvec v1.5.1
   Compiling regex v1.5.4
   Compiling memchr v2.4.1
   Compiling bit-set v0.5.2
   Compiling schemars v0.8.8
   Compiling pulldown-cmark v0.8.0
   Compiling lmdb-sys v0.8.0
   Compiling form_urlencoded v1.0.1
   Compiling semver v1.0.5
   Compiling wee_alloc v0.4.5
   Compiling itertools v0.10.3
   Compiling proc-macro2 v1.0.36
   Compiling libc v0.2.118
   Compiling wasmi-validation v0.3.0
   Compiling unicode-normalization v0.1.19
   Compiling quote v1.0.15
   Compiling getrandom v0.2.4
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.43
   Compiling hostname v0.3.1
   Compiling idna v0.2.3
   Compiling syn v1.0.86
   Compiling rand_core v0.5.1
   Compiling rand_core v0.6.3
   Compiling rusty-fork v0.3.0
   Compiling num-complex v0.4.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling url v2.2.2
   Compiling chrono v0.4.19
   Compiling lmdb v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling group v0.8.0
   Compiling rand v0.7.3
   Compiling rand v0.8.5
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling wasmi v0.8.0
   Compiling proptest v1.0.0
   Compiling zeroize_derive v1.3.1
   Compiling thiserror-impl v1.0.30
   Compiling schemars_derive v0.8.8
   Compiling datasize_derive v0.2.10
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.21
   Compiling displaydoc v0.1.7
   Compiling tracing-attributes v0.1.19
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling thiserror v1.0.30
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling tracing v0.1.31
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.5
   Compiling ed25519 v1.2.0
   Compiling toml v0.5.8
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.1
   Compiling hex-buffer-serde v0.2.2
   Compiling num v0.4.0
   Compiling ed25519-dalek v1.0.1
   Compiling pwasm-utils v0.16.0
   Compiling version-sync v0.9.4
   Compiling casper-types v1.3.2
   Compiling casper-contract v1.3.2
   Compiling casper-execution-engine v1.3.2
   Compiling casper-erc20 v0.2.1
   Compiling casper-engine-test-support v1.3.2
   Compiling tests v0.1.0 (/workspace/casper-eip-1337/tests)
warning: unused variable: `res`
  --> tests/src/integration_tests.rs:83:13
   |
83 |         let res = hasher.finalize_variable(|res| {
   |             ^^^ help: if this is intentional, prefix it with an underscore: `_res`
   |
   = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `eip_1337_contract_hash`
   --> tests/src/integration_tests.rs:557:13
    |
557 |         let eip_1337_contract_hash = s.eip_1337_contract_hash.clone();
    |             ^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_eip_1337_contract_hash`

warning: unused variable: `eip_1337_admin_pk`
   --> tests/src/integration_tests.rs:691:13
    |
691 |         let eip_1337_admin_pk = s.eip_1337_admin_pk.clone();
    |             ^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_eip_1337_admin_pk`

warning: unused variable: `sub_hex`
   --> tests/src/integration_tests.rs:717:13
    |
717 |         let sub_hex = get_hex(sub_bytes);
    |             ^^^^^^^ help: if this is intentional, prefix it with an underscore: `_sub_hex`

warning: unused variable: `user_to`
   --> tests/src/integration_tests.rs:915:13
    |
915 |         let user_to = s.user_to;
    |             ^^^^^^^ help: if this is intentional, prefix it with an underscore: `_user_to`

warning: constant is never used: `MINT_ENTRY_POINT_NAME`
  --> tests/src/integration_tests.rs:40:5
   |
40 |     const MINT_ENTRY_POINT_NAME: &str = "mint";
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: constant is never used: `ALLOWANCES_KEY_NAME`
  --> tests/src/integration_tests.rs:45:5
   |
45 |     pub const ALLOWANCES_KEY_NAME: &str = "allowances";
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `CONTRACT_NAME`
  --> tests/src/integration_tests.rs:48:5
   |
48 |     const CONTRACT_NAME: &str = "casper-contract-eip-1337"; //contract name
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `FROM`
  --> tests/src/integration_tests.rs:53:5
   |
53 |     const FROM: &str = "from_"; //the subscriber
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `GRACE_PERIOD_SECONDS`
  --> tests/src/integration_tests.rs:57:5
   |
57 |     const GRACE_PERIOD_SECONDS: &str = "grace_period_seconds"; //the grace_period in seconds for is_subscription_active
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `PUBLIC`
  --> tests/src/integration_tests.rs:59:5
   |
59 |     const PUBLIC: &str = "public"; //the Publickey
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `SIGNATURE`
  --> tests/src/integration_tests.rs:60:5
   |
60 |     const SIGNATURE: &str = "signature"; //the Signature
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: constant is never used: `NEXT_VALID_TIMESTAMP`
  --> tests/src/integration_tests.rs:61:5
   |
61 |     const NEXT_VALID_TIMESTAMP: &str= "next_valid_timestamp"; 
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: associated function is never used: `query_contract_erc20`
   --> tests/src/integration_tests.rs:245:12
    |
245 |         fn query_contract_erc20<T: CLTyped + FromBytes>(&self, name: &str) -> Option<T> {
    |            ^^^^^^^^^^^^^^^^^^^^

warning: associated function is never used: `from`
   --> tests/src/integration_tests.rs:312:16
    |
312 |         pub fn from(&self) -> AccountHash {
    |                ^^^^

warning: associated function is never used: `next_valid_timestamp`
   --> tests/src/integration_tests.rs:316:16
    |
316 |         pub fn next_valid_timestamp(&self) -> u64 {
    |                ^^^^^^^^^^^^^^^^^^^^

warning: associated function is never used: `is_subscription_ready`
   --> tests/src/integration_tests.rs:376:16
    |
376 |         pub fn is_subscription_ready(
    |                ^^^^^^^^^^^^^^^^^^^^^

warning: associated function is never used: `is_subscription_active`
   --> tests/src/integration_tests.rs:392:16
    |
392 |         pub fn is_subscription_active(
    |                ^^^^^^^^^^^^^^^^^^^^^^

warning: 18 warnings emitted

    Finished test [unoptimized + debuginfo] target(s) in 59.62s
     Running unittests (target/debug/deps/integration_tests-233bed02ef8036eb)

running 8 tests
test tests::test_eip1337_deploy ... ok
test tests::test_execute_subscription_bad_hash - should panic ... ok
test tests::test_execute_subscription_not_ready - should panic ... ok
test tests::test_execute_subscription_no_approval - should panic ... ok
test tests::test_execute_subscription_insufficient_allowance - should panic ... ok
test tests::test_execute_subscription ... ok
test tests::test_execute_subscription_repeatable ... ok
test tests::test_execute_subscription_cancellation - should panic ... ok

test result: ok. 8 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 7.27s
```

