# Test ERC20
cd ./erc20/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20-token.wasm 2>/dev/null | true
cargo build --release -p erc20-proxy --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20-proxy-token.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm erc20-tests/wasm
cargo test -p erc20-tests
    Finished test [unoptimized + debuginfo] target(s) in 0.13s
     Running unittests (target/debug/deps/erc20_tests-210c2cacc1639236)

running 10 tests
test erc20_tests::test_deploy ... ok
test erc20_tests::test_erc20_approve ... ok
test erc20_tests::test_erc20_transfer ... ok
test erc20_tests::test_erc20_mint ... ok
test erc20_tests::test_erc20_burn ... ok
test erc20_tests::test_erc20_transfer_with_same_sender_and_recipient ... ok
test erc20_tests::test_erc20_increase_allowance ... ok
test erc20_tests::test_erc20_transfer_from ... ok
test erc20_tests::test_erc20_transfer_from_too_much - should panic ... ok
test erc20_tests::test_erc20_decrease_allowance ... ok

test result: ok. 10 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 4.85s

   Doc-tests erc20-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
# Test WCSPR
cd ./wcspr/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p wcspr --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-token.wasm 2>/dev/null | true
cargo build --release -p test --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-test.wasm 2>/dev/null | true
cargo build --release -p test2 --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-test2.wasm 2>/dev/null | true
cargo build --release -p purse-proxy --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/purse-proxy.wasm 2>/dev/null | true
cargo build --release -p invalid-purse-proxy --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: unused import: `system`
  --> invalid-purse-proxy/src/main.rs:12:38
   |
12 |     contract_api::{account, runtime, system},
   |                                      ^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `invalid-purse-proxy` (bin "invalid-purse-proxy") generated 1 warning
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/invalid-purse-proxy.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm wcspr-tests/wasm
# cp test-contract/target/wasm32-unknown-unknown/release/*.wasm wcspr-tests/wasm
cargo test -p wcspr-tests
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: unused variable: `owner`
  --> wcspr-tests/src/wcspr_tests.rs:55:32
   |
55 |     let (env, token, proxy, _, owner) = deploy();
   |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`
   |
   = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `owner`
  --> wcspr-tests/src/wcspr_tests.rs:81:32
   |
81 |     let (env, token, proxy, _, owner) = deploy();
   |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `amount`
  --> wcspr-tests/src/wcspr_tests.rs:83:9
   |
83 |     let amount: U512 = 500.into();
   |         ^^^^^^ help: if this is intentional, prefix it with an underscore: `_amount`

warning: unused variable: `wcspr_package_hash_key`
  --> wcspr-tests/src/wcspr_tests.rs:85:9
   |
85 |     let wcspr_package_hash_key = Key::from(wcspr_package_hash);
   |         ^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_wcspr_package_hash_key`

warning: unused variable: `proxy`
   --> wcspr-tests/src/wcspr_tests.rs:113:22
    |
113 |     let (env, token, proxy, _, owner) = deploy();
    |                      ^^^^^ help: if this is intentional, prefix it with an underscore: `_proxy`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:113:32
    |
113 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:130:32
    |
130 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `proxy`
   --> wcspr-tests/src/wcspr_tests.rs:172:22
    |
172 |     let (env, token, proxy, _, owner) = deploy();
    |                      ^^^^^ help: if this is intentional, prefix it with an underscore: `_proxy`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:172:32
    |
172 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:190:32
    |
190 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:224:32
    |
224 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `owner`
   --> wcspr-tests/src/wcspr_tests.rs:258:32
    |
258 |     let (env, token, proxy, _, owner) = deploy();
    |                                ^^^^^ help: if this is intentional, prefix it with an underscore: `_owner`

warning: unused variable: `env`
   --> wcspr-tests/src/wcspr_tests.rs:403:10
    |
403 |     let (env, token, proxy, proxy2, owner) = deploy();
    |          ^^^ help: if this is intentional, prefix it with an underscore: `_env`

warning: unused variable: `token`
   --> wcspr-tests/src/wcspr_tests.rs:403:15
    |
403 |     let (env, token, proxy, proxy2, owner) = deploy();
    |               ^^^^^ help: if this is intentional, prefix it with an underscore: `_token`

warning: unused variable: `env`
   --> wcspr-tests/src/wcspr_tests.rs:419:10
    |
419 |     let (env, token, proxy, proxy2, owner) = deploy();
    |          ^^^ help: if this is intentional, prefix it with an underscore: `_env`

warning: unused variable: `token`
   --> wcspr-tests/src/wcspr_tests.rs:419:15
    |
419 |     let (env, token, proxy, proxy2, owner) = deploy();
    |               ^^^^^ help: if this is intentional, prefix it with an underscore: `_token`

warning: `wcspr-tests` (lib test) generated 16 warnings
    Finished test [unoptimized + debuginfo] target(s) in 0.06s
     Running unittests (target/debug/deps/wcspr_tests-82dc7f50f2424493)

