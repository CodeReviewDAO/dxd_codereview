```console
swift test -v 
/usr/bin/xcrun --sdk macosx --show-sdk-platform-path
/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/usr/bin/xcrun --sdk macosx --find xctest
/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swiftc -print-target-info
/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info -sdk /Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk
/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -print-target-info
/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/swift-frontend -frontend -emit-supported-features /var/folders/k5/clh1htq97vb_rw25vs9ttfn00000gp/T/TemporaryDirectory.0E1Cvz/dummyInput-1.swift
[0/0] Build complete!
/Applications/Xcode.app/Contents/Developer/usr/bin/xctest /Users/p35862/CasperSDKInSwift/.build/x86_64-apple-macosx/debug/CasperSDKInSwiftPackageTests.xctest
Test Suite 'All tests' started at 2022-03-04 15:47:28.349
Test Suite 'CasperSDKInSwiftPackageTests.xctest' started at 2022-03-04 15:47:28.350
Test Suite 'CasperSDKInSwiftTests' started at 2022-03-04 15:47:28.350
Test Case '-[CasperSDKInSwiftTests.CasperSDKInSwiftTests testAll]' started.
Ed25519 PublicKey in hexa
f1e2dc53cf3999d6fe3a3aef3227d6da44ca47f8a0027f2d17b9f697b2715e47
Ed25519 PrivateKey in hexa
bd37ac1a534d7b6245225cdedefc706f96dc0d159a8a7458b2757c4df0f391bd
2022-03-04 15:47:28.373 xctest[26418:2456124] Delete auto generated Ed25519 private file.
2022-03-04 15:47:28.374 xctest[26418:2456124] Delete auto generated Ed25519 private file.
Key pair generation, private key in hexa
d2f455e1d9b86bba82201fe5b436a929bee39b7376df0f945845de978db8f8e7
Key pair generation, public key in hexa
9d3206ca557079107f7537479607a5dda2c18af3566c3affbfd89e6e690fcad7
2022-03-04 15:47:29.045 xctest[26418:2456124] Private key of secp256k1 read from Pem file:
2022-03-04 15:47:29.229 xctest[26418:2456124] -----BEGIN EC PRIVATE KEY-----
MHQCAQEEILgH3Z+UnasGUDgH00EnGtrX1HmEFHafR+879tC13QzsoAcGBSuBBAAK
oUQDQgAEno6M4vcQFkO5ilpWOCwSjKZUKem01Mp+jXyfDRCyHExXonghUeSGALy0
Ww9+6vD79dMGg7VdVIxviGF9nV0mNg==
-----END EC PRIVATE KEY-----
2022-03-04 15:47:29.411 xctest[26418:2456124] Delete auto generated Secp256k1 private file.
2022-03-04 15:47:30.769 xctest[26418:2456124] Public key of secp256k1 read from Pem file:
2022-03-04 15:47:30.770 xctest[26418:2456124] -----BEGIN PUBLIC KEY-----
MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAExtEDVh+DpBKB0njgfkWQVSm/JddPoYRj
GjCa/nvD3AZbWpRrnx2PmN7Z2Ax7AFZlKkZH/DXHzTw1hEzTMIcnwA==
-----END PUBLIC KEY-----
2022-03-04 15:47:30.771 xctest[26418:2456124] Delete auto generated Secp256k1 public file.
2022-03-04 15:47:32.304 xctest[26418:2456124] Private key of secp256k1 from key pair
2022-03-04 15:47:32.488 xctest[26418:2456124] -----BEGIN EC PRIVATE KEY-----
MHQCAQEEIGChdcFAj8tyo53Mm7u+K59M9uBtXqBh5i+be+DCaaF4oAcGBSuBBAAK
oUQDQgAErOidRXsMdpKsGtiRqP9kDDqcebV/dCSwtIlpkuNW06r4tSJovyGnHGcd
Zv4vm/YqU3lbN2z0EerH0H8g2Z3gUA==
-----END EC PRIVATE KEY-----
2022-03-04 15:47:32.488 xctest[26418:2456124] Public key of secp256k1 from key pair
2022-03-04 15:47:32.489 xctest[26418:2456124] -----BEGIN PUBLIC KEY-----
MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAErOidRXsMdpKsGtiRqP9kDDqcebV/dCSw
tIlpkuNW06r4tSJovyGnHGcdZv4vm/YqU3lbN2z0EerH0H8g2Z3gUA==
-----END PUBLIC KEY-----
2022-03-04 15:47:34.985 xctest[26418:2456208] StateRootHash: 530a0bd4bc05712109e2cea9114301e4f47c1dafc1eabb44344a1cd6b9a22f9c
2022-03-04 15:47:35.128 xctest[26418:2456126] StateRootHash: 642a48f769bc09267c6dc6d01d4a0a9e57e72b0d63f66ba547f6065f11093e3e
2022-03-04 15:47:35.278 xctest[26418:2456126] StateRootHash: 642a48f769bc09267c6dc6d01d4a0a9e57e72b0d63f66ba547f6065f11093e3e
2022-03-04 15:47:35.428 xctest[26418:2456211] Error:CasperError(code: -32001, message: "block not known", methodCall: "chain_get_state_root_hash")
2022-03-04 15:47:35.883 xctest[26418:2456208] Total peers:872
2022-03-04 15:47:35.883 xctest[26418:2456208] First peerAddress:195.201.174.222:35000
2022-03-04 15:47:35.883 xctest[26418:2456208] First peerID:tls:0007..4a2f
2022-03-04 15:47:36.031 xctest[26418:2456208] Total deploy approvals:1
2022-03-04 15:47:36.031 xctest[26418:2456208] Payment:Optional(CasperSDKInSwift.ExecutableDeployItem.ModuleBytes(module_bytes: CasperSDKInSwift.Bytes, args: CasperSDKInSwift.RuntimeArgs))
2022-03-04 15:47:36.032 xctest[26418:2456208] Session:Optional(CasperSDKInSwift.ExecutableDeployItem.StoredContractByHash(hash: "a977eb2d2e091823fccfc17bea195a55176f03a1f85599368620175d6bad9d04", entry_point: "mint", args: CasperSDKInSwift.RuntimeArgs))
2022-03-04 15:47:36.032 xctest[26418:2456208] Total JsonExecutionResult:1
2022-03-04 15:47:36.032 xctest[26418:2456208] ExecutionResult block_hash:35118660a57b975fd79fada93fcff2f55f58289dfc80151f42fbc061603925de
2022-03-04 15:47:36.032 xctest[26418:2456208] ExecutionResult:Success(effect: CasperSDKInSwift.ExecutionEffect, transfers: [], cost: CasperSDKInSwift.U512Class)
2022-03-04 15:47:36.032 xctest[26418:2456208] ExecutionResult Success with cost:628662860
2022-03-04 15:47:36.032 xctest[26418:2456208] ExecutionResult total Transfer:0
2022-03-04 15:47:36.032 xctest[26418:2456208] ExecutionResult Effect, total Transform:27
2022-03-04 15:47:36.032 xctest[26418:2456208] ExecutionResult Effect, total Operation:0
2022-03-04 15:47:36.032 xctest[26418:2456208] First TransformEntry key:hash-8cf5E4aCF51f54Eb59291599187838Dc3BC234089c46fc6cA8AD17e762aE4401
2022-03-04 15:47:36.178 xctest[26418:2456208] Error:CasperError(code: -32602, message: "Invalid params", methodCall: "info_get_deploy")
2022-03-04 15:47:36.483 xctest[26418:2456209] Total peers:872
2022-03-04 15:47:36.483 xctest[26418:2456209] First peerAddress:195.201.174.222:35000
2022-03-04 15:47:36.483 xctest[26418:2456209] First peerID:tls:0007..4a2f
2022-03-04 15:47:36.628 xctest[26418:2456209] In chain_get_block_transfers, block_hash:5eee1984dcaa2e7c543f05b0e1d37546ec19f54f640ff2474c85100c4bd64d59
2022-03-04 15:47:36.628 xctest[26418:2456209] Total Transfer:0
2022-03-04 15:47:36.780 xctest[26418:2456126] In chain_get_block_transfers, block_hash:ae173969cb6ce3c99439c81e5b803c15797a8559796d980daa99f52beb7192e3
2022-03-04 15:47:36.780 xctest[26418:2456126] Total Transfer:1
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer deploy_hash:Optional("d14afb6de9b2c2552302aee107e63662cbd357c0e324e484632c13114ca8ce4d")
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer from:Optional("account-hash-668c24b8091faf295a0d686d9a4f8a40a03c756632fcd785fa084ca073f9a6a1")
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer to:Optional("account-hash-6258550585382cb823f9f0cf241466f1ce83a77fa9195b3612e443347907b40b")
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer source:Optional("uref-bbef30ab99e4827cfc16080c76b7049feaadca99d117014703afbd536e6ed2df-007")
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer target:Optional("uref-1f5e1a8fba0884969aebc870d1dc1a036d2c006fcb62623d8d549c8315b9b77a-004")
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer gas:0
2022-03-04 15:47:36.780 xctest[26418:2456126] First transfer id:Optional(1641903583371)
2022-03-04 15:47:36.928 xctest[26418:2456208] Error:CasperError(code: -32001, message: "block not known", methodCall: "chain_get_block_transfers")
2022-03-04 15:47:37.078 xctest[26418:2456126] In chain_get_block_transfers, block_hash:3f1c8b75f4e6f7310905e0e194c8e8e1e29337d08b075879870bb0aeecbcb728
2022-03-04 15:47:37.078 xctest[26418:2456126] Total Transfer:2
2022-03-04 15:47:37.078 xctest[26418:2456126] First transfer deploy_hash:Optional("f7f5e198f0b67e8bdad29c463a617098238b9c2993018f6697042dd692552f4c")
2022-03-04 15:47:37.078 xctest[26418:2456126] First transfer from:Optional("account-hash-abaf2971262c56df422b70a1ac1ccfba68a6f30aa4fbc4f2a77ca847baa9da75")
2022-03-04 15:47:37.078 xctest[26418:2456126] First transfer to:Optional("account-hash-a77c4e3b41e0f9f34271756882b4bc86b01fa7193bdbd35b54f0deeca522b91e")
2022-03-04 15:47:37.078 xctest[26418:2456126] First transfer source:Optional("uref-1c58f6e85d73837e5a950bd4c3c17a9fda1d34c946737a642f716b90f3941116-007")
2022-03-04 15:47:37.079 xctest[26418:2456126] First transfer target:Optional("uref-af57f06af99aeba0ea67e526cd09d4753bd66cf90384102c1b453d83678e8011-004")
2022-03-04 15:47:37.079 xctest[26418:2456126] First transfer gas:0
2022-03-04 15:47:37.079 xctest[26418:2456126] First transfer id:Optional(0)
2022-03-04 15:47:37.236 xctest[26418:2456211] Block body total deploy hash:0
2022-03-04 15:47:37.236 xctest[26418:2456211] Block body total transfer hash:0
2022-03-04 15:47:37.236 xctest[26418:2456211] Block body proposer:012b77bfab443aae5957d4d2d4991e55f692fa3eb56c2ac1179a188881a575292a
2022-03-04 15:47:37.236 xctest[26418:2456211] Block total proof:100
2022-03-04 15:47:37.236 xctest[26418:2456211] Block first proof public key:0101a458aa2b551c5a49e56326f9bb298bb308e1babc875647ae0290c42f13feac
2022-03-04 15:47:37.236 xctest[26418:2456211] Block first proof signature:018a8803d72a90c0bb557c7145771fa191cfbefdcff38ccbec51bbda5c853e0c1d636ad9daec1e3cd0080fa7bfb5cf7371d1561f4122f8f38a16a033954d500906
2022-03-04 15:47:37.386 xctest[26418:2456126] Block body total deploy hash:0
2022-03-04 15:47:37.387 xctest[26418:2456126] Block body total transfer hash:1
2022-03-04 15:47:37.387 xctest[26418:2456126] Block body proposer:01ace6578907bfe6eba3a618e863bbe7274284c88e405e2857be80dd094726a223
2022-03-04 15:47:37.387 xctest[26418:2456126] Block body first transfer hash:Optional("db4473a20dea79aecceb0b2b769915040cc1fb56d1c7caaf5750fef12fcbad2f")
2022-03-04 15:47:37.387 xctest[26418:2456126] Block total proof:100
2022-03-04 15:47:37.387 xctest[26418:2456126] Block first proof public key:0101a458aa2b551c5a49e56326f9bb298bb308e1babc875647ae0290c42f13feac
2022-03-04 15:47:37.387 xctest[26418:2456126] Block first proof signature:017e7c0742061a890bebcdf038c88c775d37d716560fc0b5b0711de67e65666243c705ef348ff153aab4280730fd7940354df02ff54930489b85889f15cf382602
2022-03-04 15:47:37.534 xctest[26418:2456126] Block body total deploy hash:0
2022-03-04 15:47:37.534 xctest[26418:2456126] Block body total transfer hash:2
2022-03-04 15:47:37.534 xctest[26418:2456126] Block body proposer:0107cba5b4826a87ddbe0ba8cda8064881b75882f05094c1a5f95e957512a3450e
2022-03-04 15:47:37.534 xctest[26418:2456126] Block body first transfer hash:Optional("19bc1f1f17fe55c724427862d77a9c404515a6c54604a24e65b54e8c056c1f2e")
2022-03-04 15:47:37.534 xctest[26418:2456126] Block total proof:100
2022-03-04 15:47:37.534 xctest[26418:2456126] Block first proof public key:0101f5170c996cc02b581d8200f0d95a737840234f31bf1fa21cca35137f8507b0
2022-03-04 15:47:37.534 xctest[26418:2456126] Block first proof signature:01693a9ffafc51c52d4ee7b2959ec328427c403d1b3a29f09bb78593bceab92ae79808754e6e38147e646dd5b4b9b1c8c2a45675af5d5cd0aead72bb0d6c354e08
2022-03-04 15:47:37.678 xctest[26418:2456126] Error:CasperError(code: -32001, message: "block not known", methodCall: "chain_get_block")
2022-03-04 15:47:42.647 xctest[26418:2456208] Era state root hash:d0e627faad27cc510efc524f870363646a8cd33ba6686f35d083f61b2a3a6e56
2022-03-04 15:47:42.647 xctest[26418:2456208] Era block hash:f3e4f0249ca558ed568295f5a902bd66e147447f2426191d50fa6f0b8948c357
2022-03-04 15:47:42.669 xctest[26418:2456208] Era merkle_proof length:1235350
2022-03-04 15:47:42.669 xctest[26418:2456208] Era stored_value:EraInfo(CasperSDKInSwift.EraInfo)
2022-03-04 15:47:42.669 xctest[26418:2456208] In chain_get_era_info_by_switch_block, stored_value is EraInfo
2022-03-04 15:47:42.669 xctest[26418:2456208] In chain_get_era_info_by_switch_block, total seigniorage_allocations:8605
2022-03-04 15:47:42.669 xctest[26418:2456208] Delegator amount:8898767
2022-03-04 15:47:42.669 xctest[26418:2456208] Delegator delegator_public_key:010ca8f91a2704a56701bdc4cc16f70e341e01281ef20bcb5475bf83ffe48841bd
2022-03-04 15:47:42.669 xctest[26418:2456208] Delegator validator_public_key:0101a458aa2b551c5a49e56326f9bb298bb308e1babc875647ae0290c42f13feac
2022-03-04 15:47:42.987 xctest[26418:2456209] Error:CasperError(code: -32001, message: "block not known", methodCall: "chain_get_era_info_by_switch_block")
2022-03-04 15:47:43.278 xctest[26418:2456209] In state_get_item, stored_value is Withdraw
2022-03-04 15:47:43.278 xctest[26418:2456209] Total UnbondingPurse:1
2022-03-04 15:47:43.278 xctest[26418:2456209] Withdraw first  UnbondingPurse, bonding_purse:Optional("uref-5fcc3031ea2572f9929e0cfcfc84c6c3131bfe1e78bce8cb61f99f59eace7795-007")
2022-03-04 15:47:43.278 xctest[26418:2456209] Withdraw first  UnbondingPurse, amount:500
2022-03-04 15:47:43.278 xctest[26418:2456209] Withdraw first  UnbondingPurse, era_of_creation:3319
2022-03-04 15:47:43.278 xctest[26418:2456209] Withdraw first  UnbondingPurse, unbonder_public_key:01d949a3a1963db686607a00862f79b76ceb185fc134d0aeedb686f1c151f4ae54
2022-03-04 15:47:43.278 xctest[26418:2456209] Withdraw first  UnbondingPurse, validator_public_key:01d949a3a1963db686607a00862f79b76ceb185fc134d0aeedb686f1c151f4ae54
2022-03-04 15:47:43.278 xctest[26418:2456209] StateGetItem merkle_proof length:6876
2022-03-04 15:47:43.428 xctest[26418:2456209] Error:CasperError(code: -32602, message: "Invalid params", methodCall: "state_get_item")
2022-03-04 15:47:43.578 xctest[26418:2456209] Error:CasperError(code: -32002, message: "failed to parse key: withdraw-key from string error: Invalid byte `b\'f\'`, at index 1.", methodCall: "state_get_item")
2022-03-04 15:47:43.728 xctest[26418:2456209] Error:CasperError(code: -32002, message: "failed to parse key: unknown prefix for key", methodCall: "state_get_item")
2022-03-04 15:47:43.879 xctest[26418:2456208] In state_get_dictionary_item, stored_value is CLValue
2022-03-04 15:47:43.879 xctest[26418:2456208] In state_get_dictionary_item, CLValue of stored_value, bytes:090000006162635f76616c7565
2022-03-04 15:47:43.879 xctest[26418:2456208] In state_get_dictionary_item, CLValue of stored_value,cl_type:String
2022-03-04 15:47:43.880 xctest[26418:2456208] In state_get_dictionary_item, CLValue of stored_value,parsed:String("abc_value")
2022-03-04 15:47:43.881 xctest[26418:2456208] GetDictionaryItem merkle_proof length:30330
2022-03-04 15:47:43.881 xctest[26418:2456208] GetDictionaryItemResult dictionary_key:Optional("dictionary-5d3e90f064798d54e5e53643c4fce0cbb1024aadcad1586cc4b7c1358a530373")
2022-03-04 15:47:44.028 xctest[26418:2456209] Error:CasperError(code: -32002, message: "Failed to parse key", methodCall: "state_get_dictionary_item")
2022-03-04 15:47:44.179 xctest[26418:2456211] GetBalanceResult, balance_value: 522693296224
2022-03-04 15:47:44.180 xctest[26418:2456211] GetBalanceResult, merkle_proof length:31766
2022-03-04 15:47:44.328 xctest[26418:2456126] Error got:CasperError(code: -32005, message: "failed to parse purse_uref: Hex(InvalidByte { index: 0, byte: 102 })", methodCall: "state_get_balance")
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState state_root_hash:8b463b56f2d124f43e7c157e602e31d5d2d5009659de7f1e79afbd238cbaa189
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState block_height:473576
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState total era_validator:1538
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState first bid staked_amount: 908982507030
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState first bid delegation_rate: 10
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState first bid inactive: true
2022-03-04 15:47:47.234 xctest[26418:2456209] AuctionState first bid total delegator: 1
2022-03-04 15:47:47.234 xctest[26418:2456209] Information for first bid first delegator
2022-03-04 15:47:47.234 xctest[26418:2456209] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-03-04 15:47:47.234 xctest[26418:2456209] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-03-04 15:47:47.234 xctest[26418:2456209] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-03-04 15:47:47.234 xctest[26418:2456209] First delegator staked_amount:30268476029
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState state_root_hash:8b463b56f2d124f43e7c157e602e31d5d2d5009659de7f1e79afbd238cbaa189
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState block_height:473576
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState total era_validator:1538
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState first bid staked_amount: 908982507030
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState first bid delegation_rate: 10
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState first bid inactive: true
2022-03-04 15:47:49.249 xctest[26418:2456209] AuctionState first bid total delegator: 1
2022-03-04 15:47:49.249 xctest[26418:2456209] Information for first bid first delegator
2022-03-04 15:47:49.249 xctest[26418:2456209] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-03-04 15:47:49.249 xctest[26418:2456209] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-03-04 15:47:49.249 xctest[26418:2456209] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-03-04 15:47:49.249 xctest[26418:2456209] First delegator staked_amount:30268476029
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState state_root_hash:530a0bd4bc05712109e2cea9114301e4f47c1dafc1eabb44344a1cd6b9a22f9c
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState block_height:585007
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState total era_validator:1542
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState first bid public_key:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState first bid staked_amount: 908982507030
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState first bid bonding_purse: Optional("uref-68f12244cf9e37759aa78e3146c431cc4577fc122272989b9f9ebf2e8f27d741-007")
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState first bid delegation_rate: 10
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState first bid inactive: true
2022-03-04 15:47:50.894 xctest[26418:2456209] AuctionState first bid total delegator: 1
2022-03-04 15:47:50.894 xctest[26418:2456209] Information for first bid first delegator
2022-03-04 15:47:50.894 xctest[26418:2456209] First delegator bonding_purse:Optional("uref-401f87167d733d8dd7d3efbf135a91ccd42fffb77b02d4a0075b963f14f1fbb4-007")
2022-03-04 15:47:50.894 xctest[26418:2456209] First delegator delegatee:01001b79b9a6e13d2b96e916f7fa7dff40496ba5188479263ca0fb2ccf8b714305
2022-03-04 15:47:50.894 xctest[26418:2456209] First delegator public_key:018b34b15e023844531621cb52d42e216a2ea56034f0f40bf7cee566c32eae4f83
2022-03-04 15:47:50.894 xctest[26418:2456209] First delegator staked_amount:30268476029
2022-03-04 15:47:51.033 xctest[26418:2456209] Error :CasperError(code: -32001, message: "get-auction-info failed to get specified block", methodCall: "state_get_auction_info")
Test Case '-[CasperSDKInSwiftTests.CasperSDKInSwiftTests testAll]' passed (22.685 seconds).
Test Suite 'CasperSDKInSwiftTests' passed at 2022-03-04 15:47:51.036.
	 Executed 1 test, with 0 failures (0 unexpected) in 22.685 (22.686) seconds
