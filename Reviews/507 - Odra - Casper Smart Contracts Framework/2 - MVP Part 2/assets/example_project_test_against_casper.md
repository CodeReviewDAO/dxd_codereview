'''
muharremsalel@Muharrems-MacBook-Pro myproject % cargo odra test -b casper-latest
💁  INFO : Preparing casper-latest builder in .builder_casper-latest/ directory...
💁  INFO : Generating _wasm.rs files...
    Updating crates.io index
  Downloaded pretty_assertions v1.3.0
  Downloaded yansi v0.5.1
  Downloaded odra-casper-shared v0.1.0
  Downloaded diff v0.1.13
  Downloaded odra-casper-backend v0.1.0
  Downloaded casper-contract v1.4.4
  Downloaded 6 crates (176.7 KB) in 2.02s
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
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling serde_derive v1.0.145
   Compiling serde v1.0.145
   Compiling ppv-lite86 v0.2.16
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling cfg-if v1.0.0
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.85
   Compiling cpufeatures v0.2.5
   Compiling ryu v1.0.11
   Compiling itoa v1.0.3
   Compiling hex v0.4.3
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.0
   Compiling bitflags v1.3.2
   Compiling hex_fmt v0.3.0
   Compiling either v1.8.0
   Compiling convert_case v0.5.0
   Compiling ref_thread_local v0.1.1
   Compiling yansi v0.5.1
   Compiling diff v0.1.13
   Compiling lazy_static v1.4.0
   Compiling rand_chacha v0.2.2
   Compiling generic-array v0.14.6
   Compiling proc-macro-error-attr v1.0.4
   Compiling proc-macro-error v1.0.4
   Compiling rand v0.8.5
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling bitvec v0.18.5
   Compiling itertools v0.10.5
   Compiling pretty_assertions v1.3.0
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
   Compiling odra-ir v0.1.0
   Compiling num v0.4.0
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
   Compiling casper-contract v1.4.4
   Compiling odra-utils v0.1.0
   Compiling odra-casper-shared v0.1.0
   Compiling odra-codegen v0.1.0
   Compiling odra-proc-macros v0.1.0
   Compiling odra v0.1.0
   Compiling myproject v0.1.0 (/Users/muharremsalel/Desktop/CRDao/myproject)
   Compiling odra-casper-backend v0.1.0
   Compiling builder v1.0.0 (/Users/muharremsalel/Desktop/CRDao/myproject/.builder_casper-latest)
    Finished dev [unoptimized + debuginfo] target(s) in 31.69s
     Running `target/debug/flipper_build`
💁  INFO : Generating wasm files...
   Compiling version_check v0.9.4
   Compiling typenum v1.15.0
   Compiling proc-macro2 v1.0.44
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.4
   Compiling autocfg v1.1.0
   Compiling syn v1.0.100
   Compiling unicode-xid v0.2.4
   Compiling serde v1.0.145
   Compiling serde_derive v1.0.145
   Compiling crunchy v0.2.2
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling serde_json v1.0.85
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling ppv-lite86 v0.2.16
   Compiling cfg-if v1.0.0
   Compiling byteorder v1.4.3
   Compiling opaque-debug v0.3.0
   Compiling cpufeatures v0.2.5
   Compiling static_assertions v1.1.0
   Compiling hex v0.4.3
   Compiling ryu v1.0.11
   Compiling itoa v1.0.3
   Compiling rand_core v0.6.4
   Compiling hex_fmt v0.3.0
   Compiling bitflags v1.3.2
   Compiling base64 v0.13.0
   Compiling base16 v0.2.1
   Compiling either v1.8.0
   Compiling convert_case v0.5.0
   Compiling ref_thread_local v0.1.1
   Compiling yansi v0.5.1
   Compiling diff v0.1.13
   Compiling lazy_static v1.4.0
   Compiling generic-array v0.14.6
   Compiling proc-macro-error-attr v1.0.4
   Compiling proc-macro-error v1.0.4
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling rand v0.8.5
   Compiling rand_chacha v0.2.2
   Compiling itertools v0.10.5
   Compiling bitvec v0.18.5
   Compiling pretty_assertions v1.3.0
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
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
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
   Compiling casper-contract v1.4.4
   Compiling odra-utils v0.1.0
   Compiling odra-casper-shared v0.1.0
   Compiling odra-codegen v0.1.0
   Compiling odra-proc-macros v0.1.0
   Compiling odra v0.1.0
   Compiling myproject v0.1.0 (/Users/muharremsalel/Desktop/CRDao/myproject)
   Compiling odra-casper-backend v0.1.0
   Compiling builder v1.0.0 (/Users/muharremsalel/Desktop/CRDao/myproject/.builder_casper-latest)
    Finished release [optimized] target(s) in 36.73s
💁  INFO : Copying wasm files...
💁  INFO : Saving wasm/flipper.wasm
⚠️  WARN : There was an error while running wasmstrip - is it installed? Continuing anyway...
💁  INFO : Building backend library...
  Downloaded ctor v0.1.23
  Downloaded quick-error v1.2.3
  Downloaded value-bag v1.0.0-alpha.9
  Downloaded rusty-fork v0.3.0
  Downloaded bit-set v0.5.3
  Downloaded bit-vec v0.6.3
  Downloaded match_cfg v0.1.0
  Downloaded downcast-rs v1.2.0
  Downloaded hostname v0.3.1
  Downloaded hex-buffer-serde v0.3.0
  Downloaded proptest v1.0.0
  Downloaded uuid v0.8.2
  Downloaded lmdb-sys v0.8.0
  Downloaded rand_xorshift v0.3.0
  Downloaded odra-casper-test-env v0.1.0
  Downloaded filesize v0.2.0
  Downloaded wait-timeout v0.2.0
  Downloaded datasize v0.2.10
  Downloaded serde_derive_internals v0.25.0
  Downloaded odra-test-env-wrapper v0.1.0
  Downloaded memory_units v0.3.0
  Downloaded dyn-clone v1.0.9
  Downloaded rand_chacha v0.3.1
  Downloaded bincode v1.3.3
  Downloaded tracing-core v0.1.29
  Downloaded tracing-attributes v0.1.22
  Downloaded syn v0.15.44
  Downloaded num-bigint v0.2.6
  Downloaded unicode-xid v0.1.0
  Downloaded tracing v0.1.36
  Downloaded dlopen v0.1.8
  Downloaded pin-project-lite v0.2.9
  Downloaded parity-wasm v0.41.0
  Downloaded wasmi-validation v0.3.0
  Downloaded casper-hashing v1.4.3
  Downloaded hex-buffer-serde v0.2.2
  Downloaded schemars_derive v0.8.5
  Downloaded lmdb v0.8.0
  Downloaded schemars v0.8.5
  Downloaded pwasm-utils v0.16.0
  Downloaded wasmi v0.8.0
  Downloaded dlopen_derive v0.1.4
  Downloaded proc-macro2 v0.4.30
  Downloaded num-rational v0.2.4
  Downloaded quote v0.6.13
  Downloaded num_cpus v1.13.1
  Downloaded linked-hash-map v0.5.6
  Downloaded casper-execution-engine v2.0.1
  Downloaded datasize_derive v0.2.10
  Downloaded casper-engine-test-support v2.2.0
  Downloaded 50 crates (1.9 MB) in 1.88s
warning: The package `odra_test_env` provides no linkable target. The compiler might raise an error while compiling `builder`. Consider adding 'dylib' or 'rlib' to key `crate-type` in `odra_test_env`'s Cargo.toml. This warning might turn into a hard error in the future.
   Compiling syn v1.0.100
   Compiling libc v0.2.133
   Compiling serde v1.0.145
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling ppv-lite86 v0.2.16
   Compiling funty v1.1.0
   Compiling byteorder v1.4.3
   Compiling fastrand v1.8.0
   Compiling serde_json v1.0.85
   Compiling remove_dir_all v0.5.3
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling bit-vec v0.6.3
   Compiling lazy_static v1.4.0
   Compiling schemars v0.8.5
   Compiling itoa v1.0.3
   Compiling hashbrown v0.12.3
   Compiling cpufeatures v0.2.5
   Compiling bitflags v1.3.2
   Compiling ryu v1.0.11
   Compiling quick-error v1.2.3
   Compiling once_cell v1.15.0
   Compiling fnv v1.0.7
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.9
   Compiling static_assertions v1.1.0
   Compiling regex-syntax v0.6.27
   Compiling base64 v0.13.0
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling proc-macro2 v0.4.30
   Compiling unicode-xid v0.1.0
   Compiling cc v1.0.73
   Compiling core-foundation-sys v0.8.3
   Compiling syn v0.15.44
   Compiling pkg-config v0.3.25
   Compiling parity-wasm v0.41.0
   Compiling log v0.4.17
   Compiling thiserror v1.0.36
   Compiling anyhow v1.0.65
   Compiling either v1.8.0
   Compiling downcast-rs v1.2.0
   Compiling memory_units v0.3.0
   Compiling match_cfg v0.1.0
   Compiling pin-project-lite v0.2.9
   Compiling convert_case v0.5.0
   Compiling linked-hash-map v0.5.6
   Compiling ref_thread_local v0.1.1
   Compiling filesize v0.2.0
   Compiling typenum v1.15.0
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling indexmap v1.9.1
   Compiling value-bag v1.0.0-alpha.9
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling bit-set v0.5.3
   Compiling tracing-core v0.1.29
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling itertools v0.10.5
   Compiling generic-array v0.14.6
   Compiling num-iter v0.1.43
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling lmdb-sys v0.8.0
   Compiling ff v0.8.0
   Compiling iana-time-zone v0.1.50
   Compiling getrandom v0.2.7
   Compiling tempfile v3.3.0
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.44
   Compiling num_cpus v1.13.1
   Compiling hostname v0.3.1
   Compiling group v0.8.0
   Compiling quote v0.6.13
   Compiling rand_core v0.6.4
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling rusty-fork v0.3.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling rand v0.8.5
   Compiling num-complex v0.4.2
   Compiling proptest v1.0.0
   Compiling chrono v0.4.22
   Compiling lmdb v0.8.0
   Compiling dlopen_derive v0.1.4
   Compiling dlopen v0.1.8
   Compiling wasmi v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling proc-macro-error v1.0.4
   Compiling odra-ir v0.1.0
   Compiling serde_derive v1.0.145
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling datasize_derive v0.2.10
   Compiling schemars_derive v0.8.5
   Compiling ctor v0.1.23
   Compiling thiserror-impl v1.0.36
   Compiling tracing-attributes v0.1.22
   Compiling derive_more v0.99.17
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling tracing v0.1.36
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling hex v0.4.3
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.4
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling odra-types v0.1.0
   Compiling odra-utils v0.1.0
   Compiling odra-codegen v0.1.0
   Compiling casper-hashing v1.4.3
   Compiling odra-test-env-wrapper v0.1.0
   Compiling odra-casper-shared v0.1.0
   Compiling casper-execution-engine v2.0.1
   Compiling odra-proc-macros v0.1.0
   Compiling odra v0.1.0
   Compiling casper-engine-test-support v2.2.0
   Compiling odra-casper-test-env v0.1.0
   Compiling builder v1.0.0 (/Users/muharremsalel/Desktop/CRDao/myproject/.builder_casper-latest)
    Finished release [optimized] target(s) in 1m 49s
     Running `target/release/builder`
💁  INFO : Running cargo test...
   Compiling proc-macro2 v0.4.30
   Compiling unicode-xid v0.1.0
   Compiling libc v0.2.133
   Compiling syn v0.15.44
   Compiling lazy_static v1.4.0
   Compiling quote v0.6.13
   Compiling dlopen_derive v0.1.4
   Compiling dlopen v0.1.8
   Compiling odra-test-env-wrapper v0.1.0
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
    Finished test [unoptimized + debuginfo] target(s) in 6.64s
     Running unittests src/lib.rs (target/debug/deps/myproject-4ada4ef4b4eba093)

running 2 tests
test flipper::tests::flipping ... ok
test flipper::tests::test_two_flippers ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.36s

   Doc-tests myproject

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

'''