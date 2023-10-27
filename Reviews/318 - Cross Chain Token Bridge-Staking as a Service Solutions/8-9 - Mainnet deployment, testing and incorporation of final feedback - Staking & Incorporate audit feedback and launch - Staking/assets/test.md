## `make test`

```sh
gitpod /workspace/casper_staking/staking_contract (main) $ make test
cd staking_contract && cargo build --release --target wasm32-unknown-unknown
info: syncing channel updates for 'nightly-2023-01-16-x86_64-unknown-linux-gnu'
info: latest update on 2023-01-16, rust version 1.68.0-nightly (9e75dddf6 2023-01-15)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
info: installing component 'rust-std'
info: installing component 'rustc'
info: installing component 'rustfmt'
    Finished release [optimized] target(s) in 0.82s
wasm-strip staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cd ../erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
warning: unused import: `alloc::string::String`
 --> erc20/src/error.rs:2:5
  |
2 | use alloc::string::String;
  |     ^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: missing documentation for a function
   --> erc20/src/entry_points.rs:145:1
    |
145 | pub fn mint() -> EntryPoint {
    | ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    |
note: the lint level is defined here
   --> erc20/src/lib.rs:13:9
    |
13  | #![warn(missing_docs)]
    |         ^^^^^^^^^^^^

warning: missing documentation for a variant
  --> erc20/src/error.rs:28:5
   |
28 |     UserAllowance(u16),
   |     ^^^^^^^^^^^^^

warning: `casper-erc20` (lib) generated 3 warnings (run `cargo fix --lib -p casper-erc20` to apply 1 suggestion)
warning: unused import: `core::panic::PanicInfo`
  --> erc20-token/src/main.rs:10:5
   |
10 | use core::panic::PanicInfo;
   |     ^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `erc20-token` (bin "erc20_token") generated 1 warning (run `cargo fix --bin "erc20_token"` to apply 1 suggestion)
    Finished release [optimized] target(s) in 0.37s
wasm-strip ../erc20/erc20-token/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cp staking_contract/target/wasm32-unknown-unknown/release/*.wasm staking_contract_tests/wasm
cp ../erc20/target/wasm32-unknown-unknown/release/erc20_token.wasm staking_contract_tests/wasm/erc20.wasm
cd staking_contract_tests && cargo test
warning: unused import: `std::convert::TryInto`
  --> src/staking_contract_tests.rs:15:5
   |
15 | use std::convert::TryInto;
   |     ^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `std::time::SystemTime`
  --> src/staking_contract_tests.rs:16:5
   |
16 | use std::time::SystemTime;
   |     ^^^^^^^^^^^^^^^^^^^^^

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:316:9
    |
316 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:452:9
    |
452 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:590:9
    |
590 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:745:9
    |
745 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:901:9
    |
901 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1050:9
     |
1050 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1184:9
     |
1184 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1316:9
     |
1316 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1450:9
     |
1450 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: constant `ADDRESS` is never used
  --> src/staking_contract_tests.rs:18:7
   |
18 | const ADDRESS: &str = "9e7283533626d0c7d43fa9ca745af20d8dac7fc3bfe03cdfe50d523a2a0f498d";
   |       ^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: `staking_contract_tests` (lib test) generated 12 warnings (run `cargo fix --lib -p staking_contract_tests --tests` to apply 11 suggestions)
    Finished test [unoptimized + debuginfo] target(s) in 0.33s
     Running unittests src/lib.rs (target/debug/deps/staking_contract_tests-baedd6fbbf1ca019)

running 11 tests
test staking_contract_tests::test_stake_but_not_approve - should panic ... ok
test staking_contract_tests::test_approve_and_stake ... ok
test staking_contract_tests::test_approve_and_stake_and_add_reward_withdrawable_amount_too_big - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_add_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_staker_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_get_current_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_amount_staked ... ok
test staking_contract_tests::test_approve_and_stake_and_staker_reward_wrong_address - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_withdraw_too_big_amount - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_amount_staked_wrong_address - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_withdraw ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 2.98s

   Doc-tests staking_contract_tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

gitpod /workspace/casper_staking/staking_contract (main) $
```