```bash
ndpc_contract (main)$ make test
cd contract && cargo build --release --target wasm32-unknown-unknown
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
    Finished release [optimized] target(s) in 0.05s
wasm-strip contract/target/wasm32-unknown-unknown/release/contract.wasm 2>/dev/null | true
cp contract/target/wasm32-unknown-unknown/release/contract.wasm deploy/contract.wasm
mkdir -p tests/wasm
cp contract/target/wasm32-unknown-unknown/release/contract.wasm tests/wasm
cd tests && cargo test
warning: unused import: `U256`
  --> src/integration_tests.rs:19:112
   |
19 |         account::AccountHash, runtime_args, Key, Motes, PublicKey, RuntimeArgs, SecretKey, U512, ContractHash, U256, Contract,
   |                                                                                                                ^^^^
   |
   = note: `#[warn(unused_imports)]` on by default
help: consider adding a `#[cfg(test)]` to the containing module
  --> src/integration_tests.rs:4:1
   |
4  | mod tests {
   | ^^^^^^^^^

warning: unused variable: `timestamp`
   --> src/integration_tests.rs:318:13
    |
318 |         let timestamp : u64 = 1677241273;
    |             ^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_timestamp`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `timestamp`
   --> src/integration_tests.rs:461:13
    |
461 |         let timestamp : u64 = 1677241273;
    |             ^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_timestamp`

warning: unused variable: `requests_dict_uref`
   --> src/integration_tests.rs:543:13
    |
543 |         let requests_dict_uref = contract.named_keys().get("request_objects").unwrap().into_uref().unwrap();
    |             ^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_requests_dict_uref`

warning: unused variable: `timestamp`
   --> src/integration_tests.rs:611:13
    |
611 |         let timestamp : u64 = 1677241273;
    |             ^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_timestamp`

warning: associated function is never used: `new`
  --> src/integration_tests.rs:38:16
   |
38 |         pub fn new() -> Self {
   |                ^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: associated function is never used: `remove`
  --> src/integration_tests.rs:43:16
   |
43 |         pub fn remove(&mut self, value: u64) -> u64 {
   |                ^^^^^^

warning: associated function is never used: `add`
  --> src/integration_tests.rs:47:16
   |
47 |         pub fn add(&mut self, value: u64) {
   |                ^^^

warning: associated function is never used: `contains`
  --> src/integration_tests.rs:50:16
   |
50 |         pub fn contains(self, value: u64) -> bool {
   |                ^^^^^^^^

warning: associated function is never used: `new`
   --> src/integration_tests.rs:145:16
    |
145 |         pub fn new(
    |                ^^^

warning: associated function is never used: `get_hash`
   --> src/integration_tests.rs:229:16
    |
229 |         pub fn get_hash(&self) -> MetadataHash {
    |                ^^^^^^^^

warning: associated function is never used: `new`
   --> src/integration_tests.rs:238:16
    |
238 |         pub fn new(
    |                ^^^

warning: associated function is never used: `to_json`
   --> src/integration_tests.rs:253:16
    |
253 |         pub fn to_json(&self) -> String {
    |                ^^^^^^^

warning: `tests` (bin "integration-tests" test) generated 13 warnings
    Finished test [unoptimized + debuginfo] target(s) in 0.17s
     Running unittests (target/debug/deps/integration_tests-3ec908b3a6613094)

running 5 tests
test tests::mint_entrypoint ... ok
test tests::publish_request_entry_point ... ok
test tests::cancel_request_entry_point ... ok
test tests::approve_entry_point ... ok
test tests::disapprove_entry_point ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 2.41s

```