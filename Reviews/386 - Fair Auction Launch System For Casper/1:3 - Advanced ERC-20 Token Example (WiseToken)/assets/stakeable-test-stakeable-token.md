```
$ make test-stakeable-token
cargo test -p stakeable-token-tests t1
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.08s
     Running unittests src/lib.rs (target/debug/deps/stakeable_token_tests-35df09a88d7cc645)

running 2 tests
test tests::t1::should_be_able_to_create_stake_and_end_stake_immature_no_penalty has been running for over 60 seconds
test tests::t1::should_be_able_to_create_stake_with_cspr has been running for over 60 seconds
test tests::t1::should_be_able_to_create_stake_and_end_stake_immature_no_penalty ... ok
test tests::t1::should_be_able_to_create_stake_with_cspr ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 2 filtered out; finished in 91.54s

cargo test -p stakeable-token-tests t2
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.15s
     Running unittests src/lib.rs (target/debug/deps/stakeable_token_tests-35df09a88d7cc645)

running 2 tests
test tests::t2::should_be_able_to_create_stake_and_end_stake_immature_penalty has been running for over 60 seconds
test tests::t2::should_be_able_to_create_stake_and_scrape_interest has been running for over 60 seconds
test tests::t2::should_be_able_to_create_stake_and_scrape_interest ... ok
test tests::t2::should_be_able_to_create_stake_and_end_stake_immature_penalty ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 2 filtered out; finished in 91.22s
```