Test Suite 'TestCLTypeSerialization' started at 2022-03-04 15:47:51.036
Test Case '-[CasperSDKInSwiftTests.TestCLTypeSerialization testAll]' started.
Test Case '-[CasperSDKInSwiftTests.TestCLTypeSerialization testAll]' passed (0.001 seconds).
Test Suite 'TestCLTypeSerialization' passed at 2022-03-04 15:47:51.037.
	 Executed 1 test, with 0 failures (0 unexpected) in 0.001 (0.001) seconds
Test Suite 'TestCLValueSerialization' started at 2022-03-04 15:47:51.037
Test Case '-[CasperSDKInSwiftTests.TestCLValueSerialization testAll]' started.
Test Case '-[CasperSDKInSwiftTests.TestCLValueSerialization testAll]' passed (0.009 seconds).
Test Suite 'TestCLValueSerialization' passed at 2022-03-04 15:47:51.045.
	 Executed 1 test, with 0 failures (0 unexpected) in 0.009 (0.009) seconds
Test Suite 'TestDeploySerialization' started at 2022-03-04 15:47:51.045
Test Case '-[CasperSDKInSwiftTests.TestDeploySerialization testAll]' started.
Test Case '-[CasperSDKInSwiftTests.TestDeploySerialization testAll]' passed (0.011 seconds).
Test Suite 'TestDeploySerialization' passed at 2022-03-04 15:47:51.057.
	 Executed 1 test, with 0 failures (0 unexpected) in 0.011 (0.011) seconds
