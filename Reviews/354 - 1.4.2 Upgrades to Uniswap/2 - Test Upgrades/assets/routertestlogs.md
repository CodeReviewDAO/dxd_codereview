# Test Library
cd ./uniswap-v2-library/ && make test
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cargo build --release -p uniswap-v2-library --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/uniswap-v2-library.wasm 2>/dev/null | true
cp target/wasm32-unknown-unknown/release/*.wasm uniswap-v2-library-tests/wasm
cargo test -p uniswap-v2-library-tests
   Compiling test-env v0.1.0 (/workspace/CasperLabs-UniswapV2-Router/utils/test-env)
error[E0308]: mismatched types
  --> /workspace/CasperLabs-UniswapV2-Router/utils/test-env/src/test_env.rs:83:23
   |
83 |                 .exec(fund_account(&account_hash))
   |                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^ expected struct `casper_execution_engine::core::engine_state::execute_request::ExecuteRequest`, found struct `ExecuteRequest`
   |
   = note: perhaps two different versions of crate `casper_execution_engine` are being used?

error[E0308]: mismatched types
   --> /workspace/CasperLabs-UniswapV2-Router/utils/test-env/src/test_env.rs:102:23
    |
102 |                 .exec(fund_account(&account_hash))
    |                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^ expected struct `casper_execution_engine::core::engine_state::execute_request::ExecuteRequest`, found struct `ExecuteRequest`
    |
    = note: perhaps two different versions of crate `casper_execution_engine` are being used?

error[E0308]: mismatched types
  --> /workspace/CasperLabs-UniswapV2-Router/utils/test-env/src/utils.rs:42:5
   |
29 | pub fn fund_account(account: &AccountHash) -> ExecuteRequest {
   |                                               -------------- expected `ExecuteRequest` because of return type
...
42 |     ExecuteRequestBuilder::from_deploy_item(deploy_item).build()
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ expected struct `ExecuteRequest`, found struct `casper_execution_engine::core::engine_state::execute_request::ExecuteRequest`
   |
   = note: perhaps two different versions of crate `casper_execution_engine` are being used?

For more information about this error, try `rustc --explain E0308`.
error: could not compile `test-env` due to 3 previous errors
make[1]: *** [Makefile:9: test-only] Error 101
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
make: *** [Makefile:90: test] Error 2
