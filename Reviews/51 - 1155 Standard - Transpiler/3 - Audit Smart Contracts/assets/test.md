```
$ make test
cargo build --release -p contract --target wasm32-unknown-unknown
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

warning: 3 warnings emitted

    Finished release [optimized] target(s) in 0.06s
cp target/wasm32-unknown-unknown/release/contract.wasm tests/wasm
cargo test -p tests
   Compiling tests v0.2.1 (/workspace/CSPR-1155-DEVXDAO-GRANT-RUST-BASE/tests)
   Compiling rand_core v0.5.1
   Compiling lmdb-sys v0.8.0
   Compiling rand_core v0.6.3
   Compiling digest v0.9.0
   Compiling num-integer v0.1.44
   Compiling crypto-mac v0.10.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling url v2.2.2
   Compiling num-complex v0.4.0
   Compiling pulldown-cmark v0.8.0
   Compiling serde_derive v1.0.126
   Compiling synstructure v0.12.4
   Compiling serde_derive_internals v0.25.0
   Compiling datasize_derive v0.2.9
   Compiling ctor v0.1.20
   Compiling thiserror-impl v1.0.25
   Compiling num-derive v0.3.3
   Compiling displaydoc v0.1.7
   Compiling tracing-attributes v0.1.15
   Compiling lmdb v0.8.0
   Compiling signature v1.2.2
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.5
   Compiling blake2 v0.9.1
   Compiling num-bigint v0.4.0
   Compiling num-bigint v0.2.6
   Compiling num-iter v0.1.42
   Compiling chrono v0.4.19
   Compiling zeroize_derive v1.1.0
   Compiling datasize v0.2.9
   Compiling schemars_derive v0.8.3
   Compiling value-bag v1.0.0-alpha.7
   Compiling group v0.8.0
   Compiling rand v0.7.3
   Compiling rand v0.8.4
   Compiling thiserror v1.0.25
   Compiling tracing v0.1.26
   Compiling num-rational v0.2.4
   Compiling zeroize v1.3.0
   Compiling wasmi v0.8.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.1.0
   Compiling serde v1.0.126
   Compiling tempfile v3.2.0
   Compiling ecdsa v0.10.2
   Compiling rusty-fork v0.3.0
   Compiling k256 v0.7.3
   Compiling proptest v1.0.0
   Compiling serde_bytes v0.11.5
   Compiling num-rational v0.4.0
   Compiling indexmap v1.6.2
   Compiling serde_json v1.0.64
   Compiling ed25519 v1.1.1
   Compiling toml v0.5.8
   Compiling log v0.4.14
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling hex-buffer-serde v0.2.2
   Compiling ed25519-dalek v1.0.1
   Compiling num v0.4.0
   Compiling pwasm-utils v0.16.0
   Compiling schemars v0.8.3
   Compiling version-sync v0.9.2
   Compiling casper-types v1.2.0
   Compiling casper-contract v1.2.0
   Compiling casper-execution-engine v1.2.0
   Compiling casper-engine-test-support v1.2.0
warning: unused imports: `U256`, `U512`
 --> tests/src/tests.rs:2:20
  |
2 | use casper_types::{U256, U512};
  |                    ^^^^  ^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused import: `super::*`
 --> tests/src/erc1155.rs:8:9
  |
8 |     use super::*;
  |         ^^^^^^^^

warning: variable does not need to be mutable
  --> tests/src/tests.rs:19:9
   |
19 |     let mut ids = vec![id, id1, id2];
   |         ----^^^
   |         |
   |         help: remove this `mut`
   |
   = note: `#[warn(unused_mut)]` on by default

warning: variable does not need to be mutable
  --> tests/src/tests.rs:20:9
   |
20 |     let mut quantities=vec![200.into(),200.into(),200.into()];
   |         ----^^^^^^^^^^
   |         |
   |         help: remove this `mut`

warning: variable does not need to be mutable
  --> tests/src/tests.rs:36:9
   |
36 |     let mut ids = vec![id, id1, id2];
   |         ----^^^
   |         |
   |         help: remove this `mut`

warning: variable does not need to be mutable
  --> tests/src/tests.rs:37:9
   |
37 |     let mut quantities=vec![200.into(),200.into(),200.into()];
   |         ----^^^^^^^^^^
   |         |
   |         help: remove this `mut`

warning: 6 warnings emitted

    Finished test [unoptimized + debuginfo] target(s) in 43.31s
     Running unittests (target/debug/deps/tests-10431daf6b8fde30)

running 3 tests
test tests::test_erc1155_deploy ... ok
test tests::test_erc1155_mint ... ok
test tests::test_batch_transfer ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.58s

   Doc-tests tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```

