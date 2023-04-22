# Output of the "just test" command

```sh


cargo test
    Finished test [unoptimized + debuginfo] target(s) in 0.12s
     Running unittests src/lib.rs (target/debug/deps/odra-424d654bfab1f323)

running 17 tests
test list::tests::test_double_ended_iter ... ok
test list::tests::test_fuse_iter ... ok
test list::tests::test_list_is_empty ... ok
test list::tests::test_iter ... ok
test list::tests::test_getting_items ... ok
test list::tests::test_replace ... ok
test mapping::tests::get_default_value ... ok
test list::tests::test_list_len ... ok
test mapping::tests::test_get ... ok
test mapping::tests::test_add ... ok
test mapping::tests::test_instances_with_the_same_namespace ... ok
test mapping::tests::test_subtract ... ok
test variable::tests::get_default_value ... ok
test variable::tests::test_add ... ok
test variable::tests::test_instances_with_the_same_namespace ... ok
test variable::tests::test_get ... ok
test variable::tests::test_subtract ... ok

test result: ok. 17 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_backend-1c2b7868abb3b4c2)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_codegen-f5270cc82f472756)

running 10 tests
test arg::tests::test_empty_args ... ok
test arg::tests::test_two_args ... ok
test ty::tests::test_simple_type ... ok
test ty::tests::test_complex_type ... ok
test wasm_entrypoint::tests::test_mutable ... ok
test wasm_entrypoint::tests::test_constructor ... ok
test wasm_entrypoint::tests::test_payable ... ok
test entrypoints_def::test::parse_cl_type ... ok
test constructor::tests::test_constructor ... ok
test tests::test_contract_codegen ... ok

test result: ok. 10 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.01s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_shared-4ba438f35d431569)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_test_env-1e548b06f11f3e63)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_casper_types-2b3cdab2d3d1f89c)

running 4 tests
test uints::tests::test_u256_to_512 ... ok
test casper_address::tests::test_casper_address_account_hash_conversion ... ok
test uints::tests::test_u512_to_256 ... ok
test casper_address::tests::test_casper_address_contract_package_hash_conversion ... ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_codegen-34b4c40828756f87)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_ir-162ae5190c7991e1)

running 14 tests
test attrs::tests::non_odra_attr_works ... ok
test attrs::tests::payable_attr_works ... ok
test attrs::tests::constructor_attr_works ... ok
test attrs::tests::duplicated_attrs_fail ... ok
test attrs::tests::constructor_cannot_be_payable ... ok
test module_item::impl_item::test::test_parse_other_impl_item ... ok
test module_item::tests::invalid_usage ... ok
test module_item::tests::impl_block ... ok
test module_item::constructor::test::test_attrs ... ok
test module_item::impl_item::test::test_parse_fn_with_odra_init_attr ... ok
test module_item::tests::struct_block ... ok
test module_item::module_impl::test::impl_items_filtering ... ok
test module_item::impl_item::test::test_parse_fn_without_odra_attr ... ok
test module_item::impl_item::test::test_parse_fn_without_any_attr ... ok

test result: ok. 14 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_mock_vm-081fb7eec4472fdf)

running 30 tests
test contract_container::tests::test_all_missing_args_are_caught ... ignored, At the moment is impossible to find the name of all missing args.
test contract_container::tests::test_call_invalid_constructor ... ok
test contract_container::tests::test_call_constructor_in_invalid_context ... ok
test contract_container::tests::test_call_valid_constructor ... ok
test contract_container::tests::test_call_valid_entrypoint ... ok
test contract_container::tests::test_call_valid_entrypoint_with_wrong_arg_name ... ok
test contract_container::tests::test_call_valid_constructor_with_missing_arg ... ok
test contract_container::tests::test_call_wrong_entrypoint ... ok
test contract_container::tests::test_call_valid_entrypoint_with_missing_arg ... ok
test mock_vm::tests::contracts_have_different_addresses ... ok
test mock_vm::tests::events ... ok
test mock_vm::tests::test_call_contract_with_amount ... ok
test mock_vm::tests::test_call_contract_with_amount_exceeding_balance ... ok
test mock_vm::tests::test_call_non_existing_contract ... ok
test mock_vm::tests::test_caller_switching ... ok
test mock_vm::tests::test_call_non_existing_entrypoint ... ok
test mock_vm::tests::test_current_contract_address ... ok
test mock_vm::tests::test_contract_call ... ok
test mock_vm::tests::test_read_write_value ... ok
test storage::test::override_single_value ... ok
test mock_vm::tests::test_read_write_dict ... ok
test mock_vm::tests::test_revert ... ok
test storage::test::drop_snapshot ... ok
test storage::test::read_from_non_existing_collection_returns_none ... ok
test storage::test::read_non_existing_key_returns_none ... ok
test storage::test::read_from_non_existing_key_from_existing_collection_returns_none ... ok
test storage::test::read_write_single_value ... ok
test storage::test::read_write_dict_value ... ok
test storage::test::restore_snapshot ... ok
test storage::test::test_snapshot_override ... ok

test result: ok. 29 passed; 0 failed; 1 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_mock_vm_types-c9c4225a1090f318)

running 12 tests
test call_args::test::test_args ... ok
test mock_vm_type::tests::test_address ... ok
test mock_vm_type::tests::test_basic_ints ... ok
test mock_vm_type::tests::test_bool ... ok
test mock_vm_type::tests::test_complex_example ... ok
test mock_vm_type::tests::test_large_ints ... ok
test mock_vm_type::tests::test_option ... ok
test mock_vm_type::tests::test_string ... ok
test mock_vm_type::tests::test_result ... ok
test mock_vm_type::tests::test_tuples ... ok
test mock_vm_type::tests::test_unit ... ok
test mock_vm_type::tests::test_vec ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_proc_macros-8802ad2bf95d7db4)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_types-a3f2fb91bec9e0e1)

running 2 tests
test arithmetic::test::test_add ... ok
test arithmetic::test::test_sub ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running unittests src/lib.rs (target/debug/deps/odra_utils-9345c5933459a51c)

running 2 tests
test tests::event_absolute_position_works ... ok
test tests::camel_to_snake_works ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra

running 2 tests
test src/test_utils.rs - test_utils::assert_events (line 26) ... ignored
test src/instance.rs - instance::Instance (line 9) ... ok

test result: ok. 1 passed; 0 failed; 1 ignored; 0 measured; 0 filtered out; finished in 0.20s

   Doc-tests odra-casper-backend

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-casper-codegen

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
test src/module_item/module_impl.rs - module_item::module_impl::ModuleImpl (line 10) ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.66s

   Doc-tests odra-mock-vm

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-mock-vm-types

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-proc-macros

running 6 tests
test src/lib.rs - execution_error (line 157) - compile fail ... ok
test src/lib.rs - execution_error (line 143) - compile fail ... ok
test src/lib.rs - module (line 25) ... ok
test src/lib.rs - derive_event (line 92) ... ok
test src/lib.rs - external_contract (line 68) ... ok
test src/lib.rs - execution_error (line 128) ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.34s

   Doc-tests odra-types

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-utils

running 2 tests
test src/lib.rs - event_absolute_position (line 25) ... ok
test src/lib.rs - camel_to_snake (line 7) ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.18s

cd examples && cargo odra test
💁  [1;32mINFO :[0m [32mRunning cargo test...[0m
    Finished test [unoptimized + debuginfo] target(s) in 0.05s
     Running unittests src/lib.rs (target/debug/deps/odra_examples-bec1d5abe38d9e63)

running 19 tests
test erc20::tests::transfer_error ... ok
test erc20::tests::initialization ... ok
test balance_checker::tests::balance_checker ... ok
test ownable::tests::initialization_works ... ok
test ownable::tests::non_owner_cannot_change_ownership ... ok
test erc20::tests::transfer_from_error ... ok
test erc20::tests::transfer_from_and_approval_work ... ok
test ownable::tests::owner_can_change_ownership ... ok
test erc20::tests::transfer_works ... ok
test owned_token::tests::change_ownership_error ... ok
test owned_token::tests::mint_error ... ok
test owned_token::tests::init_works ... ok
test owned_token::tests::change_ownership_works ... ok
test tlw::test::second_deposit_for_the_same_user_should_fail ... ok
test tlw::test::test_withdraw_too_much ... ok
test owned_token::tests::mint_works ... ok
test tlw::test::test_deposit ... ok
test tlw::test::test_successful_withdrawal ... ok
test tlw::test::test_too_early_withdrawal ... ok

test result: ok. 19 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-examples

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cd examples && cargo odra test -b casper
💁  [1;32mINFO :[0m [32mPreparing casper builder in .builder_casper directory...[0m
💁  [1;32mINFO :[0m [32mGenerating _wasm.rs files...[0m
    Finished release [optimized] target(s) in 0.10s
     Running `../target/release/owned_token_build`
    Finished release [optimized] target(s) in 0.10s
     Running `../target/release/balance_checker_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/ownable_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/erc20_build`
    Finished release [optimized] target(s) in 0.08s
     Running `../target/release/time_lock_wallet_build`
💁  [1;32mINFO :[0m [32mGenerating wasm files...[0m
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.47s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.42s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.40s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.45s
   Compiling builder v1.0.0 (/workspace/odra/examples/.builder_casper)
    Finished release [optimized] target(s) in 0.41s
💁  [1;32mINFO :[0m [32mCopying wasm files...[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/owned_token.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/balance_checker.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/ownable.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/erc20.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/time_lock_wallet.wasm[0m
💁  [1;32mINFO :[0m [32mRunning cargo test...[0m
   Compiling syn v1.0.107
   Compiling autocfg v1.1.0
   Compiling libc v0.2.139
   Compiling typenum v1.16.0
   Compiling serde_derive v1.0.152
   Compiling serde v1.0.152
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling unicode-xid v0.2.4
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling ppv-lite86 v0.2.17
   Compiling byteorder v1.4.3
   Compiling remove_dir_all v0.5.3
   Compiling opaque-debug v0.3.0
   Compiling fastrand v1.8.0
   Compiling serde_json v1.0.91
   Compiling ryu v1.0.12
   Compiling cpufeatures v0.2.5
   Compiling bit-vec v0.6.3
   Compiling fnv v1.0.7
   Compiling schemars v0.8.5
   Compiling bitflags v1.3.2
   Compiling quick-error v1.2.3
   Compiling once_cell v1.17.0
   Compiling hashbrown v0.12.3
   Compiling itoa v1.0.5
   Compiling regex-syntax v0.6.28
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.10
   Compiling lazy_static v1.4.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.1
   Compiling hex_fmt v0.3.0
   Compiling cc v1.0.78
   Compiling pkg-config v0.3.26
   Compiling parity-wasm v0.41.0
   Compiling thiserror v1.0.38
   Compiling log v0.4.17
   Compiling memory_units v0.3.0
   Compiling match_cfg v0.1.0
   Compiling downcast-rs v1.2.0
   Compiling iana-time-zone v0.1.53
   Compiling pin-project-lite v0.2.9
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling odra-casper-shared v0.2.0 (/workspace/odra/odra-casper/shared)
   Compiling diff v0.1.13
   Compiling yansi v0.5.1
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling bit-set v0.5.3
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling tracing-core v0.1.30
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.2
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling pretty_assertions v1.3.0
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.8
   Compiling tempfile v3.3.0
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.45
   Compiling hostname v0.3.1
   Compiling num_cpus v1.15.0
   Compiling lmdb-sys v0.8.0
   Compiling rand_core v0.6.4
   Compiling rusty-fork v0.3.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling rand v0.8.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling ff v0.8.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling group v0.8.0
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling chrono v0.4.23
   Compiling proptest v1.0.0
   Compiling wasmi v0.8.0
   Compiling lmdb v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling proc-macro-error v1.0.4
   Compiling odra-ir v0.2.0 (/workspace/odra/lang/ir)
   Compiling zeroize_derive v1.3.3
   Compiling datasize_derive v0.2.13
   Compiling schemars_derive v0.8.5
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.38
   Compiling tracing-attributes v0.1.23
   Compiling derive_more v0.99.17
   Compiling zeroize v1.3.0
   Compiling datasize v0.2.13
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling k256 v0.7.3
   Compiling ed25519-dalek v1.0.1
   Compiling odra-codegen v0.2.0 (/workspace/odra/lang/codegen)
   Compiling tracing v0.1.37
   Compiling odra-proc-macros v0.2.0 (/workspace/odra/lang/proc-macros)
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.8
   Compiling uuid v0.8.2
   Compiling bincode v1.3.3
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling odra-casper-types v0.2.0 (/workspace/odra/odra-casper/types)
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casper-execution-engine v2.0.1
   Compiling odra-casper-backend v0.2.0 (/workspace/odra/odra-casper/backend)
   Compiling odra-casper-codegen v0.2.0 (/workspace/odra/odra-casper/codegen)
   Compiling casper-engine-test-support v2.2.0
   Compiling odra-casper-test-env v0.2.0 (/workspace/odra/odra-casper/test-env)
   Compiling odra v0.2.0 (/workspace/odra/core)
   Compiling odra-modules v0.2.0 (/workspace/odra/modules)
   Compiling odra-examples v0.2.0 (/workspace/odra/examples)
    Finished test [unoptimized + debuginfo] target(s) in 1m 17s
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
test balance_checker::tests::balance_checker ... ok
test erc20::tests::transfer_works ... ok
test owned_token::tests::change_ownership_works ... ok
test owned_token::tests::mint_works ... ok
test tlw::test::test_deposit ... ok
test erc20::tests::initialization ... ok
test owned_token::tests::init_works ... ok
test tlw::test::test_withdraw_too_much ... ok
test tlw::test::test_too_early_withdrawal ... ok
test erc20::tests::transfer_from_and_approval_work ... ok
test tlw::test::test_successful_withdrawal ... ok

test result: ok. 19 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.41s

   Doc-tests odra-examples

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cd modules && cargo odra test
💁  [1;32mINFO :[0m [32mRunning cargo test...[0m
    Updating crates.io index
   Compiling proc-macro2 v1.0.49
   Compiling version_check v0.9.4
   Compiling unicode-ident v1.0.6
   Compiling quote v1.0.23
   Compiling syn v1.0.107
   Compiling serde v1.0.152
   Compiling libc v0.2.139
   Compiling cfg-if v1.0.0
   Compiling convert_case v0.5.0
   Compiling once_cell v1.17.0
   Compiling crunchy v0.2.2
   Compiling either v1.8.0
   Compiling byteorder v1.4.3
   Compiling hex v0.4.3
   Compiling static_assertions v1.1.0
   Compiling anyhow v1.0.68
   Compiling odra-types v0.2.0 (/workspace/odra/types)
   Compiling ref_thread_local v0.1.1
   Compiling itertools v0.10.5
   Compiling odra-utils v0.2.0 (/workspace/odra/utils)
   Compiling uint v0.9.5
   Compiling proc-macro-error-attr v1.0.4
   Compiling ahash v0.7.6
   Compiling proc-macro-error v1.0.4
   Compiling getrandom v0.2.8
   Compiling hashbrown v0.11.2
   Compiling toml v0.5.10
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive-internal v0.9.3
   Compiling borsh-schema-derive-internal v0.9.3
   Compiling odra-ir v0.2.0 (/workspace/odra/lang/ir)
   Compiling borsh-derive v0.9.3
   Compiling derive_more v0.99.17
   Compiling borsh v0.9.3
   Compiling odra-codegen v0.2.0 (/workspace/odra/lang/codegen)
   Compiling odra-mock-vm-types v0.2.0 (/workspace/odra/mock-vm/types)
   Compiling odra-proc-macros v0.2.0 (/workspace/odra/lang/proc-macros)
   Compiling odra-mock-vm v0.2.0 (/workspace/odra/mock-vm/backend)
   Compiling odra v0.2.0 (/workspace/odra/core)
   Compiling odra-modules v0.2.0 (/workspace/odra/modules)
    Finished test [unoptimized + debuginfo] target(s) in 17.78s
     Running unittests src/lib.rs (target/debug/deps/odra_modules-519864f62f6dd109)

running 11 tests
test erc20::tests::initialization ... ok
test erc20::tests::transfer_from_error ... ok
test erc20::tests::transfer_error ... ok
test wrapped_native::tests::test_deposit_amount_exceeding_account_balance ... ok
test erc20::tests::transfer_works ... ok
test wrapped_native::tests::test_deposit ... ok
test erc20::tests::transfer_from_and_approval_work ... ok
test wrapped_native::tests::test_init ... ok
test wrapped_native::tests::test_withdrawal_amount_exceeding_account_deposit ... ok
test wrapped_native::tests::test_minting ... ok
test wrapped_native::tests::test_withdrawal ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

   Doc-tests odra-modules

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cd modules && cargo odra test -b casper
💁  [1;32mINFO :[0m [32mPreparing casper builder in .builder_casper directory...[0m
💁  [1;32mINFO :[0m [32mGenerating _wasm.rs files...[0m
    Updating crates.io index
   Compiling proc-macro2 v1.0.49
   Compiling quote v1.0.23
   Compiling unicode-ident v1.0.6
   Compiling syn v1.0.107
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling libc v0.2.139
   Compiling serde_derive v1.0.152
   Compiling typenum v1.16.0
   Compiling serde v1.0.152
   Compiling cfg-if v1.0.0
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling ppv-lite86 v0.2.17
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.91
   Compiling remove_dir_all v0.5.3
   Compiling fastrand v1.8.0
   Compiling opaque-debug v0.3.0
   Compiling itoa v1.0.5
   Compiling hashbrown v0.12.3
   Compiling fnv v1.0.7
   Compiling quick-error v1.2.3
   Compiling ryu v1.0.12
   Compiling cpufeatures v0.2.5
   Compiling bitflags v1.3.2
   Compiling once_cell v1.17.0
   Compiling schemars v0.8.5
   Compiling bit-vec v0.6.3
   Compiling lazy_static v1.4.0
   Compiling dyn-clone v1.0.10
   Compiling quick-error v2.0.1
   Compiling static_assertions v1.1.0
   Compiling regex-syntax v0.6.28
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling base16 v0.2.1
   Compiling cc v1.0.78
   Compiling pkg-config v0.3.26
   Compiling log v0.4.17
   Compiling parity-wasm v0.41.0
   Compiling thiserror v1.0.38
   Compiling either v1.8.0
   Compiling anyhow v1.0.68
   Compiling match_cfg v0.1.0
   Compiling pin-project-lite v0.2.9
   Compiling memory_units v0.3.0
   Compiling odra-types v0.2.0 (/workspace/odra/types)
   Compiling iana-time-zone v0.1.53
   Compiling downcast-rs v1.2.0
   Compiling convert_case v0.5.0
   Compiling linked-hash-map v0.5.6
   Compiling filesize v0.2.0
   Compiling diff v0.1.13
   Compiling odra-casper-shared v0.2.0 (/workspace/odra/odra-casper/shared)
   Compiling yansi v0.5.1
   Compiling ref_thread_local v0.1.1
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling proc-macro-error-attr v1.0.4
   Compiling proc-macro-error v1.0.4
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling indexmap v1.9.2
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling tracing-core v0.1.30
   Compiling bit-set v0.5.3
   Compiling itertools v0.10.5
   Compiling odra-utils v0.2.0 (/workspace/odra/utils)
   Compiling pretty_assertions v1.3.0
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling lmdb-sys v0.8.0
   Compiling getrandom v0.2.8
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.45
   Compiling hostname v0.3.1
   Compiling num_cpus v1.15.0
   Compiling rand_core v0.6.4
   Compiling rusty-fork v0.3.0
   Compiling ff v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling group v0.8.0
   Compiling rand v0.8.5
   Compiling num-complex v0.4.2
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling chrono v0.4.23
   Compiling proptest v1.0.0
   Compiling lmdb v0.8.0
   Compiling wasmi v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling odra-ir v0.2.0 (/workspace/odra/lang/ir)
   Compiling zeroize_derive v1.3.3
   Compiling schemars_derive v0.8.5
   Compiling datasize_derive v0.2.13
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.38
   Compiling tracing-attributes v0.1.23
   Compiling derive_more v0.99.17
   Compiling datasize v0.2.13
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling odra-codegen v0.2.0 (/workspace/odra/lang/codegen)
   Compiling tracing v0.1.37
   Compiling odra-proc-macros v0.2.0 (/workspace/odra/lang/proc-macros)
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.8
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling pwasm-utils v0.16.0
   Compiling num v0.4.0
   Compiling casper-types v1.5.0
   Compiling odra-casper-types v0.2.0 (/workspace/odra/odra-casper/types)
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling odra-casper-codegen v0.2.0 (/workspace/odra/odra-casper/codegen)
   Compiling odra-casper-backend v0.2.0 (/workspace/odra/odra-casper/backend)
   Compiling casper-execution-engine v2.0.1
   Compiling casper-engine-test-support v2.2.0
   Compiling odra-casper-test-env v0.2.0 (/workspace/odra/odra-casper/test-env)
   Compiling odra v0.2.0 (/workspace/odra/core)
   Compiling odra-modules v0.2.0 (/workspace/odra/modules)
   Compiling builder v1.0.0 (/workspace/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 2m 59s
     Running `../target/release/erc20_build`
   Compiling builder v1.0.0 (/workspace/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 1.01s
     Running `../target/release/wrapped_native_token_build`
💁  [1;32mINFO :[0m [32mGenerating wasm files...[0m
   Compiling syn v1.0.107
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling funty v1.1.0
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling serde v1.0.152
   Compiling opaque-debug v0.3.0
   Compiling ppv-lite86 v0.2.17
   Compiling cfg-if v1.0.0
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling serde_json v1.0.91
   Compiling proc-macro2 v1.0.49
   Compiling ryu v1.0.12
   Compiling hex v0.4.3
   Compiling rand_core v0.6.4
   Compiling itoa v1.0.5
   Compiling static_assertions v1.1.0
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.1
   Compiling quote v1.0.23
   Compiling bitflags v1.3.2
   Compiling unicode-ident v1.0.6
   Compiling odra-types v0.2.0 (/workspace/odra/types)
   Compiling convert_case v0.5.0
   Compiling lazy_static v1.4.0
   Compiling odra-casper-shared v0.2.0 (/workspace/odra/odra-casper/shared)
   Compiling ref_thread_local v0.1.1
   Compiling typenum v1.16.0
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-rational v0.4.1
   Compiling rand v0.8.5
   Compiling rand_chacha v0.2.2
   Compiling generic-array v0.14.6
   Compiling num-iter v0.1.43
   Compiling odra-utils v0.2.0 (/workspace/odra/utils)
   Compiling bitvec v0.18.5
   Compiling rand v0.7.3
   Compiling uint v0.9.5
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling signature v1.2.2
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling hmac v0.10.1
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
   Compiling proc-macro-error v1.0.4
   Compiling odra-ir v0.2.0 (/workspace/odra/lang/ir)
   Compiling zeroize_derive v1.3.3
   Compiling serde_derive v1.0.152
   Compiling num-derive v0.3.3
   Compiling derive_more v0.99.17
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling odra-codegen v0.2.0 (/workspace/odra/lang/codegen)
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling odra-proc-macros v0.2.0 (/workspace/odra/lang/proc-macros)
   Compiling serde_bytes v0.11.8
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling odra-casper-types v0.2.0 (/workspace/odra/odra-casper/types)
   Compiling odra-casper-backend v0.2.0 (/workspace/odra/odra-casper/backend)
   Compiling odra v0.2.0 (/workspace/odra/core)
   Compiling odra-modules v0.2.0 (/workspace/odra/modules)
   Compiling builder v1.0.0 (/workspace/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 41.34s
   Compiling builder v1.0.0 (/workspace/odra/modules/.builder_casper)
    Finished release [optimized] target(s) in 0.45s
💁  [1;32mINFO :[0m [32mCopying wasm files...[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/erc20.wasm[0m
💁  [1;32mINFO :[0m [32mSaving ./wasm/wrapped_native_token.wasm[0m
💁  [1;32mINFO :[0m [32mRunning cargo test...[0m
   Compiling syn v1.0.107
   Compiling autocfg v1.1.0
   Compiling libc v0.2.139
   Compiling typenum v1.16.0
   Compiling serde_derive v1.0.152
   Compiling serde v1.0.152
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling unicode-xid v0.2.4
   Compiling funty v1.1.0
   Compiling ppv-lite86 v0.2.17
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling byteorder v1.4.3
   Compiling fastrand v1.8.0
   Compiling opaque-debug v0.3.0
   Compiling remove_dir_all v0.5.3
   Compiling serde_json v1.0.91
   Compiling quick-error v1.2.3
   Compiling itoa v1.0.5
   Compiling once_cell v1.17.0
   Compiling hashbrown v0.12.3
   Compiling cpufeatures v0.2.5
   Compiling fnv v1.0.7
   Compiling bit-vec v0.6.3
   Compiling bitflags v1.3.2
   Compiling ryu v1.0.12
   Compiling schemars v0.8.5
   Compiling regex-syntax v0.6.28
   Compiling lazy_static v1.4.0
   Compiling dyn-clone v1.0.10
   Compiling quick-error v2.0.1
   Compiling base16 v0.2.1
   Compiling base64 v0.13.1
   Compiling hex_fmt v0.3.0
   Compiling pkg-config v0.3.26
   Compiling cc v1.0.78
   Compiling thiserror v1.0.38
   Compiling log v0.4.17
   Compiling parity-wasm v0.41.0
   Compiling iana-time-zone v0.1.53
   Compiling match_cfg v0.1.0
   Compiling pin-project-lite v0.2.9
   Compiling downcast-rs v1.2.0
   Compiling memory_units v0.3.0
   Compiling linked-hash-map v0.5.6
   Compiling yansi v0.5.1
   Compiling odra-casper-shared v0.2.0 (/workspace/odra/odra-casper/shared)
   Compiling filesize v0.2.0
   Compiling diff v0.1.13
   Compiling generic-array v0.14.6
   Compiling value-bag v1.0.0-alpha.9
   Compiling tracing-core v0.1.30
   Compiling rand_chacha v0.2.2
   Compiling bitvec v0.18.5
   Compiling bit-set v0.5.3
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling indexmap v1.9.2
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling num-bigint v0.2.6
   Compiling num-rational v0.2.4
   Compiling pretty_assertions v1.3.0
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling getrandom v0.2.8
   Compiling wait-timeout v0.2.0
   Compiling tempfile v3.3.0
   Compiling time v0.1.45
   Compiling num_cpus v1.15.0
   Compiling hostname v0.3.1
   Compiling lmdb-sys v0.8.0
   Compiling rand_core v0.6.4
   Compiling rusty-fork v0.3.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling ff v0.8.0
   Compiling blake2 v0.9.2
   Compiling ed25519 v1.2.0
   Compiling group v0.8.0
   Compiling rand v0.8.5
   Compiling num-complex v0.4.2
   Compiling chrono v0.4.23
   Compiling proptest v1.0.0
   Compiling wasmi v0.8.0
   Compiling synstructure v0.12.6
   Compiling serde_derive_internals v0.25.0
   Compiling proc-macro-error v1.0.4
   Compiling lmdb v0.8.0
   Compiling odra-ir v0.2.0 (/workspace/odra/lang/ir)
   Compiling zeroize_derive v1.3.3
   Compiling schemars_derive v0.8.5
   Compiling datasize_derive v0.2.13
   Compiling num-derive v0.3.3
   Compiling ctor v0.1.26
   Compiling thiserror-impl v1.0.38
   Compiling tracing-attributes v0.1.23
   Compiling derive_more v0.99.17
   Compiling datasize v0.2.13
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling odra-codegen v0.2.0 (/workspace/odra/lang/codegen)
   Compiling tracing v0.1.37
   Compiling odra-proc-macros v0.2.0 (/workspace/odra/lang/proc-macros)
   Compiling hex v0.4.3
   Compiling serde_bytes v0.11.8
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling uint v0.9.5
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling num v0.4.0
   Compiling pwasm-utils v0.16.0
   Compiling casper-types v1.5.0
   Compiling odra-casper-types v0.2.0 (/workspace/odra/odra-casper/types)
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.4
   Compiling casper-execution-engine v2.0.1
   Compiling odra-casper-codegen v0.2.0 (/workspace/odra/odra-casper/codegen)
   Compiling odra-casper-backend v0.2.0 (/workspace/odra/odra-casper/backend)
   Compiling casper-engine-test-support v2.2.0
   Compiling odra-casper-test-env v0.2.0 (/workspace/odra/odra-casper/test-env)
   Compiling odra v0.2.0 (/workspace/odra/core)
   Compiling odra-modules v0.2.0 (/workspace/odra/modules)
    Finished test [unoptimized + debuginfo] target(s) in 1m 18s
     Running unittests src/lib.rs (target/debug/deps/odra_modules-9d4cc23bc8e9662f)

running 11 tests
test wrapped_native::tests::test_deposit_amount_exceeding_account_balance ... ok
test wrapped_native::tests::test_withdrawal_amount_exceeding_account_deposit ... ok
test erc20::tests::transfer_error ... ok
test erc20::tests::transfer_from_error ... ok
test erc20::tests::transfer_works ... ok
test wrapped_native::tests::test_deposit ... ok
test wrapped_native::tests::test_withdrawal ... ok
test wrapped_native::tests::test_minting ... ok
test wrapped_native::tests::test_init ... ok
test erc20::tests::initialization ... ok
test erc20::tests::transfer_from_and_approval_work ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 5.45s

   Doc-tests odra-modules

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

```

