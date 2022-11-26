(base) mdidin@Muhammed-MacBook-Air CasperLabs-ERC777 % make test
cargo build --release --target wasm32-unknown-unknown  -p erc777-token  -p erc1820-registry  -p erc777-recipient-contract  -p erc777-sender-contract
    Finished release [optimized] target(s) in 0.10s
wasm-strip target/wasm32-unknown-unknown/release/erc777_token.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc1820_registry.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc777_recipient_contract.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc777_sender_contract.wasm 2>/dev/null | true;
cargo test
   Compiling cfg-if v1.0.0
   Compiling cfg-if v0.1.10
   Compiling subtle v2.4.1
   Compiling ppv-lite86 v0.2.10
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling byteorder v1.4.3
   Compiling regex-syntax v0.6.25
   Compiling remove_dir_all v0.5.3
   Compiling tinyvec_macros v0.1.0
   Compiling lazy_static v1.4.0
   Compiling opaque-debug v0.3.0
   Compiling fnv v1.0.7
   Compiling itoa v0.4.5
   Compiling quick-error v1.2.3
   Compiling hashbrown v0.11.2
   Compiling bit-vec v0.6.3
   Compiling matches v0.1.9
   Compiling cpufeatures v0.2.1
   Compiling dyn-clone v1.0.4
   Compiling quick-error v2.0.1
   Compiling percent-encoding v2.1.0
   Compiling unicode-bidi v0.3.6
   Compiling static_assertions v1.1.0
   Compiling base64 v0.13.0
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling once_cell v1.8.0
   Compiling memory_units v0.4.0
   Compiling semver-parser v0.9.0
   Compiling parity-wasm v0.41.0
   Compiling either v1.6.1
   Compiling downcast-rs v1.2.0
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling pin-project-lite v0.2.7
   Compiling linked-hash-map v0.5.4
   Compiling tinyvec v1.3.1
   Compiling tracing-core v0.1.19
   Compiling bit-set v0.5.2
   Compiling form_urlencoded v1.0.1
   Compiling bitvec v0.18.5
   Compiling itertools v0.10.1
   Compiling libc v0.2.101
   Compiling typenum v1.14.0
   Compiling bitflags v1.2.1
   Compiling ryu v1.0.3
   Compiling crunchy v0.2.2
   Compiling memchr v2.4.1
   Compiling anyhow v1.0.43
   Compiling getrandom v0.1.14
   Compiling getrandom v0.2.3
   Compiling wait-timeout v0.2.0
   Compiling wee_alloc v0.4.5
   Compiling time v0.1.43
   Compiling hostname v0.3.1
   Compiling num-traits v0.2.14
   Compiling unicase v2.6.0
   Compiling unicode-normalization v0.1.19
   Compiling lmdb-sys v0.8.0
   Compiling generic-array v0.14.4
   Compiling wasmi-validation v0.3.0
   Compiling rand_core v0.5.1
   Compiling rand_core v0.6.3
   Compiling regex v1.5.4
   Compiling pulldown-cmark v0.8.0
   Compiling lmdb v0.8.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling num-integer v0.1.44
   Compiling num-complex v0.4.0
   Compiling idna v0.2.3
   Compiling serde v1.0.105
   Compiling datasize v0.2.9
   Compiling thiserror v1.0.29
   Compiling value-bag v1.0.0-alpha.7
   Compiling tracing v0.1.26
   Compiling group v0.8.0
   Compiling rand v0.7.3
   Compiling rand v0.8.4
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.8
   Compiling blake2 v0.9.2
   Compiling num-bigint v0.4.2
   Compiling num-bigint v0.2.6
   Compiling num-iter v0.1.42
   Compiling chrono v0.4.19
   Compiling zeroize v1.4.1
   Compiling url v2.2.2
   Compiling tempfile v3.2.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.0
   Compiling rusty-fork v0.3.0
   Compiling ecdsa v0.10.2
   Compiling proptest v1.0.0
   Compiling num-rational v0.2.4
   Compiling k256 v0.7.3
   Compiling wasmi v0.8.0
   Compiling hex v0.4.3
   Compiling serde_json v1.0.67
   Compiling ed25519 v1.2.0
   Compiling indexmap v1.7.0
   Compiling num-rational v0.4.0
   Compiling serde_bytes v0.11.5
   Compiling toml v0.5.8
   Compiling log v0.4.14
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling ed25519-dalek v1.0.1
   Compiling uint v0.9.1
   Compiling hex-buffer-serde v0.2.2
   Compiling num v0.4.0
   Compiling pwasm-utils v0.16.0
   Compiling schemars v0.8.3
   Compiling version-sync v0.9.2
   Compiling casper-types v1.3.2
   Compiling casper-contract v1.3.2
   Compiling casper-execution-engine v1.3.2
   Compiling casper-erc1820 v0.1.0 (/Users/mdidin/Desktop/CasperLabs-ERC777/erc1820)
   Compiling casper-erc777 v0.2.1 (/Users/mdidin/Desktop/CasperLabs-ERC777/erc777)
   Compiling casper-erc777-sender v0.1.0 (/Users/mdidin/Desktop/CasperLabs-ERC777/erc777-sender)
   Compiling casper-erc777-recipient v0.1.0 (/Users/mdidin/Desktop/CasperLabs-ERC777/erc777-recipient)
   Compiling casper-engine-test-support v1.3.2
   Compiling erc777-sender-tests v0.0.1 (/Users/mdidin/Desktop/CasperLabs-ERC777/example/tests/erc777-sender-tests)
   Compiling erc20-tests v0.0.1 (/Users/mdidin/Desktop/CasperLabs-ERC777/example/tests/erc20-tests)
   Compiling erc777-tests v0.0.1 (/Users/mdidin/Desktop/CasperLabs-ERC777/example/tests/erc777-tests)
   Compiling erc1820-tests v0.1.0 (/Users/mdidin/Desktop/CasperLabs-ERC777/example/tests/erc1820-tests)
   Compiling erc777-recipient-tests v0.0.1 (/Users/mdidin/Desktop/CasperLabs-ERC777/example/tests/erc777-recipient-tests)
    Finished test [unoptimized + debuginfo] target(s) in 59.95s
     Running unittests src/lib.rs (target/debug/deps/casper_erc1820-ede179038e33af18)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/casper_erc777-64a79988674ce842)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/casper_erc777_recipient-c17d199f293c21de)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/casper_erc777_sender-926acfbe1dec1c46)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/integration_tests.rs (target/debug/deps/erc1820_tests-8312d925de82584d)

