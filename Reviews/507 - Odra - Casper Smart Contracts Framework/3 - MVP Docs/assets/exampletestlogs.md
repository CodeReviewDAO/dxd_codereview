# Output of the "cargo odra test -b casper" command for examples of the project

```sh

💁  [1;32mINFO :[0m [32mPreparing casper builder in .builder_casper directory...[0m
💁  [1;32mINFO :[0m [32mGenerating _wasm.rs files...[0m
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/owned_token_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/balance_checker_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/ownable_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/erc20_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/time_lock_wallet_build`
💁  [1;32mINFO :[0m [32mGenerating wasm files...[0m
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.58s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.39s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.39s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.46s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.43s
💁  [1;32mINFO :[0m [32mCopying wasm files...[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/owned_token.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/balance_checker.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/ownable.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/erc20.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/time_lock_wallet.wasm[0m
💁  [1;32mINFO :[0m [32mRunning cargo test...[0m
    Finished test [unoptimized + debuginfo] target(s) in 0.08s
     Running unittests src/lib.rs (target/debug/deps/odra_examples-2da85d0cd3bba6c1)

running 19 tests
test ownable::tests::initialization_works ... ok
test ownable::tests::owner_can_change_ownership ... ok
test ownable::tests::non_owner_cannot_change_ownership ... ok
test erc20::tests::transfer_from_error ... ok
test erc20::tests::transfer_error ... ok
test tlw::test::second_deposit_for_the_same_user_should_fail ... ok
test owned_token::tests::change_ownership_error ... ok
test owned_token::tests::mint_error ... ok
test erc20::tests::transfer_works ... ok
test owned_token::tests::change_ownership_works ... ok
test erc20::tests::initialization ... ok
test owned_token::tests::mint_works ... ok
test tlw::test::test_deposit ... ok
test balance_checker::tests::balance_checker ... ok
test tlw::test::test_too_early_withdrawal ... ok
test owned_token::tests::init_works ... ok
test erc20::tests::transfer_from_and_approval_work ... ok
test tlw::test::test_withdraw_too_much ... ok
test tlw::test::test_successful_withdrawal ... ok

test result: ok. 19 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.12s

   Doc-tests odra-examples

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

```

