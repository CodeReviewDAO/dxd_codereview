```bash
ndpc_contract (main)$ make test
cd contract && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip contract/target/wasm32-unknown-unknown/release/contract.wasm 2>/dev/null | true
cp contract/target/wasm32-unknown-unknown/release/contract.wasm deploy/contract.wasm
mkdir -p tests/wasm
cp contract/target/wasm32-unknown-unknown/release/contract.wasm tests/wasm
cd tests && cargo test
    Finished test [unoptimized + debuginfo] target(s) in 0.09s
     Running unittests (target/debug/deps/integration_tests-3ec908b3a6613094)

running 16 tests
test tests::cancel_request_entry_point_with_error ... ok
test tests::approve_entry_point_with_error ... ok
test tests::cancel_request_entry_point_with_auth_error ... ok
test tests::approve_entry_point_with_auth_error ... ok
test tests::cancel_request_entry_point ... ok
test tests::approve_entry_point ... ok
test tests::disapprove_entry_point_auth_error ... ok
test tests::disapprove_entry_point ... ok
test tests::install_contract_with_error ... ok
test tests::install_contract_test ... ok
test tests::mint_product_with_error ... ok
test tests::mint_entrypoint ... ok
test tests::publish_request_entry_point ... ok
test tests::publish_request_with_error ... ok
test tests::disapprove_entry_point_error_approved_id ... ok
test tests::disapprove_entry_point_error_amount ... ok

test result: ok. 16 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 4.55s

```