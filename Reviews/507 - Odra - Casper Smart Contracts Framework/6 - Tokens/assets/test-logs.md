```bash
mehmet@fedora~/Desktop/odra (release/0.5.0)$ just test
cargo test
    Finished test [unoptimized + debuginfo] target(s) in 0.23s
     Running unittests src/lib.rs (target/debug/deps/odra-3fb4729dbda7e219)

running 19 tests
test list::tests::test_getting_items ... ok
test list::tests::test_fuse_iter ... ok
test list::tests::test_list_len ... ok
test list::tests::test_double_ended_iter ... ok
test list::tests::test_pop ... ok
test list::tests::test_iter ... ok
test list::tests::test_list_is_empty ... ok
test mapping::tests::test_get ... ok
test mapping::tests::get_default_value ... ok
test mapping::tests::test_instances_with_the_same_namespace ... ok
test sequence::tests::it_works ... ok
test mapping::tests::test_add ... ok
test list::tests::test_replace ... ok
test mapping::tests::test_subtract ... ok
test variable::tests::test_get ... ok
test variable::tests::test_add ... ok
test variable::tests::get_default_value ... ok
test variable::tests::test_instances_with_the_same_namespace ... ok
test variable::tests::test_subtract ... ok

test result: ok. 19 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_backend-e6ddc588256b4879)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_codegen-8d93dcb580f1f557)

running 26 tests
test arg::tests::test_empty_args ... ok
test arg::tests::test_two_args ... ok
test ty::odra::tests::test_bool ... ok
test ty::odra::tests::test_complex_map ... ok
test ty::odra::tests::test_complex_option ... ok
test ty::odra::tests::test_byte_array ... ok
test ty::odra::tests::test_i32 ... ok
test ty::casper::tests::test_complex_type ... ok
test ty::odra::tests::test_complex_vec ... ok
test entrypoints_def::test::parse_cl_type ... ok
test ty::odra::tests::test_option ... ok
test ty::odra::tests::test_map ... ok
test ty::odra::tests::test_result ... ok
test ty::odra::tests::test_slice ... ok
test ty::odra::tests::test_tuple1 ... ok
test ty::odra::tests::test_tuple2 ... ok
test ty::casper::tests::test_simple_type ... ok
test ty::odra::tests::test_u256 ... ok
test ty::odra::tests::test_tuple3 ... ok
test ty::odra::tests::test_vec ... ok
test ty::odra::tests::test_complex_result ... ok
test constructor::tests::test_constructor ... ok
test wasm_entrypoint::tests::test_mutable ... ok
test wasm_entrypoint::tests::test_constructor ... ok
test wasm_entrypoint::tests::test_payable ... ok
test tests::test_contract_codegen ... ok

test result: ok. 26 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.01s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_livenet-fcb1d66ab253e6c0)

running 6 tests
test casper_client::tests::client_works ... ignored
test casper_client::tests::discover_contract_address ... ignored
test casper_client::tests::get_deploy ... ignored
test casper_client::tests::parsing ... ignored
test casper_client::tests::query_global_state_for_contract ... ignored
test casper_client::tests::state_root_hash ... ignored

test result: ok. 0 passed; 0 failed; 6 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_proxy_caller-af0700ea66c968cc)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_shared-1001d09a68c1497d)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_test_env-5ce1f778f8922212)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_types-842d8e9143694fe6)

running 5 tests
test uints::tests::test_u256_to_512 ... ok
test casper_address::tests::test_casper_address_contract_package_hash_conversion ... ok
test casper_address::tests::test_casper_address_from_to_string ... ok
test casper_address::tests::test_casper_address_account_hash_conversion ... ok
test uints::tests::test_u512_to_256 ... ok

test result: ok. 5 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_codegen-32e3a154fa391733)

running 1 test
test generator::module_item::test::test ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_ir-26121f81c234e8f2)

running 18 tests
test attrs::tests::non_odra_attr_works ... ok
test attrs::tests::constructor_attr_works ... ok
test attrs::tests::payable_attr_works ... ok
test attrs::tests::duplicated_attrs_fail ... ok
test attrs::tests::constructor_cannot_be_payable ... ok
test mapping::test::parsing_complex_expressions_works ... ok
test mapping::test::basic_parsing_works ... ok
test module_item::constructor::test::test_attrs ... ok
test mapping::test::assigning_parsing_works ... ok
test module_item::impl_item::test::test_parse_other_impl_item ... ok
test module_item::impl_item::test::test_parse_fn_without_odra_attr ... ok
test module_item::impl_item::test::test_parse_fn_without_any_attr ... ok
test module_item::tests::impl_block ... ok
test module_item::tests::invalid_usage ... ok
test module_item::tests::struct_block ... ok
test module_item::impl_item::test::test_parse_fn_with_odra_init_attr ... ok
test module_item::module_struct::test::test ... ok
test module_item::module_impl::test::impl_items_filtering ... ok

test result: ok. 18 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_mock_vm-f355a5f5411d519a)

running 31 tests
test contract_container::tests::test_all_missing_args_are_caught ... ignored, At the moment is impossible to find the name of all missing args.
test contract_container::tests::test_call_invalid_constructor ... ok
test contract_container::tests::test_call_constructor_in_invalid_context ... ok
test contract_container::tests::test_call_valid_constructor ... ok
test contract_container::tests::test_call_valid_entrypoint ... ok
test contract_container::tests::test_call_valid_constructor_with_missing_arg ... ok
test contract_container::tests::test_call_valid_entrypoint_with_missing_arg ... ok
test contract_container::tests::test_call_valid_entrypoint_with_wrong_arg_name ... ok
test contract_container::tests::test_call_wrong_entrypoint ... ok
test mock_vm::tests::addresses_have_different_type ... ok
test mock_vm::tests::contracts_have_different_addresses ... ok
test mock_vm::tests::events ... ok
test mock_vm::tests::test_call_non_existing_contract ... ok
test mock_vm::tests::test_call_contract_with_amount ... ok
test mock_vm::tests::test_call_non_existing_entrypoint ... ok
test mock_vm::tests::test_call_contract_with_amount_exceeding_balance - should panic ... ok
test mock_vm::tests::test_caller_switching ... ok
test mock_vm::tests::test_contract_call ... ok
test mock_vm::tests::test_current_contract_address ... ok
test mock_vm::tests::test_read_write_value ... ok
test storage::test::drop_snapshot ... ok
test mock_vm::tests::test_revert ... ok
test storage::test::override_single_value ... ok
test storage::test::read_from_non_existing_collection_returns_none ... ok
test storage::test::read_from_non_existing_key_from_existing_collection_returns_none ... ok
test storage::test::read_non_existing_key_returns_none ... ok
test storage::test::read_write_dict_value ... ok
test storage::test::read_write_single_value ... ok
test storage::test::restore_snapshot ... ok
test mock_vm::tests::test_read_write_dict ... ok
test storage::test::test_snapshot_override ... ok

test result: ok. 30 passed; 0 failed; 1 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_mock_vm_types-fd4934a71e99d5ee)

running 12 tests
test mock_vm_type::tests::test_bool ... ok
test mock_vm_type::tests::test_basic_ints ... ok
test mock_vm_type::tests::test_address ... ok
test call_args::test::test_args ... ok
test mock_vm_type::tests::test_complex_example ... ok
test mock_vm_type::tests::test_large_ints ... ok
test mock_vm_type::tests::test_option ... ok
test mock_vm_type::tests::test_result ... ok
test mock_vm_type::tests::test_string ... ok
test mock_vm_type::tests::test_tuples ... ok
test mock_vm_type::tests::test_unit ... ok
test mock_vm_type::tests::test_vec ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_proc_macros-a46b1da314dfc534)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_types-227328c3bcb129a3)

running 2 tests
test arithmetic::test::test_add ... ok
test arithmetic::test::test_sub ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_utils-9110730918e9ea7e)

running 2 tests
test tests::event_absolute_position_works ... ok
test tests::camel_to_snake_works ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra

running 2 tests
test src/test_utils.rs - test_utils::assert_events (line 26) ... ignored
test src/instance.rs - instance::Instance (line 9) ... ok

test result: ok. 1 passed; 0 failed; 1 ignored; 0 measured; 0 filtered out; finished in 0.33s

   Doc-tests odra-casper-backend

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-codegen

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-livenet

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-proxy-caller

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-shared

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-test-env

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-types

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-codegen

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-ir

running 3 tests
test src/module_item/constructor.rs - module_item::constructor::Constructor (line 11) ... ok
test src/module_item/method.rs - module_item::method::Method (line 10) ... ok
test src/module_item/module_impl.rs - module_item::module_impl::ModuleImpl (line 13) ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.87s

   Doc-tests odra-mock-vm

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-mock-vm-types

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-proc-macros

running 7 tests
test src/lib.rs - execution_error (line 168) - compile fail ... ok
test src/lib.rs - execution_error (line 154) - compile fail ... ok
test src/lib.rs - module (line 27) ... ok
test src/lib.rs - map (line 199) ... ok
test src/lib.rs - derive_event (line 94) ... ok
test src/lib.rs - external_contract (line 70) ... ok
test src/lib.rs - execution_error (line 139) ... ok

test result: ok. 7 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.53s

   Doc-tests odra-types

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-utils

running 2 tests
test src/lib.rs - event_absolute_position (line 25) ... ok
test src/lib.rs - camel_to_snake (line 7) ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.25s

cd examples && cargo odra test
💁  INFO : Testing against MockVM ...
💁  INFO : Running cargo test...
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/odra_examples-d6503b58b854de55)

running 35 tests
test contracts::balance_checker::tests::is_module ... ok
test contracts::owned_token::tests::change_ownership_works ... ok
test contracts::balance_checker::tests::balance_checker ... ok
test contracts::owned_token::tests::init_works ... ok
test contracts::owned_token::tests::mint_works ... ok
test contracts::tlw::test::second_deposit_for_the_same_user_should_fail ... ok
test contracts::owned_token::tests::change_ownership_error ... ok
test contracts::tlw::test::test_successful_withdrawal ... ok
test contracts::tlw::test::test_too_early_withdrawal ... ok
test contracts::owned_token::tests::mint_error ... ok
test contracts::tlw::test::test_withdraw_too_much ... ok
test contracts::tlw::test::test_deposit ... ok
test contracts::token_manager::test::tokens_count_works ... ok
test features::events::tests::test_party ... ok
test features::cross_calls::tests::test_cross_calls ... ok
test contracts::token_manager::test::get_owner_works ... ok
test features::composer::test::t ... ok
test features::handling_errors::tests::test_owner ... ok
test features::host_functions::tests::host_test ... ok
test features::handling_errors::tests::test_owner_error ... ok
test features::module_nesting::tests::nested_odra_types ... ok
test features::modules::tests::test_modules ... ok
test features::native_token::tests::test_modules ... ok
test contracts::token_manager::test::minting_works ... ok
test features::reentrancy_guard::test::local_recursion_allowed ... ok
test features::reentrancy_guard::test::non_reentrant_function_can_be_called ... ok
test features::reentrancy_guard::test::ref_recursion_not_allowed ... ok
test features::storage::list::tests::init_test ... ok
test features::module_nesting::tests::module_in_mapping_in_mapping ... ok
test features::signature_verifier::test::signature_verification_works ... ok
test features::nested_mapping::test::nested_mapping_works ... ok
test features::storage::mapping::tests::visit_test ... ok
test features::storage::variable::tests::init_test ... ok
test features::testing::tests::test_env ... ok
test contracts::token_manager::test::many_tokens_works ... ok

test result: ok. 35 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.01s

   Doc-tests odra-examples

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cd examples && cargo odra test -b casper
💁  INFO : Preparing casper builder in /home/mehmet/Desktop/odra/examples/.builder_casper directory...
💁  INFO : Generating _wasm.rs files...
    Finished release [optimized] target(s) in 0.15s
     Running `../target/release/contracts_build owned_token balance_checker token_manager nested_mapping time_lock_wallet reentrancy_mock signature_verifier composable_contract nested_odra_types_contract dog_contract dog_contract2 dog_contract3 testing_contract host_contract owned_contract party_contract cross_contract math_engine modules_contract public_wallet`
💁  INFO : Generating wasm files...
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.50s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.39s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.46s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.47s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.42s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.40s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.41s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.44s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.43s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.40s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.32s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.36s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.31s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.35s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.35s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.27s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.35s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.27s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.27s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.30s
💁  INFO : Copying wasm files...
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/owned_token.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/balance_checker.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/token_manager.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/nested_mapping.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/time_lock_wallet.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/reentrancy_mock.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/signature_verifier.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/composable_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/nested_odra_types_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/dog_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/dog_contract2.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/dog_contract3.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/testing_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/host_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/owned_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/party_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/cross_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/math_engine.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/modules_contract.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/examples/wasm/public_wallet.wasm
💁  INFO : Optimizing wasm files...
💁  INFO : Building finished.
💁  INFO : Testing backend: casper...
💁  INFO : Running cargo test...
    Finished test [unoptimized + debuginfo] target(s) in 0.11s
     Running unittests src/lib.rs (target/debug/deps/odra_examples-438153185e9500ca)

running 36 tests
test contracts::balance_checker::tests::is_module ... ok
test contracts::owned_token::tests::change_ownership_error ... ok
test contracts::owned_token::tests::mint_error ... ok
test contracts::tlw::test::second_deposit_for_the_same_user_should_fail ... ok
test contracts::owned_token::tests::change_ownership_works ... ok
test contracts::tlw::test::test_deposit ... ok
test contracts::owned_token::tests::mint_works ... ok
test contracts::balance_checker::tests::balance_checker ... ok
test contracts::owned_token::tests::init_works ... ok
test contracts::tlw::test::test_too_early_withdrawal ... ok
test contracts::tlw::test::test_withdraw_too_much ... ok
test contracts::tlw::test::test_successful_withdrawal ... ok
test features::events::tests::test_party ... ok
test features::composer::test::t ... ok
test contracts::token_manager::test::tokens_count_works ... ok
test features::cross_calls::tests::test_cross_calls ... ok
test features::handling_errors::tests::test_owner ... ok
test features::handling_errors::tests::test_owner_error ... ok
test features::host_functions::tests::host_test ... ok
test features::modules::tests::test_modules ... ok
test contracts::token_manager::test::get_owner_works ... ok
test features::native_token::tests::test_modules ... ok
test features::module_nesting::tests::nested_odra_types ... ok
test features::reentrancy_guard::test::local_recursion_allowed ... ok
test features::reentrancy_guard::test::ref_recursion_not_allowed ... ok
test features::reentrancy_guard::test::non_reentrant_function_can_be_called ... ok
test features::nested_mapping::test::nested_mapping_works ... ok
test contracts::token_manager::test::minting_works ... ok
test features::storage::mapping::tests::visit_test ... ok
test features::storage::list::tests::init_test ... ok
test features::storage::variable::tests::init_test ... ok
test features::signature_verifier::test::signature_verification_works ... ok
test features::module_nesting::tests::module_in_mapping_in_mapping ... ok
test features::testing::tests::test_env ... ok
test features::signature_verifier::test::verify_signature_casper_wallet ... ok
test contracts::token_manager::test::many_tokens_works ... ok

test result: ok. 36 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 8.02s

   Doc-tests odra-examples

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cd modules && cargo odra test
💁  INFO : Testing against MockVM ...
💁  INFO : Running cargo test...
    Finished test [unoptimized + debuginfo] target(s) in 0.07s
     Running unittests src/lib.rs (target/debug/deps/odra_modules-f2bae6dedce5169b)

running 77 tests
test access::ownable::test::plain_ownership_transfer ... ok
test access::ownable::test::init ... ok
test access::ownable::test::two_step_ownership_transfer ... ok
test access::ownable::test::failing_plain_ownership_transfer ... ok
test access::ownable::test::failing_two_step_transfer ... ok
test access::ownable::test::renounce_ownership ... ok
test access::ownable::test::renounce_ownership_fail ... ok
test erc1155_token::tests::balance_of_batch ... ok
test erc1155_token::tests::burn ... ok
test erc1155_token::tests::burn_batch ... ok
test erc1155_token::tests::burn_batch_errors ... ok
test erc1155_token::tests::balance_of_batch_errors ... ok
test erc1155_token::tests::balance_of ... ok
test erc1155_token::tests::burn_errors ... ok
test erc1155_token::tests::mint_batch_errors ... ok
test erc1155_token::tests::mint_batch ... ok
test erc1155_token::tests::mint ... ok
test erc1155_token::tests::safe_batch_transfer_to_invalid_receiver ... ok
test erc1155_token::tests::safe_batch_transfer_errors ... ok
test erc1155_token::tests::safe_transfer_from ... ok
test erc1155_token::tests::safe_batch_transfer_to_valid_receiver_with_data ... ok
test erc1155_token::tests::safe_batch_transfer_from_approved ... ok
test erc1155_token::tests::safe_batch_transfer_from ... ok
test erc1155_token::tests::safe_transfer_to_valid_receiver ... ok
test erc1155_token::tests::safe_transfer_from_approved ... ok
test erc1155_token::tests::safe_transfer_to_valid_receiver_with_data ... ok
test erc1155_token::tests::set_approval_for_all ... ok
test erc1155_token::tests::safe_batch_transfer_to_valid_receiver ... ok
test erc1155_token::tests::safe_transfer_from_errors ... ok
test erc1155_token::tests::set_approval_to_self ... ok
test erc1155_token::tests::unset_approval_for_all ... ok
test erc20::tests::transfer_works ... ok
test erc20::tests::transfer_from_and_approval_work ... ok
test erc20::tests::transfer_error ... ok
test erc721_token::tests::approve_non_existing_token ... ok
test erc20::tests::initialization ... ok
test erc721_token::tests::approve_not_owned_token ... ok
test erc721_token::tests::approve ... ok
test erc721_token::tests::balance_of ... ok
test erc20::tests::transfer_from_error ... ok
test erc721_token::tests::burn_error ... ok
test erc721_token::tests::burn_non_existing_nft ... ok
test erc721_token::tests::metadata ... ok
test erc721_token::tests::cancel_approve ... ok
test erc1155_token::tests::safe_transfer_to_invalid_receiver ... ok
test erc721_token::tests::finding_owner ... ok
test erc721_token::tests::cancel_an_operator ... ok
test erc721_token::tests::finding_owner_of_non_existing_token ... ok
test erc721_token::tests::minting_by_not_an_owner ... ok
test erc721_token::tests::burn ... ok
test erc721_token::tests::minting_same_id ... ok
test erc721_token::tests::mints_nft ... ok
test erc721_token::tests::safe_transfer_to_contract_which_does_not_support_nft ... ok
test erc721_token::tests::set_an_operator ... ok
test erc721_token::tests::safe_transfer ... ok
test erc721_token::tests::transfer_approved ... ok
test erc721_token::tests::transfer_nft ... ok
test erc721_token::tests::transfer_not_owned ... ok
test erc721_token::tests::safe_transfer_to_contract_which_supports_nft ... ok
test erc721_token::tests::transferring_invalid_nft ... ok
test erc721_token::tests::safe_transfer_to_contract_with_data ... ok
test erc721_token::tests::transfer_operator ... ok
test mock::access_control::test::add_admin ... ok
test mock::pauseable::test::cannot_pause_paused ... ok
test mock::access_control::test::add_moderators ... ok
test mock::pauseable::test::pause_works ... ok
test mock::pauseable::test::increment_only_if_unpaused ... ok
test wrapped_native::tests::test_deposit ... ok
test wrapped_native::tests::test_deposit_amount_exceeding_account_balance ... ok
test wrapped_native::tests::test_init ... ok
test wrapped_native::tests::test_withdrawal ... ok
test mock::access_control::test::deploy_works ... ok
test wrapped_native::tests::test_withdrawal_amount_exceeding_account_deposit ... ok
test wrapped_native::tests::test_minting ... ok
test mock::pauseable::test::cannot_unpause_unpaused ... ok
test mock::access_control::test::renounce_moderator_role ... ok
test mock::access_control::test::remove_moderator ... ok

test result: ok. 77 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.01s

   Doc-tests odra-modules

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cd modules && cargo odra test -b casper
💁  INFO : Preparing casper builder in /home/mehmet/Desktop/odra/modules/.builder_casper directory...
💁  INFO : Generating _wasm.rs files...
    Finished release [optimized] target(s) in 0.09s
     Running `../target/release/contracts_build erc20 erc721_token erc721_receiver erc1155_token erc1155_receiver wrapped_native_token ownable ownable2_step mock_moderated pauseable_counter`
💁  INFO : Generating wasm files...
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.39s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.46s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.34s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.42s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.29s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.39s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.33s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.29s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.31s
   Compiling builder v1.0.0 (/home/mehmet/Desktop/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.28s
💁  INFO : Copying wasm files...
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/erc20.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/erc721_token.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/erc721_receiver.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/erc1155_token.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/erc1155_receiver.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/wrapped_native_token.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/ownable.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/ownable2_step.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/mock_moderated.wasm
💁  INFO : Saving /home/mehmet/Desktop/odra/modules/wasm/pauseable_counter.wasm
💁  INFO : Optimizing wasm files...
💁  INFO : Building finished.
💁  INFO : Testing backend: casper...
💁  INFO : Running cargo test...
    Finished test [unoptimized + debuginfo] target(s) in 0.11s
     Running unittests src/lib.rs (target/debug/deps/odra_modules-dbde20de66e11a6d)

running 77 tests
test access::ownable::test::failing_plain_ownership_transfer ... ok
test access::ownable::test::plain_ownership_transfer ... ok
test access::ownable::test::init ... ok
test access::ownable::test::two_step_ownership_transfer ... ok
test access::ownable::test::renounce_ownership_fail ... ok
test access::ownable::test::failing_two_step_transfer ... ok
test access::ownable::test::renounce_ownership ... ok
test erc1155_token::tests::balance_of_batch_errors ... ok
test erc1155_token::tests::balance_of_batch ... ok
test erc1155_token::tests::balance_of ... ok
test erc1155_token::tests::burn ... ok
test erc1155_token::tests::burn_batch ... ok
test erc1155_token::tests::mint ... ok
test erc1155_token::tests::mint_batch_errors ... ok
test erc1155_token::tests::mint_batch ... ok
test erc1155_token::tests::burn_errors ... ok
test erc1155_token::tests::burn_batch_errors ... ok
test erc1155_token::tests::safe_batch_transfer_from ... ok
test erc1155_token::tests::safe_batch_transfer_to_invalid_receiver ... ok
test erc1155_token::tests::safe_transfer_from ... ok
test erc1155_token::tests::safe_batch_transfer_errors ... ok
test erc1155_token::tests::safe_batch_transfer_from_approved ... ok
test erc1155_token::tests::safe_batch_transfer_to_valid_receiver ... ok
test erc1155_token::tests::safe_batch_transfer_to_valid_receiver_with_data ... ok
test erc1155_token::tests::safe_transfer_from_approved ... ok
test erc1155_token::tests::set_approval_for_all ... ok
test erc1155_token::tests::set_approval_to_self ... ok
test erc1155_token::tests::safe_transfer_to_invalid_receiver ... ok
test erc1155_token::tests::safe_transfer_to_valid_receiver ... ok
test erc1155_token::tests::safe_transfer_to_valid_receiver_with_data ... ok
test erc1155_token::tests::safe_transfer_from_errors ... ok
test erc20::tests::initialization ... ok
test erc20::tests::transfer_error ... ok
test erc1155_token::tests::unset_approval_for_all ... ok
test erc20::tests::transfer_from_error ... ok
test erc20::tests::transfer_works ... ok
test erc721_token::tests::approve_non_existing_token ... ok
test erc20::tests::transfer_from_and_approval_work ... ok
test erc721_token::tests::approve ... ok
test erc721_token::tests::approve_not_owned_token ... ok
test erc721_token::tests::burn_error ... ok
test erc721_token::tests::burn ... ok
test erc721_token::tests::balance_of ... ok
test erc721_token::tests::burn_non_existing_nft ... ok
test erc721_token::tests::finding_owner_of_non_existing_token ... ok
test erc721_token::tests::finding_owner ... ok
test erc721_token::tests::cancel_an_operator ... ok
test erc721_token::tests::minting_by_not_an_owner ... ok
test erc721_token::tests::cancel_approve ... ok
test erc721_token::tests::metadata ... ok
test erc721_token::tests::minting_same_id ... ok
test erc721_token::tests::mints_nft ... ok
test erc721_token::tests::safe_transfer ... ok
test erc721_token::tests::set_an_operator ... ok
test erc721_token::tests::safe_transfer_to_contract_which_does_not_support_nft ... ok
test erc721_token::tests::transfer_nft ... ok
test erc721_token::tests::transfer_approved ... ok
test erc721_token::tests::safe_transfer_to_contract_which_supports_nft ... ok
test erc721_token::tests::safe_transfer_to_contract_with_data ... ok
test erc721_token::tests::transfer_not_owned ... ok
test erc721_token::tests::transferring_invalid_nft ... ok
test mock::pauseable::test::cannot_pause_paused ... ok
test mock::access_control::test::deploy_works ... ok
test erc721_token::tests::transfer_operator ... ok
test mock::pauseable::test::cannot_unpause_unpaused ... ok
test mock::access_control::test::add_admin ... ok
test mock::access_control::test::add_moderators ... ok
test mock::access_control::test::renounce_moderator_role ... ok
test wrapped_native::tests::test_deposit_amount_exceeding_account_balance ... ok
test mock::pauseable::test::increment_only_if_unpaused ... ok
test mock::pauseable::test::pause_works ... ok
test wrapped_native::tests::test_deposit ... ok
test mock::access_control::test::remove_moderator ... ok
test wrapped_native::tests::test_withdrawal_amount_exceeding_account_deposit ... ok
test wrapped_native::tests::test_init ... ok
test wrapped_native::tests::test_minting ... ok
test wrapped_native::tests::test_withdrawal ... ok

test result: ok. 77 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.61s

   Doc-tests odra-modules

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

```