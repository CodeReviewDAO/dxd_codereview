```sh
@ggurbet ➜ /workspaces/dao-contracts (7c24f46 ✗) $ make test
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc20
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc721
cargo test -p casper-dao-macros -- --skip verify_expand_output
   Compiling syn v1.0.86
   Compiling casper-dao-macros v0.1.0 (/workspaces/dao-contracts/dao-macros)
    Finished test [unoptimized + debuginfo] target(s) in 13.11s
     Running unittests (target/debug/deps/casper_dao_macros-357edf81363ddbb2)

running 11 tests
test contract::caller::tests::generating_caller_struct_works ... ok
test contract::contract_struct::tests::generating_entry_points_works ... ok
test contract::contract_struct::tests::generating_install_no_args ... ok
test contract::contract_struct::tests::generating_install_with_args ... ok
test contract::contract_struct::tests::generating_install_without_init_method_fails ... ok
test contract::contract_test::tests::generating_test_constructor_with_args_works ... ok
test contract::contract_test::tests::generating_test_constructor_without_init_method_fails ... ok
test contract::contract_test::tests::generating_test_contract_constructor_works ... ok
test instance::tests::parsing_struct_data_works ... ok
test contract::contract_bin::tests::generating_no_mangles_works ... ok
test contract::caller::tests::generating_caller_impl_works ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.01s

     Running tests/expand_tests.rs (target/debug/deps/tests-40f623ad7bdfbfa7)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 2 filtered out; finished in 0.00s

   Doc-tests casper-dao-macros

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-utils --bin getter_proxy
mkdir -p dao-contracts/wasm
cp target/wasm32-unknown-unknown/release/*.wasm dao-contracts/wasm
cargo test --features=test-support --no-default-features -p casper-dao-contracts $TEST_NAME --tests
  Downloaded proc-macro-error-attr v1.0.4
  Downloaded proc-macro2 v0.4.30
  Downloaded quote v0.6.13
  Downloaded unicode-xid v0.1.0
  Downloaded test-case v2.0.2
  Downloaded speculate v0.1.2
  Downloaded syn v0.14.9
  Downloaded proc-macro-error v1.0.4
  Downloaded 8 crates (257.4 KB) in 0.66s
   Compiling cfg-if v1.0.0
   Compiling subtle v2.4.1
   Compiling rand_core v0.5.1
   Compiling ppv-lite86 v0.2.16
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling byteorder v1.4.3
   Compiling remove_dir_all v0.5.3
   Compiling opaque-debug v0.3.0
   Compiling fastrand v1.7.0
   Compiling lazy_static v1.4.0
   Compiling hashbrown v0.11.2
   Compiling bitflags v1.3.2
   Compiling bit-vec v0.6.3
   Compiling fnv v1.0.7
   Compiling quick-error v1.2.3
   Compiling cpufeatures v0.2.1
   Compiling ryu v1.0.9
   Compiling itoa v1.0.1
   Compiling static_assertions v1.1.0
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.4
   Compiling regex-syntax v0.6.25
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling base64 v0.13.0
   Compiling once_cell v1.9.0
   Compiling parity-wasm v0.41.0
   Compiling either v1.6.1
   Compiling memory_units v0.3.0
   Compiling downcast-rs v1.2.0
   Compiling match_cfg v0.1.0
   Compiling pin-project-lite v0.2.8
   Compiling linked-hash-map v0.5.3
   Compiling proc-macro2 v0.4.30
   Compiling unicode-xid v0.1.0
   Compiling proc-macro-error-attr v1.0.4
   Compiling proc-macro-error v1.0.4
   Compiling rand_chacha v0.2.2
   Compiling tracing-core v0.1.21
   Compiling bitvec v0.18.5
   Compiling bit-set v0.5.2
   Compiling itertools v0.10.3
   Compiling libc v0.2.113
   Compiling typenum v1.15.0
   Compiling rand v0.7.3
   Compiling wasmi-validation v0.3.0
   Compiling crunchy v0.2.2
   Compiling anyhow v1.0.53
   Compiling num-traits v0.2.14
   Compiling ff v0.8.0
   Compiling getrandom v0.2.4
   Compiling tempfile v3.3.0
   Compiling wait-timeout v0.2.0
   Compiling time v0.1.43
   Compiling hostname v0.3.1
   Compiling generic-array v0.14.5
   Compiling lmdb-sys v0.8.0
   Compiling group v0.8.0
   Compiling rand_core v0.6.3
   Compiling quote v0.6.13
   Compiling num-integer v0.1.44
   Compiling num-complex v0.4.0
   Compiling rusty-fork v0.3.0
   Compiling lmdb v0.8.0
   Compiling digest v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.8.0
   Compiling syn v0.14.9
   Compiling rand_chacha v0.3.1
   Compiling rand_xorshift v0.3.0
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.42
   Compiling num-bigint v0.2.6
   Compiling chrono v0.4.19
   Compiling serde v1.0.134
   Compiling datasize v0.2.10
   Compiling value-bag v1.0.0-alpha.8
   Compiling thiserror v1.0.30
   Compiling tracing v0.1.29
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling sha2 v0.9.9
   Compiling blake2 v0.9.2
   Compiling rand v0.8.4
   Compiling num-rational v0.2.4
   Compiling zeroize v1.5.0
   Compiling ed25519 v1.2.0
   Compiling test-case v2.0.2
   Compiling hex v0.4.3
   Compiling num-rational v0.4.0
   Compiling indexmap v1.8.0
   Compiling serde_json v1.0.76
   Compiling serde_bytes v0.11.5
   Compiling log v0.4.14
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling wasmi v0.8.0
   Compiling proptest v1.0.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.0
   Compiling speculate v0.1.2
   Compiling uint v0.9.1
   Compiling hex-buffer-serde v0.3.0
   Compiling hex-buffer-serde v0.2.2
   Compiling num v0.4.0
   Compiling pwasm-utils v0.16.0
   Compiling schemars v0.8.5
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling casper-types v1.4.6
   Compiling casper-hashing v1.4.3
   Compiling casper-contract v1.4.3
   Compiling casper-execution-engine v1.4.4
   Compiling casper-engine-test-support v2.0.3
   Compiling casper-dao-utils v0.1.0 (/workspaces/dao-contracts/dao-utils)
   Compiling casper-dao-erc721 v0.1.0 (/workspaces/dao-contracts/dao-erc721)
   Compiling casper-dao-modules v0.1.0 (/workspaces/dao-contracts/dao-modules)
   Compiling casper-dao-contracts v0.1.0 (/workspaces/dao-contracts/dao-contracts)
    Finished test [unoptimized + debuginfo] target(s) in 2m 03s
     Running unittests (target/debug/deps/casper_dao_contracts-383e5a226efbadda)

running 3 tests
test action::test_action ... ok
test voting::governance_voting::voting::test_voting_serialization ... ok
test voting::ballot::test_vote_serialization ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running tests/governance_voting_common.rs (target/debug/deps/governance_voting_common-180fdf754e0824f4)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running tests/test_admin.rs (target/debug/deps/test_admin-ce0ea424e6f3fca2)

running 3 tests
test speculate_0::admin_with_voting_set_up_for_adding_an_address_to_a_whitelist::when_voting_passes::test_address_cann_perform_action ... ok
test speculate_0::admin_with_voting_set_up_for_adding_an_address_to_a_whitelist::test_address_cannot_perform_action_before_voting_finishes ... ok
test speculate_0::admin_with_voting_set_up_for_adding_an_address_to_a_whitelist::when_voting_is_rejected::test_address_cannot_perform_action_on_rejected_voting ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 12.75s

     Running tests/test_governance_results.rs (target/debug/deps/test_governance_results-2847906963f51457)

running 15 tests
test test_formal_voting_result::exact_number_of_votes ... ok
test test_formal_voting_result::exact_number_of_votes_againts ... ok
test test_formal_voting_result::exact_number_of_votes_10_onboarded ... ok
test test_formal_voting_result::nobody_votes ... ok
test test_formal_voting_result::everybody_votes_in_favor_10_onboarded ... ok
test test_formal_voting_result::exact_number_of_votes_in_favor ... ok
test test_formal_voting_result::one_vote_less_than_quorum_4_onboarded ... ok
test test_informal_voting_result::exact_number_of_votes_10_onboarded ... ok
test test_informal_voting_result::everybody_votes_in_favor_10_onboarded ... ok
test test_formal_voting_result::one_vote_less_than_quorum_10_onboarded ... ok
test test_informal_voting_result::exact_number_of_votes_againts ... ok
test test_informal_voting_result::exact_number_of_votes_in_favor ... ok
test test_informal_voting_result::nobody_votes ... ok
test test_informal_voting_result::exact_number_of_votes_tie ... ok
test test_informal_voting_result::one_vote_less_than_quorum ... ok

test result: ok. 15 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 88.60s

     Running tests/test_governance_voting.rs (target/debug/deps/test_governance_voting-088bbce33fdd5b54)

running 27 tests
test speculate_0::governance_voting::creating_formal_voting::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_ends_without_reaching_quorum::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_ends_without_reaching_quorum::test_does_not_perform_its_action ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_ends_without_reaching_quorum::test_is_completed ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_completed::test_does_perform_its_action ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_completed::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_rejected::test_does_not_perform_its_action ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_completed::test_is_completed ... ok
test speculate_0::governance_voting::creating_informal_voting::test_emits_an_event ... ok
test speculate_0::governance_voting::creating_informal_voting::test_that_creator_cannot_vote_on_his_own_voting ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_rejected::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_rejected::test_is_completed ... ok
test speculate_0::governance_voting::creating_informal_voting::test_that_someone_else_cannot_vote_twice_on_the_same_voting ... ok
test speculate_0::governance_voting::creating_informal_voting::test_that_voting_is_created_correctly ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_ends_without_reaching_quorum::test_doesn_t_create_new_voting ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_ends_without_reaching_quorum::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_ends_without_reaching_quorum::test_is_completed ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_completed::test_created_new_formal_voting ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_completed::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_completed::test_is_completed ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_rejected::test_doesn_t_create_new_voting ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_rejected::test_emits_proper_event ... ok
test speculate_0::governance_voting::voting_contact::test_disallows_creating_voting_with_not_enough_reputation_staked ... ok
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_rejected::test_is_completed ... ok
test speculate_0::governance_voting::voting_contact::test_can_count_votings ... ok
test speculate_0::governance_voting::voting_contact::test_disallows_creating_voting_with_reputation_that_creator_doesn_t_have ... ok
test speculate_0::governance_voting::voting_contact::test_emits_event_with_correct_values ... ok

test result: ok. 27 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 103.90s

     Running tests/test_kyc_voter.rs (target/debug/deps/test_kyc_voter-ad9c5c7f0ba650aa)

running 9 tests
test speculate_0::voting::applicant_is_kyced::test_voting_cannot_be_created ... ok
test speculate_0::voting::applicant_is_not_kyced::test_voting_creation_succeeds ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::rejected::test_applicant_does_not_own_kyc_token ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::passed::test_applicant_owns_kyc_token ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::test_cannot_create_next_voting_for_the_same_applicant ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::rejected::test_next_voting_creation_for_the_same_applicant_succeeds ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::test_cannot_create_next_voting_for_the_same_applicant ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::test_can_create_next_voting_for_a_different_applicant ... ok
test speculate_0::voting::test_kyc_token_address_is_set ... ok

test result: ok. 9 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 26.51s

     Running tests/test_onboarding_voter.rs (target/debug/deps/test_onboarding_voter-84ec4252d96f6b26)

running 20 tests
test speculate_0::voting::test_va_token_address_it_set ... ok
test speculate_0::voting::test_kyc_token_address_is_set ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_passed::test_that_user_has_no_va_token ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_passed::test_add_voting_creation_succeeds ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_rejected::test_that_user_still_owns_va_token ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_rejected::test_next_remove_voting_creation_succeeds ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::test_that_add_voting_cannot_be_created ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::test_that_remove_voting_cannot_be_created ... ok
test speculate_0::voting::user_is_already_onboarded::test_that_add_user_voting_cannot_be_created ... ok
test speculate_0::voting::user_is_already_onboarded::when_user_has_no_reputation::test_that_voting_creation_fails ... ok
test speculate_0::voting::user_is_not_onboarded::test_remove_user_voting_creation_fails ... ok
test speculate_0::voting::user_is_not_onboarded::user_has_no_reputation::test_voting_creation_fails ... ok
test speculate_0::voting::user_is_not_onboarded::user_is_not_kyced::test_voting_creation_fails ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::informal_voting_passed::test_that_add_voting_cannot_be_created ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::informal_voting_passed::voting_passed::test_remove_voting_creation_succeeds ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::informal_voting_passed::voting_passed::test_user_owns_a_va_token ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::informal_voting_passed::voting_rejected::test_next_add_voting_creation_succeeds ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::informal_voting_passed::voting_rejected::test_user_does_not_own_va_token ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::test_that_add_voting_cannot_be_created ... ok
test speculate_0::voting::user_is_not_onboarded::voting_is_created::test_that_remove_voting_cannot_be_created ... ok

test result: ok. 20 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 69.51s

     Running tests/test_repo_voter.rs (target/debug/deps/test_repo_voter-7b1bbab912e3bf18)

running 3 tests
test speculate_0::repo_voter::test_action_was_not_performed_before_finish ... ok
test speculate_0::repo_voter::test_action_was_performed_after_finish ... ok
test speculate_0::repo_voter::test_action_was_not_performed_on_rejected_voting ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 13.98s

     Running tests/test_reputation.rs (target/debug/deps/test_reputation-12fd6d4afe7093d9)

running 25 tests
test test_buring_amount_exceeding_balance ... ok
test test_burn_staked_tokens ... ok
test test_deploy ... ok
test test_duplicated_whitelisting ... ok
test test_init_cannot_be_called_twice ... ok
test test_mint_as_non_owner ... ok
test test_mint_as_owner ... ok
test test_non_whitelisted_user_burn ... ok
test test_new_owner_whitelisting ... ok
test test_not_whitelisted_user_removal_has_no_effect ... ok
test test_stake_amount_exceeding_balance ... ok
test test_ownership ... ok
test test_stake_not_whitelisted ... ok
test test_stake ... ok
test test_total_supply_overflow ... ok
test test_that_contract_have_different_hashes ... ok
test test_transfer_amount_higher_than_balance ... ok
test test_transfer_from ... ok
test test_transfer_from_not_whitelisted_user ... ok
test test_transfer_staked_tokens ... ok
test test_unstake ... ok
test test_unstake_amount_exceeding_staked_balance ... ok
test test_whitelisting_as_non_owner ... ok
test test_whitelisted_user_burn ... ok
test test_whitelisting_as_owner ... ok

test result: ok. 25 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 12.25s

     Running tests/test_variable_repository.rs (target/debug/deps/test_variable_repository-f83a236a7bc148c4)

running 24 tests
test test_anyone_can_read_data ... ok
test test_change_ownership ... ok
test test_duplicated_whitelisting ... ok
test test_get_uninitialized_value ... ok
test test_getting_key_with_nonexistent_index_returns_none ... ok
test test_deploy ... ok
test test_new_owner_whitelisting ... ok
test test_keys_indexing ... ok
test test_update_at_case_1 ... ok
test test_not_whitelisted_user_removal_has_no_effect ... ok
test test_update_at_case_2 ... ok
test test_update_at_case_10 ... ok
test test_update_at_case_11 ... ok
test test_update_at_case_12 ... ok
test test_update_at_case_3 ... ok
test test_update_at_case_4 ... ok
test test_update_at_case_5 ... ok
test test_update_at_case_6 ... ok
test test_update_at_case_7 ... ok
test test_whitelisted_only_has_write_access ... ok
test test_update_at_case_8 ... ok
test test_update_at_case_9 ... ok
test test_whitelisting_as_non_owner ... ok
test test_whitelisting ... ok

test result: ok. 24 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 17.82s

mkdir -p dao-erc20/wasm
cp target/wasm32-unknown-unknown/release/*.wasm dao-erc20/wasm
cargo test --features=test-support --no-default-features -p casper-dao-erc20 $TEST_NAME --tests
   Compiling casper-dao-erc20 v0.1.0 (/workspaces/dao-contracts/dao-erc20)
    Finished test [unoptimized + debuginfo] target(s) in 9.14s
     Running unittests (target/debug/deps/casper_dao_erc20-1a5f7877a182d9bd)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running tests/test_erc20.rs (target/debug/deps/test_erc20-0284ed1a11443164)

running 3 tests
test test_erc20_transfer ... ok
test test_erc20_initial_state ... ok
test test_erc20_transfer_from ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 2.27s

mkdir -p dao-erc721/wasm
cp target/wasm32-unknown-unknown/release/*.wasm dao-erc721/wasm
cargo test --features=test-support --no-default-features -p casper-dao-erc721 $TEST_NAME --tests
   Compiling casper-dao-erc721 v0.1.0 (/workspaces/dao-contracts/dao-erc721)
    Finished test [unoptimized + debuginfo] target(s) in 11.85s
     Running unittests (target/debug/deps/casper_dao_erc721-4325aaa58b76fb27)

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

     Running tests/test_erc721_spec.rs (target/debug/deps/test_erc721_spec-0a35906ee6fdabc9)

running 67 tests
test test::speculate_0::erc721::deploy::once_the_contract_is_deployed::test_sets_the_given_symbole ... ok
test test::speculate_0::erc721::deploy::once_the_contract_is_deployed::test_has_no_initial_supply ... ok
test test::speculate_0::erc721::deploy::once_the_contract_is_deployed::test_sets_the_given_name ... ok
test test::speculate_0::erc721::mint::minting_an_existing_token::test_reverts ... ok
test test::speculate_0::erc721::mint::test_emits_a_Transfer_event ... ok
test test::speculate_0::erc721::mint::test_increases_balance_of_the_owner ... ok
test test::speculate_0::erc721::mint::test_increases_total_supply ... ok
test test::speculate_0::erc721::mint::test_sets_the_ownership_to_the_new_token_owner ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_approving_a_non_zero_address::when_there_was_no_prior_approval::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_address_that_receives_the_approval_is_the_owner::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_clearing_approval::when_there_was_no_prior_approval::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_clearing_approval::when_there_was_a_prior_approval::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_sender_does_not_own_the_given_token_ID::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_sender_is_approved_for_the_given_token_ID::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_sender_is_an_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_there_was_a_prior_approval_to_a_different_address::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_there_was_a_prior_approval_to_the_same_address::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::balance_of::when_the_given_address_does_not_own_any_tokens::test_returns_the_amount_of_tokens_owned_by_the_given_address ... ok
test test::speculate_0::erc721::with_minted_tokens::balance_of::when_the_given_address_owns_some_tokens::test_returns_the_amount_of_tokens_owned_by_the_given_address ... ok
test test::speculate_0::erc721::with_minted_tokens::get_approved::when_token_has_been_minted::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::owner_of::when_the_given_token_id_was_not_tracked_by_this_token::test_should_panic - should panic ... ok
test test::speculate_0::erc721::with_minted_tokens::get_approved::when_token_is_not_minted::test_should_panic - should panic ... ok
test test::speculate_0::erc721::with_minted_tokens::get_approved::when_token_has_been_minted::when_account_has_been_approved::test_returns_approved_account ... ok
test test::speculate_0::erc721::with_minted_tokens::owner_of::when_the_given_token_id_was_tracked_by_this_token::test_returns_the_owner_of_the_given_token_ID ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_is_the_owner::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_was_already_approved::test_emits_an_approval_event ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_was_already_approved::test_keeps_the_approval_to_the_given_address ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_was_set_as_not_approved::test_approves_the_operator ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_was_set_as_not_approved::test_can_unset_the_operator_approval ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_was_set_as_not_approved::test_emits_an_approval_event ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_willing_to_approve_is_not_the_owner::when_there_is_no_operator_approval_set_by_the_sender::test_approves_the_operator ... ok
test test::speculate_0::erc721::with_minted_tokens::set_approval_for_all::when_the_operator_willing_to_approve_is_not_the_owner::when_there_is_no_operator_approval_set_by_the_sender::test_emits_an_approval_event ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_contract_that_does_not_implement_the_required_function::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_called_by_the_approved_individual::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_called_by_the_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_called_by_the_owner::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_clears_the_approval_for_the_token_id ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_emits_only_a_transfer_event ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_called_by_the_owner_without_an_approved_user::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_keeps_ownership_of_the_token ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_the_address_of_the_previous_owner_is_incorrect::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_keeps_the_owner_balance ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_the_sender_is_not_authorized_for_the_token_id::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_approved_individual::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_owner::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_owner_without_an_approved_user::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_the_address_of_the_previous_owner_is_incorrect::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_the_sender_is_not_authorized_for_the_token_id::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::with_data::test_calls_on_ERC721_received ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::without_data::test_calls_on_ERC721_received_from_approved ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::with_data::test_calls_on_ERC721_received_from_approved ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::without_data::test_calls_on_ERC721_received ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_approved_individual::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_owner::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_owner_without_an_approved_user::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_clears_the_approval_for_the_token_id ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_emits_only_a_transfer_event ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_keeps_ownership_of_the_token ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_keeps_the_owner_balance ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_the_address_of_the_previous_owner_is_incorrect::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_the_sender_is_not_authorized_for_the_token_id::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_the_given_token_id_does_not_exist::test_reverts ... ok

test result: ok. 67 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 55.27s
```