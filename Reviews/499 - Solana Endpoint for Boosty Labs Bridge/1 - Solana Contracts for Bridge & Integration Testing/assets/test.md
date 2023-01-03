```
gitpod /workspace/CasperLabs-Solana-bridge (main) $ npm test

> casperlabs-solana-bridge@1.0.0 test
> npm run build:program && npm run test-host && npm run test-client


> casperlabs-solana-bridge@1.0.0 build:program
> cargo build-bpf --manifest-path=./Cargo.toml

Warning: cargo-build-bpf is deprecated. Please, use cargo-build-sbf
cargo-build-bpf child: /home/gitpod/.local/share/solana/install/active_release/bin/cargo-build-sbf --manifest-path=./Cargo.toml --arch bpf
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling once_cell v1.16.0
   Compiling itoa v1.0.4
   Compiling ryu v1.0.11
   Compiling bs58 v0.4.0
   Compiling keccak v0.1.3
   Compiling lazy_static v1.4.0
   Compiling arrayvec v0.7.2
   Compiling either v1.8.0
   Compiling constant_time_eq v0.2.4
   Compiling arrayref v0.3.6
   Compiling typenum v1.15.0
   Compiling memoffset v0.6.5
   Compiling num-traits v0.2.15
   Compiling serde v1.0.148
   Compiling thiserror v1.0.37
   Compiling bytemuck v1.12.3
   Compiling log v0.4.17
   Compiling num_enum v0.5.7
   Compiling ahash v0.7.6
   Compiling itertools v0.10.5
   Compiling hashbrown v0.11.2
   Compiling borsh v0.9.3
   Compiling generic-array v0.14.6
   Compiling bv v0.11.1
   Compiling serde_bytes v0.11.7
   Compiling serde_json v1.0.89
   Compiling bincode v1.3.3
   Compiling block-buffer v0.10.3
   Compiling crypto-common v0.1.6
   Compiling digest v0.10.6
   Compiling sha2 v0.10.6
   Compiling sha3 v0.10.6
   Compiling blake3 v1.3.3
   Compiling solana-frozen-abi v1.14.9
   Compiling solana-program v1.14.9
   Compiling spl-token v3.5.0
   Compiling bridge v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/Bridge)
    Finished release [optimized] target(s) in 36.43s
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling once_cell v1.16.0
   Compiling ryu v1.0.11
   Compiling itoa v1.0.4
   Compiling keccak v0.1.3
   Compiling either v1.8.0
   Compiling lazy_static v1.4.0
   Compiling constant_time_eq v0.2.4
   Compiling arrayvec v0.7.2
   Compiling bs58 v0.4.0
   Compiling arrayref v0.3.6
   Compiling typenum v1.15.0
   Compiling memoffset v0.6.5
   Compiling num-traits v0.2.15
   Compiling serde v1.0.148
   Compiling thiserror v1.0.37
   Compiling bytemuck v1.12.3
   Compiling log v0.4.17
   Compiling num_enum v0.5.7
   Compiling ahash v0.7.6
   Compiling itertools v0.10.5
   Compiling hashbrown v0.11.2
   Compiling borsh v0.9.3
   Compiling generic-array v0.14.6
   Compiling bv v0.11.1
   Compiling serde_json v1.0.89
   Compiling serde_bytes v0.11.7
   Compiling bincode v1.3.3
   Compiling crypto-common v0.1.6
   Compiling block-buffer v0.10.3
   Compiling digest v0.10.6
   Compiling sha2 v0.10.6
   Compiling blake3 v1.3.3
   Compiling sha3 v0.10.6
   Compiling solana-frozen-abi v1.14.9
   Compiling solana-program v1.14.9
   Compiling spl-token v3.5.0
   Compiling w_pokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPokt)
    Finished release [optimized] target(s) in 30.37s
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling once_cell v1.16.0
   Compiling ryu v1.0.11
   Compiling itoa v1.0.4
   Compiling bs58 v0.4.0
   Compiling constant_time_eq v0.2.4
   Compiling arrayref v0.3.6
   Compiling arrayvec v0.7.2
   Compiling either v1.8.0
   Compiling keccak v0.1.3
   Compiling lazy_static v1.4.0
   Compiling typenum v1.15.0
   Compiling log v0.4.17
   Compiling num-traits v0.2.15
   Compiling memoffset v0.6.5
   Compiling serde v1.0.148
   Compiling thiserror v1.0.37
   Compiling bytemuck v1.12.3
   Compiling num_enum v0.5.7
   Compiling itertools v0.10.5
   Compiling ahash v0.7.6
   Compiling hashbrown v0.11.2
   Compiling borsh v0.9.3
   Compiling generic-array v0.14.6
   Compiling serde_json v1.0.89
   Compiling bv v0.11.1
   Compiling serde_bytes v0.11.7
   Compiling bincode v1.3.3
   Compiling crypto-common v0.1.6
   Compiling block-buffer v0.10.3
   Compiling digest v0.10.6
   Compiling sha2 v0.10.6
   Compiling sha3 v0.10.6
   Compiling blake3 v1.3.3
   Compiling solana-frozen-abi v1.14.9
   Compiling solana-program v1.14.9
   Compiling spl-token v3.5.0
   Compiling wpokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPOKT)
    Finished release [optimized] target(s) in 30.14s


> casperlabs-solana-bridge@1.0.0 test-host
> cargo test-bpf --manifest-path=./Cargo.toml

Warning: cargo-test-bpf is deprecated. Please, use cargo-test-sbf
cargo-test-bpf child: /home/gitpod/.local/share/solana/install/active_release/bin/cargo-test-sbf --manifest-path=./Cargo.toml --arch bpf
   Compiling subtle v2.4.1
   Compiling once_cell v1.16.0
   Compiling cfg-if v1.0.0
   Compiling itoa v1.0.4
   Compiling ryu v1.0.11
   Compiling arrayref v0.3.6
   Compiling either v1.8.0
   Compiling arrayvec v0.7.2
   Compiling constant_time_eq v0.2.4
   Compiling keccak v0.1.3
   Compiling bs58 v0.4.0
   Compiling lazy_static v1.4.0
   Compiling typenum v1.15.0
   Compiling num-traits v0.2.15
   Compiling memoffset v0.6.5
   Compiling log v0.4.17
   Compiling serde v1.0.148
   Compiling thiserror v1.0.37
   Compiling bytemuck v1.12.3
   Compiling num_enum v0.5.7
   Compiling itertools v0.10.5
   Compiling ahash v0.7.6
   Compiling hashbrown v0.11.2
   Compiling borsh v0.9.3
   Compiling generic-array v0.14.6
   Compiling bv v0.11.1
   Compiling serde_bytes v0.11.7
   Compiling serde_json v1.0.89
   Compiling bincode v1.3.3
   Compiling crypto-common v0.1.6
   Compiling block-buffer v0.10.3
   Compiling digest v0.10.6
   Compiling sha2 v0.10.6
   Compiling sha3 v0.10.6
   Compiling blake3 v1.3.3
   Compiling solana-frozen-abi v1.14.9
   Compiling solana-program v1.14.9
   Compiling spl-token v3.5.0
   Compiling bridge v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/Bridge)
    Finished release [optimized] target(s) in 33.28s
   Compiling memchr v2.5.0
   Compiling num-integer v0.1.45
   Compiling pin-project-lite v0.2.9
   Compiling futures-core v0.3.25
   Compiling lock_api v0.4.9
   Compiling fnv v1.0.7
   Compiling bytes v1.3.0
   Compiling smallvec v1.10.0
   Compiling percent-encoding v2.2.0
   Compiling slab v0.4.7
   Compiling futures-sink v0.3.25
   Compiling parking_lot_core v0.8.5
   Compiling instant v0.1.12
   Compiling regex-syntax v0.6.28
   Compiling tokio v1.14.1
   Compiling futures-channel v0.3.25
   Compiling futures-task v0.3.25
   Compiling tokio-macros v1.8.2
   Compiling signal-hook-registry v1.4.0
   Compiling mio v0.7.14
   Compiling futures-util v0.3.25
   Compiling ring v0.16.20
   Compiling futures-macro v0.3.25
   Compiling atty v0.2.14
   Compiling futures-io v0.3.25
   Compiling pin-utils v0.1.0
   Compiling parking_lot v0.11.2
   Compiling signature v1.6.4
   Compiling termcolor v1.1.3
   Compiling humantime v2.1.0
   Compiling ed25519 v1.5.2
   Compiling time v0.1.45
   Compiling tracing-core v0.1.30
   Compiling untrusted v0.7.1
   Compiling iana-time-zone v0.1.53
   Compiling spin v0.5.2
   Compiling aho-corasick v0.7.20
   Compiling ed25519-dalek v1.0.1
   Compiling hmac v0.12.1
   Compiling solana-sdk v1.14.9
   Compiling tracing-attributes v0.1.23
   Compiling chrono v0.4.23
   Compiling derivation-path v0.2.0
   Compiling qstring v0.7.2
   Compiling uriparse v0.6.4
   Compiling pbkdf2 v0.11.0
   Compiling assert_matches v1.5.0
   Compiling rustls v0.20.7
   Compiling ed25519-dalek-bip32 v0.2.0
   Compiling indexmap v1.9.2
   Compiling http v0.2.8
   Compiling httparse v1.8.0
   Compiling form_urlencoded v1.1.0
   Compiling socket2 v0.4.7
   Compiling unicode-bidi v0.3.8
   Compiling rustls-pemfile v1.0.1
   Compiling crc32fast v1.3.2
   Compiling regex v1.7.0
   Compiling idna v0.3.0
   Compiling alloc-no-stdlib v2.0.4
   Compiling try-lock v0.2.3
   Compiling adler v1.0.2
   Compiling alloc-stdlib v0.2.2
   Compiling want v0.3.0
   Compiling miniz_oxide v0.6.2
   Compiling brotli-decompressor v2.3.2
   Compiling http-body v0.4.5
   Compiling httpdate v1.0.2
   Compiling url v2.3.1
   Compiling tower-service v0.3.2
   Compiling encoding_rs v0.8.31
   Compiling serde_urlencoded v0.7.1
   Compiling env_logger v0.9.3
   Compiling flate2 v1.0.25
   Compiling ipnet v2.5.1
   Compiling mime v0.3.16
   Compiling solana-logger v1.14.9
   Compiling brotli v3.3.4
   Compiling solana-program-runtime v1.14.9
   Compiling enum-iterator-derive v0.8.1
   Compiling gethostname v0.2.3
   Compiling libloading v0.7.4
   Compiling eager v0.1.0
   Compiling rand_chacha v0.3.1
   Compiling cipher v0.3.0
   Compiling universal-hash v0.4.1
   Compiling solana-vote-program v1.14.9
   Compiling num-bigint v0.4.3
   Compiling proc-macro2 v0.4.30
   Compiling rand v0.8.5
   Compiling ctr v0.8.0
   Compiling aes v0.7.5
   Compiling tracing v0.1.37
   Compiling webpki v0.22.0
   Compiling sct v0.7.0
   Compiling webpki-roots v0.22.5
   Compiling polyval v0.5.3
   Compiling inout v0.1.3
   Compiling aead v0.4.3
   Compiling unicode-xid v0.1.0
   Compiling cipher v0.4.3
   Compiling aes-gcm-siv v0.10.3
   Compiling merlin v3.0.0
   Compiling sha3 v0.9.1
   Compiling time-core v0.1.0
   Compiling syn v0.15.44
   Compiling unicode-width v0.1.10
   Compiling time-macros v0.2.6
   Compiling zstd-sys v2.0.4+zstd.1.5.2
   Compiling fastrand v1.8.0
   Compiling remove_dir_all v0.5.3
   Compiling quote v0.6.13
   Compiling tempfile v3.3.0
   Compiling futures-executor v0.3.25
   Compiling tokio-util v0.7.2
   Compiling enum-iterator v0.8.1
   Compiling terminal_size v0.1.17
   Compiling async-trait v0.1.59
   Compiling minimal-lexical v0.2.1
   Compiling parking_lot_core v0.9.5
   Compiling console v0.15.2
   Compiling spl-memo v3.0.1
   Compiling nix v0.24.3
   Compiling nom v7.1.1
   Compiling solana-rayon-threadlimit v1.14.9
   Compiling h2 v0.3.15
   Compiling num-bigint v0.2.6
   Compiling solana-perf v1.14.9
   Compiling zstd-safe v5.0.2+zstd.1.5.2
   Compiling time v0.3.17
   Compiling Inflector v0.11.4
   Compiling tokio-rustls v0.23.4
   Compiling caps v0.5.5
   Compiling async-compression v0.3.15
   Compiling asn1-rs-derive v0.4.0
   Compiling pin-project-internal v1.0.12
   Compiling solana-address-lookup-table-program v1.14.9
   Compiling rusticata-macros v4.1.0
   Compiling displaydoc v0.2.3
   Compiling asn1-rs-impl v0.1.0
   Compiling num-complex v0.2.4
   Compiling proc-macro-error-attr v1.0.4
   Compiling num-iter v0.1.43
   Compiling num-rational v0.2.4
   Compiling static_assertions v1.1.0
   Compiling openssl-probe v0.1.5
   Compiling rustls-native-certs v0.6.2
   Compiling parking_lot v0.12.1
   Compiling dialoguer v0.10.2
   Compiling futures v0.3.25
   Compiling textwrap v0.11.0
   Compiling rustls-pemfile v0.2.1
   Compiling solana-version v1.14.9
   Compiling fxhash v0.2.1
   Compiling dlopen_derive v0.1.4
   Compiling proc-macro-error v1.0.4
   Compiling pkg-config v0.3.26
   Compiling strsim v0.8.0
   Compiling const-oid v0.7.1
   Compiling oid-registry v0.6.0
   Compiling linked-hash-map v0.5.6
   Compiling asn1-rs v0.5.1
   Compiling vec_map v0.8.2
   Compiling ansi_term v0.12.1
   Compiling yaml-rust v0.4.5
   Compiling pin-project v1.0.12
   Compiling clap v2.34.0
   Compiling der v0.5.1
   Compiling hyper v0.14.23
   Compiling quinn-proto v0.8.4
   Compiling dlopen v0.1.8
   Compiling bzip2-sys v0.1.11+1.0.8
   Compiling enum-ordinalize v3.1.12
   Compiling rpassword v6.0.1
   Compiling lz4-sys v1.9.4
   Compiling sharded-slab v0.1.4
   Compiling dirs-sys-next v0.1.2
   Compiling thread_local v1.1.4
   Compiling os_str_bytes v6.4.1
   Compiling base64ct v1.5.3
   Compiling spki v0.5.4
   Compiling clap_lex v0.2.4
   Compiling dirs-next v2.0.0
   Compiling num v0.2.1
   Compiling tracing-subscriber v0.3.16
   Compiling der-parser v8.1.0
   Compiling serde_yaml v0.8.26
   Compiling opentelemetry v0.17.0
   Compiling yasna v0.5.0
   Compiling sha-1 v0.10.1
   Compiling solana-measure v1.14.9
   Compiling solana-zk-token-sdk v1.14.9
   Compiling solana-remote-wallet v1.14.9
   Compiling educe v0.4.20
   Compiling pem v1.1.0
   Compiling modular-bitfield-impl v0.11.2
   Compiling solana-stake-program v1.14.9
   Compiling same-file v1.0.6
   Compiling textwrap v0.16.0
   Compiling quinn-udp v0.1.4
   Compiling heck v0.4.0
   Compiling strsim v0.10.0
   Compiling utf-8 v0.7.6
   Compiling data-encoding v2.3.2
   Compiling hyper-rustls v0.23.1
   Compiling strum_macros v0.24.3
   Compiling x509-parser v0.14.0
   Compiling clap v3.2.23
   Compiling reqwest v0.11.13
   Compiling tungstenite v0.17.3
   Compiling quinn v0.8.5
   Compiling tracing-opentelemetry v0.17.4
   Compiling walkdir v2.3.2
   Compiling rcgen v0.9.3
   Compiling tokio-serde v0.8.0
   Compiling ouroboros_macro v0.15.5
   Compiling percentage v0.1.0
   Compiling pkcs8 v0.8.0
   Compiling modular-bitfield v0.11.2
   Compiling tokio-util v0.6.10
   Compiling solana-metrics v1.14.9
   Compiling scroll_derive v0.11.0
   Compiling solana-runtime v1.14.9
   Compiling tarpc-plugins v0.12.0
   Compiling xattr v0.2.3
   Compiling filetime v0.2.18
   Compiling void v1.0.2
   Compiling event-listener v2.5.3
   Compiling aliasable v0.1.3
   Compiling number_prefix v0.4.0
   Compiling histogram v0.6.9
   Compiling solana-net-utils v1.14.9
   Compiling tar v0.4.38
   Compiling indicatif v0.16.2
   Compiling solana-config-program v1.14.9
   Compiling scroll v0.11.0
   Compiling strum v0.24.1
   Compiling solana-compute-budget-program v1.14.9
   Compiling async-mutex v1.4.0
   Compiling unreachable v1.0.0
   Compiling solana-bucket-map v1.14.9
   Compiling dir-diff v0.3.2
   Compiling tokio-tungstenite v0.17.2
   Compiling solana-clap-utils v1.14.9
   Compiling tarpc v0.29.0
   Compiling solana-streamer v1.14.9
   Compiling jsonrpc-core v18.0.0
   Compiling tokio-stream v0.1.11
   Compiling ouroboros v0.15.5
   Compiling dashmap v4.0.2
   Compiling enum_dispatch v0.3.8
   Compiling index_list v0.2.7
   Compiling ascii v0.9.3
   Compiling spl-token-2022 v0.4.3
   Compiling spl-token-2022 v0.5.0
   Compiling solana-cli-config v1.14.9
   Compiling solana-zk-token-proof-program v1.14.9
   Compiling solana-faucet v1.14.9
   Compiling plain v0.2.3
   Compiling symlink v0.1.0
   Compiling goblin v0.5.4
   Compiling combine v3.8.1
   Compiling hash32 v0.2.1
   Compiling rustc-demangle v0.1.21
   Compiling chrono-humanize v0.2.2
   Compiling bridge v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/Bridge)
   Compiling solana-banks-interface v1.14.9
   Compiling solana-banks-client v1.14.9
   Compiling bzip2 v0.4.3
   Compiling spl-associated-token-account v1.1.1
   Compiling solana_rbpf v0.2.31
   Compiling zstd v0.11.2+zstd.1.5.2
   Compiling solana-account-decoder v1.14.9
   Compiling lz4 v1.24.0
   Compiling solana-bpf-loader-program v1.14.9
   Compiling solana-transaction-status v1.14.9
   Compiling solana-client v1.14.9
   Compiling solana-send-transaction-service v1.14.9
   Compiling solana-banks-server v1.14.9
   Compiling solana-program-test v1.14.9
    Finished test [unoptimized + debuginfo] target(s) in 3m 40s
     Running unittests src/lib.rs (target/debug/deps/bridge-c2248e4fd865ac14)
     Running tests/lib.rs (target/debug/deps/lib-a8c4b10bfb69ea7d)
   Doc-tests bridge
   Compiling w_pokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPokt)
    Finished release [optimized] target(s) in 1.42s
   Compiling w_pokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPokt)
    Finished test [unoptimized + debuginfo] target(s) in 1.68s
     Running unittests src/lib.rs (target/debug/deps/w_pokt-f1f496e20af576a8)
   Doc-tests w_pokt
   Compiling wpokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPOKT)
    Finished release [optimized] target(s) in 1.33s
   Compiling wpokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPOKT)
    Finished test [unoptimized + debuginfo] target(s) in 1.83s
     Running unittests src/lib.rs (target/debug/deps/wpokt-03a817558112a24c)
   Doc-tests wpokt
cargo-test-sbf child: /home/gitpod/.local/share/solana/install/active_release/bin/cargo-build-sbf --manifest-path /workspace/CasperLabs-Solana-bridge/src/program/Bridge/Cargo.toml --sbf-out-dir /workspace/CasperLabs-Solana-bridge/target/deploy --arch bpf
cargo-test-sbf child: /home/gitpod/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/bin/cargo test --manifest-path /workspace/CasperLabs-Solana-bridge/src/program/Bridge/Cargo.toml --features test-bpf

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cargo-test-sbf child: /home/gitpod/.local/share/solana/install/active_release/bin/cargo-build-sbf --manifest-path /workspace/CasperLabs-Solana-bridge/src/program/WPokt/Cargo.toml --sbf-out-dir /workspace/CasperLabs-Solana-bridge/target/deploy --arch bpf
cargo-test-sbf child: /home/gitpod/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/bin/cargo test --manifest-path /workspace/CasperLabs-Solana-bridge/src/program/WPokt/Cargo.toml --features test-bpf

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cargo-test-sbf child: /home/gitpod/.local/share/solana/install/active_release/bin/cargo-build-sbf --manifest-path /workspace/CasperLabs-Solana-bridge/src/program/WPOKT/Cargo.toml --sbf-out-dir /workspace/CasperLabs-Solana-bridge/target/deploy --arch bpf
cargo-test-sbf child: /home/gitpod/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/bin/cargo test --manifest-path /workspace/CasperLabs-Solana-bridge/src/program/WPOKT/Cargo.toml --features test-bpf

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s



> casperlabs-solana-bridge@1.0.0 test-client
> start-server-and-test 'solana-test-validator --reset --quiet' http://localhost:8899/health start-client

1: starting server using command "solana-test-validator --reset --quiet"
and when url "[ 'http://localhost:8899/health' ]" is responding with HTTP status code 200
running tests using command "npm run start-client"


Notice! No wallet available. `solana airdrop` localnet SOL after creating one

Waiting for fees to stabilize 1...
Waiting for fees to stabilize 2...

> casperlabs-solana-bridge@1.0.0 start-client
> npm run start-client:bridge && npm run start-client:wpokt && npm run start-client:w_pokt


> casperlabs-solana-bridge@1.0.0 start-client:bridge
> npm run deploy:bridge && ts-node src/client/bridge.ts


> casperlabs-solana-bridge@1.0.0 deploy:bridge
> solana program deploy target/deploy/bridge.so

gitpod /workspace/CasperLabs-Solana-bridge (main) $

```


