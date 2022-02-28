```sh
$ make build-signer
cargo build --release -p subscription_hash_signer
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/casper-contract-eip-1337/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/casper-eip-1337/subscription_hash_signer/Cargo.toml
workspace: /workspace/casper-eip-1337/Cargo.toml
   Compiling proc-macro2 v1.0.36
   Compiling libc v0.2.118
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling cc v1.0.73
   Compiling pkg-config v0.3.24
   Compiling serde v1.0.136
   Compiling ppv-lite86 v0.2.16
   Compiling crunchy v0.2.2
   Compiling opaque-debug v0.3.0
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.79
   Compiling cpufeatures v0.2.1
   Compiling foreign-types-shared v0.1.1
   Compiling static_assertions v1.1.0
   Compiling bitflags v1.3.2
   Compiling openssl v0.10.38
   Compiling itoa v1.0.1
   Compiling rand_core v0.6.3
   Compiling once_cell v1.9.0
   Compiling ryu v1.0.9
   Compiling base64 v0.13.0
   Compiling hex v0.4.3
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling untrusted v0.7.1
   Compiling typenum v1.15.0
   Compiling getrandom v0.1.16
   Compiling bitvec v0.18.5
   Compiling foreign-types v0.3.2
   Compiling rand v0.8.5
   Compiling openssl-sys v0.9.72
   Compiling pem v1.0.2
   Compiling generic-array v0.14.5
   Compiling num-traits v0.2.14
   Compiling num-integer v0.1.44
   Compiling num-rational v0.4.0
   Compiling derp v0.0.14
   Compiling uint v0.9.1
   Compiling quote v1.0.15
   Compiling syn v1.0.86
   Compiling rand_core v0.5.1
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.2.2
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling group v0.8.0
   Compiling ed25519 v1.2.0
   Compiling rand v0.7.3
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.1
   Compiling serde_derive v1.0.136
   Compiling datasize_derive v0.2.10
   Compiling num-derive v0.3.3
   Compiling thiserror-impl v1.0.30
   Compiling displaydoc v0.1.7
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.10
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling thiserror v1.0.30
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling casper-types v1.3.2
   Compiling subscription_hash_signer v0.1.0 (/workspace/casper-eip-1337/subscription_hash_signer)
warning: type alias is never used: `Result`
  --> subscription_hash_signer/src/der/errors.rs:12:1
   |
12 | pub type Result<T> = result::Result<T, Error>;
   | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: 1 warning emitted

    Finished release [optimized] target(s) in 35.76s
mkdir -p bin
cp target/release/subscription_hash_signer bin
```

