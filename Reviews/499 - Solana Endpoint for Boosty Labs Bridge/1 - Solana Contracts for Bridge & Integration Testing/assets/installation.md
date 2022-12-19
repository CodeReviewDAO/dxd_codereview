```
gitpod /workspace/CasperLabs-Solana-bridge (main) $ sh -c "$(curl -sSfL https://release.solana.com/v1.14.9/install)"
downloading v1.14.9 installer
  ✨ 1.14.9 initialized
Adding 
export PATH="/home/gitpod/.local/share/solana/install/active_release/bin:$PATH" to /home/gitpod/.profile
Adding 
export PATH="/home/gitpod/.local/share/solana/install/active_release/bin:$PATH" to /home/gitpod/.bash_profile

Close and reopen your terminal to apply the PATH changes or run the following in your existing shell:
  
export PATH="/home/gitpod/.local/share/solana/install/active_release/bin:$PATH"

gitpod /workspace/CasperLabs-Solana-bridge (main) $ export PATH="/home/gitpod/.local/share/solana/install/active_release/bin:$PATH"
gitpod /workspace/CasperLabs-Solana-bridge (main) $ solana --version
solana-cli 1.14.9 (src:af329cf4; feat:3036606309)
gitpod /workspace/CasperLabs-Solana-bridge (main) $ npm i

up to date, audited 143 packages in 709ms

15 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
gitpod /workspace/CasperLabs-Solana-bridge (main) $ rustup default stable
info: using existing install for 'stable-x86_64-unknown-linux-gnu'
info: default toolchain set to 'stable-x86_64-unknown-linux-gnu'

  stable-x86_64-unknown-linux-gnu unchanged - rustc 1.65.0 (897e37553 2022-11-02)

gitpod /workspace/CasperLabs-Solana-bridge (main) $ npm run build:program

> casperlabs-solana-bridge@1.0.0 build:program
> cargo build-bpf --manifest-path=./Cargo.toml

Warning: cargo-build-bpf is deprecated. Please, use cargo-build-sbf
cargo-build-bpf child: /home/gitpod/.local/share/solana/install/active_release/bin/cargo-build-sbf --manifest-path=./Cargo.toml --arch bpf
   Compiling proc-macro2 v1.0.47
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.5
   Compiling syn v1.0.105
   Compiling serde_derive v1.0.148
   Compiling serde v1.0.148
   Compiling version_check v0.9.4
   Compiling semver v1.0.14
   Compiling typenum v1.15.0
   Compiling libc v0.2.138
   Compiling thiserror v1.0.37
   Compiling autocfg v1.1.0
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling feature-probe v0.1.1
   Compiling once_cell v1.16.0
   Compiling serde_json v1.0.89
   Compiling rustversion v1.0.9
   Compiling log v0.4.17
   Compiling ryu v1.0.11
   Compiling itoa v1.0.4
   Compiling lazy_static v1.4.0
   Compiling bs58 v0.4.0
   Compiling arrayref v0.3.6
   Compiling keccak v0.1.3
   Compiling either v1.8.0
   Compiling constant_time_eq v0.2.4
   Compiling arrayvec v0.7.2
   Compiling bv v0.11.1
   Compiling generic-array v0.14.6
   Compiling ahash v0.7.6
   Compiling itertools v0.10.5
   Compiling num-traits v0.2.15
   Compiling memoffset v0.6.5
   Compiling rustc_version v0.4.0
   Compiling hashbrown v0.11.2
   Compiling solana-frozen-abi-macro v1.14.9
   Compiling solana-frozen-abi v1.14.9
   Compiling jobserver v0.1.25
   Compiling cc v1.0.77
   Compiling blake3 v1.3.3
   Compiling solana-program v1.14.9
   Compiling borsh-derive-internal v0.9.3
   Compiling borsh-schema-derive-internal v0.9.3
   Compiling thiserror-impl v1.0.37
   Compiling bytemuck_derive v1.3.0
   Compiling num-derive v0.3.3
   Compiling solana-sdk-macro v1.14.9
   Compiling bytemuck v1.12.3
   Compiling serde_bytes v0.11.7
   Compiling bincode v1.3.3
   Compiling toml v0.5.9
   Compiling crypto-common v0.1.6
   Compiling block-buffer v0.10.3
   Compiling digest v0.10.6
   Compiling sha2 v0.10.6
   Compiling sha3 v0.10.6
   Compiling proc-macro-crate v0.1.5
   Compiling proc-macro-crate v1.2.1
   Compiling borsh-derive v0.9.3
   Compiling num_enum_derive v0.5.7
   Compiling borsh v0.9.3
   Compiling num_enum v0.5.7
   Compiling spl-token v3.5.0
   Compiling bridge v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/Bridge)
    Finished release [optimized] target(s) in 55.37s
+ wget https://github.com/Snaipe/Criterion/releases/download/v2.3.3/criterion-v2.3.3-linux-x86_64.tar.bz2 -O criterion-v2.3.3-linux-x86_64.tar.bz2 --progress=dot:giga --retry-connrefused --read-timeout=30
--2022-12-04 16:00:47--  https://github.com/Snaipe/Criterion/releases/download/v2.3.3/criterion-v2.3.3-linux-x86_64.tar.bz2
Resolving github.com (github.com)... 140.82.121.4
Connecting to github.com (github.com)|140.82.121.4|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://objects.githubusercontent.com/github-production-release-asset-2e65be/30111969/98b27400-e1f1-11e8-8f10-e43f4ef84b92?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20221204%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20221204T160047Z&X-Amz-Expires=300&X-Amz-Signature=dc7bf5f3f3300bec0bb26fd09c7f2efab28e294ab094b236f63aee80cb2a2228&X-Amz-SignedHeaders=host&actor_id=0&key_id=0&repo_id=30111969&response-content-disposition=attachment%3B%20filename%3Dcriterion-v2.3.3-linux-x86_64.tar.bz2&response-content-type=application%2Foctet-stream [following]
--2022-12-04 16:00:47--  https://objects.githubusercontent.com/github-production-release-asset-2e65be/30111969/98b27400-e1f1-11e8-8f10-e43f4ef84b92?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20221204%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20221204T160047Z&X-Amz-Expires=300&X-Amz-Signature=dc7bf5f3f3300bec0bb26fd09c7f2efab28e294ab094b236f63aee80cb2a2228&X-Amz-SignedHeaders=host&actor_id=0&key_id=0&repo_id=30111969&response-content-disposition=attachment%3B%20filename%3Dcriterion-v2.3.3-linux-x86_64.tar.bz2&response-content-type=application%2Foctet-stream
Resolving objects.githubusercontent.com (objects.githubusercontent.com)... 185.199.110.133, 185.199.111.133, 185.199.108.133, ...
Connecting to objects.githubusercontent.com (objects.githubusercontent.com)|185.199.110.133|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 677858 (662K) [application/octet-stream]
Saving to: ‘criterion-v2.3.3-linux-x86_64.tar.bz2’

     0K                                    100% 31.4M=0.02s

2022-12-04 16:00:48 (31.4 MB/s) - ‘criterion-v2.3.3-linux-x86_64.tar.bz2’ saved [677858/677858]

+ tar --strip-components 1 -jxf criterion-v2.3.3-linux-x86_64.tar.bz2
+ ./bpf-tools/rust/bin/rustc --version
+ ./bpf-tools/rust/bin/rustc --print sysroot
+ set +e
+ rustup toolchain uninstall bpf
info: uninstalling toolchain 'bpf'
info: toolchain 'bpf' uninstalled
+ set -e
+ rustup toolchain link bpf bpf-tools/rust
+ exit 0
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling once_cell v1.16.0
   Compiling itoa v1.0.4
   Compiling ryu v1.0.11
   Compiling arrayref v0.3.6
   Compiling bs58 v0.4.0
   Compiling arrayvec v0.7.2
   Compiling keccak v0.1.3
   Compiling either v1.8.0
   Compiling constant_time_eq v0.2.4
   Compiling lazy_static v1.4.0
   Compiling typenum v1.15.0
   Compiling log v0.4.17
   Compiling memoffset v0.6.5
   Compiling num-traits v0.2.15
   Compiling serde v1.0.148
   Compiling thiserror v1.0.37
   Compiling bytemuck v1.12.3
   Compiling num_enum v0.5.7
   Compiling ahash v0.7.6
   Compiling itertools v0.10.5
   Compiling hashbrown v0.11.2
   Compiling borsh v0.9.3
   Compiling generic-array v0.14.6
   Compiling serde_bytes v0.11.7
   Compiling serde_json v1.0.89
   Compiling bv v0.11.1
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
   Compiling w_pokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPokt)
    Finished release [optimized] target(s) in 23.52s
   Compiling subtle v2.4.1
   Compiling once_cell v1.16.0
   Compiling cfg-if v1.0.0
   Compiling itoa v1.0.4
   Compiling ryu v1.0.11
   Compiling arrayvec v0.7.2
   Compiling arrayref v0.3.6
   Compiling bs58 v0.4.0
   Compiling either v1.8.0
   Compiling constant_time_eq v0.2.4
   Compiling lazy_static v1.4.0
   Compiling keccak v0.1.3
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
   Compiling serde_bytes v0.11.7
   Compiling bv v0.11.1
   Compiling serde_json v1.0.89
   Compiling bincode v1.3.3
   Compiling block-buffer v0.10.3
   Compiling crypto-common v0.1.6
   Compiling digest v0.10.6
   Compiling sha2 v0.10.6
   Compiling blake3 v1.3.3
   Compiling sha3 v0.10.6
   Compiling solana-frozen-abi v1.14.9
   Compiling solana-program v1.14.9
   Compiling spl-token v3.5.0
   Compiling wpokt v0.1.0 (/workspace/CasperLabs-Solana-bridge/src/program/WPOKT)
    Finished release [optimized] target(s) in 22.89s

gitpod /workspace/CasperLabs-Solana-bridge (main) $ ls target/bpfel-unknown-unknown/release/*.so
target/bpfel-unknown-unknown/release/bridge.so  target/bpfel-unknown-unknown/release/wpokt.so
target/bpfel-unknown-unknown/release/w_pokt.so
gitpod /workspace/CasperLabs-Solana-bridge (main) $
```
