'''
💁  INFO : Running cargo test...
    Updating crates.io index
  Downloaded block-buffer v0.9.0
  Downloaded zeroize v1.3.0
  Downloaded unicode-xid v0.2.4
  Downloaded zeroize_derive v1.3.2
  Downloaded crunchy v0.2.2
  Downloaded byteorder v1.4.3
  Downloaded num v0.4.0
  Downloaded num-derive v0.3.3
  Downloaded opaque-debug v0.3.0
  Downloaded derive_more v0.99.17
  Downloaded num-bigint v0.4.3
  Downloaded num-complex v0.4.2
  Downloaded ppv-lite86 v0.2.16
  Downloaded rand v0.7.3
  Downloaded rand_chacha v0.2.2
  Downloaded rand v0.8.5
  Downloaded sha2 v0.9.9
  Downloaded serde_bytes v0.11.7
  Downloaded rand_core v0.6.4
  Downloaded synstructure v0.12.6
  Downloaded curve25519-dalek v3.2.1
  Downloaded wyz v0.2.0
  Downloaded casper-types v1.5.0
  Downloaded hex_fmt v0.3.0
  Downloaded odra-mock-vm v0.1.0
  Downloaded signature v1.2.2
  Downloaded odra-types v0.1.0
  Downloaded ff v0.8.0
  Downloaded group v0.8.0
  Downloaded k256 v0.7.3
  Downloaded hmac v0.10.1
  Downloaded crypto-mac v0.10.1
  Downloaded ed25519 v1.2.0
  Downloaded elliptic-curve v0.8.5
  Downloaded uint v0.9.4
  Downloaded digest v0.9.0
  Downloaded funty v1.1.0
  Downloaded crypto-mac v0.8.0
  Downloaded ed25519-dalek v1.0.1
  Downloaded rand_core v0.5.1
  Downloaded subtle v2.4.1
  Downloaded odra-codegen v0.1.0
  Downloaded base16 v0.2.1
  Downloaded blake2 v0.9.2
  Downloaded odra-proc-macros v0.1.0
  Downloaded odra-utils v0.1.0
  Downloaded odra-ir v0.1.0
  Downloaded num-rational v0.4.1
  Downloaded num-iter v0.1.43
  Downloaded odra v0.1.0
  Downloaded radium v0.3.0
  Downloaded ref_thread_local v0.1.1
  Downloaded ecdsa v0.10.2
  Downloaded bitvec v0.18.5
  Downloaded base64 v0.13.0
  Downloaded 55 crates (1.9 MB) in 2.06s
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.44
   Compiling unicode-ident v1.0.4
   Compiling quote v1.0.21
   Compiling syn v1.0.100
   Compiling typenum v1.15.0
   Compiling autocfg v1.1.0
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling serde_derive v1.0.145
   Compiling serde v1.0.145
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling ppv-lite86 v0.2.16
   Compiling cfg-if v1.0.0
   Compiling crunchy v0.2.2
   Compiling cpufeatures v0.2.5
   Compiling serde_json v1.0.85
   Compiling ryu v1.0.11
   Compiling hex v0.4.3
   Compiling itoa v1.0.3
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling bitflags v1.3.2
   Compiling base64 v0.13.0
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling convert_case v0.5.0
   Compiling either v1.8.0
   Compiling ref_thread_local v0.1.1
   Compiling rand v0.8.5
   Compiling generic-array v0.14.6
   Compiling proc-macro-error-attr v1.0.4
   Compiling proc-macro-error v1.0.4
   Compiling rand_chacha v0.2.2
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling bitvec v0.18.5
   Compiling itertools v0.10.5
   Compiling rand v0.7.3
   Compiling uint v0.9.4
   Compiling ff v0.8.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling group v0.8.0
   Compiling signature v1.2.2
   Compiling blake2 v0.9.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling synstructure v0.12.6
   Compiling num v0.4.0
   Compiling odra-ir v0.1.0
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling derive_more v0.99.17
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling odra-types v0.1.0
   Compiling odra-utils v0.1.0
   Compiling odra-codegen v0.1.0
   Compiling odra-mock-vm v0.1.0
   Compiling odra-proc-macros v0.1.0
   Compiling odra v0.1.0
   Compiling odra-examples v0.0.1 (/Users/muharremsalel/Desktop/CRDao/odra-examples)
    Finished test [unoptimized + debuginfo] target(s) in 36.19s
     Running unittests src/lib.rs (target/debug/deps/odra_examples-cc43d271f38c9a9a)

running 14 tests
test ownable::tests::initialization_works ... ok
test ownable::tests::owner_can_change_ownership ... ok
test ownable::tests::non_owner_cannot_change_ownership ... ok
test erc20::tests::transfer_from_error ... ok
test erc20::tests::transfer_error ... ok
test balance_checker::tests::balance_checker ... ok
test erc20::tests::initialization ... ok
test owned_token::tests::change_ownership_works ... ok
test owned_token::tests::mint_error ... ok
test owned_token::tests::change_ownership_error ... ok
test erc20::tests::transfer_works ... ok
test owned_token::tests::mint_works ... ok
test owned_token::tests::init_works ... ok
test erc20::tests::transfer_from_and_approval_work ... ok

test result: ok. 14 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-examples

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

'''