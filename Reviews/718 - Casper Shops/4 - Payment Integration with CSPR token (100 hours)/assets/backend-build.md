```bash
ndpc_contract (main)$ make build-contract
cd contract && cargo build --release --target wasm32-unknown-unknown
   Compiling typenum v1.15.0
   Compiling proc-macro2 v1.0.47
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.5
   Compiling syn v1.0.104
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling serde_derive v1.0.148
   Compiling serde v1.0.148
   Compiling opaque-debug v0.3.0
   Compiling byteorder v1.4.3
   Compiling cfg-if v1.0.0
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.17
   Compiling serde_json v1.0.89
   Compiling ryu v1.0.11
   Compiling hex v0.4.3
   Compiling rand_core v0.6.4
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.4
   Compiling static_assertions v1.1.0
   Compiling memory_units v0.4.0
   Compiling bitflags v1.3.2
   Compiling cfg-if v0.1.10
   Compiling base64 v0.13.1
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling signature v2.0.0
   Compiling generic-array v0.14.6
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling bitvec v0.18.5
   Compiling rand_chacha v0.2.2
   Compiling rand v0.8.5
   Compiling ed25519 v2.0.1
   Compiling rand v0.7.3
   Compiling uint v0.9.4
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
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling synstructure v0.12.6
   Compiling num v0.4.0
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling casper-types v2.0.0
   Compiling casper-contract v2.0.0
   Compiling contract v0.1.0 (/home/mehmet/Desktop/droplinked_casper/ndpc_contract/contract)
warning: unused imports: `ApprovedNFT`, `AsStrized`, `NAMED_KEY_APPROVED_CNT`, `NAMED_KEY_HOLDERSCNT`, `NAMED_KEY_REQ_CNT`, `NFTHolder`, `NftMetadata`, `PublishRequest`, `U64list`, `ndpc_utils`
 --> src/init.rs:5:72
  |
5 |     NAMED_KEY_DICT_TOKEN_ID_BY_HASH_NAME, NAMED_KEY_DICT_TOTAL_SUPPLY, NAMED_KEY_HOLDERSCNT, NAMED_KEY_APPROVED_CNT, NAMED_KEY_REQ_CNT,
  |                                                                        ^^^^^^^^^^^^^^^^^^^^  ^^^^^^^^^^^^^^^^^^^^^^  ^^^^^^^^^^^^^^^^^
6 | }, ndpc_types::{NftMetadata, NFTHolder, PublishRequest, AsStrized, U64list, ApprovedNFT}, ndpc_utils};
  |                 ^^^^^^^^^^^  ^^^^^^^^^  ^^^^^^^^^^^^^^  ^^^^^^^^^  ^^^^^^^  ^^^^^^^^^^^   ^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused imports: `borrow::ToOwned`, `string::ToString`
 --> src/init.rs:7:13
  |
7 | use alloc::{string::ToString, borrow::ToOwned};
  |             ^^^^^^^^^^^^^^^^  ^^^^^^^^^^^^^^^

warning: unused imports: `get_caller`, `self`
 --> src/init.rs:8:57
  |
8 | use casper_contract::{contract_api::{storage, runtime::{get_caller, self}}, unwrap_or_revert::UnwrapOrRevert};
  |                                                         ^^^^^^^^^^  ^^^^

warning: unused imports: `Div`, `Mul`
 --> src/payment.rs:1:22
  |
1 | use core::ops::{Add, Div, Mul, Sub};
  |                      ^^^  ^^^

warning: unused imports: `NAMED_KEY_HOLDERSCNT`, `U64list`, `get_holder_by_id`
  --> src/payment.rs:7:42
   |
7  |         NAMED_KEY_DICT_PUBAPPROVED_NAME, NAMED_KEY_HOLDERSCNT, RUNTIME_ARG_AMOUNT,
   |                                          ^^^^^^^^^^^^^^^^^^^^
...
13 |     ndpc_types::{self, AsStrized, U64list},
   |                                   ^^^^^^^
...
16 |         get_holder_by_id, get_nft_metadata, get_ratio_verifier, verify_signature, get_fee,
   |         ^^^^^^^^^^^^^^^^

warning: unused variable: `owners_dict`
   --> src/payment.rs:101:9
    |
101 |         owners_dict,
    |         ^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_owners_dict`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `publishers_approved_dict`
   --> src/payment.rs:103:9
    |
103 |         publishers_approved_dict,
    |         ^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_publishers_approved_dict`

warning: unused variable: `producers_approved_dict`
   --> src/payment.rs:104:9
    |
104 |         producers_approved_dict,
    |         ^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_producers_approved_dict`

warning: unused variable: `holders_dict`
   --> src/payment.rs:105:9
    |
105 |         holders_dict,
    |         ^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_holders_dict`

warning: variable does not need to be mutable
   --> src/payment.rs:113:9
    |
113 |     let mut approved_holder: ndpc_types::ApprovedNFT = get_approved_holder_by_id(approved_dict, approved_id); //1)
    |         ----^^^^^^^^^^^^^^^
    |         |
    |         help: remove this `mut`
    |
    = note: `#[warn(unused_mut)]` on by default

warning: variant is never constructed: `NotEnoughBalance`
  --> src/main.rs:36:5
   |
36 |     NotEnoughBalance = 7,
   |     ^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: variant is never constructed: `ApprovedListDoesentExist`
  --> src/main.rs:39:5
   |
39 |     ApprovedListDoesentExist = 10,
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: `contract` (bin "contract") generated 12 warnings
    Finished release [optimized] target(s) in 22.59s
wasm-strip contract/target/wasm32-unknown-unknown/release/contract.wasm 2>/dev/null | true
cp contract/target/wasm32-unknown-unknown/release/contract.wasm deploy/contract.wasm

```