```bash
$ make prepare
rustup target add wasm32-unknown-unknown
info: syncing channel updates for 'nightly-2023-01-16-x86_64-unknown-linux-gnu'
info: latest update on 2023-01-16, rust version 1.68.0-nightly (9e75dddf6 2023-01-15)
info: downloading component 'cargo'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: installing component 'cargo'
info: installing component 'rust-std'
 29.8 MiB /  29.8 MiB (100 %)  14.7 MiB/s in  2s ETA:  0s
info: installing component 'rustc'
 67.6 MiB /  67.6 MiB (100 %)  16.2 MiB/s in  4s ETA:  0s
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
 19.2 MiB /  19.2 MiB (100 %)  14.2 MiB/s in  1s ETA:  0s
gitpod /workspace/casper_staking/erc20 (main) $ make build-contracts
cargo build --release --target wasm32-unknown-unknown  -p erc20-token  -p erc20-test  -p erc20-test-call
    Updating crates.io index
  Downloaded num-bigint v0.4.3
  Downloaded serde_bytes v0.11.7
  Downloaded num-derive v0.3.3
  Downloaded num-complex v0.4.2
  Downloaded hex v0.4.3
  Downloaded rand v0.7.3
  Downloaded proc-macro2 v1.0.43
  Downloaded hex_fmt v0.3.0
  Downloaded memory_units v0.4.0
  Downloaded funty v1.1.0
  Downloaded subtle v2.4.1
  Downloaded autocfg v1.1.0
  Downloaded ff v0.8.0
  Downloaded crypto-mac v0.10.1
  Downloaded crunchy v0.2.2
  Downloaded cpufeatures v0.2.2
  Downloaded once_cell v1.13.0
  Downloaded ecdsa v0.10.2
  Downloaded num-iter v0.1.43
  Downloaded wyz v0.2.0
  Downloaded rand_core v0.6.3
  Downloaded hmac v0.10.1
  Downloaded ed25519 v1.2.0
  Downloaded num-integer v0.1.45
  Downloaded ppv-lite86 v0.2.16
  Downloaded ed25519-dalek v1.0.1
  Downloaded crypto-mac v0.8.0
  Downloaded zeroize_derive v1.3.2
  Downloaded digest v0.9.0
  Downloaded block-buffer v0.9.0
  Downloaded itoa v1.0.3
  Downloaded ryu v1.0.11
  Downloaded num-traits v0.2.15
  Downloaded k256 v0.7.3
  Downloaded serde_derive v1.0.143
  Downloaded num-rational v0.4.1
  Downloaded unicode-ident v1.0.3
  Downloaded bitflags v1.3.2
  Downloaded elliptic-curve v0.8.5
  Downloaded cfg-if v1.0.0
  Downloaded zeroize v1.3.0
  Downloaded num v0.4.0
  Downloaded base64 v0.13.0
  Downloaded rand v0.8.5
  Downloaded bitvec v0.18.5
  Downloaded byteorder v1.4.3
  Downloaded blake2 v0.9.2
  Downloaded group v0.8.0
  Downloaded wee_alloc v0.4.5
  Downloaded unicode-xid v0.2.3
  Downloaded typenum v1.15.0
  Downloaded serde_json v1.0.83
  Downloaded cfg-if v0.1.10
  Downloaded version_check v0.9.4
  Downloaded opaque-debug v0.3.0
  Downloaded radium v0.3.0
  Downloaded synstructure v0.12.6
  Downloaded sha2 v0.9.9
  Downloaded rand_core v0.5.1
  Downloaded generic-array v0.14.6
  Downloaded base16 v0.2.1
  Downloaded quote v1.0.21
  Downloaded static_assertions v1.1.0
  Downloaded serde v1.0.143
  Downloaded uint v0.9.3
  Downloaded rand_chacha v0.2.2
  Downloaded syn v1.0.99
  Downloaded libc v0.2.131
  Downloaded signature v1.2.2
  Downloaded casper-contract v1.4.4
  Downloaded curve25519-dalek v3.2.1
  Downloaded casper-types v1.5.0
  Downloaded 72 crates (3.4 MB) in 0.68s
error: package ID specification `erc20-test` did not match any packages
make: *** [Makefile:9: build-contracts] Error 101
```