```
gitpod /workspace/CasperLabs-Solana-bridge (main) $ solana-keygen new -o /home/gitpod/.config/solana/id.json
Generating a new keypair

For added security, enter a BIP39 passphrase

NOTE! This passphrase improves security of the recovery seed phrase NOT the
keypair file itself, which is stored as insecure plain text

BIP39 Passphrase (empty for none): 

Wrote new keypair to /home/gitpod/.config/solana/id.json
============================================================================
pubkey: H61gTKGCggsMd8f8p8aRibpfHwqKmP7GuuiTbTMCp6Su
============================================================================
Save this seed phrase and your BIP39 passphrase to recover your new keypair:
assume patrol design hint river decrease cute index valve tongue chuckle eye
============================================================================
gitpod /workspace/CasperLabs-Solana-bridge (main) $
```

```
gitpod /workspace/CasperLabs-Solana-bridge (main) $ npm run start-client:wpokt

> casperlabs-solana-bridge@1.0.0 start-client:wpokt
> npm run deploy:wpokt && ts-node src/client/wpokt.ts


> casperlabs-solana-bridge@1.0.0 deploy:wpokt
> solana program deploy target/deploy/wpokt.so

Program Id: C2JNNw8wsGE97pcbpXKfmcwjTTHFxJQqpEXdJdyrih7z

Connection to cluster established: https://api.testnet.solana.com { 'feature-set': 3036606309, 'solana-core': '1.14.9' }
TSX - main(): Established Connection at https://api.testnet.solana.com
TSX - main(): Established Payer at H61gTKGCggsMd8f8p8aRibpfHwqKmP7GuuiTbTMCp6Su
TSX - wpoktTests(): wpokt deployed at C2JNNw8wsGE97pcbpXKfmcwjTTHFxJQqpEXdJdyrih7z...
TSX - wpoktTests(): wpokt Mint Account Created at 4iZUQCeNsjyLvftv1JFUTnUhvRULgxhjGBRrtYUEeFi7...
TSX - wpoktTests(): wpokt PDA Key Created at 8fwGjn9C4JQrCbMbivkErvDqvrwhbHb6AifoPBgprxzX...
TSX - wpoktTests(): wpokt Accounts Created and Verified...
TSX - wpoktTests(): wpokt Instruction::Construct...
TSX - wpoktTests(): wpokt Instruction::Construct Verified...
TSX - wpoktTests(): wpokt Instruction::MintOnlyMinter...
TSX - wpoktTests(): wpokt Instruction::MintOnlyMinter Verified...
TSX - wpoktTests(): wpokt newMinter account created at E4munxyuZycM2E2E6JseRXCfBsCsGrnk154rQRaKui4X...
TSX - wpoktTests(): wpokt Instruction::ChangeMinter...
TSX - wpoktTests(): wpokt Instruction::ChangeMinter Verified...
TSX - wpoktTests(): wpokt NoncesDictionary PDA generated at 6gV9vvwNkVa9R7DvKphLm82nLtd7kARhAAwKDQUwtb9b...
TSX - wpoktTests(): wpokt NoncesDictionary PDA Account Initialized. 6gV9vvwNkVa9R7DvKphLm82nLtd7kARhAAwKDQUwtb9b...
TSX - wpoktTests(): wpokt NoncesDictionary PDA Account Initialization Verified. 6gV9vvwNkVa9R7DvKphLm82nLtd7kARhAAwKDQUwtb9b...
TSX - wpoktTests(): wpokt Delegate Token Account created. 8x5ckwXkKLwaFGSwjgDvwmAXHWHipCMJvrpWn3yktywQ...
TSX - wpoktTests(): wpokt WPOKTInstruction::Permit...
TSX - wpoktTests(): wpokt WPOKTInstruction::Permit Verified...
TSX - wpoktTests(): wpokt WPOKTInstruction::InitializeAuthorizationStatePdaAccount...
TSX - wpoktTests(): wpokt WPOKTInstruction::InitializeAuthorizationStatePdaAccount Verified...
Server responded with 429 Too Many Requests.  Retrying after 500ms delay...
TSX - wpoktTests(): wpokt WPOKTInstruction::TransferWithAuthorization...
Server responded with 429 Too Many Requests.  Retrying after 500ms delay...
Server responded with 429 Too Many Requests.  Retrying after 500ms delay...
Server responded with 429 Too Many Requests.  Retrying after 1000ms delay...
TSX - main(): Finished...
gitpod /workspace/CasperLabs-Solana-bridge (main) $
```

