```
$ make build-contract-liquid-helper
cargo build --release -p liquid-helper -p liquid-helper-proxy --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Updating crates.io index
  Downloaded ahash v0.4.7
  Downloaded rustc-hex v2.1.0
  Downloaded hashbrown v0.9.1
  Downloaded tiny-keccak v2.0.2
  Downloaded sha2 v0.8.2
  Downloaded proc-macro-crate v0.1.5
  Downloaded generic-array v0.12.4
  Downloaded getrandom v0.1.16
  Downloaded darling_macro v0.10.2
  Downloaded hmac-drbg v0.2.0
  Downloaded darling v0.10.2
  Downloaded derive_builder_core v0.9.0
  Downloaded derive_builder v0.9.0
  Downloaded fake-simd v0.1.2
  Downloaded opaque-debug v0.2.3
  Downloaded casper_types_derive v0.1.0
  Downloaded borsh-schema-derive-internal v0.8.2
  Downloaded borsh-derive-internal v0.8.2
  Downloaded borsh-derive v0.8.2
  Downloaded arrayref v0.3.6
  Downloaded strsim v0.9.3
  Downloaded keccak v0.1.2
  Downloaded block-padding v0.1.5
  Downloaded block-buffer v0.7.3
  Downloaded borsh v0.8.2
  Downloaded casperlabs-contract-utils v0.1.4
  Downloaded casper-contract v1.4.4
  Downloaded byte-tools v0.3.1
  Downloaded block-padding v0.2.1
  Downloaded wee_alloc v0.4.5
  Downloaded sha3 v0.9.1
  Downloaded ident_case v1.0.1
  Downloaded digest v0.8.1
  Downloaded darling_core v0.10.2
  Downloaded libsecp256k1 v0.3.5
  Downloaded subtle v1.0.0
  Downloaded memory_units v0.4.0
  Downloaded hmac v0.7.1
  Downloaded renvm-sig v0.1.1
  Downloaded crypto-mac v0.7.0
  Downloaded cryptoxide v0.3.6
  Downloaded 41 crates (2.8 MB) in 2.90s (largest was `libsecp256k1` at 1.6 MB)
   Compiling proc-macro2 v1.0.43
   Compiling unicode-ident v1.0.3
   Compiling quote v1.0.21
   Compiling syn v1.0.99
   Compiling typenum v1.15.0
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling getrandom v0.1.16
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling serde_derive v1.0.144
   Compiling serde v1.0.144
   Compiling unicode-xid v0.2.3
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling opaque-debug v0.3.0
   Compiling ppv-lite86 v0.2.16
   Compiling block-padding v0.2.1
   Compiling serde_json v1.0.85
   Compiling ryu v1.0.11
   Compiling rand_core v0.6.3
   Compiling ident_case v1.0.1
   Compiling hex v0.4.3
   Compiling static_assertions v1.1.0
   Compiling strsim v0.9.3
   Compiling wee_alloc v0.4.5
   Compiling fnv v1.0.7
   Compiling itoa v1.0.3
   Compiling memory_units v0.4.0
   Compiling byte-tools v0.3.1
   Compiling base64 v0.13.0
   Compiling base16 v0.2.1
   Compiling subtle v1.0.0
   Compiling cfg-if v0.1.10
   Compiling hex_fmt v0.3.0
   Compiling bitflags v1.3.2
   Compiling ahash v0.4.7
   Compiling fake-simd v0.1.2
   Compiling opaque-debug v0.2.3
   Compiling tiny-keccak v2.0.2
   Compiling derive_builder v0.9.0
   Compiling arrayref v0.3.6
   Compiling keccak v0.1.2
   Compiling rustc-hex v2.1.0
   Compiling cryptoxide v0.3.6
   Compiling generic-array v0.14.6
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand v0.8.5
   Compiling bitvec v0.18.5
   Compiling block-padding v0.1.5
   Compiling hashbrown v0.9.1
   Compiling uint v0.9.3
   Compiling rand_core v0.5.1
   Compiling generic-array v0.12.4
   Compiling rand_chacha v0.2.2
   Compiling digest v0.8.1
   Compiling crypto-mac v0.7.0
   Compiling block-buffer v0.7.3
   Compiling rand v0.7.3
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling hmac v0.7.1
   Compiling sha2 v0.8.2
   Compiling signature v1.2.2
   Compiling sha2 v0.9.9
   Compiling sha3 v0.9.1
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling hmac-drbg v0.2.0
   Compiling num-complex v0.4.2
   Compiling ff v0.8.0
   Compiling ed25519 v1.2.0
   Compiling libsecp256k1 v0.3.5
   Compiling group v0.8.0
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
   Compiling darling_core v0.10.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling borsh-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling thiserror-impl v1.0.34
   Compiling casper_types_derive v0.1.0
   Compiling darling_macro v0.10.2
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling darling v0.10.2
   Compiling derive_builder_core v0.9.0
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling thiserror v1.0.34
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling toml v0.5.9
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1
   Compiling casper-contract v1.4.4
   Compiling common v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/common)
   Compiling casperlabs-contract-utils v0.1.4
   Compiling liquid-base-crate v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-base-crate)
   Compiling liquid-helper-crate v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-helper/liquid-helper-crate)
   Compiling liquid-helper-proxy v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-helper/liquid-helper-proxy)
   Compiling liquid-helper v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-helper/liquid-helper)
    Finished release [optimized] target(s) in 2m 11s


$ make build-contract-liquid-locker
cargo build --release -p liquid-locker -p liquid-locker-proxy -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
  Downloaded casperlabs-erc20 v0.2.3
  Downloaded casperlabs-cep47 v0.2.1
  Downloaded 2 crates (10.0 KB) in 0.82s
   Compiling liquid-locker-proxy v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker-proxy)
   Compiling liquid-transfer-crate v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-transfer-crate)
   Compiling casperlabs-cep47 v0.2.1
   Compiling casperlabs-erc20 v0.2.3
   Compiling liquid-locker-crate v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker-crate)
   Compiling liquid-locker v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker)
   Compiling erc20 v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/mock-erc20)
   Compiling cep47 v0.2.0 (/home/kara/CasperLabs-LiquidNFT/Contracts/mock-cep47)
    Finished release [optimized] target(s) in 18.90s
````
