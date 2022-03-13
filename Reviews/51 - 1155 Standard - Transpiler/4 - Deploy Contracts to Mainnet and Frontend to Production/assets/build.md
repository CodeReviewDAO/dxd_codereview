```
$ make build-contract
cargo build --release -p contract --target wasm32-unknown-unknown
   Compiling cfg-if v1.0.0
   Compiling autocfg v1.0.1
   Compiling serde_derive v1.0.126
   Compiling subtle v2.4.0
   Compiling serde v1.0.126
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling tinyvec_macros v0.1.0
   Compiling ryu v1.0.5
   Compiling bitflags v1.2.1
   Compiling matches v0.1.8
   Compiling opaque-debug v0.3.0
   Compiling unicode-xid v0.2.2
   Compiling ppv-lite86 v0.2.10
   Compiling byteorder v1.4.3
   Compiling memchr v2.4.0
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.64
   Compiling itoa v0.4.7
   Compiling percent-encoding v2.1.0
   Compiling pulldown-cmark v0.8.0
   Compiling hashbrown v0.9.1
   Compiling schemars v0.8.3
   Compiling dyn-clone v1.0.4
   Compiling regex-syntax v0.6.25
   Compiling static_assertions v1.1.0
   Compiling rand_core v0.6.3
   Compiling hex v0.4.3
   Compiling wee_alloc v0.4.5
   Compiling memory_units v0.4.0
   Compiling semver-parser v0.9.0
   Compiling base64 v0.13.0
   Compiling base16 v0.2.1
   Compiling cfg-if v0.1.10
   Compiling once_cell v1.8.0
   Compiling hex_fmt v0.3.0
   Compiling proc-macro2 v1.0.27
   Compiling syn v1.0.73
   Compiling generic-array v0.14.4
   Compiling typenum v1.13.0
   Compiling getrandom v0.1.16
   Compiling unicase v2.6.0
   Compiling tinyvec v1.2.0
   Compiling bitvec v0.18.5
   Compiling unicode-bidi v0.3.5
   Compiling num-traits v0.2.14
   Compiling indexmap v1.6.2
   Compiling num-integer v0.1.44
   Compiling num-rational v0.4.0
   Compiling form_urlencoded v1.0.1
   Compiling rand v0.8.4
   Compiling unicode-normalization v0.1.19
   Compiling regex v1.5.4
   Compiling rand_core v0.5.1
   Compiling quote v1.0.9
   Compiling uint v0.9.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling idna v0.2.3
   Compiling group v0.8.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling rand v0.7.3
   Compiling url v2.2.2
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.5
   Compiling blake2 v0.9.1
   Compiling synstructure v0.12.4
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.1.0
   Compiling datasize_derive v0.2.9
   Compiling schemars_derive v0.8.3
   Compiling thiserror-impl v1.0.25
   Compiling displaydoc v0.1.7
   Compiling num-derive v0.3.3
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.9
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.1.0
   Compiling ecdsa v0.10.2
   Compiling thiserror v1.0.25
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.5
   Compiling ed25519 v1.1.1
   Compiling toml v0.5.8
   Compiling ed25519-dalek v1.0.1
   Compiling version-sync v0.9.2
   Compiling casper-types v1.2.0
   Compiling casper-contract v1.2.0
   Compiling contract v0.1.0 (/workspace/CSPR-1155-DEVXDAO-GRANT-RUST-BASE/contract)
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

    Finished release [optimized] target(s) in 48.52s
```
