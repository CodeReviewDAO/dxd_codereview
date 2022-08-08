```sh
@ggurbet ➜ /workspaces/dao-contracts (7c24f46 ✗) $ make docs
cargo doc --features test-support --workspace --exclude sample-contract --lib --no-deps --open
   Compiling proc-macro2 v1.0.36
   Compiling syn v1.0.86
   Compiling unicode-xid v0.2.2
   Compiling autocfg v1.0.1
   Compiling version_check v0.9.4
   Compiling libc v0.2.113
   Compiling serde_derive v1.0.134
   Compiling typenum v1.15.0
   Compiling serde v1.0.134
    Checking cfg-if v1.0.0
    Checking rand_core v0.5.1
    Checking subtle v2.4.1
    Checking ppv-lite86 v0.2.16
    Checking radium v0.3.0
    Checking wyz v0.2.0
    Checking funty v1.1.0
    Checking byteorder v1.4.3
    Checking fastrand v1.7.0
   Compiling serde_json v1.0.76
    Checking remove_dir_all v0.5.3
    Checking lazy_static v1.4.0
   Compiling crunchy v0.2.2
    Checking opaque-debug v0.3.0
    Checking bit-vec v0.6.3
    Checking itoa v1.0.1
   Compiling schemars v0.8.5
    Checking fnv v1.0.7
    Checking quick-error v1.2.3
    Checking bitflags v1.3.2
    Checking hashbrown v0.11.2
    Checking cpufeatures v0.2.1
    Checking ryu v1.0.9
   Compiling pkg-config v0.3.24
    Checking regex-syntax v0.6.25
    Checking static_assertions v1.1.0
   Compiling cc v1.0.72
    Checking dyn-clone v1.0.4
    Checking quick-error v2.0.1
    Checking base16 v0.2.1
   Compiling log v0.4.14
    Checking base64 v0.13.0
    Checking once_cell v1.9.0
    Checking hex_fmt v0.3.0
    Checking parity-wasm v0.41.0
    Checking either v1.6.1
   Compiling anyhow v1.0.53
    Checking pin-project-lite v0.2.8
    Checking match_cfg v0.1.0
    Checking downcast-rs v1.2.0
    Checking memory_units v0.3.0
    Checking linked-hash-map v0.5.3
   Compiling ansi_term v0.12.1
   Compiling diff v0.1.12
   Compiling convert_case v0.5.0
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.0
   Compiling num-iter v0.1.42
   Compiling indexmap v1.8.0
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling generic-array v0.14.5
   Compiling value-bag v1.0.0-alpha.8
    Checking rand_chacha v0.2.2
    Checking tracing-core v0.1.21
    Checking bitvec v0.18.5
    Checking bit-set v0.5.2
    Checking itertools v0.10.3
   Compiling lmdb-sys v0.8.0
   Compiling pretty_assertions v1.2.0
    Checking wasmi-validation v0.3.0
    Checking rand v0.7.3
   Compiling quote v1.0.15
    Checking ff v0.8.0
    Checking getrandom v0.2.4
    Checking tempfile v3.3.0
    Checking wait-timeout v0.2.0
    Checking time v0.1.43
    Checking hostname v0.3.1
    Checking group v0.8.0
    Checking rand_core v0.6.3
    Checking rusty-fork v0.3.0
    Checking num-complex v0.4.0
    Checking digest v0.9.0
    Checking crypto-mac v0.10.1
    Checking block-buffer v0.9.0
    Checking crypto-mac v0.8.0
    Checking rand_chacha v0.3.1
    Checking rand_xorshift v0.3.0
    Checking chrono v0.4.19
    Checking signature v1.2.2
    Checking hmac v0.10.1
    Checking sha2 v0.9.9
    Checking blake2 v0.9.2
    Checking rand v0.8.4
 Documenting casper-dao-macros v0.1.0 (/workspaces/dao-contracts/dao-macros)
    Checking ed25519 v1.2.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
    Checking lmdb v0.8.0
    Checking wasmi v0.8.0
    Checking proptest v1.0.0
   Compiling zeroize_derive v1.3.1
   Compiling datasize_derive v0.2.10
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.21
   Compiling thiserror-impl v1.0.30
   Compiling tracing-attributes v0.1.18
   Compiling casper-dao-macros v0.1.0 (/workspaces/dao-contracts/dao-macros)
   Compiling delegate v0.6.2
    Checking datasize v0.2.10
    Checking zeroize v1.5.0
    Checking thiserror v1.0.30
    Checking tracing v0.1.29
    Checking elliptic-curve v0.8.5
    Checking curve25519-dalek v3.2.0
    Checking ecdsa v0.10.2
    Checking k256 v0.7.3
    Checking ed25519-dalek v1.0.1
    Checking hex v0.4.3
    Checking serde_bytes v0.11.5
    Checking bincode v1.3.3
    Checking uuid v0.8.2
    Checking uint v0.9.1
    Checking hex-buffer-serde v0.3.0
    Checking hex-buffer-serde v0.2.2
    Checking num v0.4.0
    Checking pwasm-utils v0.16.0
    Checking casper-types v1.4.6
    Checking casper-hashing v1.4.3
    Checking casper-contract v1.4.3
    Checking casper-execution-engine v1.4.4
    Checking casper-engine-test-support v2.0.3
    Checking casper-dao-utils v0.1.0 (/workspaces/dao-contracts/dao-utils)
 Documenting casper-dao-utils v0.1.0 (/workspaces/dao-contracts/dao-utils)
    Checking casper-dao-erc721 v0.1.0 (/workspaces/dao-contracts/dao-erc721)
    Checking casper-dao-modules v0.1.0 (/workspaces/dao-contracts/dao-modules)
 Documenting casper-dao-erc721 v0.1.0 (/workspaces/dao-contracts/dao-erc721)
 Documenting casper-dao-erc20 v0.1.0 (/workspaces/dao-contracts/dao-erc20)
 Documenting casper-dao-modules v0.1.0 (/workspaces/dao-contracts/dao-modules)
 Documenting casper-dao-contracts v0.1.0 (/workspaces/dao-contracts/dao-contracts)
warning: unresolved link to `Error:InvalidTokenOwner`
  --> dao-contracts/src/voting/onboarding_info.rs:53:85
   |
53 |     /// If the `address` does not own any token, reverts with [`InvalidTokenOwner`](Error:InvalidTokenOwner) error.
   |                                                                                     ^^^^^^^^^^^^^^^^^^^^^^^ no item named `Error:InvalidTokenOwner` in scope
   |
   = note: `#[warn(rustdoc::broken_intra_doc_links)]` on by default
   = help: to escape `[` and `]` characters, add '\' before them like `\[` or `\]`

warning: 1 warning emitted

    Finished dev [unoptimized + debuginfo] target(s) in 1m 01s
     Opening /workspaces/dao-contracts/target/doc/casper_dao_contracts/index.html
```