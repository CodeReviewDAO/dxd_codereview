 Downloading crates ...
  Downloaded itoa v1.0.6
  Downloaded wasm-bindgen-shared v0.2.86
  Downloaded block-buffer v0.10.4
  Downloaded cpufeatures v0.2.7
  Downloaded cfg-if v0.1.10
  Downloaded digest v0.10.6
  Downloaded getrandom v0.2.7
  Downloaded js-sys v0.3.63
  Downloaded keccak v0.1.4
  Downloaded block-padding v0.2.1
  Downloaded crypto-common v0.1.6
  Downloaded wasm-bindgen-macro-support v0.2.86
  Downloaded tiny-keccak v2.0.2
  Downloaded quote v1.0.27
  Downloaded memory_units v0.4.0
  Downloaded wasm-bindgen-macro v0.2.86
  Downloaded serde_bytes v0.11.9
  Downloaded num v0.4.0
  Downloaded wee_alloc v0.4.5
  Downloaded unicode-ident v1.0.8
  Downloaded casper-contract v3.0.0
  Downloaded wasm-bindgen-backend v0.2.86
  Downloaded once_cell v1.17.1
  Downloaded proc-macro2 v1.0.58
  Downloaded log v0.4.17
  Downloaded ryu v1.0.13
  Downloaded secp256k1 v0.27.0
  Downloaded num-traits v0.2.15
  Downloaded serde_derive v1.0.163
  Downloaded cc v1.0.79
  Downloaded bumpalo v3.12.2
  Downloaded serde v1.0.163
  Downloaded serde_json v1.0.96
  Downloaded wasm-bindgen v0.2.86
  Downloaded syn v2.0.16
  Downloaded sha3 v0.9.1
  Downloaded libc v0.2.144
  Downloaded sha3 v0.10.8
  Downloaded secp256k1-sys v0.8.1
   Compiling proc-macro2 v1.0.58
   Compiling version_check v0.9.4
   Compiling quote v1.0.27
   Compiling typenum v1.16.0
   Compiling unicode-ident v1.0.8
   Compiling autocfg v1.1.0
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling block-padding v0.2.1
   Compiling log v0.4.17
   Compiling opaque-debug v0.3.0
   Compiling wasm-bindgen-shared v0.2.86
   Compiling crunchy v0.2.2
   Compiling serde v1.0.163
   Compiling bumpalo v3.12.2
   Compiling keccak v0.1.4
   Compiling byteorder v1.4.3
   Compiling ppv-lite86 v0.2.17
   Compiling syn v1.0.109
   Compiling once_cell v1.17.1
   Compiling cc v1.0.79
   Compiling generic-array v0.14.7
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling bitvec v0.18.5
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling rand_chacha v0.2.2
   Compiling serde_json v1.0.96
   Compiling wee_alloc v0.4.5
   Compiling wasm-bindgen v0.2.86
   Compiling hex v0.4.3
   Compiling ryu v1.0.13
   Compiling rand v0.7.3
   Compiling itoa v1.0.6
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling uint v0.9.5
   Compiling base64 v0.13.1
   Compiling memory_units v0.4.0
   Compiling rand v0.8.5
   Compiling tiny-keccak v2.0.2
   Compiling bitflags v1.3.2
   Compiling hex_fmt v0.3.0
   Compiling cfg-if v0.1.10
   Compiling base16 v0.2.1
   Compiling syn v2.0.16
   Compiling secp256k1-sys v0.8.1
   Compiling num-complex v0.4.3
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling block-buffer v0.10.4
   Compiling crypto-common v0.1.6
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling sha3 v0.9.1
   Compiling digest v0.10.6
   Compiling ed25519 v1.2.0
   Compiling ff v0.8.0
   Compiling sha3 v0.10.8
   Compiling group v0.8.0
   Compiling num-derive v0.3.3
   Compiling num v0.4.0
   Compiling wasm-bindgen-backend v0.2.86
   Compiling wasm-bindgen-macro-support v0.2.86
   Compiling zeroize_derive v1.4.2
   Compiling serde_derive v1.0.163
   Compiling zeroize v1.3.0
   Compiling wasm-bindgen-macro v0.2.86
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling js-sys v0.3.63
   Compiling secp256k1 v0.27.0
   Compiling getrandom v0.2.7
   Compiling serde_bytes v0.11.9
   Compiling casper-types v3.0.0
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

   Compiling bridge_pool v1.0.0 (/workspace/bridge-casper-smart-contracts/contract)
