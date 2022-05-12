make test
cargo +nightly build --release -p did --target wasm32-unknown-unknown
   Compiling did v0.1.0 (/mnt/b/projects/VCRegistry/contract/did)
    Finished release [optimized] target(s) in 12.93s
cargo +nightly build --release -p demovcregistry --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 2.54s
cp target/wasm32-unknown-unknown/release/did.wasm tests/did/wasm
cp target/wasm32-unknown-unknown/release/demovcregistry.wasm tests/demovcregistry/wasm
cargo test -p did_tests -- --nocapture --test-threads=1
   Compiling protobuf v2.8.2
   Compiling num-bigint v0.3.3
   Compiling num-rational v0.3.2
   Compiling casper-types v1.1.1
   Compiling num v0.3.1
   Compiling casper-execution-engine v1.1.1
   Compiling casper-contract v1.1.1
   Compiling casper-engine-test-support v1.1.1
   Compiling did_tests v0.1.0 (/mnt/b/projects/VCRegistry/tests/did)
    Finished test [unoptimized + debuginfo] target(s) in 1m 59s
     Running unittests src/did_tests.rs (target/debug/deps/did_tests-3c26090cda2bb0cd)

running 3 tests
test tests::should_add_attribute ... 
attribute length before: 0
attribute before: ("", "", 0)
attribute length after:  1
attribute before: ("KEY", "VALUE", 9999999999999999)
attribute before: ("KEY", "VALUE", 0)
ok
test tests::should_add_delegate ... 
delegate length before: 0
Delegate before: ("", "", 0)
delegate length after:  1
Delegate after: ("KEY", "VALUE", 9999999999999999)
Delegate after revoke: ("KEY", "VALUE", 0)
ok
test tests::should_change_owner ... 
Owner before: 0000000000000000000000000000000000000000000000000000000000000000
Owner after:  3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d
ok

test result: ok. 3 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.96s

cargo test -p demovcregistry_tests -- --nocapture --test-threads=1
    Blocking waiting for file lock on build directory
   Compiling demovcregistry_tests v0.1.0 (/mnt/b/projects/VCRegistry/tests/demovcregistry)
    Finished test [unoptimized + debuginfo] target(s) in 1m 33s
     Running unittests src/demovcregistry_tests.rs (target/debug/deps/demovcregistry_tests-a7ae21286eff3f6f)

running 4 tests
test tests::should_issueDemoVC ... 
vc length before: 0
vc before: ([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(0000000000000000000000000000000000000000000000000000000000000000), false)
vc length after: 1
vc after: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2], [3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), true)
vc after changeRevocationFlag: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2], [3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), false)
ok
test tests::should_sendVP_and_changeVPRequestStatus_to_approve ... 
vp length before: 0
vp before: ([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(0000000000000000000000000000000000000000000000000000000000000000), 0)
vp after: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), 0)
vp after changeStatus: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), 1)
ok
test tests::should_sendVP_and_changeVPRequestStatus_to_reject ... 
vp length before: 0
vp before: ([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(0000000000000000000000000000000000000000000000000000000000000000), 0)
vp after: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), 0)
vp after changeStatus: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), 2)
ok
test tests::should_sendVP_and_changeVPRequestStatus_to_revert_by_verifier ... 
vp length before: 0
vp before: ([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(0000000000000000000000000000000000000000000000000000000000000000), 0)
vp after: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), 0)
vp after changeStatus: ([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], AccountHash(3e582ebb478a2bdd1aa58bd99503b20cb7e31ff5a1220cf8ae4da2dbafae0e8d), 3)
ok

test result: ok. 4 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 1.20s