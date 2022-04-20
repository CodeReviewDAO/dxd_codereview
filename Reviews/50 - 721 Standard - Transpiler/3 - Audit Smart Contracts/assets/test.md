```
$ make test
cargo build --release -p contract --target wasm32-unknown-unknown
warning: unused variable: `contract_owner`
   --> contract/src/main.rs:291:9
    |
291 |     let contract_owner: AccountHash = get_key("owner");
    |         ^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_contract_owner`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: variant is never constructed: `Zero`
  --> contract/src/main.rs:29:5
   |
29 |     Zero = 0, // 65,536 as an ApiError::User
   |     ^^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: variant is never constructed: `One`
  --> contract/src/main.rs:30:5
   |
30 |     One,      // 65,537 as an ApiError::User
   |     ^^^

warning: variant is never constructed: `Two`
  --> contract/src/main.rs:31:5
   |
31 |     Two,      // 65,538 as an ApiError::User
   |     ^^^

warning: 4 warnings emitted

    Finished release [optimized] target(s) in 0.08s
cp target/wasm32-unknown-unknown/release/contract.wasm tests/wasm
cargo test -p tests
   Compiling tests v0.2.1 (/workspace/CSPR-721-DEVXDAO-GRANT-RUST-BASE/tests)
   Compiling idna v0.2.3
   Compiling syn v1.0.73
   Compiling lmdb-sys v0.8.0
   Compiling digest v0.9.0
   Compiling num-integer v0.1.44
   Compiling crypto-mac v0.10.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling num-complex v0.4.0
   Compiling pulldown-cmark v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling rand_xorshift v0.3.0
   Compiling lmdb v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.5
   Compiling blake2 v0.9.1
   Compiling num-bigint v0.4.0
   Compiling num-bigint v0.2.6
   Compiling num-iter v0.1.42
   Compiling chrono v0.4.19
   Compiling rand v0.8.4
   Compiling url v2.2.2
   Compiling group v0.8.0
   Compiling rand v0.7.3
   Compiling num-rational v0.2.4
   Compiling tempfile v3.2.0
   Compiling wasmi v0.8.0
   Compiling rusty-fork v0.3.0
   Compiling synstructure v0.12.4
   Compiling serde_derive_internals v0.25.0
   Compiling proptest v1.0.0
   Compiling serde_derive v1.0.126
   Compiling zeroize_derive v1.1.0
   Compiling thiserror-impl v1.0.25
   Compiling ctor v0.1.20
   Compiling datasize_derive v0.2.9
   Compiling schemars_derive v0.8.3
   Compiling displaydoc v0.1.7
   Compiling num-derive v0.3.3
   Compiling tracing-attributes v0.1.15
   Compiling value-bag v1.0.0-alpha.7
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.9
   Compiling thiserror v1.0.25
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.1.0
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling tracing v0.1.26
   Compiling serde v1.0.126
   Compiling num-rational v0.4.0
   Compiling indexmap v1.6.2
   Compiling serde_json v1.0.64
   Compiling ed25519 v1.1.1
   Compiling serde_bytes v0.11.5
   Compiling toml v0.5.8
   Compiling log v0.4.14
   Compiling uuid v0.8.2
   Compiling hex-buffer-serde v0.2.2
   Compiling bincode v1.3.3
   Compiling ed25519-dalek v1.0.1
   Compiling num v0.4.0
   Compiling pwasm-utils v0.16.0
   Compiling schemars v0.8.3
   Compiling version-sync v0.9.2
   Compiling casper-types v1.2.0
   Compiling casper-execution-engine v1.2.0
   Compiling casper-contract v1.2.0
   Compiling casper-engine-test-support v1.2.0
warning: unused import: `U512`
 --> tests/src/tests.rs:2:26
  |
2 | use casper_types::{U256, U512};
  |                          ^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused import: `super::*`
 --> tests/src/erc721.rs:8:9
  |
8 |     use super::*;
  |         ^^^^^^^^

warning: 2 warnings emitted

    Finished test [unoptimized + debuginfo] target(s) in 1m 07s
     Running unittests (target/debug/deps/tests-10431daf6b8fde30)

running 6 tests
test tests::test_erc721_deploy ... ok
test tests::test_erc721_test_uri ... ok
test tests::test_erc721_transfer_too_much ... ok
test tests::test_erc721_transfer ... ok
test tests::test_erc721_approve_transfer ... ok
test tests::test_erc721_approve_all ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.01s

   Doc-tests tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```

