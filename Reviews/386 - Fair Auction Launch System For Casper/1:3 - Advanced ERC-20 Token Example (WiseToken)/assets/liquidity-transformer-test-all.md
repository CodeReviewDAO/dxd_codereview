```bash
$ make test-all
make build-all && make test
make[1]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
make build-contract
make[2]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cargo build --release -p liquidity_transformer -p scspr -p session-code-lt -p session-code-scspr --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_crate/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_tests/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
    Finished release [optimized] target(s) in 0.06s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
cd ../CasperLabs-UniswapV2-Core/erc20/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20 --target wasm32-unknown-unknown
warning: unused imports: `BlockTime`, `ContractHash`
 --> erc20/src/erc20.rs:8:49
  |
8 |     system::mint::Error as MintError, ApiError, BlockTime, ContractHash, ContractPackageHash, Key,
  |                                                 ^^^^^^^^^  ^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused import: `hex::encode`
  --> erc20/src/erc20.rs:13:5
   |
13 | use hex::encode;
   |     ^^^^^^^^^^^

warning: unused imports: `hash_message`, `keccak256`
  --> erc20/src/erc20.rs:14:17
   |
14 | use renvm_sig::{hash_message, keccak256};
   |                 ^^^^^^^^^^^^  ^^^^^^^^^

warning: `erc20` (lib) generated 3 warnings
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20-token.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cd ../CasperLabs-UniswapV2-Core/factory/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cargo build --release -p factory --target wasm32-unknown-unknown
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/factory.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cd ../CasperLabs-UniswapV2-Core/flashswapper/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cargo build --release -p flashswapper --target wasm32-unknown-unknown
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/flashswapper-token.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cd ../CasperLabs-UniswapV2-Core/pair/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p pair --target wasm32-unknown-unknown
warning: unused import: `BlockTime`
  --> pair/src/pair.rs:13:29
   |
13 |     runtime_args, ApiError, BlockTime, ContractPackageHash, Key, RuntimeArgs, URef, U128, U256,
   |                             ^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::hash_message`
  --> pair/src/pair.rs:17:5
   |
17 | use renvm_sig::hash_message;
   |     ^^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `renvm_sig::keccak256`
  --> pair/src/pair.rs:18:5
   |
18 | use renvm_sig::keccak256;
   |     ^^^^^^^^^^^^^^^^^^^^

warning: value assigned to `liquidity` is never read
   --> pair/src/pair.rs:932:17
    |
932 |         let mut liquidity: U256 = 0.into();
    |                 ^^^^^^^^^
    |
    = note: `#[warn(unused_assignments)]` on by default
    = help: maybe it is overwritten before being read?

warning: `pair` (lib) generated 4 warnings
warning: unused import: `hex::encode`
  --> pair/bin/pair_token.rs:18:5
   |
18 | use hex::encode;
   |     ^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::keccak256`
  --> pair/bin/pair_token.rs:20:5
   |
20 | use renvm_sig::keccak256;
   |     ^^^^^^^^^^^^^^^^^^^^

warning: `pair` (bin "pair-token") generated 2 warnings
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/pair-token.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cd ../CasperLabs-UniswapV2-Core/wcspr/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p wcspr --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-token.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cd ../CasperLabs-UniswapV2-Router/uniswap-v2-library/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cargo build --release -p uniswap-v2-library --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.06s
wasm-strip target/wasm32-unknown-unknown/release/uniswap-v2-library.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cd ../CasperLabs-UniswapV2-Router/uniswap-v2-router/ && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
cargo build --release -p uniswap-v2-router --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.06s
wasm-strip uniswap-v2-router/target/wasm32-unknown-unknown/release/uniswap-v2-router.wasm 2>/dev/null | true
make[2]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
cd ../CasperLabs-StakeableToken/ && make build-all
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
make build-stakeable-token
make[3]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p stakeable-token -p session-code-stakeable --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.07s
make[3]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make build-liquidity-guard
make[3]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p liquidity-guard -p session-code-liquidity-guard --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.06s
make[3]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
cd . && make build-contract
make[2]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cargo build --release -p liquidity_transformer -p scspr -p session-code-lt -p session-code-scspr --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_crate/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_tests/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
make copy-wasm-file
make[2]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-router/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-library/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-StakeableToken/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ./target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-router/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-library/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-StakeableToken/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ./target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
make[2]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
make[1]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
make test-liquidity-transformer && make test-scspr
make[2]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cargo test -p liquidity_transformer_tests
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_crate/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_tests/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.07s
     Running unittests src/lib.rs (target/debug/deps/liquidity_transformer_tests-304fc08f6adbe81c)

running 12 tests
test liquidity_transformer_tests::test_set_settings ... ok
test liquidity_transformer_tests::test_prepare_path ... ok
test liquidity_transformer_tests::test_renounce_keeper ... ok
test liquidity_transformer_tests::test_current_stakeable_day ... ok
test liquidity_transformer_tests::test_deploy ... ok
test liquidity_transformer_tests::test_reserve_wise ... ok
test liquidity_transformer_tests::test_request_refund ... ok
test liquidity_transformer_flow_tests::test_reserve_claim_flow has been running for over 60 seconds
test liquidity_transformer_tests::test_forward_liquidity has been running for over 60 seconds
test liquidity_transformer_tests::test_get_my_tokens has been running for over 60 seconds
test liquidity_transformer_tests::test_payout_investor_address has been running for over 60 seconds
test liquidity_transformer_tests::test_reserve_wise_with_token has been running for over 60 seconds
test liquidity_transformer_tests::test_reserve_wise_with_token ... ok
test liquidity_transformer_tests::test_forward_liquidity ... ok
test liquidity_transformer_tests::test_get_my_tokens ... ok
test liquidity_transformer_tests::test_payout_investor_address ... ok
test liquidity_transformer_flow_tests::test_reserve_claim_flow ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 72.95s

   Doc-tests liquidity_transformer_tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
make[2]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cargo test -p scspr_tests
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_crate/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_tests/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.07s
     Running unittests src/lib.rs (target/debug/deps/scspr_tests-7c5ca533da1bbbeb)

running 3 tests
test scspr_tests::should_not_allow_to_withdraw_cspr_if_user_do_not_have_scspr - should panic ... ok
test scspr_tests::should_allow_to_do_deposit_cspr_and_withdraw_scspr ... ok
test scspr_tests::master_add_lp_tokens_should_work_correctly has been running for over 60 seconds
test scspr_tests::master_add_lp_tokens_should_work_correctly ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 70.65s

   Doc-tests scspr_tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
make[1]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
```