```
gitpod /workspace/CasperLabs-Solana-bridge (main) $ npm run test-client:wpokt

> casperlabs-solana-bridge@1.0.0 test-client:wpokt
> start-server-and-test 'solana-test-validator --reset --quiet' http://localhost:8899/health start-client:wpokt

1: starting server using command "solana-test-validator --reset --quiet"
and when url "[ 'http://localhost:8899/health' ]" is responding with HTTP status code 200
running tests using command "npm run start-client:wpokt"

Waiting for fees to stabilize 1...
Waiting for fees to stabilize 2...

> casperlabs-solana-bridge@1.0.0 start-client:wpokt
> npm run deploy:wpokt && ts-node src/client/wpokt.ts


> casperlabs-solana-bridge@1.0.0 deploy:wpokt
> solana program deploy target/deploy/wpokt.so

Program Id: C2JNNw8wsGE97pcbpXKfmcwjTTHFxJQqpEXdJdyrih7z

Connection to cluster established: https://api.testnet.solana.com { 'feature-set': 3036606309, 'solana-core': '1.14.9' }
TSX - main(): Established Connection at https://api.testnet.solana.com
TSX - main(): Established Payer at H61gTKGCggsMd8f8p8aRibpfHwqKmP7GuuiTbTMCp6Su
TSX - wpoktTests(): wpokt deployed at C2JNNw8wsGE97pcbpXKfmcwjTTHFxJQqpEXdJdyrih7z...
TSX - wpoktTests(): wpokt Mint Account Created at 82WcK6KbrMFo1pM5qvdSLeNJEvDpoTkYKQkp1aWv7UX3...
TSX - wpoktTests(): wpokt PDA Key Created at AmcV5fcuhbnacBmQtbSwFvskw1Msx9izaQiK38zacV99...
TSX - wpoktTests(): wpokt Accounts Created and Verified...
TSX - wpoktTests(): wpokt Instruction::Construct...
TSX - wpoktTests(): wpokt Instruction::Construct Verified...
TSX - wpoktTests(): wpokt Instruction::MintOnlyMinter...
TSX - wpoktTests(): wpokt Instruction::MintOnlyMinter Verified...
TSX - wpoktTests(): wpokt newMinter account created at EYbRRGYbQ13zia94bBfpVCoJygDt4ei2GZScD36xEyYf...
TSX - wpoktTests(): wpokt Instruction::ChangeMinter...
TSX - wpoktTests(): wpokt Instruction::ChangeMinter Verified...
TSX - wpoktTests(): wpokt NoncesDictionary PDA generated at ChaUkQtqjfiPbhr4ETKVwuihQ7k5BKfHw5pCaBZqAARo...
TSX - wpoktTests(): wpokt NoncesDictionary PDA Account Initialized. ChaUkQtqjfiPbhr4ETKVwuihQ7k5BKfHw5pCaBZqAARo...
TSX - wpoktTests(): wpokt NoncesDictionary PDA Account Initialization Verified. ChaUkQtqjfiPbhr4ETKVwuihQ7k5BKfHw5pCaBZqAARo...
TSX - wpoktTests(): wpokt Delegate Token Account created. FmRZTMNQAAQdNRtZ3oFQCweDBa7JJo82DY4byiZ87qVP...
TSX - wpoktTests(): wpokt WPOKTInstruction::Permit...
TSX - wpoktTests(): wpokt WPOKTInstruction::Permit Verified...
TSX - wpoktTests(): wpokt WPOKTInstruction::InitializeAuthorizationStatePdaAccount...
TSX - wpoktTests(): wpokt WPOKTInstruction::InitializeAuthorizationStatePdaAccount Verified...
TSX - wpoktTests(): wpokt WPOKTInstruction::TransferWithAuthorization...
TSX - main(): Finished...
gitpod /workspace/CasperLabs-Solana-bridge (main) $
```
