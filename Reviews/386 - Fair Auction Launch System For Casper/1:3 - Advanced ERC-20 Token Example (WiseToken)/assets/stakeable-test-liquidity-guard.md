```
$ make test-liquidity-guard
cargo test -p liquidity-guard-tests
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.16s
     Running unittests src/lib.rs (target/debug/deps/liquidity_guard_tests-c5504e092c5b0cf1)

running 2 tests
test tests::get_inflation ... ok
test tests::assign_inflation ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.82s

   Doc-tests liquidity-guard-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```
