## `make prepare`

```sh
gitpod /workspace/casper_staking/staking_contract (main) $ make prepare
rustup target add wasm32-unknown-unknown
info: syncing channel updates for 'nightly-2023-01-16-x86_64-unknown-linux-gnu'
info: latest update on 2023-01-16, rust version 1.68.0-nightly (9e75dddf6 2023-01-15)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
 19.4 MiB /  19.4 MiB (100 %)   4.0 MiB/s in  3s ETA:  0s
info: installing component 'rust-std'
 29.8 MiB /  29.8 MiB (100 %)  13.7 MiB/s in  2s ETA:  0s
info: installing component 'rustc'
 67.6 MiB /  67.6 MiB (100 %)  15.5 MiB/s in  4s ETA:  0s
info: installing component 'rustfmt'
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
 19.2 MiB /  19.2 MiB (100 %)  14.2 MiB/s in  1s ETA:  0s
gitpod /workspace/casper_staking/staking_contract (main) $
```

## `make build-contract`

```sh
gitpod /workspace/casper_staking/staking_contract (main) $ make build-contract 
cd staking_contract && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
  Downloaded ed25519 v1.2.0
  Downloaded js-sys v0.3.61
  Downloaded rand_chacha v0.2.2
  Downloaded log v0.4.17
  Downloaded ff v0.8.0
  Downloaded wasm-bindgen-shared v0.2.84
  Downloaded proc-macro2 v1.0.56
  Downloaded ryu v1.0.13
  Downloaded autocfg v1.1.0
  Downloaded wasm-bindgen-macro-support v0.2.84
  Downloaded version_check v0.9.4
  Downloaded num v0.4.0
  Downloaded serde_derive v1.0.160
  Downloaded ed25519-dalek v1.0.1
  Downloaded num-rational v0.4.1
  Downloaded cfg-if v1.0.0
  Downloaded rand v0.7.3
  Downloaded base64 v0.13.1
  Downloaded zeroize v1.3.0
  Downloaded zeroize_derive v1.4.2
  Downloaded sha2 v0.9.9
  Downloaded byteorder v1.4.3
  Downloaded bitflags v1.3.2
  Downloaded itoa v1.0.6
  Downloaded signature v1.2.2
  Downloaded wasm-bindgen-backend v0.2.84
  Downloaded rand_core v0.6.4
  Downloaded num-integer v0.1.45
  Downloaded group v0.8.0
  Downloaded wyz v0.2.0
  Downloaded radium v0.3.0
  Downloaded wasm-bindgen-macro v0.2.84
  Downloaded blake2 v0.9.2
  Downloaded block-buffer v0.9.0
  Downloaded elliptic-curve v0.8.5
  Downloaded serde v1.0.160
  Downloaded crunchy v0.2.2
  Downloaded hex v0.4.3
  Downloaded serde_json v1.0.96
  Downloaded opaque-debug v0.3.0
  Downloaded bitvec v0.18.5
  Downloaded funty v1.1.0
  Downloaded rand v0.8.5
  Downloaded num-derive v0.3.3
  Downloaded crypto-mac v0.8.0
  Downloaded wasm-bindgen v0.2.84
  Downloaded cfg-if v0.1.10
  Downloaded ecdsa v0.10.2
  Downloaded subtle v2.4.1
  Downloaded serde_bytes v0.11.9
  Downloaded num-iter v0.1.43
  Downloaded digest v0.9.0
  Downloaded cpufeatures v0.2.7
  Downloaded base16 v0.2.1
  Downloaded typenum v1.16.0
  Downloaded num-bigint v0.4.3
  Downloaded rand_core v0.5.1
  Downloaded ppv-lite86 v0.2.17
  Downloaded hmac v0.10.1
  Downloaded static_assertions v1.1.0
  Downloaded getrandom v0.2.9
  Downloaded unicode-ident v1.0.8
  Downloaded curve25519-dalek v3.2.1
  Downloaded once_cell v1.17.1
  Downloaded casper-contract v1.4.4
  Downloaded bumpalo v3.12.1
  Downloaded uint v0.9.5
  Downloaded generic-array v0.14.7
  Downloaded libc v0.2.142
  Downloaded hex_fmt v0.3.0
  Downloaded crypto-mac v0.10.1
  Downloaded syn v1.0.109
  Downloaded syn v2.0.15
  Downloaded quote v1.0.26
  Downloaded num-complex v0.4.3
  Downloaded num-traits v0.2.15
  Downloaded wee_alloc v0.4.5
  Downloaded casper-types v1.5.0
  Downloaded memory_units v0.4.0
  Downloaded k256 v0.7.3
  Downloaded 80 crates (4.2 MB) in 0.59s
   Compiling proc-macro2 v1.0.56
   Compiling quote v1.0.26
   Compiling unicode-ident v1.0.8
   Compiling typenum v1.16.0
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling syn v1.0.109
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling cfg-if v1.0.0
   Compiling serde_derive v1.0.160
   Compiling log v0.4.17
   Compiling wasm-bindgen-shared v0.2.84
   Compiling serde v1.0.160
   Compiling ppv-lite86 v0.2.17
   Compiling bumpalo v3.12.1
   Compiling opaque-debug v0.3.0
   Compiling once_cell v1.17.1
   Compiling crunchy v0.2.2
   Compiling byteorder v1.4.3
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling generic-array v0.14.7
   Compiling num-bigint v0.4.3
   Compiling bitvec v0.18.5
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling rand_chacha v0.2.2
   Compiling serde_json v1.0.96
   Compiling wee_alloc v0.4.5
   Compiling rand_core v0.6.4
   Compiling wasm-bindgen v0.2.84
   Compiling rand v0.7.3
   Compiling ryu v1.0.13
   Compiling static_assertions v1.1.0
   Compiling itoa v1.0.6
   Compiling hex v0.4.3
   Compiling rand v0.8.5
   Compiling base64 v0.13.1
   Compiling memory_units v0.4.0
   Compiling cfg-if v0.1.10
   Compiling base16 v0.2.1
   Compiling bitflags v1.3.2
   Compiling hex_fmt v0.3.0
   Compiling syn v2.0.15
   Compiling uint v0.9.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.3
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling wasm-bindgen-backend v0.2.84
   Compiling num v0.4.0
   Compiling num-derive v0.3.3
   Compiling wasm-bindgen-macro-support v0.2.84
   Compiling wasm-bindgen-macro v0.2.84
   Compiling zeroize_derive v1.4.2
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling js-sys v0.3.61
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling getrandom v0.2.9
   Compiling serde_bytes v0.11.9
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling contract-utils v0.1.0 (/workspace/casper_staking/staking_contract/utils/contract-utils)
   Compiling staking_contract v0.1.0 (/workspace/casper_staking/staking_contract/staking_contract)
    Finished release [optimized] target(s) in 3m 50s
wasm-strip staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cd ../erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
  Downloaded serde_bytes v0.11.7
  Downloaded ryu v1.0.11
  Downloaded itoa v1.0.3
  Downloaded ppv-lite86 v0.2.16
  Downloaded base64 v0.13.0
  Downloaded cpufeatures v0.2.2
  Downloaded rand_core v0.6.3
  Downloaded unicode-xid v0.2.3
  Downloaded zeroize_derive v1.3.2
  Downloaded unicode-ident v1.0.3
  Downloaded generic-array v0.14.6
  Downloaded once_cell v1.13.0
  Downloaded synstructure v0.12.6
  Downloaded uint v0.9.3
  Downloaded typenum v1.15.0
  Downloaded proc-macro2 v1.0.43
  Downloaded serde_derive v1.0.143
  Downloaded num-complex v0.4.2
  Downloaded quote v1.0.21
  Downloaded serde v1.0.143
  Downloaded serde_json v1.0.83
  Downloaded syn v1.0.99
  Downloaded libc v0.2.131
  Downloaded 23 crates (1.6 MB) in 0.42s
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.43
   Compiling typenum v1.15.0
   Compiling autocfg v1.1.0
   Compiling unicode-ident v1.0.3
   Compiling quote v1.0.21
   Compiling syn v1.0.99
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.3
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling serde_derive v1.0.143
   Compiling serde v1.0.143
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.16
   Compiling cfg-if v1.0.0
   Compiling opaque-debug v0.3.0
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.83
   Compiling rand_core v0.6.3
   Compiling wee_alloc v0.4.5
   Compiling hex v0.4.3
   Compiling itoa v1.0.3
   Compiling ryu v1.0.11
   Compiling generic-array v0.14.6
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling bitvec v0.18.5
   Compiling rand_chacha v0.2.2
   Compiling static_assertions v1.1.0
   Compiling rand v0.8.5
   Compiling memory_units v0.4.0
   Compiling uint v0.9.3
   Compiling base64 v0.13.0
   Compiling bitflags v1.3.2
   Compiling cfg-if v0.1.10
   Compiling hex_fmt v0.3.0
   Compiling rand v0.7.3
   Compiling base16 v0.2.1
   Compiling once_cell v1.13.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling blake2 v0.9.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling num v0.4.0
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling casper-erc20 v0.2.1 (/workspace/casper_staking/erc20/erc20)
warning: unused import: `alloc::string::String`
 --> erc20/src/error.rs:2:5
  |
2 | use alloc::string::String;
  |     ^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: missing documentation for a function
   --> erc20/src/entry_points.rs:145:1
    |
145 | pub fn mint() -> EntryPoint {
    | ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    |
note: the lint level is defined here
   --> erc20/src/lib.rs:13:9
    |
13  | #![warn(missing_docs)]
    |         ^^^^^^^^^^^^

warning: missing documentation for a variant
  --> erc20/src/error.rs:28:5
   |
28 |     UserAllowance(u16),
   |     ^^^^^^^^^^^^^

warning: `casper-erc20` (lib) generated 3 warnings (run `cargo fix --lib -p casper-erc20` to apply 1 suggestion)
   Compiling erc20-token v0.1.0 (/workspace/casper_staking/erc20/erc20-token)
warning: unused import: `core::panic::PanicInfo`
  --> erc20-token/src/main.rs:10:5
   |
10 | use core::panic::PanicInfo;
   |     ^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `erc20-token` (bin "erc20_token") generated 1 warning (run `cargo fix --bin "erc20_token"` to apply 1 suggestion)
    Finished release [optimized] target(s) in 32.42s
wasm-strip ../erc20/erc20-token/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
gitpod /workspace/casper_staking/staking_contract (main) $
```