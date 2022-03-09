```sh
$ make build-contract
cargo build --release -p casper-contract-eip-1337 --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/casper-contract-eip-1337/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/subscription_hash_signer/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
   Compiling proc-macro2 v1.0.36
   Compiling syn v1.0.86
   Compiling unicode-xid v0.2.2
   Compiling version_check v0.9.4
   Compiling typenum v1.15.0
   Compiling cfg-if v1.0.0
   Compiling getrandom v0.1.16
   Compiling autocfg v1.1.0
   Compiling subtle v2.4.1
   Compiling serde_derive v1.0.136
   Compiling serde v1.0.136
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling tinyvec_macros v0.1.0
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling matches v0.1.9
   Compiling serde_json v1.0.79
   Compiling memchr v2.4.1
   Compiling ppv-lite86 v0.2.16
   Compiling unicode-bidi v0.3.7
   Compiling bitflags v1.3.2
   Compiling ryu v1.0.9
   Compiling semver v1.0.5
   Compiling pulldown-cmark v0.8.0
   Compiling schemars v0.8.8
   Compiling percent-encoding v2.1.0
   Compiling hashbrown v0.11.2
   Compiling itoa v1.0.1
   Compiling static_assertions v1.1.0
   Compiling regex-syntax v0.6.25
   Compiling wee_alloc v0.4.5
   Compiling rand_core v0.6.3
   Compiling dyn-clone v1.0.4
   Compiling hex v0.4.3
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.0
   Compiling cfg-if v0.1.10
   Compiling memory_units v0.4.0
   Compiling once_cell v1.9.0
   Compiling base16 v0.2.1
   Compiling generic-array v0.14.5
   Compiling unicase v2.6.0
   Compiling num-traits v0.2.14
   Compiling indexmap v1.8.0
   Compiling num-integer v0.1.44
   Compiling num-rational v0.4.0
   Compiling tinyvec v1.5.1
   Compiling bitvec v0.18.5
   Compiling form_urlencoded v1.0.1
   Compiling rand v0.8.5
   Compiling regex v1.5.4
   Compiling unicode-normalization v0.1.19
   Compiling quote v1.0.15
   Compiling rand_core v0.5.1
   Compiling uint v0.9.1
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling idna v0.2.3
   Compiling group v0.8.0
   Compiling rand v0.7.3
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling url v2.2.2
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.1
   Compiling schemars_derive v0.8.8
   Compiling datasize_derive v0.2.10
   Compiling thiserror-impl v1.0.30
   Compiling displaydoc v0.1.7
   Compiling num-derive v0.3.3
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling thiserror v1.0.30
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.5
   Compiling ed25519 v1.2.0
   Compiling toml v0.5.8
   Compiling ed25519-dalek v1.0.1
   Compiling version-sync v0.9.4
   Compiling casper-types v1.3.2
   Compiling casper-contract v1.3.2
   Compiling casper-erc20 v0.2.1
   Compiling casper-contract-eip-1337 v0.1.0 (/workspace/casper-eip-1337/casper-contract-eip-1337)
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

    Finished release [optimized] target(s) in 43.20s
wasm-strip target/wasm32-unknown-unknown/release/*.wasm
```
