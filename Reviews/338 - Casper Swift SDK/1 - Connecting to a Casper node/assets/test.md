```
swift test -v
  shell: /bin/bash -e {0}
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun --sdk macosx --find xctest
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -emit-supported-features /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.UUgQTN/dummyInput-1.swift
Planning build
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI/libPackageDescription.dylib
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk -F /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk -package-description-version 5.5.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.2ViBw6/caspersdkinswift-manifest
/usr/bin/sandbox-exec -p '(version 1)
(deny default)
(import "system.sb")
(allow file-read*)
(allow process*)
(allow file-write*
    (subpath "/Users/runner/Library/Caches/org.swift.swiftpm/manifests")
)
' /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.2ViBw6/caspersdkinswift-manifest -fileno 7
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk iphoneos --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.1.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk appletvos --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.1.app/Contents/Developer/Platforms/AppleTVOS.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk watchos --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.1.app/Contents/Developer/Platforms/WatchOS.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -module-name CasperSDKInSwiftTests -incremental -emit-dependencies -emit-module -emit-module-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftmodule -output-file-map /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/output-file-map.json -parse-as-library -c /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Tests/CasperSDKInSwiftTests/CasperSDKInSwiftTests.swift -I /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -target x86_64-apple-macosx11.0 -swift-version 5 -enable-batch-mode -index-store-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/index/store -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk -F /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -Onone -enable-testing -g -j3 -DSWIFT_PACKAGE -DDEBUG -module-cache-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/ModuleCache -parseable-output -parse-as-library
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -c -primary-file /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Tests/CasperSDKInSwiftTests/CasperSDKInSwiftTests.swift -emit-module-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftmodule -emit-module-doc-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftdoc -emit-module-source-info-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftsourceinfo -emit-dependencies-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests.d -emit-reference-dependencies-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests.swiftdeps -target x86_64-apple-macosx11.0 -enable-objc-interop -stack-check -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk -I /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -I /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -F /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -enable-testing -g -module-cache-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/ModuleCache -swift-version 5 -Onone -D SWIFT_PACKAGE -D DEBUG -new-driver-path /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-driver -resource-dir /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift -enable-anonymous-context-mangled-names -module-name CasperSDKInSwiftTests -target-sdk-version 12.0.0 -parse-as-library -o /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests.swift.o -index-store-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/index/store -index-system-modules
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -merge-modules -emit-module /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftmodule -parse-as-library -disable-diagnostic-passes -disable-sil-perf-optzns -target x86_64-apple-macosx11.0 -enable-objc-interop -stack-check -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk -I /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -I /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -F /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -enable-testing -g -module-cache-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/ModuleCache -swift-version 5 -Onone -D SWIFT_PACKAGE -D DEBUG -new-driver-path /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-driver -resource-dir /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift -enable-anonymous-context-mangled-names -module-name CasperSDKInSwiftTests -target-sdk-version 12.0.0 -emit-module-doc-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftdoc -emit-module-source-info-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftsourceinfo -o /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftmodule
/Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -sdk /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.0.sdk -F /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -o /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.xctest/Contents/MacOS/CasperSDKInSwiftPackageTests -module-name CasperSDKInSwiftPackageTests -Xlinker -bundle -Xlinker -rpath -Xlinker @loader_path/../../../ @/Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.product/Objects.LinkFileList -Xlinker -rpath -Xlinker /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/macosx -target x86_64-apple-macosx11.0 -Xlinker -add_ast_path -Xlinker /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwift.swiftmodule -Xlinker -add_ast_path -Xlinker /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftmodule -L /Applications/Xcode_13.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib
[0/0] Build complete!
/Applications/Xcode_13.1.app/Contents/Developer/usr/bin/xctest /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.xctest
Test Suite 'All tests' started at 2022-01-23 16:22:48.283
Test Suite 'CasperSDKInSwiftPackageTests.xctest' started at 2022-01-23 16:22:48.284
Test Suite 'CasperSDKInSwiftTests' started at 2022-01-23 16:22:48.284
Test Case '-[CasperSDKInSwiftTests.CasperSDKInSwiftTests testAll]' started.
2022-01-23 16:22:48.745 xctest[5305:18236] StateRootHash: 8e2e8aecd0250b7c50c1f4531eea5a4561e5ce3457261ae55ffceb7015b02592
2022-01-23 16:22:48.758 xctest[5305:18235] StateRootHash: 642a48f769bc09267c6dc6d01d4a0a9e57e72b0d63f66ba547f6065f11093e3e
2022-01-23 16:22:48.765 xctest[5305:18235] StateRootHash: 642a48f769bc09267c6dc6d01d4a0a9e57e72b0d63f66ba547f6065f11093e3e
2022-01-23 16:22:48.778 xctest[5305:18277] Total peers:361
2022-01-23 16:22:48.778 xctest[5305:18277] First peerAddress:138.201.54.44:35000
2022-01-23 16:22:48.778 xctest[5305:18277] First peerID:tls:005b..f2c8
2022-01-23 16:22:48.787 xctest[5305:18277] Total JsonExecutionResult:0
2022-01-23 16:22:48.787 xctest[5305:18277] Total deploy approvals:1
2022-01-23 16:22:48.788 xctest[5305:18277] Payment:Optional(CasperSDKInSwift.ExecutableDeployItem.ModuleBytes(module_bytes: CasperSDKInSwift.Bytes, args: CasperSDKInSwift.RuntimeArgs))
2022-01-23 16:22:48.788 xctest[5305:18277] Session:Optional(CasperSDKInSwift.ExecutableDeployItem.StoredContractByHash("a977eb2d2e091823fccfc17bea195a55176f03a1f85599368620175d6bad9d04", "mint", CasperSDKInSwift.RuntimeArgs))
2022-01-23 16:22:48.798 xctest[5305:18236] Total peers:361
2022-01-23 16:22:48.798 xctest[5305:18236] First peerAddress:138.201.54.44:35000
2022-01-23 16:22:48.798 xctest[5305:18236] First peerID:tls:005b..f2c8
2022-01-23 16:22:48.811 xctest[5305:18235] In chain_get_block_transfers, block_hash:ae173969cb6ce3c99439c81e5b803c15797a8559796d980daa99f52beb7192e3
2022-01-23 16:22:48.811 xctest[5305:18235] Total Transfer:1
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer deploy_hash:Optional("d14afb6de9b2c2552302aee107e63662cbd357c0e324e484632c13114ca8ce4d")
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer from:Optional("account-hash-668c24b8091faf295a0d686d9a4f8a40a03c756632fcd785fa084ca073f9a6a1")
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer to:Optional("account-hash-6258550585382cb823f9f0cf241466f1ce83a77fa9195b3612e443347907b40b")
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer source:Optional("uref-bbef30ab99e4827cfc16080c76b7049feaadca99d117014703afbd536e6ed2df-007")
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer target:Optional("uref-1f5e1a8fba0884969aebc870d1dc1a036d2c006fcb62623d8d549c8315b9b77a-004")
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer gas:0
2022-01-23 16:22:48.812 xctest[5305:18235] First transfer id:Optional(1641903583371)
2022-01-23 16:22:48.825 xctest[5305:18236] Block body total deploy hash:0
2022-01-23 16:22:48.825 xctest[5305:18236] Block body total transfer hash:0
2022-01-23 16:22:48.825 xctest[5305:18236] Block body proposer:012b77bfab443aae5957d4d2d4991e55f692fa3eb56c2ac1179a188881a575292a
2022-01-23 16:22:48.825 xctest[5305:18236] Block total proof:100
2022-01-23 16:22:48.826 xctest[5305:18236] Block first proof public key:0101a458aa2b551c5a49e56326f9bb298bb308e1babc875647ae0290c42f13feac
2022-01-23 16:22:48.826 xctest[5305:18236] Block first proof signature:018a8803d72a90c0bb557c7145771fa191cfbefdcff38ccbec51bbda5c853e0c1d636ad9daec1e3cd0080fa7bfb5cf7371d1561f4122f8f38a16a033954d500906
2022-01-23 16:22:49.113 xctest[5305:18235] Era state root hash:d0e627faad27cc510efc524f870363646a8cd33ba6686f35d083f61b2a3a6e56
2022-01-23 16:22:49.113 xctest[5305:18235] Era block hash:f3e4f0249ca558ed568295f5a902bd66e147447f2426191d50fa6f0b8948c357
2022-01-23 16:22:49.149 xctest[5305:18235] Era merkle_proof length:1235350
2022-01-23 16:22:49.150 xctest[5305:18235] Era stored_value:EraInfo(CasperSDKInSwift.EraInfo)
2022-01-23 16:22:49.150 xctest[5305:18235] In chain_get_era_info_by_switch_block, stored_value is EraInfo
2022-01-23 16:22:49.150 xctest[5305:18235] In chain_get_era_info_by_switch_block, total seigniorage_allocations:8605
2022-01-23 16:22:49.150 xctest[5305:18235] Delegator amount:8898767
2022-01-23 16:22:49.150 xctest[5305:18235] Delegator delegator_public_key:010ca8f91a2704a56701bdc4cc16f70e341e01281ef20bcb5475bf83ffe48841bd
2022-01-23 16:22:49.150 xctest[5305:18235] Delegator validator_public_key:0101a458aa2b551c5a49e56326f9bb298bb308e1babc875647ae0290c42f13feac
2022-01-23 16:22:49.202 xctest[5305:18235] In state_get_item, stored_value is Withdraw
2022-01-23 16:22:49.202 xctest[5305:18235] Total UnbondingPurse:1
2022-01-23 16:22:49.202 xctest[5305:18235] Withdraw first  UnbondingPurse, bonding_purse:Optional("uref-5fcc3031ea2572f9929e0cfcfc84c6c3131bfe1e78bce8cb61f99f59eace7795-007")
2022-01-23 16:22:49.202 xctest[5305:18235] Withdraw first  UnbondingPurse, amount:500
2022-01-23 16:22:49.202 xctest[5305:18235] Withdraw first  UnbondingPurse, era_of_creation:3319
2022-01-23 16:22:49.202 xctest[5305:18235] Withdraw first  UnbondingPurse, unbonder_public_key:01d949a3a1963db686607a00862f79b76ceb185fc134d0aeedb686f1c151f4ae54
2022-01-23 16:22:49.202 xctest[5305:18235] Withdraw first  UnbondingPurse, validator_public_key:01d949a3a1963db686607a00862f79b76ceb185fc134d0aeedb686f1c151f4ae54
2022-01-23 16:22:49.202 xctest[5305:18235] StateGetItem merkle_proof length:6876
2022-01-23 16:22:49.211 xctest[5305:18235] In state_get_dictionary_item, stored_value is CLValue
2022-01-23 16:22:49.211 xctest[5305:18235] In state_get_dictionary_item, CLValue of stored_value, bytes:090000006162635f76616c7565
2022-01-23 16:22:49.211 xctest[5305:18235] In state_get_dictionary_item, CLValue of stored_value,cl_type:String
2022-01-23 16:22:49.212 xctest[5305:18235] In state_get_dictionary_item, CLValue of stored_value,parsed:String("abc_value")
2022-01-23 16:22:49.213 xctest[5305:18235] GetDictionaryItem merkle_proof length:30330
2022-01-23 16:22:49.214 xctest[5305:18235] GetDictionaryItemResult dictionary_key:Optional("dictionary-5d3e90f064798d54e5e53643c4fce0cbb1024aadcad1586cc4b7c1358a530373")
2022-01-23 16:22:49.222 xctest[5305:18277] GetBalanceResult, balance_value: 522693296224
2022-01-23 16:22:49.223 xctest[5305:18277] GetBalanceResult, merkle_proof length:31766
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState state_root_hash:8b463b56f2d124f43e7c157e602e31d5d2d5009659de7f1e79afbd238cbaa189
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState block_height:473576
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState total era_validator:1538
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState first bid staked_amount: 908982507030
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState first bid delegation_rate: 10
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState first bid inactive: true
2022-01-23 16:22:49.995 xctest[5305:18236] AuctionState first bid total delegator: 1
2022-01-23 16:22:49.995 xctest[5305:18236] Information for first bid first delegator
2022-01-23 16:22:49.995 xctest[5305:18236] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-01-23 16:22:49.995 xctest[5305:18236] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-01-23 16:22:49.996 xctest[5305:18236] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-01-23 16:22:49.996 xctest[5305:18236] First delegator staked_amount:30268476029
Test Case '-[CasperSDKInSwiftTests.CasperSDKInSwiftTests testAll]' passed (1.723 seconds).
Test Suite 'CasperSDKInSwiftTests' passed at 2022-01-23 16:22:50.008.
	 Executed 1 test, with 0 failures (0 unexpected) in 1.723 (1.724) seconds
Test Suite 'CasperSDKInSwiftPackageTests.xctest' passed at 2022-01-23 16:22:50.008.
	 Executed 1 test, with 0 failures (0 unexpected) in 1.723 (1.724) seconds
Test Suite 'All tests' passed at 2022-01-23 16:22:50.008.
	 Executed 1 test, with 0 failures (0 unexpected) in 1.723 (1.725) seconds
```
