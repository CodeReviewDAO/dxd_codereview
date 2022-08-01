```sh
gitpod /workspace/Verified-Impact-NFTs/contracts (main) $ make prepare
rustup target add wasm32-unknown-unknown
info: syncing channel updates for 'nightly-2022-03-17-x86_64-unknown-linux-gnu'
info: latest update on 2022-03-17, rust version 1.61.0-nightly (461e80780 2022-03-16)
info: downloading component 'cargo'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: installing component 'cargo'
info: installing component 'rust-std'
 26.6 MiB /  26.6 MiB (100 %)  13.2 MiB/s in  1s ETA:  0s
info: installing component 'rustc'
 55.3 MiB /  55.3 MiB (100 %)  15.8 MiB/s in  3s ETA:  0s
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
 16.6 MiB /  16.6 MiB (100 %)  13.8 MiB/s in  1s ETA:  0s
```

```sh
gitpod /workspace/Verified-Impact-NFTs/contracts (main) $ make build-contract
cargo build --release -p vi_nft --target wasm32-unknown-unknown
    Updating crates.io index
    Updating git repository `https://github.com/casper-ecosystem/casper-nft-cep47`
  Downloaded opaque-debug v0.3.0
  Downloaded num-derive v0.3.3
  Downloaded serde_bytes v0.11.6
  Downloaded subtle v2.4.1
  Downloaded unicode-ident v1.0.2
  Downloaded wyz v0.2.0
  Downloaded bitflags v1.3.2
  Downloaded crypto-mac v0.8.0
  Downloaded blake2 v0.9.2
  Downloaded crunchy v0.2.2
  Downloaded num v0.4.0
  Downloaded proc-macro2 v1.0.42
  Downloaded synstructure v0.12.6
  Downloaded rand_chacha v0.2.2
  Downloaded radium v0.3.0
  Downloaded version_check v0.9.4
  Downloaded num-complex v0.4.2
  Downloaded typenum v1.15.0
  Downloaded zeroize_derive v1.3.2
  Downloaded curve25519-dalek v3.2.1
  Downloaded num-rational v0.4.1
  Downloaded elliptic-curve v0.8.5
  Downloaded ed25519-dalek v1.0.1
  Downloaded autocfg v1.1.0
  Downloaded cpufeatures v0.2.2
  Downloaded hex v0.4.3
  Downloaded unicode-xid v0.2.3
  Downloaded block-buffer v0.9.0
  Downloaded static_assertions v1.1.0
  Downloaded rand_core v0.5.1
  Downloaded generic-array v0.14.5
  Downloaded serde v1.0.140
  Downloaded ff v0.8.0
  Downloaded ecdsa v0.10.2
  Downloaded k256 v0.7.3
  Downloaded group v0.8.0
  Downloaded rand v0.7.3
  Downloaded quote v1.0.20
  Downloaded uint v0.9.3
  Downloaded rand v0.8.5
  Downloaded num-iter v0.1.43
  Downloaded syn v1.0.98
  Downloaded serde_json v1.0.82
  Downloaded hmac v0.10.1
  Downloaded num-bigint v0.4.3
  Downloaded libc v0.2.126
  Downloaded ed25519 v1.2.0
  Downloaded hex_fmt v0.3.0
  Downloaded serde_derive v1.0.140
  Downloaded byteorder v1.4.3
  Downloaded itoa v1.0.2
  Downloaded crypto-mac v0.10.1
  Downloaded funty v1.1.0
  Downloaded bitvec v0.18.5
  Downloaded rand_core v0.6.3
  Downloaded num-traits v0.2.15
  Downloaded num-integer v0.1.45
  Downloaded digest v0.9.0
  Downloaded base64 v0.13.0
  Downloaded ppv-lite86 v0.2.16
  Downloaded cfg-if v1.0.0
  Downloaded cfg-if v0.1.10
  Downloaded base16 v0.2.1
  Downloaded zeroize v1.3.0
  Downloaded signature v1.2.2
  Downloaded sha2 v0.9.9
  Downloaded ryu v1.0.10
  Downloaded memory_units v0.4.0
  Downloaded wee_alloc v0.4.5
  Downloaded casper-contract v1.4.4
  Downloaded casper-types v1.5.0
  Downloaded 71 crates (3.4 MB) in 1.26s
   Compiling typenum v1.15.0
   Compiling proc-macro2 v1.0.42
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling quote v1.0.20
   Compiling unicode-ident v1.0.2
   Compiling syn v1.0.98
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.3
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling serde_derive v1.0.140
   Compiling serde v1.0.140
   Compiling opaque-debug v0.3.0
   Compiling crunchy v0.2.2
   Compiling cfg-if v1.0.0
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.82
   Compiling rand_core v0.6.3
   Compiling static_assertions v1.1.0
   Compiling ryu v1.0.10
   Compiling hex v0.4.3
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.2
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling bitflags v1.3.2
   Compiling base64 v0.13.0
   Compiling cfg-if v0.1.10
   Compiling memory_units v0.4.0
   Compiling rand v0.8.5
   Compiling rand_chacha v0.2.2
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling generic-array v0.14.5
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling uint v0.9.3
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling num-complex v0.4.2
   Compiling ed25519 v1.2.0
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling synstructure v0.12.6
   Compiling num v0.4.0
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.6
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling contract-utils v0.1.0 (https://github.com/casper-ecosystem/casper-nft-cep47?branch=master#896e198f)
   Compiling cep47 v0.2.0 (https://github.com/casper-ecosystem/casper-nft-cep47?branch=master#896e198f)
   Compiling vi_nft v0.2.0 (/workspace/Verified-Impact-NFTs/contracts/vi_nft)
    Finished release [optimized] target(s) in 47.63s
wasm-strip target/wasm32-unknown-unknown/release/vi_nft.wasm 2>/dev/null | true
```