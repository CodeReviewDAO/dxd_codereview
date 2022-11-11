'''
muharremsalel@Muharrems-MacBook-Pro devxdao-m2 %  make clean test
cd contract && cargo clean
cd tests && cargo clean
rm -rf tests/wasm
cd contract && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
    Updating git repository `https://github.com/darthsiroftardis/casper-serde-json-wasm`
  Downloaded unicode-ident v1.0.5
  Downloaded proc-macro2 v1.0.47
  Downloaded memory_units v0.4.0
  Downloaded serde_derive v1.0.147
  Downloaded serde_json v1.0.87
  Downloaded serde v1.0.147
  Downloaded base64 v0.13.1
  Downloaded syn v1.0.103
  Downloaded libc v0.2.135
  Downloaded itoa v1.0.4
  Downloaded wee_alloc v0.4.5
  Downloaded 11 crates (1.3 MB) in 1.62s
   Compiling proc-macro2 v1.0.47
   Compiling version_check v0.9.4
   Compiling typenum v1.15.0
   Compiling unicode-ident v1.0.5
   Compiling autocfg v1.1.0
   Compiling quote v1.0.21
   Compiling syn v1.0.103
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling serde_json v1.0.87
   Compiling cfg-if v1.0.0
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling ryu v1.0.11
   Compiling itoa v1.0.4
   Compiling rand_core v0.6.4
   Compiling wee_alloc v0.4.5
   Compiling static_assertions v1.1.0
   Compiling hex v0.4.3
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling bitflags v1.3.2
   Compiling base16 v0.2.1
   Compiling memory_units v0.4.0
   Compiling cfg-if v0.1.10
   Compiling rand v0.8.5
   Compiling generic-array v0.14.6
   Compiling rand_chacha v0.2.2
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling uint v0.9.4
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num-complex v0.4.2
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
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
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling casper-serde-json-wasm v0.4.1 (https://github.com/darthsiroftardis/casper-serde-json-wasm?branch=casper-no-std#6b72ee20)
   Compiling casper-contract v1.4.4
   Compiling contract v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/contract)
    Finished release [optimized] target(s) in 6m 13s
cd client/mint_session && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
   Compiling proc-macro2 v1.0.47
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling typenum v1.15.0
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.5
   Compiling syn v1.0.103
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling ppv-lite86 v0.2.16
   Compiling cfg-if v1.0.0
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.87
   Compiling wee_alloc v0.4.5
   Compiling ryu v1.0.11
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling hex v0.4.3
   Compiling itoa v1.0.4
   Compiling bitflags v1.3.2
   Compiling base64 v0.13.1
   Compiling base16 v0.2.1
   Compiling memory_units v0.4.0
   Compiling hex_fmt v0.3.0
   Compiling cfg-if v0.1.10
   Compiling rand v0.8.5
   Compiling rand_chacha v0.2.2
   Compiling generic-array v0.14.6
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand v0.7.3
   Compiling bitvec v0.18.5
   Compiling uint v0.9.4
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling num v0.4.0
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling mint_session v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/client/mint_session)
    Finished release [optimized] target(s) in 36.15s
cd client/balance_of_session && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.47
   Compiling typenum v1.15.0
   Compiling unicode-ident v1.0.5
   Compiling quote v1.0.21
   Compiling syn v1.0.103
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling cfg-if v1.0.0
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.16
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.87
   Compiling hex v0.4.3
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.4
   Compiling static_assertions v1.1.0
   Compiling ryu v1.0.11
   Compiling rand_core v0.6.4
   Compiling cfg-if v0.1.10
   Compiling base64 v0.13.1
   Compiling hex_fmt v0.3.0
   Compiling memory_units v0.4.0
   Compiling base16 v0.2.1
   Compiling bitflags v1.3.2
   Compiling generic-array v0.14.6
   Compiling rand v0.8.5
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling uint v0.9.4
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling ff v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling group v0.8.0
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
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
   Compiling balance_of_session v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/client/balance_of_session)
    Finished release [optimized] target(s) in 34.61s
cd client/owner_of_session && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
   Compiling typenum v1.15.0
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling proc-macro2 v1.0.47
   Compiling unicode-ident v1.0.5
   Compiling quote v1.0.21
   Compiling syn v1.0.103
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling cfg-if v1.0.0
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.87
   Compiling itoa v1.0.4
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling wee_alloc v0.4.5
   Compiling hex v0.4.3
   Compiling ryu v1.0.11
   Compiling base64 v0.13.1
   Compiling hex_fmt v0.3.0
   Compiling bitflags v1.3.2
   Compiling memory_units v0.4.0
   Compiling cfg-if v0.1.10
   Compiling base16 v0.2.1
   Compiling generic-array v0.14.6
   Compiling rand v0.8.5
   Compiling rand_chacha v0.2.2
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand v0.7.3
   Compiling bitvec v0.18.5
   Compiling uint v0.9.4
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling ff v0.8.0
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
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
   Compiling owner_of_session v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/client/owner_of_session)
    Finished release [optimized] target(s) in 34.31s
cd client/get_approved_session && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
   Compiling typenum v1.15.0
   Compiling proc-macro2 v1.0.47
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.5
   Compiling syn v1.0.103
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling cfg-if v1.0.0
   Compiling ppv-lite86 v0.2.16
   Compiling opaque-debug v0.3.0
   Compiling crunchy v0.2.2
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.87
   Compiling itoa v1.0.4
   Compiling hex v0.4.3
   Compiling wee_alloc v0.4.5
   Compiling ryu v1.0.11
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling memory_units v0.4.0
   Compiling base16 v0.2.1
   Compiling bitflags v1.3.2
   Compiling base64 v0.13.1
   Compiling cfg-if v0.1.10
   Compiling hex_fmt v0.3.0
   Compiling generic-array v0.14.6
   Compiling rand v0.8.5
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling uint v0.9.4
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling ff v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling group v0.8.0
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
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
   Compiling get_approved_session v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/client/get_approved_session)
    Finished release [optimized] target(s) in 34.61s
cd client/minting_contract && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.47
   Compiling autocfg v1.1.0
   Compiling typenum v1.15.0
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.5
   Compiling syn v1.0.103
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling opaque-debug v0.3.0
   Compiling byteorder v1.4.3
   Compiling cfg-if v1.0.0
   Compiling ppv-lite86 v0.2.16
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.87
   Compiling rand_core v0.6.4
   Compiling ryu v1.0.11
   Compiling hex v0.4.3
   Compiling itoa v1.0.4
   Compiling wee_alloc v0.4.5
   Compiling static_assertions v1.1.0
   Compiling base64 v0.13.1
   Compiling memory_units v0.4.0
   Compiling bitflags v1.3.2
   Compiling cfg-if v0.1.10
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling rand v0.8.5
   Compiling generic-array v0.14.6
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling uint v0.9.4
   Compiling ff v0.8.0
   Compiling group v0.8.0
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
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling zeroize v1.3.0
   Compiling num v0.4.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling minting_contract v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/client/minting_contract)
    Finished release [optimized] target(s) in 35.22s
cd client/transfer_session && cargo build --release --target wasm32-unknown-unknown
    Updating crates.io index
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling typenum v1.15.0
   Compiling proc-macro2 v1.0.47
   Compiling unicode-ident v1.0.5
   Compiling quote v1.0.21
   Compiling syn v1.0.103
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling serde_derive v1.0.147
   Compiling serde v1.0.147
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.16
   Compiling cfg-if v1.0.0
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.87
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.4
   Compiling rand_core v0.6.4
   Compiling hex v0.4.3
   Compiling static_assertions v1.1.0
   Compiling ryu v1.0.11
   Compiling base16 v0.2.1
   Compiling base64 v0.13.1
   Compiling memory_units v0.4.0
   Compiling bitflags v1.3.2
   Compiling hex_fmt v0.3.0
   Compiling cfg-if v0.1.10
   Compiling generic-array v0.14.6
   Compiling rand v0.8.5
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling uint v0.9.4
   Compiling rand v0.7.3
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling ff v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling group v0.8.0
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
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
   Compiling transfer_session v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/client/transfer_session)
    Finished release [optimized] target(s) in 34.57s
wasm-strip contract/target/wasm32-unknown-unknown/release/contract.wasm 2>/dev/null | true
wasm-strip entrypoint_session/target/wasm32-unknown-unknown/release/entrypoint_call.wasm 2>/dev/null | true
wasm-strip client/mint_session/target/wasm32-unknown-unknown/release/mint_call.wasm 2>/dev/null | true
wasm-strip client/balance_of_session/target/wasm32-unknown-unknown/release/balance_of_call.wasm 2>/dev/null | true
wasm-strip client/owner_of_session/target/wasm32-unknown-unknown/release/owner_of_call.wasm 2>/dev/null | true
wasm-strip client/get_approved_session/target/wasm32-unknown-unknown/release/get_approved_call.wasm 2>/dev/null | true
wasm-strip client/minting_contract/target/wasm32-unknown-unknown/release/minting_contract.wasm 2>/dev/null | true
wasm-strip client/transfer_session/target/wasm32-unknown-unknown/release/transfer_call.wasm 2>/dev/null | true
mkdir -p tests/wasm
cp contract/target/wasm32-unknown-unknown/release/contract.wasm tests/wasm
cp client/mint_session/target/wasm32-unknown-unknown/release/mint_call.wasm tests/wasm
cp client/balance_of_session/target/wasm32-unknown-unknown/release/balance_of_call.wasm tests/wasm
cp client/owner_of_session/target/wasm32-unknown-unknown/release/owner_of_call.wasm tests/wasm
cp client/get_approved_session/target/wasm32-unknown-unknown/release/get_approved_call.wasm tests/wasm
cp client/minting_contract/target/wasm32-unknown-unknown/release/minting_contract.wasm tests/wasm
cp client/transfer_session/target/wasm32-unknown-unknown/release/transfer_call.wasm tests/wasm
cd tests && cargo test
    Updating crates.io index
  Downloaded getrandom v0.2.8
  Downloaded thiserror-impl v1.0.37
  Downloaded thiserror v1.0.37
  Downloaded ctor v0.1.26
  Downloaded tracing-attributes v0.1.23
  Downloaded tracing v0.1.37
  Downloaded iana-time-zone v0.1.51
  Downloaded tracing-core v0.1.30
  Downloaded anyhow v1.0.66
  Downloaded 9 crates (303.4 KB) in 0.67s
   Compiling proc-macro2 v1.0.47
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.5
   Compiling syn v1.0.103
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.135
   Compiling serde_derive v1.0.147
   Compiling typenum v1.15.0
   Compiling serde v1.0.147
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling fastrand v1.8.0
   Compiling remove_dir_all v0.5.3
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.87
   Compiling crunchy v0.2.2
   Compiling pkg-config v0.3.25
   Compiling quick-error v1.2.3
   Compiling cpufeatures v0.2.5
   Compiling ryu v1.0.11
   Compiling cc v1.0.73
   Compiling core-foundation-sys v0.8.3
   Compiling bit-vec v0.6.3
   Compiling itoa v1.0.4
   Compiling fnv v1.0.7
   Compiling once_cell v1.15.0
   Compiling hashbrown v0.12.3
   Compiling schemars v0.8.5
   Compiling bitflags v1.3.2
   Compiling thiserror v1.0.37
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.9
   Compiling parity-wasm v0.41.0
   Compiling static_assertions v1.1.0
   Compiling log v0.4.17
   Compiling regex-syntax v0.6.27
   Compiling lazy_static v1.4.0
   Compiling anyhow v1.0.66
   Compiling base64 v0.13.1
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling either v1.8.0
   Compiling downcast-rs v1.2.0
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling pin-project-lite v0.2.9
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling indexmap v1.9.1
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.3
   Compiling tracing-core v0.1.30
   Compiling rand_chacha v0.2.2
   Compiling itertools v0.10.5
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.8
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.44
   Compiling hostname v0.3.1
   Compiling num_cpus v1.13.1
   Compiling lmdb-sys v0.8.0
   Compiling iana-time-zone v0.1.51
   Compiling rand_core v0.6.4
   Compiling ff v0.8.0
   Compiling rusty-fork v0.3.0
   Compiling group v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling rand v0.8.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling proptest v1.0.0
   Compiling chrono v0.4.22
   Compiling wasmi v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling zeroize_derive v1.3.2
   Compiling datasize_derive v0.2.10
   Compiling ctor v0.1.26
   Compiling schemars_derive v0.8.5
   Compiling thiserror-impl v1.0.37
   Compiling num-derive v0.3.3
   Compiling tracing-attributes v0.1.23
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling tracing v0.1.37
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling lmdb v0.8.0
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.7
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.4
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling casper-hashing v1.4.3
   Compiling casper-execution-engine v2.0.1
   Compiling casper-engine-test-support v2.2.0
   Compiling tests v0.1.0 (/Users/muharremsalel/Desktop/CRDao/devxdao-m2/tests)
    Finished test [unoptimized + debuginfo] target(s) in 56.93s
     Running unittests src/lib.rs (target/debug/deps/tests-8e75749f98e6497b)

running 56 tests
test installer::should_reject_invalid_collection_symbol ... ok
test metadata::get_schema ... ok
test installer::should_reject_invalid_collection_name ... ok
test installer::should_reject_non_numerical_total_token_supply_value ... ok
test metadata::should_prevent_install_with_hash_identifier_in_mutable_mode ... ok
test installer::should_disallow_installation_of_contract_with_empty_locked_whitelist ... ok
test installer::should_install_with_allow_minting_set_to_false ... ok
test installer::should_install_with_contract_holder_mode ... ok
test installer::should_install_contract ... ok
test installer::should_only_allow_init_during_installation_session ... ok
test burn::should_return_expected_error_when_burning_non_existing_token ... ok
test account_whitelist::should_add_account_to_whitelist ... ok
test account_whitelist::should_remove_account_from_whitelist ... ok
test burn::should_return_expected_error_when_burning_not_owned_token_only_contract_creator_can_burn ... ok
test burn::should_return_expected_error_burning_of_others_users_token_only_contract_creator_can_burn ... ok
test burn::should_burn_minted_token ... ok
test burn::should_not_burn_previously_burnt_token ... ok
test burn::should_allow_contract_to_burn_token ... ok
test metadata::should_prevent_update_for_invalid_metadata ... ok
test metadata::should_prevent_metadata_update_by_non_owner_key ... ok
test metadata::should_prevent_update_in_immutable_mode ... ok
test metadata::should_update_metadata_for_cep78_using_token_id ... ok
test mint::should_allow_public_minting_with_flag_set_to_true ... ok
test mint::should_allow_minting_for_different_public_key_with_minting_mode_set_to_public ... ok
test metadata::should_update_metadata_for_nft721_using_token_id ... ok
test metadata::should_update_metadata_for_custom_validated_using_token_id ... ok
test mint::should_disallow_minting_when_allow_minting_is_set_to_false ... ok
test mint::mint_should_increment_number_of_minted_tokens_by_one_and_add_public_key_to_token_owners ... ok
test mint::mint_should_return_dictionary_key_to_callers_owned_tokens ... ok
test mint::should_disallow_public_minting_with_flag_set_to_false ... ok
test mint::should_allow_whitelisted_contract_to_mint ... ok
test mint::should_fail_to_mint_when_immediate_caller_is_account_in_contract_mode ... ok
test mint::should_disallow_unlisted_contract_from_minting ... ok
test mint::should_mint ... ok
test mint::entry_points_with_ret_should_return_correct_value ... ok
test mint::should_be_able_to_update_whitelist_for_minting ... ok
test mint::should_mint_with_compactified_metadata ... ok
test mint::should_mint_with_custom_metadata_validation ... ok
test mint::should_not_mint_with_invalid_nft721_metadata ... ok
test mint::should_mint_with_raw_metadata ... ok
test mint::should_mint_with_hash_identifier_mode ... ok
test mint::should_mint_with_valid_cep99_metadata ... ok
test mint::should_set_issuer ... ok
test mint::should_set_meta_data ... ok
test set_variables::only_installer_should_be_able_to_toggle_allow_minting ... ok
test mint::should_track_token_balance_by_owner ... ok
test transfer::approve_token_for_transfer_should_add_entry_to_approved_dictionary ... ok
test transfer::should_disallow_approving_when_ownership_mode_is_minter_or_assigned ... ok
test transfer::should_disallow_transfer_with_minter_or_assigned_ownership_mode ... ok
test transfer::should_be_able_to_transfer_token_using_approved_operator ... ok
test mint::should_set_approval_for_all ... ok
test transfer::should_prevent_transfer_when_caller_is_not_owner ... ok
test transfer::should_disallow_same_operator_to_tranfer_token_twice ... ok
test transfer::should_transfer_token_from_sender_to_receiver ... ok
test transfer::should_transfer_token_in_hash_identifier_mode ... ok
test transfer::should_transfer_between_contract_to_account ... ok

test result: ok. 56 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 7.96s

   Doc-tests tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

'''