Test Suite 'TestEd25519KeyWrapper' started at 2022-03-04 15:47:51.057
Test Case '-[CasperSDKInSwiftTests.TestEd25519KeyWrapper testAll]' started.
Ed25519 PublicKey in hexa
f1e2dc53cf3999d6fe3a3aef3227d6da44ca47f8a0027f2d17b9f697b2715e47
Ed25519 PrivateKey in hexa
bd37ac1a534d7b6245225cdedefc706f96dc0d159a8a7458b2757c4df0f391bd
2022-03-04 15:47:51.057 xctest[26418:2456124] Delete auto generated Ed25519 private file.
2022-03-04 15:47:51.058 xctest[26418:2456124] Delete auto generated Ed25519 private file.
Key pair generation, private key in hexa
e111168abcc56c462eb49966dd11cdc5280d811e9d89341e97ff44d356842780
Key pair generation, public key in hexa
f6d5b421a389b80bbcfbc5d13e71dba9b6f1288ab5ca1ba159035db2ecd0557d
Test Case '-[CasperSDKInSwiftTests.TestEd25519KeyWrapper testAll]' passed (0.003 seconds).
Test Suite 'TestEd25519KeyWrapper' passed at 2022-03-04 15:47:51.060.
	 Executed 1 test, with 0 failures (0 unexpected) in 0.003 (0.003) seconds
