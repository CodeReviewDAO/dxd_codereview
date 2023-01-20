```     
make test 
cargo build --release --target wasm32-unknown-unknown  -p erc777-token  -p erc1820-registry  -p erc777-recipient-contract  -p erc777-sender-contract
   Compiling casper-erc777 v0.2.1 (CasperLabs-ERC777/erc777)
   Compiling erc777-token v0.0.1 (CasperLabs-ERC777/example/implementations/erc777-token)
    Finished release [optimized] target(s) in 20.48s
wasm-strip target/wasm32-unknown-unknown/release/erc777_token.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc1820_registry.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc777_recipient_contract.wasm 2>/dev/null | true;  wasm-strip target/wasm32-unknown-unknown/release/erc777_sender_contract.wasm 2>/dev/null | true;
cargo test
   Compiling casper-erc777 v0.2.1 (CasperLabs-ERC777/erc777)
   Compiling erc777-sender-tests v0.0.1 (CasperLabs-ERC777/example/tests/erc777-sender-tests)
   Compiling erc777-tests v0.0.1 (CasperLabs-ERC777/example/tests/erc777-tests)
   Compiling erc777-recipient-tests v0.0.1 (CasperLabs-ERC777/example/tests/erc777-recipient-tests)
   Compiling erc20-tests v0.0.1 (CasperLabs-ERC777/example/tests/erc20-tests)
    Finished test [unoptimized + debuginfo] target(s) in 2m 36s
     Running unittests src/lib.rs (target/debug/deps/casper_erc1820-b21b20798f1c9ffa)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/casper_erc777-2218461044877a0e)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/casper_erc777_recipient-aa25bc5b1664ff5d)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/casper_erc777_sender-dc113c818c8e8300)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/integration_tests.rs (target/debug/deps/erc1820_tests-04a61298e9cd027f)

running 7 tests
test tests::should_not_set_manager - should panic ... ok
test tests::should_not_register_an_implementer_with_same_caller_address - should panic ... ok
test tests::should_not_register_an_implementer_with_address_zero - should panic ... ok
test tests::should_not_register_an_implementer - should panic ... ok
test tests::should_register_a_recipient ... ok
test tests::should_register_a_sender ... ok
test tests::should_set_manager ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 2.08s

     Running unittests src/integration_tests.rs (target/debug/deps/erc20_tests-47a987e23bd5da4e)

running 6 tests
test tests::should_install ... ok
test tests::should_not_transfer_with_insufficient_balance - should panic ... ok
test tests::should_not_transfer_from_more_than_approved - should panic ... ok
test tests::should_transfer ... ok
test tests::should_transfer_from ... ok
test tests::should_transfer_full_amount ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 2.46s

     Running unittests src/integration_tests.rs (target/debug/deps/erc777_recipient_tests-0e7e607aa65b1743)

running 9 tests
test tests::should_install ... ok
test tests::should_send_and_burn ... ok
test tests::should_burn_on_behalf_of ... ok
test tests::should_burn_from_erc777_recipient ... ok
test tests::should_send_on_behalf_of ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_burn_tokens - should panic ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_send_tokens - should panic ... ok
test tests::should_transfer_tokens_by_using_other_owner ... ok
test tests::should_transfer_tokens_from_erc777_recipient ... ok

test result: ok. 9 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 6.75s

     Running unittests src/integration_tests.rs (target/debug/deps/erc777_sender_tests-47801499b226fb30)

running 8 tests
test tests::should_install ... ok
test tests::should_send_and_burn ... ok
test tests::should_burn_on_behalf_of ... ok
test tests::should_burn_from_erc777_sender ... ok
test tests::should_send_on_behalf_of ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_burn_tokens - should panic ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_send_tokens - should panic ... ok
test tests::should_transfer_tokens_from_erc777_sender ... ok

test result: ok. 8 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 5.46s

     Running unittests src/integration_tests.rs (target/debug/deps/erc777_tests-bb58b40ea0d479ab)

running 6 tests
test tests::should_install ... ok
test tests::should_send_on_behalf_of ... ok
test tests::should_send_and_burn ... ok
test tests::should_burn_on_behalf_of ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_burn_tokens - should panic ... ok
test tests::should_throw_an_exception_by_not_having_assigned_operator_to_send_tokens - should panic ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.63s

   Doc-tests casper-erc1820

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests casper-erc777

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests casper-erc777-recipient

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests casper-erc777-sender

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```