running 14 tests
test wcspr_tests::test_wcspr_deposit_more_than_u256_limit - should panic ... ok
test wcspr_tests::test_wcspr_deploy ... ok
test wcspr_tests::test_wcspr_deposit_invalid_access_rights_purse - should panic ... ok
test wcspr_tests::test_wcspr_approve ... ok
test wcspr_tests::test_wcspr_transfer_too_much - should panic ... ok
test wcspr_tests::test_wcspr_withdraw_no_deposit - should panic ... ok
test wcspr_tests::test_wcspr_deposit_too_much - should panic ... ok
test wcspr_tests::test_wcspr_transfer_from_too_much - should panic ... ok
test wcspr_tests::test_wcspr_deposit ... ok
test wcspr_tests::test_wcspr_withdraw_too_much - should panic ... ok
test wcspr_tests::test_wcspr_withdraw_more_than_u256_limit - should panic ... ok
test wcspr_tests::test_wcspr_increase_allowance ... ok
test wcspr_tests::test_wcspr_decrease_allowance ... ok
test wcspr_tests::test_wcspr_withdraw ... ok

test result: ok. 14 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 6.23s

   Doc-tests wcspr-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
# Test Factory
cd ./factory/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cargo build --release -p factory --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/factory.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../flashswapper/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../pair/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../wcspr/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
# cp ../erc20/target/wasm32-unknown-unknown/release/*.wasm factory-tests/wasm
cargo test -p factory-tests
warning: unused import: `std::collections::BTreeMap`
 --> factory-tests/src/factory_tests.rs:1:5
  |
1 | use std::collections::BTreeMap;
  |     ^^^^^^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default
help: consider adding a `#[cfg(test)]` to the containing module
 --> factory-tests/src/lib.rs:2:1
  |
2 | pub mod factory_tests;
  | ^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `ContractPackageHash`
 --> factory-tests/src/factory_tests.rs:4:41
  |
4 |     account::AccountHash, runtime_args, ContractPackageHash, Key, RuntimeArgs, U256,
  |                                         ^^^^^^^^^^^^^^^^^^^
  |
help: consider adding a `#[cfg(test)]` to the containing module
 --> factory-tests/src/lib.rs:2:1
  |
2 | pub mod factory_tests;
  | ^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `std::collections::BTreeMap`
 --> factory-tests/src/factory_instance.rs:1:5
  |
1 | use std::collections::BTreeMap;
  |     ^^^^^^^^^^^^^^^^^^^^^^^^^^

warning: unused imports: `CLTyped`, `ContractPackageHash`, `U256`
 --> factory-tests/src/factory_instance.rs:8:61
  |
8 |     account::AccountHash, bytesrepr::ToBytes, runtime_args, CLTyped, ContractPackageHash, Key,
  |                                                             ^^^^^^^  ^^^^^^^^^^^^^^^^^^^
9 |     RuntimeArgs, U256,
  |                  ^^^^

warning: `factory-tests` (lib test) generated 4 warnings
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests (target/debug/deps/factory_tests-4c5d57042d9748b4)

running 7 tests
test factory_tests::test_factory_deploy ... ok
test factory_tests::test_calling_construction - should panic ... ok
test factory_tests::test_factory_set_fee_to_setter ... ok
test factory_tests::test_factory_set_white_list_with_non_owner - should panic ... ok
test factory_tests::test_factory_set_white_list ... ok
test factory_tests::test_factory_set_fee_to ... ok
test factory_tests::test_factory_create_pair ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 7.63s

   Doc-tests factory-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
# Test Flashswapper
cd ./flashswapper/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cargo build --release -p flashswapper --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/flashswapper-token.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm flashswapper-tests/wasm
cargo test -p flashswapper-tests
    Finished test [unoptimized + debuginfo] target(s) in 0.06s
     Running unittests (target/debug/deps/flashswapper_tests-c4cacba29e659e05)

running 2 tests
test flash_swapper_tests::test_flash_swapper_deploy ... ok
test flash_swapper_tests::test_calling_construction - should panic ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.77s

   Doc-tests flashswapper-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
# Test Pair
cd ./pair/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p pair --target wasm32-unknown-unknown
warning: value assigned to `liquidity` is never read
    --> pair/src/pair.rs:1005:17
     |
1005 |         let mut liquidity: U256 = 0.into();
     |                 ^^^^^^^^^
     |
     = note: `#[warn(unused_assignments)]` on by default
     = help: maybe it is overwritten before being read?

warning: `pair` (lib) generated 1 warning
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/pair-token.wasm 2>/dev/null | true
cargo build --release -p test --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/pair-test.wasm 2>/dev/null | true
cargo build --release -p test2 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.06s
wasm-strip target/wasm32-unknown-unknown/release/pair-test2.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm pair-tests/wasm
cargo test -p pair-tests
    Finished test [unoptimized + debuginfo] target(s) in 0.06s
     Running unittests (target/debug/deps/pair_tests-4668cd4577f5973b)

running 15 tests
test pair_tests::test_calling_construction - should panic ... ok
test pair_tests::test_pair_transfer_too_much - should panic ... ok
test pair_tests::test_pair_deploy ... ok
test pair_tests::test_pair_approve ... ok
test pair_tests::test_pair_transfer ... ok
test pair_tests::test_pair_transfer_with_same_sender_and_recipient ... ok
test pair_tests::test_pair_set_treasury_fee_percent ... ok
test pair_tests::test_pair_transfer_from ... ok
test pair_tests::test_pair_transfer_from_too_much - should panic ... ok
test pair_tests::test_pair_initialize ... ok
test pair_tests::test_pair_sync ... ok
test pair_tests::test_pair_mint ... ok
test pair_tests::test_pair_skim ... ok
test pair_tests::test_pair_swap ... ok
test pair_tests::test_pair_burn ... ok

test result: ok. 15 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 23.48s

   Doc-tests pair-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