Test Suite 'TestPutDeploy' started at 2022-03-04 15:47:51.060
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testAll]' started.
Test Case '-[CasperSDKInSwiftTests.TestPutDeploy testAll]' passed (1.030 seconds).
Test Suite 'TestPutDeploy' passed at 2022-03-04 15:47:52.090.
	 Executed 1 test, with 0 failures (0 unexpected) in 1.030 (1.030) seconds
Test Suite 'TestSecp256k1KeyWrapper' started at 2022-03-04 15:47:52.090
Test Case '-[CasperSDKInSwiftTests.TestSecp256k1KeyWrapper testAll]' started.
2022-03-04 15:47:52.765 xctest[26418:2456124] Private key of secp256k1 read from Pem file:
2022-03-04 15:47:52.942 xctest[26418:2456124] -----BEGIN EC PRIVATE KEY-----
MHQCAQEEILgH3Z+UnasGUDgH00EnGtrX1HmEFHafR+879tC13QzsoAcGBSuBBAAK
oUQDQgAEno6M4vcQFkO5ilpWOCwSjKZUKem01Mp+jXyfDRCyHExXonghUeSGALy0
Ww9+6vD79dMGg7VdVIxviGF9nV0mNg==
-----END EC PRIVATE KEY-----
2022-03-04 15:47:53.120 xctest[26418:2456124] Delete auto generated Secp256k1 private file.
2022-03-04 15:47:54.455 xctest[26418:2456124] Public key of secp256k1 read from Pem file:
2022-03-04 15:47:54.455 xctest[26418:2456124] -----BEGIN PUBLIC KEY-----
MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAExtEDVh+DpBKB0njgfkWQVSm/JddPoYRj
GjCa/nvD3AZbWpRrnx2PmN7Z2Ax7AFZlKkZH/DXHzTw1hEzTMIcnwA==
-----END PUBLIC KEY-----
2022-03-04 15:47:54.456 xctest[26418:2456124] Delete auto generated Secp256k1 public file.
2022-03-04 15:47:55.961 xctest[26418:2456124] Private key of secp256k1 from key pair
2022-03-04 15:47:56.140 xctest[26418:2456124] -----BEGIN EC PRIVATE KEY-----
MHQCAQEEIOboe43BWXwRiM5GXuDmPOutrOeudrQ9YOHTsHA0oPxaoAcGBSuBBAAK
oUQDQgAEIqWY8rLYQe4A0reKnCqgc9HGb442xRPBziQ/8qX04xETdaKJaP4yx2eM
Me8v6cye47nexwIvSNrDOxTwLuB7LQ==
-----END EC PRIVATE KEY-----
2022-03-04 15:47:56.140 xctest[26418:2456124] Public key of secp256k1 from key pair
2022-03-04 15:47:56.141 xctest[26418:2456124] -----BEGIN PUBLIC KEY-----
MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAEIqWY8rLYQe4A0reKnCqgc9HGb442xRPB
ziQ/8qX04xETdaKJaP4yx2eMMe8v6cye47nexwIvSNrDOxTwLuB7LQ==
-----END PUBLIC KEY-----
Test Case '-[CasperSDKInSwiftTests.TestSecp256k1KeyWrapper testAll]' passed (4.609 seconds).
Test Suite 'TestSecp256k1KeyWrapper' passed at 2022-03-04 15:47:56.699.
	 Executed 1 test, with 0 failures (0 unexpected) in 4.609 (4.609) seconds
Test Suite 'CasperSDKInSwiftPackageTests.xctest' passed at 2022-03-04 15:47:56.699.
	 Executed 7 tests, with 0 failures (0 unexpected) in 28.348 (28.349) seconds
Test Suite 'All tests' passed at 2022-03-04 15:47:56.699.
	 Executed 7 tests, with 0 failures (0 unexpected) in 28.348 (28.350) seconds
```