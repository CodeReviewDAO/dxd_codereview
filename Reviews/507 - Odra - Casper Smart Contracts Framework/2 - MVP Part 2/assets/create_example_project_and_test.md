'''
muharremsalel@Muharrems-MacBook-Pro CRDao % cargo odra new --name myproject && cd myproject
⚠️   Favorite `odradev/odra-template` not found in config, using it as a git repository: https://github.com/odradev/odra-template.git
date => '2022-09-25'
🔧   Basedir: /Users/muharremsalel/Desktop/CRDao ...
🔧   Generating template ...
[1/8]   Done: .gitignore
[2/8]   Done: CHANGELOG.md
[3/8]   Done: Cargo.toml
[4/8]   Done: Odra.toml
[5/8]   Done: README.md
[6/8]   Done: src/flipper.rs
[7/8]   Done: src/lib.rs
[8/8]   Done: src
🔧   Moving generated files into: `/Users/muharremsalel/Desktop/CRDao/myproject`...
💡   Initializing a fresh Git repository
✨   Done! New project created /Users/muharremsalel/Desktop/CRDao/myproject
muharremsalel@Muharrems-MacBook-Pro myproject % cargo odra test
💁  INFO : Running cargo test...
    Updating crates.io index
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.44
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.4
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
   Compiling ppv-lite86 v0.2.16
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling cfg-if v1.0.0
   Compiling opaque-debug v0.3.0
   Compiling serde_json v1.0.85
   Compiling cpufeatures v0.2.5
   Compiling ryu v1.0.11
   Compiling rand_core v0.6.4
   Compiling hex v0.4.3
   Compiling static_assertions v1.1.0
   Compiling itoa v1.0.3
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.0
   Compiling bitflags v1.3.2
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
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling itertools v0.10.5
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
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling serde_bytes v0.11.7
   Compiling casper-types v1.5.0
   Compiling odra-types v0.1.0
   Compiling odra-utils v0.1.0
   Compiling odra-codegen v0.1.0
   Compiling odra-mock-vm v0.1.0
   Compiling odra-proc-macros v0.1.0
   Compiling odra v0.1.0
   Compiling myproject v0.1.0 (/Users/muharremsalel/Desktop/CRDao/myproject)
warning: unused doc comment
  --> src/flipper.rs:49:9
   |
49 | /         /// To test a module we need to deploy it. 
50 | |         /// To do so, Odra generates for us deploy() function.
51 | |         /// To call a constructor we don't do it directly. In this case to call
52 | |         /// a constructor, we would call deploy_initial_settings() function.
   | |____________________________________________________________________________^
53 |           let contract = Flipper::deploy();
   |           --------------------------------- rustdoc does not generate documentation for statements
   |
   = note: `#[warn(unused_doc_comments)]` on by default
   = help: use `//` for a plain comment

warning: associated function `deploy_initial_settings` is never used
  --> src/flipper.rs:22:12
   |
22 |     pub fn initial_settings(&self) {
   |            ^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: `myproject` (lib test) generated 2 warnings
    Finished test [unoptimized + debuginfo] target(s) in 28.84s
     Running unittests src/lib.rs (target/debug/deps/myproject-e16e6a7c2bd89247)

running 2 tests
test flipper::tests::flipping ... ok
test flipper::tests::test_two_flippers ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests myproject

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

'''