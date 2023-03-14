# Output of the "make all" command

```sh

gitpod /workspace/CasperLabs-LiquidNFT (main) $ make all
make build-contract-liquid-factory && make build-contract-liquid-locker
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cargo build --release -p liquid-factory -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
   Compiling proc-macro2 v1.0.49
   Compiling unicode-ident v1.0.6
   Compiling quote v1.0.23
   Compiling syn v1.0.107
   Compiling typenum v1.16.0
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling getrandom v0.1.16
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling serde_derive v1.0.151
   Compiling serde v1.0.151
   Compiling unicode-xid v0.2.4
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling opaque-debug v0.3.0
   Compiling ppv-lite86 v0.2.17
   Compiling block-padding v0.2.1
   Compiling serde_json v1.0.91
   Compiling ryu v1.0.12
   Compiling rand_core v0.6.4
   Compiling wee_alloc v0.4.5
   Compiling static_assertions v1.1.0
   Compiling itoa v1.0.5
   Compiling hex v0.4.3
   Compiling base16 v0.2.1
   Compiling bitflags v1.3.2
   Compiling cfg-if v0.1.10
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling memory_units v0.4.0
   Compiling fnv v1.0.7
   Compiling ident_case v1.0.1
   Compiling strsim v0.9.3
   Compiling subtle v1.0.0
   Compiling byte-tools v0.3.1
   Compiling opaque-debug v0.2.3
   Compiling derive_builder v0.9.0
   Compiling ahash v0.4.7
   Compiling thiserror v1.0.38
   Compiling tiny-keccak v2.0.2
   Compiling fake-simd v0.1.2
   Compiling cryptoxide v0.3.6
   Compiling arrayref v0.3.6
   Compiling keccak v0.1.3
   Compiling rustc-hex v2.1.0
   Compiling rand v0.8.5
   Compiling generic-array v0.14.6
   Compiling bitvec v0.18.5
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling block-padding v0.1.5
   Compiling hashbrown v0.9.1
   Compiling uint v0.9.5
   Compiling rand_core v0.5.1
   Compiling rand_chacha v0.2.2
   Compiling rand v0.7.3
   Compiling generic-array v0.12.4
   Compiling digest v0.8.1
   Compiling crypto-mac v0.7.0
   Compiling block-buffer v0.7.3
   Compiling hmac v0.7.1
   Compiling sha2 v0.8.2
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling hmac-drbg v0.2.0
   Compiling num-complex v0.4.2
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling sha3 v0.9.1
   Compiling libsecp256k1 v0.3.5
   Compiling ed25519 v1.2.0
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
   Compiling darling_core v0.10.2
   Compiling borsh-derive-internal v0.8.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.3
   Compiling num-derive v0.3.3
   Compiling casper_types_derive v0.1.0
   Compiling thiserror-impl v1.0.38
   Compiling darling_macro v0.10.2
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling darling v0.10.2
   Compiling k256 v0.7.3
   Compiling derive_builder_core v0.9.0
   Compiling serde_bytes v0.11.8
   Compiling toml v0.5.10
   Compiling casper-types v1.5.0
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.1.4
   Compiling common v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/common)
   Compiling liquid-base-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/crates/liquid-base-crate)
   Compiling liquid-transfer-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/crates/liquid-transfer-crate)
   Compiling casperlabs-erc20 v0.3.0
   Compiling casperlabs-cep47 v0.2.1
   Compiling liquid-helper-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/crates/liquid-helper-crate)
   Compiling liquid-locker-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker-crate)
   Compiling liquid-factory-crate v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-factory/liquid-factory-crate)
   Compiling erc20 v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/mock-erc20)
   Compiling liquid-factory v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-factory/liquid-factory)
   Compiling cep47 v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/mock-cep47)
    Finished release [optimized] target(s) in 53.85s
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
make[1]: Entering directory '/workspace/CasperLabs-LiquidNFT'
cargo build --release -p liquid-locker -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
   Compiling liquid-locker v0.2.0 (/workspace/CasperLabs-LiquidNFT/Contracts/liquid-locker/liquid-locker)
    Finished release [optimized] target(s) in 3.90s
make[1]: Leaving directory '/workspace/CasperLabs-LiquidNFT'
```
