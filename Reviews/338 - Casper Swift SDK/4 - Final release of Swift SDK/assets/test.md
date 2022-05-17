```bash
  swift test -v
  shell: /bin/bash -e {0}
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun --sdk macosx --find xctest
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -emit-supported-features /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.V4TOnw/dummyInput-1.swift
Planning build
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI/libPackageDescription.dylib
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -package-description-version 5.5.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.fOfNwm/caspersdkinswift-manifest
/usr/bin/sandbox-exec -p '(version 1)
(deny default)
(import "system.sb")
(allow file-read*)
(allow process*)
(allow file-write*
    (subpath "/Users/runner/Library/Caches/org.swift.swiftpm/manifests")
)
' /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.fOfNwm/caspersdkinswift-manifest -fileno 7
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -package-description-version 5.5.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/checkouts/SwiftECC/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.8FGyxc/swiftecc-manifest
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -package-description-version 5.0.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/checkouts/Blake2.swift/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.v4uVQR/blake2.swift-manifest
/usr/bin/sandbox-exec -p '(version 1)
(deny default)
(import "system.sb")
(allow file-read*)
(allow process*)
(allow file-write*
    (subpath "/Users/runner/Library/Caches/org.swift.swiftpm/manifests")
)
' /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.8FGyxc/swiftecc-manifest -fileno 14
/usr/bin/sandbox-exec -p '(version 1)
(deny default)
(import "system.sb")
(allow file-read*)
(allow process*)
(allow sysctl*)
(allow file-write*
    (subpath "/Users/runner/Library/Caches/org.swift.swiftpm/manifests")
    (regex #"^/private/var/tmp/org\.llvm\.clang.*")
    (regex #"^/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/org\.llvm\.clang.*")
    (regex #"^/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/org\.llvm\.clang.*")
    (regex #"^/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/C/org\.llvm\.clang.*")
)
' /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.v4uVQR/blake2.swift-manifest -fileno 7
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -package-description-version 5.5.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/checkouts/ASN1/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.CBVqI5/asn1-manifest
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -package-description-version 5.5.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/checkouts/BigInt/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.EoqiF6/bigint-manifest
2022-04-07 02:23:14.676 xctest[2548:22878] 963a1591733026733f2fa41d06469700d8e30c358491d703a5962ace2e39bbbd
Test Case '-[CasperSDKInSwiftTests.TestEd25519KeyWrapper testAll]' passed (0.006 seconds).
Test Suite 'TestEd25519KeyWrapper' passed at 2022-04-07 02:23:14.679.
	 Executed 1 test, with 0 failures (0 unexpected) in 0.006 (0.007) seconds
Test Suite 'TestPutDeploy' started at 2022-04-07 02:23:14.679
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testAll]' started.
2022-04-07 02:23:14.704 xctest[2548:22897] Put deploy successful with deploy_hash: 6470ff98a57dcb74011a4067ad4f1c680a36403bb2c2a62dc33b6441d2da60ac
2022-04-07 02:23:17.562 xctest[2548:22894] Put deploy successful with deploy_hash: 3ca9649c10ea9117a6bc364773e60f3eac74c1c1c37f997b7dd63c5067c72e4d
2022-04-07 02:23:20.433 xctest[2548:22897] Error put deploy, with Error code: -32008 and message: 
2022-04-07 02:23:20.433 xctest[2548:22897] invalid deploy: the approval at index 0 is invalid: asymmetric key error: failed to verify secp256k1 signature: signature error
2022-04-07 02:23:20.459 xctest[2548:22897] Put deploy successful with deploy_hash: 181099a806b388675de21ff6d9b3d7da4427c8f1829057d563a2f9b5901106d7
2022-04-07 02:23:20.486 xctest[2548:22893] Put deploy successful with deploy_hash: f44313f97491121d91eb0acccb3ea48b3800b160f51ccaf30cfc90da9bc82b3f
2022-04-07 02:23:20.514 xctest[2548:22894] Put deploy successful with deploy_hash: 95debc3d81d1d7daa6c50a0394208e16e7492158b9d5faa00c88f601f9502df0
2022-04-07 02:23:23.359 xctest[2548:22893] Error put deploy, with Error code: -32008 and message: 
2022-04-07 02:23:23.359 xctest[2548:22893] invalid deploy: the approval at index 0 is invalid: asymmetric key error: failed to verify secp256k1 signature: signature error
2022-04-07 02:23:26.213 xctest[2548:22894] Put deploy successful with deploy_hash: 86987741c505fd895d6c976a043d2974543d36002a04b671fe9de6e89ab97015
2022-04-07 02:23:26.236 xctest[2548:22897] Error put deploy, with Error code: -32008 and message: 
2022-04-07 02:23:26.236 xctest[2548:22897] deploy parameter failure: insufficient balance in account abaf2971262c56df422b70a1ac1ccfba68a6f30aa4fbc4f2a77ca847baa9da75 at prestate_hash: eec769812751ee2e1daf2ce7173298e2832da5ea227acba24e94c8dfdf030d1c
2022-04-07 02:23:29.074 xctest[2548:22894] Error put deploy, with Error code: -32602 and message: 
2022-04-07 02:23:29.074 xctest[2548:22894] Invalid params
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testAll]' passed (14.397 seconds).
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testPutDeployStoredContractByName]' started.
2022-04-07 02:23:29.105 xctest[2548:22897] Put deploy successful with deploy_hash: e8848c0fbf89b6232d409ec484cfa1778fd7b3b60dc6b1418cb60ac36f89c2cc
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testPutDeployStoredContractByName]' passed (0.031 seconds).
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testPutDeployStoredVersionedContractByHash]' started.
2022-04-07 02:23:29.132 xctest[2548:22897] Put deploy successful with deploy_hash: 4e3cd2b90cecd75b69725f1c7f1170696b587734461283d0493ade4d89f64b72
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testPutDeployStoredVersionedContractByHash]' passed (0.026 seconds).
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testPutDeployStoredVersionedContractByName]' started.
2022-04-07 02:23:29.159 xctest[2548:22893] Put deploy successful with deploy_hash: 4a1b959d1550bbac74fd95137672f2bf62b6d3bf8831495bb4a639d136b96658
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testPutDeployStoredVersionedContractByName]' passed (0.027 seconds).
Test Suite 'TestPutDeploy' passed at 2022-04-07 02:23:29.160.
	 Executed 4 tests, with 0 failures (0 unexpected) in 14.481 (14.482) seconds
Test Suite 'TestSecp256k1KeyWrapper' started at 2022-04-07 02:23:29.160
Test Case '-[CasperSDKInSwiftTests.TestSecp256k1KeyWrapper testAll]' started.
2022-04-07 02:23:30.409 xctest[2548:22878] Private key of secp256k1 read from Pem file: 
2022-04-07 02:23:30.763 xctest[2548:22878] -----BEGIN EC PRIVATE KEY-----
MHQCAQEEII5bEBxW2DyGWsZyjMV9/5+/Vxs47z3osjUac01eO9mkoAcGBSuBBAAK
oUQDQgAEuM2ado6pY94J824W3wUy40OP65R3csCN8NinJQykro3+ng5PIICrN02V
GrFR/69mpEP5nax85b+WD9jotMYPww==
-----END EC PRIVATE KEY-----
2022-04-07 02:23:33.590 xctest[2548:22878] Public key of secp256k1 read from Pem file: 
2022-04-07 02:23:33.591 xctest[2548:22878] -----BEGIN PUBLIC KEY-----
MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAExtEDVh+DpBKB0njgfkWQVSm/JddPoYRj
GjCa/nvD3AZbWpRrnx2PmN7Z2Ax7AFZlKkZH/DXHzTw1hEzTMIcnwA==
-----END PUBLIC KEY-----
2022-04-07 02:23:36.412 xctest[2548:22878] Private key of secp256k1 from key pair
2022-04-07 02:23:36.761 xctest[2548:22878] -----BEGIN EC PRIVATE KEY-----
MHQCAQEEIGhMP0PcRkn8w3RxrRP+Y6in/Ueo8LMY/PNnQbsw6WZRoAcGBSuBBAAK
oUQDQgAEF7oqKKwGEgVA7GpniNp3/PYCorL42EF3sT3a1eU8YU3YvGYg+rgz4ZCG
ir9kprIeF81d4iQ6BIjJKFTNExU4kQ==
-----END EC PRIVATE KEY-----
2022-04-07 02:23:36.761 xctest[2548:22878] Public key of secp256k1 from key pair
2022-04-07 02:23:36.762 xctest[2548:22878] -----BEGIN PUBLIC KEY-----
MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAEF7oqKKwGEgVA7GpniNp3/PYCorL42EF3
sT3a1eU8YU3YvGYg+rgz4ZCGir9kprIeF81d4iQ6BIjJKFTNExU4kQ==
-----END PUBLIC KEY-----
Test Case '-[CasperSDKInSwiftTests.TestSecp256k1KeyWrapper testAll]' passed (16.398 seconds).
Test Suite 'TestSecp256k1KeyWrapper' passed at 2022-04-07 02:23:45.558.
	 Executed 1 test, with 0 failures (0 unexpected) in 16.398 (16.398) seconds
Test Suite 'CasperSDKInSwiftPackageTests.xctest' passed at 2022-04-07 02:23:45.558.
	 Executed 10 tests, with 0 failures (0 unexpected) in 34.692 (34.694) seconds
Test Suite 'All tests' passed at 2022-04-07 02:23:45.558.
	 Executed 10 tests, with 0 failures (0 unexpected) in 34.692 (34.695) seconds

```
