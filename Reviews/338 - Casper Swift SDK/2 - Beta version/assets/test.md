```
  swift test -v
  shell: /bin/bash -e {0}
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun --sdk macosx --find xctest
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -emit-supported-features /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.lA4nBS/dummyInput-1.swift
Planning build
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI/libPackageDescription.dylib
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -lPackageDescription -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -target x86_64-apple-macosx11.0 -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -swift-version 5 -I /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/pm/ManifestAPI -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -package-description-version 5.5.0 /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Package.swift -Xfrontend -disable-implicit-concurrency-module-import -o /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.IyXkkM/caspersdkinswift-manifest
/usr/bin/sandbox-exec -p '(version 1)
(deny default)
(import "system.sb")
(allow file-read*)
(allow process*)
(allow file-write*
    (subpath "/Users/runner/Library/Caches/org.swift.swiftpm/manifests")
)
' /var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/TemporaryDirectory.IyXkkM/caspersdkinswift-manifest -fileno 7
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk iphoneos --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk appletvos --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/AppleTVOS.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/usr/bin/xcrun --sdk watchos --show-sdk-platform-path
/usr/bin/xcrun vtool -show-build /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/WatchOS.platform/Developer/Library/Frameworks/XCTest.framework/XCTest
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -module-name CasperSDKInSwiftTests -incremental -emit-dependencies -emit-module -emit-module-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftmodule -output-file-map /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/output-file-map.json -parse-as-library -c /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Tests/CasperSDKInSwiftTests/CasperSDKInSwiftTests.swift -I /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -target x86_64-apple-macosx11.0 -swift-version 5 -enable-batch-mode -index-store-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/index/store -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -Onone -enable-testing -g -j3 -DSWIFT_PACKAGE -DDEBUG -module-cache-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/ModuleCache -parseable-output -parse-as-library
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -c -primary-file /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/Tests/CasperSDKInSwiftTests/CasperSDKInSwiftTests.swift -emit-module-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftmodule -emit-module-doc-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftdoc -emit-module-source-info-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftsourceinfo -emit-dependencies-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests.d -emit-reference-dependencies-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests.swiftdeps -target x86_64-apple-macosx11.0 -enable-objc-interop -stack-check -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -I /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -enable-testing -g -module-cache-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/ModuleCache -swift-version 5 -Onone -D SWIFT_PACKAGE -D DEBUG -new-driver-path /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-driver -resource-dir /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift -enable-anonymous-context-mangled-names -module-name CasperSDKInSwiftTests -target-sdk-version 12.1.0 -parse-as-library -o /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests.swift.o -index-store-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/index/store -index-system-modules
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -merge-modules -emit-module /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.build/CasperSDKInSwiftTests~partial.swiftmodule -parse-as-library -disable-diagnostic-passes -disable-sil-perf-optzns -target x86_64-apple-macosx11.0 -enable-objc-interop -stack-check -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -I /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -enable-testing -g -module-cache-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/ModuleCache -swift-version 5 -Onone -D SWIFT_PACKAGE -D DEBUG -new-driver-path /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-driver -resource-dir /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift -enable-anonymous-context-mangled-names -module-name CasperSDKInSwiftTests -target-sdk-version 12.1.0 -emit-module-doc-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftdoc -emit-module-source-info-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftsourceinfo -o /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftmodule -emit-abi-descriptor-path /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.abi.json
/Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -sdk /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk -F /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/Library/Frameworks -I /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/usr/lib -L /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug -o /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.xctest/Contents/MacOS/CasperSDKInSwiftPackageTests -module-name CasperSDKInSwiftPackageTests -Xlinker -bundle -Xlinker -rpath -Xlinker @loader_path/../../../ @/Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.product/Objects.LinkFileList -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift/macosx -Xlinker -rpath -Xlinker /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/swift-5.5/macosx -target x86_64-apple-macosx11.0 -Xlinker -add_ast_path -Xlinker /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwift.swiftmodule -Xlinker -add_ast_path -Xlinker /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftTests.swiftmodule -L /Applications/Xcode_13.2.1.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib
[0/0] Build complete!
/Applications/Xcode_13.2.1.app/Contents/Developer/usr/bin/xctest /Users/runner/work/CasperSDKInSwift/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.xctest
Test Suite 'All tests' started at 2022-02-06 11:23:22.799
Test Suite 'CasperSDKInSwiftPackageTests.xctest' started at 2022-02-06 11:23:22.800
Test Suite 'CasperSDKInSwiftTests' started at 2022-02-06 11:23:22.800
Test Case '-[CasperSDKInSwiftTests.CasperSDKInSwiftTests testAll]' started.
2022-02-06 11:23:22.983 xctest[2224:38207] StateRootHash: c6397cbffadb0e1c2350b363f65d303a8998c23b53a5727fb64e22b79f39c136
2022-02-06 11:23:23.009 xctest[2224:38228] StateRootHash: 642a48f769bc09267c6dc6d01d4a0a9e57e72b0d63f66ba547f6065f11093e3e
2022-02-06 11:23:23.029 xctest[2224:38207] StateRootHash: 642a48f769bc09267c6dc6d01d4a0a9e57e72b0d63f66ba547f6065f11093e3e
2022-02-06 11:23:23.049 xctest[2224:38207] Error:CasperError(code: -32001, message: "block not known", methodCall: "chain_get_state_root_hash")
2022-02-06 11:23:23.095 xctest[2224:38206] Total peers:381
2022-02-06 11:23:23.095 xctest[2224:38206] First peerAddress:195.201.174.222:35000
2022-02-06 11:23:23.095 xctest[2224:38206] First peerID:tls:0007..4a2f
2022-02-06 11:23:23.640 xctest[2224:38228] Era block hash:f3e4f0249ca558ed568295f5a902bd66e147447f2426191d50fa6f0b8948c357
2022-02-06 11:23:23.675 xctest[2224:38228] Era merkle_proof length:1235350
2022-02-06 11:23:23.676 xctest[2224:38228] Era stored_value:EraInfo(CasperSDKInSwift.EraInfo)
2022-02-06 11:23:23.676 xctest[2224:38228] In chain_get_era_info_by_switch_block, stored_value is EraInfo
2022-02-06 11:23:23.676 xctest[2224:38228] In chain_get_era_info_by_switch_block, total seigniorage_allocations:8605
2022-02-06 11:23:23.676 xctest[2224:38228] Delegator amount:8898767
2022-02-06 11:23:23.676 xctest[2224:38228] Delegator delegator_public_key:010ca8f91a2704a56701bdc4cc16f70e341e01281ef20bcb5475bf83ffe48841bd
2022-02-06 11:23:23.676 xctest[2224:38228] Delegator validator_public_key:0101a458aa2b551c5a49e56326f9bb298bb308e1babc875647ae0290c42f13feac
2022-02-06 11:23:23.760 xctest[2224:38206] Error:CasperError(code: -32001, message: "block not known", methodCall: "chain_get_era_info_by_switch_block")
2022-02-06 11:23:23.799 xctest[2224:38228] In state_get_item, stored_value is Withdraw
2022-02-06 11:23:23.799 xctest[2224:38228] Total UnbondingPurse:1
2022-02-06 11:23:23.799 xctest[2224:38228] Withdraw first  UnbondingPurse, bonding_purse:Optional("uref-5fcc3031ea2572f9929e0cfcfc84c6c3131bfe1e78bce8cb61f99f59eace7795-007")
2022-02-06 11:23:23.800 xctest[2224:38228] Withdraw first  UnbondingPurse, amount:500
2022-02-06 11:23:23.800 xctest[2224:38228] Withdraw first  UnbondingPurse, era_of_creation:3319
2022-02-06 11:23:23.800 xctest[2224:38228] Withdraw first  UnbondingPurse, unbonder_public_key:01d949a3a1963db686607a00862f79b76ceb185fc134d0aeedb686f1c151f4ae54
2022-02-06 11:23:23.800 xctest[2224:38228] Withdraw first  UnbondingPurse, validator_public_key:01d949a3a1963db686607a00862f79b76ceb185fc134d0aeedb686f1c151f4ae54
2022-02-06 11:23:23.800 xctest[2224:38228] StateGetItem merkle_proof length:6876
2022-02-06 11:23:23.820 xctest[2224:38228] Error:CasperError(code: -32602, message: "Invalid params", methodCall: "state_get_item")
2022-02-06 11:23:23.839 xctest[2224:38207] Error:CasperError(code: -32002, message: "failed to parse key: withdraw-key from string error: Invalid byte `b\'f\'`, at index 1.", methodCall: "state_get_item")
2022-02-06 11:23:23.858 xctest[2224:38228] Error:CasperError(code: -32002, message: "failed to parse key: unknown prefix for key", methodCall: "state_get_item")
2022-02-06 11:23:23.879 xctest[2224:38228] In state_get_dictionary_item, stored_value is CLValue
2022-02-06 11:23:23.879 xctest[2224:38228] In state_get_dictionary_item, CLValue of stored_value, bytes:090000006162635f76616c7565
2022-02-06 11:23:23.879 xctest[2224:38228] In state_get_dictionary_item, CLValue of stored_value,cl_type:String
2022-02-06 11:23:23.879 xctest[2224:38228] In state_get_dictionary_item, CLValue of stored_value,parsed:String("abc_value")
2022-02-06 11:23:23.880 xctest[2224:38228] GetDictionaryItem merkle_proof length:30330
2022-02-06 11:23:23.881 xctest[2224:38228] GetDictionaryItemResult dictionary_key:Optional("dictionary-5d3e90f064798d54e5e53643c4fce0cbb1024aadcad1586cc4b7c1358a530373")
2022-02-06 11:23:23.901 xctest[2224:38228] Error:CasperError(code: -32002, message: "Failed to parse key", methodCall: "state_get_dictionary_item")
2022-02-06 11:23:23.922 xctest[2224:38218] GetBalanceResult, balance_value: 522693296224
2022-02-06 11:23:23.923 xctest[2224:38218] GetBalanceResult, merkle_proof length:31766
2022-02-06 11:23:23.944 xctest[2224:38206] Error got:CasperError(code: -32005, message: "failed to parse purse_uref: Hex(InvalidByte { index: 0, byte: 102 })", methodCall: "state_get_balance")
2022-02-06 11:23:24.719 xctest[2224:38207] AuctionState state_root_hash:8b463b56f2d124f43e7c157e602e31d5d2d5009659de7f1e79afbd238cbaa189
2022-02-06 11:23:24.719 xctest[2224:38207] AuctionState block_height:473576
2022-02-06 11:23:24.719 xctest[2224:38207] AuctionState total era_validator:1538
2022-02-06 11:23:24.719 xctest[2224:38207] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-02-06 11:23:24.720 xctest[2224:38207] AuctionState first bid staked_amount: 908982507030
2022-02-06 11:23:24.720 xctest[2224:38207] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-02-06 11:23:24.720 xctest[2224:38207] AuctionState first bid delegation_rate: 10
2022-02-06 11:23:24.720 xctest[2224:38207] AuctionState first bid inactive: true
2022-02-06 11:23:24.720 xctest[2224:38207] AuctionState first bid total delegator: 1
2022-02-06 11:23:24.720 xctest[2224:38207] Information for first bid first delegator
2022-02-06 11:23:24.720 xctest[2224:38207] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-02-06 11:23:24.720 xctest[2224:38207] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-02-06 11:23:24.720 xctest[2224:38207] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-02-06 11:23:24.720 xctest[2224:38207] First delegator staked_amount:30268476029
2022-02-06 11:23:25.498 xctest[2224:38218] AuctionState state_root_hash:8b463b56f2d124f43e7c157e602e31d5d2d5009659de7f1e79afbd238cbaa189
2022-02-06 11:23:25.498 xctest[2224:38218] AuctionState block_height:473576
2022-02-06 11:23:25.498 xctest[2224:38218] AuctionState total era_validator:1538
2022-02-06 11:23:25.498 xctest[2224:38218] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-02-06 11:23:25.498 xctest[2224:38218] AuctionState first bid staked_amount: 908982507030
2022-02-06 11:23:25.499 xctest[2224:38218] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-02-06 11:23:25.499 xctest[2224:38218] AuctionState first bid delegation_rate: 10
2022-02-06 11:23:25.499 xctest[2224:38218] AuctionState first bid inactive: true
2022-02-06 11:23:25.499 xctest[2224:38218] AuctionState first bid total delegator: 1
2022-02-06 11:23:25.499 xctest[2224:38218] Information for first bid first delegator
2022-02-06 11:23:25.499 xctest[2224:38218] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-02-06 11:23:25.499 xctest[2224:38218] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-02-06 11:23:25.499 xctest[2224:38218] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-02-06 11:23:25.499 xctest[2224:38218] First delegator staked_amount:30268476029
2022-02-06 11:23:26.314 xctest[2224:38218] AuctionState state_root_hash:c6397cbffadb0e1c2350b363f65d303a8998c23b53a5727fb64e22b79f39c136
2022-02-06 11:23:26.314 xctest[2224:38218] AuctionState block_height:516283
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState total era_validator:1540
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState first bid staked_amount: 908982507030
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState first bid delegation_rate: 10
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState first bid inactive: true
2022-02-06 11:23:26.315 xctest[2224:38218] AuctionState first bid total delegator: 1
2022-02-06 11:23:26.315 xctest[2224:38218] Information for first bid first delegator
2022-02-06 11:23:26.315 xctest[2224:38218] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-02-06 11:23:26.315 xctest[2224:38218] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-02-06 11:23:26.315 xctest[2224:38218] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-02-06 11:23:26.315 xctest[2224:38218] First delegator staked_amount:30268476029
2022-02-06 11:23:26.346 xctest[2224:38207] Error :CasperError(code: -32001, message: "get-auction-info failed to get specified block", methodCall: "state_get_auction_info")
Test Case '-[CasperSDKInSwiftTests.CasperSDKInSwiftTests testAll]' passed (3.549 seconds).
Test Suite 'CasperSDKInSwiftTests' passed at 2022-02-06 11:23:26.349.
	 Executed 1 test, with 0 failures (0 unexpected) in 3.549 (3.549) seconds
Test Suite 'CasperSDKInSwiftPackageTests.xctest' passed at 2022-02-06 11:23:26.349.
	 Executed 1 test, with 0 failures (0 unexpected) in 3.549 (3.549) seconds
Test Suite 'All tests' passed at 2022-02-06 11:23:26.349.
	 Executed 1 test, with 0 failures (0 unexpected) in 3.549 (3.550) seconds
```