warning: `contract-utils` (lib) generated 4 warnings (run `cargo fix --lib -p contract-utils` to apply 4 suggestions)
    Finished release [optimized] target(s) in 59.43s
cd counter-call && cargo build --release --target wasm32-unknown-unknown
   Compiling typenum v1.16.0
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.58
   Compiling unicode-ident v1.0.8
   Compiling quote v1.0.27
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling opaque-debug v0.3.0
   Compiling serde v1.0.163
   Compiling ppv-lite86 v0.2.17
   Compiling cfg-if v1.0.0
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling syn v1.0.109
   Compiling serde_json v1.0.96
   Compiling wee_alloc v0.4.5
   Compiling hex v0.4.3
   Compiling static_assertions v1.1.0
   Compiling itoa v1.0.6
   Compiling ryu v1.0.13
   Compiling rand_chacha v0.2.2
   Compiling rand_core v0.6.4
   Compiling base64 v0.13.1
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling generic-array v0.14.7
   Compiling bitvec v0.18.5
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand v0.7.3
   Compiling rand v0.8.5
   Compiling cfg-if v0.1.10
   Compiling uint v0.9.5
   Compiling memory_units v0.4.0
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling bitflags v1.3.2
   Compiling syn v2.0.16
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling blake2 v0.9.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.3
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num-derive v0.3.3
   Compiling num v0.4.0
   Compiling zeroize_derive v1.4.2
   Compiling serde_derive v1.0.163
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.9
   Compiling casper-types v3.0.0
   Compiling casper-contract v3.0.0
   Compiling counter-call v1.0.0 (/workspace/bridge-casper-smart-contracts/counter-call)
    Finished release [optimized] target(s) in 50.95s
cd erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
   Compiling proc-macro2 v1.0.58
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling typenum v1.16.0
   Compiling quote v1.0.27
   Compiling unicode-ident v1.0.8
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling opaque-debug v0.3.0
   Compiling serde v1.0.163
   Compiling cfg-if v1.0.0
   Compiling crunchy v0.2.2
   Compiling byteorder v1.4.3
   Compiling ppv-lite86 v0.2.17
   Compiling syn v1.0.109
   Compiling serde_json v1.0.96
   Compiling hex v0.4.3
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.6
   Compiling ryu v1.0.13
   Compiling rand v0.8.5
   Compiling rand_chacha v0.2.2
   Compiling generic-array v0.14.7
   Compiling base16 v0.2.1
   Compiling base64 v0.13.1
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling bitvec v0.18.5
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand v0.7.3
   Compiling hex_fmt v0.3.0
   Compiling cfg-if v0.1.10
   Compiling uint v0.9.5
   Compiling memory_units v0.4.0
   Compiling bitflags v1.3.2
   Compiling once_cell v1.17.1
   Compiling syn v2.0.16
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.3
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num-derive v0.3.3
   Compiling num v0.4.0
   Compiling zeroize_derive v1.4.2
   Compiling serde_derive v1.0.163
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.9
   Compiling casper-types v3.0.0
   Compiling casper-contract v3.0.0
   Compiling casper-erc20 v0.2.1 (/workspace/bridge-casper-smart-contracts/erc20/erc20)
   Compiling erc20-token v0.1.0 (/workspace/bridge-casper-smart-contracts/erc20/erc20-token)
    Finished release [optimized] target(s) in 34.59s
wasm-strip contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm 2>/dev/null | true
wasm-strip counter-call/target/wasm32-unknown-unknown/release/counter-call.wasm 2>/dev/null | true
