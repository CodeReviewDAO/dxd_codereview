# Output of "make build-contract" command

```sh

cargo build --manifest-path ./contracts/Cargo.toml --release -p vi_nft --target wasm32-unknown-unknown
   Compiling typenum v1.16.0
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling ppv-lite86 v0.2.17
   Compiling proc-macro2 v1.0.50
   Compiling generic-array v0.14.6
   Compiling quote v1.0.23
   Compiling syn v1.0.107
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling serde_derive v1.0.152
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling serde v1.0.152
   Compiling crunchy v0.2.2
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling cfg-if v1.0.0
   Compiling serde_json v1.0.91
   Compiling static_assertions v1.1.0
   Compiling wee_alloc v0.4.5
   Compiling rand_core v0.6.4
   Compiling rand_chacha v0.2.2
   Compiling hex v0.4.3
   Compiling itoa v1.0.5
   Compiling ryu v1.0.12
   Compiling base64 v0.13.1
   Compiling bitvec v0.18.5
   Compiling rand v0.8.5
   Compiling rand v0.7.3
   Compiling hex_fmt v0.3.0
   Compiling memory_units v0.4.0
   Compiling base16 v0.2.1
   Compiling uint v0.9.5
   Compiling bitflags v1.3.2
   Compiling cfg-if v0.1.10
   Compiling once_cell v1.17.0
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
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.3
   Compiling num-derive v0.3.3
   Compiling num v0.4.0
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.8
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling contract-utils v0.1.0 (https://github.com/Ebrahim-hamdy/casper-nft-cep47?branch=master#0b8095d6)
   Compiling cep47 v0.2.0 (https://github.com/Ebrahim-hamdy/casper-nft-cep47?branch=master#0b8095d6)
   Compiling vi_nft v0.2.0 (/workspace/Verified-Impact-NFTs/contracts/vi_nft)
    Finished release [optimized] target(s) in 39.34s
wasm-strip contracts/target/wasm32-unknown-unknown/release/vi_nft.wasm 2>/dev/null | true

```
