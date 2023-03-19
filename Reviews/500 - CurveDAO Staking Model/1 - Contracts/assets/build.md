```bash
$ make build-contract-curve-token-v3
cargo build --release -p curve-erc20 -p curve-rewards -p curve-token-v3 -p test-session-code --target wasm32-unknown-unknown
    Updating git repository `https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git`
    Updating crates.io index
  Downloaded arrayref v0.3.6
  Downloaded darling v0.10.2
  Downloaded darling_macro v0.10.2
  Downloaded casperlabs-contract-utils v0.2.2
  Downloaded derive_builder v0.9.0
  Downloaded getrandom v0.1.16
  Downloaded keccak v0.1.3
  Downloaded proc-macro-crate v0.1.5
  Downloaded memory_units v0.4.0
  Downloaded rustc-hex v2.1.0
  Downloaded libsecp256k1-gen-ecmult v0.2.1
  Downloaded libsecp256k1-core v0.2.2
  Downloaded strsim v0.9.3
  Downloaded wee_alloc v0.4.5
  Downloaded ident_case v1.0.1
  Downloaded crv20 v0.1.0
  Downloaded darling_core v0.10.2
  Downloaded curve-casper-erc20 v0.1.0
  Downloaded hmac v0.8.1
  Downloaded sha3 v0.9.1
  Downloaded base64 v0.12.3
  Downloaded derive_builder_core v0.9.0
  Downloaded cryptoxide v0.3.6
  Downloaded casper_types_derive v0.1.0
  Downloaded casper-contract v1.4.4
  Downloaded borsh-schema-derive-internal v0.8.2
  Downloaded borsh-derive-internal v0.8.2
  Downloaded borsh-derive v0.8.2
  Downloaded borsh v0.8.2
  Downloaded block-padding v0.2.1
  Downloaded ahash v0.4.7
  Downloaded tiny-keccak v2.0.2
  Downloaded libsecp256k1-gen-genmult v0.2.1
  Downloaded libsecp256k1 v0.5.0
  Downloaded hmac-drbg v0.3.0
  Downloaded hashbrown v0.9.1
  Downloaded 36 crates (1.2 MB) in 0.31s
   Compiling proc-macro2 v1.0.50
   Compiling quote v1.0.23
   Compiling unicode-ident v1.0.6
   Compiling typenum v1.16.0
   Compiling syn v1.0.107
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling getrandom v0.1.16
   Compiling subtle v2.4.1
   Compiling cfg-if v1.0.0
   Compiling crunchy v0.2.2
   Compiling serde v1.0.152
   Compiling serde_derive v1.0.152
   Compiling unicode-xid v0.2.4
   Compiling wyz v0.2.0
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling opaque-debug v0.3.0
   Compiling block-padding v0.2.1
   Compiling ppv-lite86 v0.2.17
   Compiling byteorder v1.4.3
   Compiling serde_json v1.0.91
   Compiling ryu v1.0.12
   Compiling rand_core v0.6.4
   Compiling static_assertions v1.1.0
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.5
   Compiling hex v0.4.3
   Compiling base16 v0.2.1
   Compiling cfg-if v0.1.10
   Compiling bitflags v1.3.2
   Compiling memory_units v0.4.0
   Compiling base64 v0.13.1
   Compiling hex_fmt v0.3.0
   Compiling strsim v0.9.3
   Compiling ident_case v1.0.1
   Compiling fnv v1.0.7
   Compiling thiserror v1.0.38
   Compiling tiny-keccak v2.0.2
   Compiling once_cell v1.17.0
   Compiling ahash v0.4.7
   Compiling derive_builder v0.9.0
   Compiling base64 v0.12.3
   Compiling keccak v0.1.3
   Compiling arrayref v0.3.6
   Compiling rustc-hex v2.1.0
   Compiling cryptoxide v0.3.6
   Compiling generic-array v0.14.6
   Compiling rand v0.8.5
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling bitvec v0.18.5
   Compiling hashbrown v0.9.1
   Compiling rand_core v0.5.1
   Compiling uint v0.9.5
   Compiling rand_chacha v0.2.2
   Compiling rand v0.7.3
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling crypto-mac v0.10.1
   Compiling libsecp256k1-core v0.2.2
   Compiling signature v1.2.2
   Compiling sha2 v0.9.9
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling hmac v0.8.1
   Compiling sha3 v0.9.1
   Compiling num-complex v0.4.3
   Compiling ed25519 v1.2.0
   Compiling hmac-drbg v0.3.0
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling libsecp256k1-gen-genmult v0.2.1
   Compiling libsecp256k1-gen-ecmult v0.2.1
   Compiling libsecp256k1 v0.5.0
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
   Compiling darling_core v0.10.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling borsh-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.3
   Compiling num-derive v0.3.3
   Compiling thiserror-impl v1.0.38
   Compiling casper_types_derive v0.1.0
   Compiling darling_macro v0.10.2
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling darling v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling derive_builder_core v0.9.0
   Compiling toml v0.5.11
   Compiling serde_bytes v0.11.8
   Compiling casper-types v1.5.0
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.2.2
   Compiling curve-casper-erc20 v0.1.0
   Compiling common v0.2.0 (/workspace/CasperLabs-Curve-DAO/common)
   Compiling crv20 v0.1.0
   Compiling casperlabs-ownable v0.1.0 (/workspace/CasperLabs-Curve-DAO/ownable/ownable-crate)
   Compiling casperlabs-lp-token-wrapper v0.1.0 (/workspace/CasperLabs-Curve-DAO/lp-token-wrapper/lp-token-wrapper-crate)
   Compiling curve-token-v3-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/curve-token-v3/curve-token-v3-crate)
   Compiling casperlabs-i-reward-distribution-recipient v0.1.0 (/workspace/CasperLabs-Curve-DAO/i-reward-distribution-recipient/i-reward-distribution-recipient-crate)
   Compiling curve-rewards-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/curve-rewards/curve-rewards-crate)
   Compiling curve-rewards v0.2.0 (/workspace/CasperLabs-Curve-DAO/curve-rewards/curve-rewards)
   Compiling curve-erc20 v0.1.0 (/workspace/CasperLabs-Curve-DAO/curve-erc20/curve-erc20)
   Compiling test-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/test-session-code)
   Compiling curve-token-v3 v0.2.0 (/workspace/CasperLabs-Curve-DAO/curve-token-v3/curve-token-v3)
    Finished release [optimized] target(s) in 1m 11s
wasm-strip target/wasm32-unknown-unknown/release/curve-token-v3.wasm 2>/dev/null | true

############################################################################################################################

$ make build-liquidity-gauge-reward-wrapper-session-code
cargo build --release -p liquidity-gauge-reward-wrapper-session-code --target wasm32-unknown-unknown
   Compiling base64 v0.13.1
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling common v0.2.0 (/workspace/CasperLabs-Curve-DAO/common)
   Compiling liquidity-gauge-reward-wrapper-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-session-code)
    Finished release [optimized] target(s) in 18.41s

############################################################################################################################

$ make build-i-reward-distribution-recipient
cargo build --release -p i-reward-distribution-recipient --target wasm32-unknown-unknown
   Compiling casperlabs-contract-utils v0.2.2
   Compiling casperlabs-ownable v0.1.0 (/workspace/CasperLabs-Curve-DAO/ownable/ownable-crate)
   Compiling casperlabs-i-reward-distribution-recipient v0.1.0 (/workspace/CasperLabs-Curve-DAO/i-reward-distribution-recipient/i-reward-distribution-recipient-crate)
   Compiling i-reward-distribution-recipient v0.2.0 (/workspace/CasperLabs-Curve-DAO/i-reward-distribution-recipient/i-reward-distribution-recipient)
    Finished release [optimized] target(s) in 4.66s

############################################################################################################################

$ make build-liquidity-gauge-wrapper-session-code
cargo build --release -p liquidity-gauge-wrapper-session-code --target wasm32-unknown-unknown
   Compiling liquidity-gauge-wrapper-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-wrapper/liquidity-gauge-wrapper-session-code)
    Finished release [optimized] target(s) in 1.72s

#############################################################################################################################

$ make build-contract-erc20-crv
cargo build --release -p test-session-code -p erc20-crv-session-code -p erc20-crv --target wasm32-unknown-unknown
   Compiling erc20-crv v0.1.0 (/workspace/CasperLabs-Curve-DAO/erc20-crv/erc20-crv)
   Compiling erc20-crv-session-code v0.2.0 (/workspace/CasperLabs-Curve-DAO/erc20-crv/erc20-crv-session-code)
    Finished release [optimized] target(s) in 5.35s
wasm-strip target/wasm32-unknown-unknown/release/erc20-crv.wasm 2>/dev/null | true

#############################################################################################################################

$ make build-contract-fee-distributor
cargo build --release -p test-session-code -p curve-erc20 -p fee-distributor-session-code -p voting-escrow -p fee-distributor -p erc20-crv --target wasm32-unknown-unknown
  Downloaded casperlabs-contract-utils v0.1.4
  Downloaded 1 crate (3.2 KB) in 0.34s
   Compiling casperlabs-contract-utils v0.1.4
   Compiling fee-distributor-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/fee-distributor/session-code)
   Compiling fee-distributor-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/fee-distributor/fee-distributor-crate)
   Compiling voting-escrow-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/voting-escrow/voting-escrow-crate)
   Compiling fee-distributor v0.2.0 (/workspace/CasperLabs-Curve-DAO/fee-distributor/fee-distributor)
   Compiling voting-escrow v0.2.0 (/workspace/CasperLabs-Curve-DAO/voting-escrow/voting-escrow)
    Finished release [optimized] target(s) in 7.86s
wasm-strip target/wasm32-unknown-unknown/release/fee-distributor.wasm 2>/dev/null | true

################################################################################################################################

$ make build-contract-gauge-controller
cargo build --release -p minter -p test-session-code -p erc20-crv -p liquidity-gauge-v3 -p gauge-controller-session-code -p curve-erc20 -p voting-escrow -p gauge-controller --target wasm32-unknown-unknown
   Compiling minter-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/minter/minter-crate)
   Compiling gauge-controller-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/gauge-controller/gauge-controller-crate)
   Compiling gauge-controller-session-code v0.2.0 (/workspace/CasperLabs-Curve-DAO/gauge-controller/session-code)
   Compiling liquidity-gauge-v3-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-v3/liquidity-gauge-v3-crate)
   Compiling minter v0.2.0 (/workspace/CasperLabs-Curve-DAO/minter/minter)
   Compiling gauge-controller v0.2.0 (/workspace/CasperLabs-Curve-DAO/gauge-controller/gauge-controller)
   Compiling liquidity-gauge-v3 v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-v3/liquidity-gauge-v3)
    Finished release [optimized] target(s) in 9.27s
wasm-strip target/wasm32-unknown-unknown/release/gauge-controller-token.wasm 2>/dev/null | true

##############################################################################################################################

$ make build-contract-gauge-proxy
cargo build --release -p gauge-proxy --target wasm32-unknown-unknown
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.1.4
   Compiling common v0.2.0 (/workspace/CasperLabs-Curve-DAO/common)
   Compiling gauge-proxy-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/gauge-proxy/gauge-proxy-crate)
   Compiling gauge-proxy v0.2.0 (/workspace/CasperLabs-Curve-DAO/gauge-proxy/gauge-proxy)
    Finished release [optimized] target(s) in 5.87s
wasm-strip target/wasm32-unknown-unknown/release/gauge-proxy.wasm 2>/dev/null | true

###############################################################################################################################

$ make build-contract-liquidity-gauge-reward
cargo build --release -p liquidity-gauge-reward-session-code -p test-session-code -p curve-rewards -p erc20-crv -p curve-erc20 -p voting-escrow -p gauge-controller  -p minter -p liquidity-gauge-reward --target wasm32-unknown-unknown
   Compiling liquidity-gauge-reward-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward/liquidity-gauge-reward-session-code)
   Compiling liquidity-gauge-reward-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward/liquidity-gauge-reward-crate)
   Compiling liquidity-gauge-reward v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward/liquidity-gauge-reward)
    Finished release [optimized] target(s) in 5.99s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-reward.wasm 2>/dev/null | true

##############################################################################################################################

$ make build-contract-liquidity-gauge-reward-wrapper
cargo build --release -p erc20-crv -p curve-erc20 -p test-session-code -p minter -p voting-escrow -p gauge-controller -p liquidity-gauge-reward -p liquidity-gauge-reward-wrapper -p liquidity-gauge-reward-wrapper-session-code -p curve-rewards --target wasm32-unknown-unknown
   Compiling liquidity-gauge-reward-wrapper-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-session-code)
   Compiling liquidity-gauge-reward-wrapper-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper-crate)
   Compiling liquidity-gauge-reward-wrapper v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-reward-wrapper/liquidity-gauge-reward-wrapper)
    Finished release [optimized] target(s) in 7.42s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-reward-wrapper.wasm 2>/dev/null | true

###############################################################################################################################

$ make build-contract-liquidity-gauge-wrapper
cargo build --release -p erc20-crv -p curve-erc20 -p test-session-code -p minter -p liquidity-gauge-v3 -p voting-escrow -p gauge-controller -p liquidity-gauge-wrapper-session-code -p liquidity-gauge-wrapper --target wasm32-unknown-unknown
   Compiling liquidity-gauge-wrapper-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-wrapper/liquidity-gauge-wrapper-session-code)
   Compiling liquidity-gauge-wrapper-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-wrapper/liquidity-gauge-wrapper-crate)
   Compiling liquidity-gauge-wrapper v0.2.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-wrapper/liquidity-gauge-wrapper)
    Finished release [optimized] target(s) in 6.41s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-wrapper.wasm 2>/dev/null | true

##############################################################################################################################

$ make build-contract-minter
cargo build --release -p curve-erc20 -p erc20-crv -p erc20-crv-session-code -p liquidity-gauge-v3 -p liquidity-gauge-reward -p voting-escrow -p gauge-controller -p minter --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.11s
wasm-strip target/wasm32-unknown-unknown/release/minter-token.wasm 2>/dev/null | true

###################################################################################################################################

$ make build-contract-reward-only-gauge
cargo build --release -p test-session-code -p curve-erc20 -p erc20-crv -p curve-rewards -p reward-only-gauge -p reward-only-gauge-session-code --target wasm32-unknown-unknown
   Compiling reward-only-gauge-session-code v0.2.0 (/workspace/CasperLabs-Curve-DAO/reward-only-gauge/session-code)
   Compiling reward-only-gauge-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/reward-only-gauge/reward-only-gauge-crate)
   Compiling reward-only-gauge v0.2.0 (/workspace/CasperLabs-Curve-DAO/reward-only-gauge/reward-only-gauge)
    Finished release [optimized] target(s) in 6.37s
wasm-strip target/wasm32-unknown-unknown/release/reward-only-gauge.wasm 2>/dev/null | true

##################################################################################################################################

$ make build-contract-vesting-escrow
cargo build --release -p test-session-code -p vesting-escrow-session-code  -p curve-erc20 -p vesting-escrow --target wasm32-unknown-unknown
   Compiling vesting-escrow-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow/vesting-escrow-crate)
   Compiling vesting-escrow-session-code v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow/session-code)
   Compiling vesting-escrow v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow/vesting-escrow)
    Finished release [optimized] target(s) in 5.27s
wasm-strip target/wasm32-unknown-unknown/release/vesting-escrow.wasm 2>/dev/null | true

#################################################################################################################################

$ make build-contract-vesting-escrow-factory
cargo build --release -p vesting-escrow-simple -p curve-erc20 -p vesting-escrow-factory -p vesting-escrow-factory-session-code --target wasm32-unknown-unknown
  Downloaded casperlabs-erc20 v0.2.3
  Downloaded 1 crate (5.8 KB) in 0.22s
   Compiling casperlabs-erc20 v0.2.3
   Compiling vesting-escrow-factory-session-code v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow-factory/session-code)
   Compiling vesting-escrow-simple-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow-simple/vesting-escrow-simple-crate)
   Compiling vesting-escrow-factory-crate v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow-factory/vesting-escrow-factory-crate)
   Compiling vesting-escrow-factory v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow-factory/vesting-escrow-factory)
   Compiling vesting-escrow-simple v0.2.0 (/workspace/CasperLabs-Curve-DAO/vesting-escrow-simple/vesting-escrow-simple)
    Finished release [optimized] target(s) in 7.00s
wasm-strip target/wasm32-unknown-unknown/release/vesting-escrow-factory.wasm 2>/dev/null | true

###################################################################################################################################

$ make build-contract-liquidity-gauge-v3
cargo build --release -p test-session-code -p liquidity-gauge-v3-session-code -p liquidity-gauge-v3 -p curve-erc20 -p minter -p voting-escrow -p gauge-controller -p erc20-crv  --target wasm32-unknown-unknown
   Compiling liquidity-gauge-v3-session-code v0.1.0 (/workspace/CasperLabs-Curve-DAO/liquidity-gauge-v3/liquidity-gauge-v3-session-code)
    Finished release [optimized] target(s) in 1.97s
wasm-strip target/wasm32-unknown-unknown/release/liquidity-gauge-v3.wasm 2>/dev/null | true

###################################################################################################################################

$ make build-contract-vesting-escrow-simple
cargo build --release -p curve-erc20 -p vesting-escrow-simple --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.15s
wasm-strip target/wasm32-unknown-unknown/release/vesting-escrow-simple.wasm 2>/dev/null | true

##################################################################################################################################

$ make build-contract-voting-escrow
cargo build --release -p test-session-code -p erc20-crv -p voting-escrow --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.09s
wasm-strip target/wasm32-unknown-unknown/release/vesting_escrow_simple.wasm 2>/dev/null | true

######################################################################################################################################

$ make build-contract-ownable
cargo build --release -p test-session-code -p ownable --target wasm32-unknown-unknown
   Compiling ownable v0.2.0 (/workspace/CasperLabs-Curve-DAO/ownable/ownable)
    Finished release [optimized] target(s) in 3.05s

###################################################################################################################################

$ make build-lp-token-wrapper
cargo build --release  -p test-session-code -p lp-token-wrapper --target wasm32-unknown-unknown
   Compiling lp-token-wrapper v0.2.0 (/workspace/CasperLabs-Curve-DAO/lp-token-wrapper/lp-token-wrapper)
    Finished release [optimized] target(s) in 2.97s

##############################################################################################################################

$ make build-curve-rewards
cargo build --release -p curve-erc20 -p test-session-code -p curve-rewards --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.09s
```
