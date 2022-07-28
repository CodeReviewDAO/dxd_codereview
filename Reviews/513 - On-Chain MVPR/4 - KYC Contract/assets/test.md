cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc20
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc721
cargo test -p casper-dao-macros -- --skip verify_expand_output

running 11 tests
test contract::caller::tests::generating_caller_struct_works ... ok
test contract::caller::tests::generating_caller_impl_works ... ok
test contract::contract_bin::tests::generating_no_mangles_works ... ok
test contract::contract_struct::tests::generating_install_no_args ... ok
test contract::contract_struct::tests::generating_entry_points_works ... ok
test contract::contract_struct::tests::generating_install_with_args ... ok
test contract::contract_struct::tests::generating_install_without_init_method_fails ... ok
test contract::contract_test::tests::generating_test_constructor_without_init_method_fails ... ok
test contract::contract_test::tests::generating_test_contract_constructor_works ... ok
test contract::contract_test::tests::generating_test_constructor_with_args_works ... ok
test instance::tests::parsing_struct_data_works ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 2 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-utils --bin getter_proxy
mkdir -p dao-contracts/wasm
cp target/wasm32-unknown-unknown/release/*.wasm dao-contracts/wasm
cargo test --features=test-support --no-default-features -p casper-dao-contracts $TEST_NAME --tests

running 3 tests
test action::test_action ... ok
test voting::ballot::test_vote_serialization ... ok
test voting::governance_voting::voting::test_voting_serialization ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 3 tests
test speculate_0::admin_with_voting_set_up_for_adding_an_address_to_a_whitelist::test_address_cannot_perform_action_before_voting_finishes ... ok
test speculate_0::admin_with_voting_set_up_for_adding_an_address_to_a_whitelist::when_voting_is_rejected::test_address_cannot_perform_action_on_rejected_voting ... ok
test speculate_0::admin_with_voting_set_up_for_adding_an_address_to_a_whitelist::when_voting_passes::test_address_can_perform_action ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 18.70s


running 15 tests
test test_formal_voting_result::exact_number_of_votes ... ok
test test_formal_voting_result::everybody_votes_in_favor_10_onboarded ... ok
test test_formal_voting_result::exact_number_of_votes_10_onboarded ... ok
test test_formal_voting_result::exact_number_of_votes_againts ... ok
test test_formal_voting_result::exact_number_of_votes_in_favor ... ok
test test_formal_voting_result::nobody_votes ... ok
test test_formal_voting_result::one_vote_less_than_quorum_4_onboarded ... ok
test test_formal_voting_result::one_vote_less_than_quorum_10_onboarded ... ok
test test_informal_voting_result::everybody_votes_in_favor_10_onboarded ... ok
test test_informal_voting_result::exact_number_of_votes_10_onboarded ... ok
test test_informal_voting_result::exact_number_of_votes_againts ... ok
test test_informal_voting_result::exact_number_of_votes_in_favor ... ok
test test_informal_voting_result::exact_number_of_votes_tie ... ok
test test_informal_voting_result::nobody_votes ... ok
test test_informal_voting_result::one_vote_less_than_quorum ... ok

test result: ok. 15 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 117.96s


running 27 tests
test speculate_0::governance_voting::creating_formal_voting::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_ends_without_reaching_quorum::test_does_not_perform_its_action ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_ends_without_reaching_quorum::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_ends_without_reaching_quorum::test_is_completed ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_completed::test_does_perform_its_action ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_completed::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_completed::test_is_completed ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_rejected::test_does_not_perform_its_action ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_rejected::test_emits_proper_event ... ok
test speculate_0::governance_voting::creating_formal_voting::when_formal_voting_is_rejected::test_is_completed ... ok
test speculate_0::governance_voting::creating_informal_voting::test_emits_an_event ... ok
test speculate_0::governance_voting::creating_informal_voting::test_that_creator_cannot_vote_on_his_own_voting ... ok
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
test speculate_0::governance_voting::creating_informal_voting::when_informal_voting_is_rejected::test_is_completed ... ok
test speculate_0::governance_voting::voting_contact::test_can_count_votings ... ok
test speculate_0::governance_voting::voting_contact::test_disallows_creating_voting_with_not_enough_reputation_staked ... ok
test speculate_0::governance_voting::voting_contact::test_disallows_creating_voting_with_reputation_that_creator_doesn_t_have ... ok
test speculate_0::governance_voting::voting_contact::test_emits_event_with_correct_values ... ok

test result: ok. 27 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 138.78s


running 9 tests
test speculate_0::voting::applicant_is_kyced::test_voting_cannot_be_created ... ok
test speculate_0::voting::applicant_is_not_kyced::test_voting_creation_succeeds ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::passed::test_applicant_owns_kyc_token ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::rejected::test_applicant_does_not_own_kyc_token ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::test_cannot_create_next_voting_for_the_same_applicant ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::informal_voting_passed::rejected::test_next_voting_creation_for_the_same_applicant_succeeds ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::test_can_create_next_voting_for_a_different_applicant ... ok
test speculate_0::voting::applicant_is_not_kyced::voting_is_created::test_cannot_create_next_voting_for_the_same_applicant ... ok
test speculate_0::voting::test_kyc_token_address_is_set ... ok

test result: ok. 9 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 36.11s


running 20 tests
test speculate_0::voting::test_va_token_address_it_set ... ok
test speculate_0::voting::test_kyc_token_address_is_set ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_passed::test_that_user_has_no_va_token ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_passed::test_add_voting_creation_succeeds ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_rejected::test_next_remove_voting_creation_succeeds ... ok
test speculate_0::voting::user_is_already_onboarded::remove_voting_is_created::informal_voting_passed::voting_rejected::test_that_user_still_owns_va_token ... ok
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

test result: ok. 20 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 77.01s


running 3 tests
test speculate_0::repo_voter::test_action_was_not_performed_before_finish ... ok
test speculate_0::repo_voter::test_action_was_not_performed_on_rejected_voting ... ok
test speculate_0::repo_voter::test_action_was_performed_after_finish ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 20.03s


running 18 tests
test test_buring_amount_exceeding_balance ... ok
test test_deploy ... ok
test test_init_cannot_be_called_twice ... ok
test test_duplicated_whitelisting ... ok
test test_mint_as_non_owner ... ok
test test_mint_as_owner ... ok
test test_new_owner_whitelisting ... ok
test test_non_whitelisted_user_burn ... ok
test test_not_whitelisted_user_removal_has_no_effect ... ok
test test_ownership ... ok
test test_that_contract_have_different_hashes ... ok
test test_total_supply_overflow ... ok
test test_transfer_amount_higher_than_balance ... ok
test test_transfer_from_not_whitelisted_user ... ok
test test_transfer_from ... ok
test test_whitelisting_as_non_owner ... ok
test test_whitelisted_user_burn ... ok
test test_whitelisting_as_owner ... ok

test result: ok. 18 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 9.62s


running 24 tests
test test_anyone_can_read_data ... ok
test test_change_ownership ... ok
test test_duplicated_whitelisting ... ok
test test_deploy ... ok
test test_get_uninitialized_value ... ok
test test_getting_key_with_nonexistent_index_returns_none ... ok
test test_keys_indexing ... ok
test test_new_owner_whitelisting ... ok
test test_not_whitelisted_user_removal_has_no_effect ... ok
test test_update_at_case_1 ... ok
test test_update_at_case_10 ... ok
test test_update_at_case_11 ... ok
test test_update_at_case_2 ... ok
test test_update_at_case_12 ... ok
test test_update_at_case_3 ... ok
test test_update_at_case_4 ... ok
test test_update_at_case_5 ... ok
test test_update_at_case_6 ... ok
test test_update_at_case_7 ... ok
test test_update_at_case_8 ... ok
test test_update_at_case_9 ... ok
test test_whitelisted_only_has_write_access ... ok
test test_whitelisting_as_non_owner ... ok
test test_whitelisting ... ok

test result: ok. 24 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 19.30s

mkdir -p dao-erc20/wasm
cp target/wasm32-unknown-unknown/release/*.wasm dao-erc20/wasm
cargo test --features=test-support --no-default-features -p casper-dao-erc20 $TEST_NAME --tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 3 tests
test test_erc20_initial_state ... ok
test test_erc20_transfer ... ok
test test_erc20_transfer_from ... ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.03s

mkdir -p dao-erc721/wasm
cp target/wasm32-unknown-unknown/release/*.wasm dao-erc721/wasm
cargo test --features=test-support --no-default-features -p casper-dao-erc721 $TEST_NAME --tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s


running 67 tests
test test::speculate_0::erc721::deploy::once_the_contract_is_deployed::test_sets_the_given_name ... ok
test test::speculate_0::erc721::deploy::once_the_contract_is_deployed::test_has_no_initial_supply ... ok
test test::speculate_0::erc721::deploy::once_the_contract_is_deployed::test_sets_the_given_symbole ... ok
test test::speculate_0::erc721::mint::minting_an_existing_token::test_reverts ... ok
test test::speculate_0::erc721::mint::test_emits_a_Transfer_event ... ok
test test::speculate_0::erc721::mint::test_increases_balance_of_the_owner ... ok
test test::speculate_0::erc721::mint::test_increases_total_supply ... ok
test test::speculate_0::erc721::mint::test_sets_the_ownership_to_the_new_token_owner ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_approving_a_non_zero_address::when_there_was_no_prior_approval::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_clearing_approval::when_there_was_a_prior_approval::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_clearing_approval::when_there_was_no_prior_approval::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_address_that_receives_the_approval_is_the_owner::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_sender_does_not_own_the_given_token_ID::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_sender_is_an_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_the_sender_is_approved_for_the_given_token_ID::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_there_was_a_prior_approval_to_a_different_address::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::approve::when_there_was_a_prior_approval_to_the_same_address::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::balance_of::when_the_given_address_does_not_own_any_tokens::test_returns_the_amount_of_tokens_owned_by_the_given_address ... ok
test test::speculate_0::erc721::with_minted_tokens::balance_of::when_the_given_address_owns_some_tokens::test_returns_the_amount_of_tokens_owned_by_the_given_address ... ok
test test::speculate_0::erc721::with_minted_tokens::get_approved::when_token_has_been_minted::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::get_approved::when_token_has_been_minted::when_account_has_been_approved::test_returns_approved_account ... ok
test test::speculate_0::erc721::with_minted_tokens::get_approved::when_token_is_not_minted::test_should_panic - should panic ... ok
test test::speculate_0::erc721::with_minted_tokens::owner_of::when_the_given_token_id_was_not_tracked_by_this_token::test_should_panic - should panic ... ok
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
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_called_by_the_owner_without_an_approved_user::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_clears_the_approval_for_the_token_id ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_emits_only_a_transfer_event ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_keeps_ownership_of_the_token ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_sent_to_the_owner::test_keeps_the_owner_balance ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_the_address_of_the_previous_owner_is_incorrect::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_user_account::when_the_sender_is_not_authorized_for_the_token_id::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_approved_individual::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_owner::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_called_by_the_owner_without_an_approved_user::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_the_address_of_the_previous_owner_is_incorrect::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::when_the_sender_is_not_authorized_for_the_token_id::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::with_data::test_calls_on_ERC721_received ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::with_data::test_calls_on_ERC721_received_from_approved ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::without_data::test_calls_on_ERC721_received ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::safe_transfer_from::to_a_valid_receiver_contract::without_data::test_calls_on_ERC721_received_from_approved ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_approved_individual::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_operator::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_owner::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_called_by_the_owner_without_an_approved_user::test_works ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_clears_the_approval_for_the_token_id ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_emits_only_a_transfer_event ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_keeps_ownership_of_the_token ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_sent_to_the_owner::test_keeps_the_owner_balance ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_the_address_of_the_previous_owner_is_incorrect::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_the_given_token_id_does_not_exist::test_reverts ... ok
test test::speculate_0::erc721::with_minted_tokens::transfers::transfer_from::when_the_sender_is_not_authorized_for_the_token_id::test_reverts ... ok

test result: ok. 67 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 63.75s