running 7 tests
test tests::should_not_register_an_implementer_with_address_zero - should panic ... ok
test tests::should_set_manager ... ok
test tests::should_not_set_manager - should panic ... ok
test tests::should_not_register_an_implementer - should panic ... ok
test tests::should_not_register_an_implementer_with_same_caller_address - should panic ... ok
test tests::should_register_a_sender ... ok
test tests::should_register_a_recipient ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.59s

     Running unittests src/integration_tests.rs (target/debug/deps/erc20_tests-e1504fc63c489369)

running 6 tests
test tests::should_install ... ok
test tests::should_not_transfer_with_insufficient_balance - should panic ... ok
test tests::should_transfer_full_amount ... ok
test tests::should_transfer ... ok
test tests::should_not_transfer_from_more_than_approved - should panic ... ok
test tests::should_transfer_from ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.16s

     Running unittests src/integration_tests.rs (target/debug/deps/erc777_recipient_tests-fb38a0d688892d62)

running 9 tests
test tests::should_install ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_send_tokens - should panic ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_burn_tokens - should panic ... ok
test tests::should_send_on_behalf_of ... ok
test tests::should_send_and_burn ... ok
test tests::should_burn_from_erc777_recipient ... ok
test tests::should_burn_on_behalf_of ... ok
test tests::should_transfer_tokens_by_using_other_owner ... ok
test tests::should_transfer_tokens_from_erc777_recipient ... ok

test result: ok. 9 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 4.27s

     Running unittests src/integration_tests.rs (target/debug/deps/erc777_sender_tests-a513c85d1330b297)

running 8 tests
test tests::should_install ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_burn_tokens - should panic ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_send_tokens - should panic ... ok
test tests::should_send_on_behalf_of ... ok
test tests::should_transfer_tokens_from_erc777_sender ... ok
test tests::should_send_and_burn ... ok
test tests::should_burn_on_behalf_of ... ok
test tests::should_burn_from_erc777_sender ... ok

test result: ok. 8 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.48s

     Running unittests src/integration_tests.rs (target/debug/deps/erc777_tests-bba7b666aad0d711)

running 6 tests
test tests::should_install ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_burn_tokens - should panic ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_send_tokens - should panic ... ok
test tests::should_send_on_behalf_of ... ok
test tests::should_send_and_burn ... ok
test tests::should_burn_on_behalf_of ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.92s

   Doc-tests casper-erc1820

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests casper-erc777

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests casper-erc777-recipient

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests casper-erc777-sender

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s