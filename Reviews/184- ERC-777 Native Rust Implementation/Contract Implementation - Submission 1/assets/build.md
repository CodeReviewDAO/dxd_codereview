(base) mdidin@Muhammed-MacBook-Air CasperLabs-ERC777 % make build-contracts
cargo build --release --target wasm32-unknown-unknown  -p erc777-token  -p erc1820-registry  -p erc777-recipient-contract  -p erc777-sender-contract
   Compiling proc-macro2 v1.0.29
   Compiling syn v1.0.76
   Compiling unicode-xid v0.2.0
   Compiling version_check v0.9.3
   Compiling typenum v1.14.0
   Compiling cfg-if v0.1.10
   Compiling getrandom v0.1.14
   Compiling autocfg v1.0.0
   Compiling subtle v2.4.1
   Compiling serde v1.0.105
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling tinyvec_macros v0.1.0
   Compiling bitflags v1.2.1
   Compiling ryu v1.0.3
   Compiling cfg-if v1.0.0
   Compiling crunchy v0.2.2
   Compiling matches v0.1.9
   Compiling serde_json v1.0.67
   Compiling ppv-lite86 v0.2.10
   Compiling byteorder v1.4.3
   Compiling memchr v2.4.1
   Compiling opaque-debug v0.3.0
   Compiling hashbrown v0.11.2
   Compiling pulldown-cmark v0.8.0
   Compiling unicode-bidi v0.3.6
   Compiling percent-encoding v2.1.0
   Compiling schemars v0.8.3
   Compiling itoa v0.4.5
   Compiling hex v0.4.3
   Compiling dyn-clone v1.0.4
   Compiling static_assertions v1.1.0
   Compiling wee_alloc v0.4.5
   Compiling rand_core v0.6.3
   Compiling regex-syntax v0.6.25
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.0
   Compiling base16 v0.2.1
   Compiling once_cell v1.8.0
   Compiling memory_units v0.4.0
   Compiling semver-parser v0.9.0
   Compiling generic-array v0.14.4
   Compiling unicase v2.6.0
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling indexmap v1.7.0
   Compiling num-rational v0.4.0
   Compiling tinyvec v1.3.1
   Compiling bitvec v0.18.5
   Compiling form_urlencoded v1.0.1
   Compiling rand v0.8.4
   Compiling unicode-normalization v0.1.19
   Compiling regex v1.5.4
   Compiling rand_core v0.5.1
   Compiling quote v1.0.9
   Compiling uint v0.9.1
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling idna v0.2.3
   Compiling group v0.8.0
   Compiling rand v0.7.3
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling url v2.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.8
   Compiling blake2 v0.9.2
   Compiling synstructure v0.12.3
   Compiling serde_derive_internals v0.25.0
   Compiling serde_derive v1.0.105
   Compiling zeroize_derive v1.1.0
   Compiling datasize_derive v0.2.9
   Compiling schemars_derive v0.8.3
   Compiling thiserror-impl v1.0.29
   Compiling num-derive v0.3.0
   Compiling displaydoc v0.1.7
   Compiling zeroize v1.4.1
   Compiling datasize v0.2.9
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.0
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling thiserror v1.0.29
   Compiling ed25519 v1.2.0
   Compiling serde_bytes v0.11.5
   Compiling toml v0.5.8
   Compiling ed25519-dalek v1.0.1
   Compiling version-sync v0.9.2
   Compiling casper-types v1.3.2
   Compiling casper-contract v1.3.2
   Compiling casper-erc777-sender v0.1.0 (/Users/mdidin/CasperLabs-ERC777/erc777-sender)
   Compiling casper-erc777-recipient v0.1.0 (/Users/mdidin/CasperLabs-ERC777/erc777-recipient)
   Compiling casper-erc777 v0.2.1 (/Users/mdidin/CasperLabs-ERC777/erc777)
   Compiling casper-erc1820 v0.1.0 (/Users/mdidin/CasperLabs-ERC777/erc1820)
   Compiling erc777-recipient-contract v0.0.1 (/Users/mdidin/CasperLabs-ERC777/example/implementations/erc777-recipient-contract)
   Compiling erc777-token v0.0.1 (/Users/mdidin/CasperLabs-ERC777/example/implementations/erc777-token)
   Compiling erc777-sender-contract v0.0.1 (/Users/mdidin/CasperLabs-ERC777/example/implementations/erc777-sender-contract)
   Compiling erc1820-registry v0.1.0 (/Users/mdidin/CasperLabs-ERC777/example/implementations/erc1820-registry)
    Finished release [optimized] target(s) in 1m 19s
wasm-strip target/wasm32-unknown-unknown/release/erc777_token.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc1820_registry.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc777_recipient_contract.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc777_sender_contract.wasm 2>/dev/null | true;