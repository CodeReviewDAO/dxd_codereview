```bash
[info] welcome to sbt 1.5.7 (Azul Systems, Inc. Java 11.0.13)
[info] loading project definition from /workspace/casper-scala-sdk/project
[info] loading settings for project casper-scala-sdk from build.sbt,build_.sbt ...
[info] set current project to casper-scala-sdk (in build file:/workspace/casper-scala-sdk/)
[info] JsonConverterTest:
[info] KeyAlgorithmTest:
[info] ByteUtilTest:
[info] URefDeserializerTest:
[info] RPCResultDeserializerTest:
[info] CLPublicKeyDeserializerTest:
[info] - Deserialize CLPublicKey
[info]   + PublicKey is not null 
[info]   + pubKey.bytes  is the same as new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e").bytes 
[info] CLTypeDeserialiserTest:
[info] - Deserialize  U512 CLType
[info] - Deserialize  ByteArray CLType
[info] - Deserialize  Option CLType
[info] CLValueSerializerTest:
[info] - Deserialize U512 value
[info]   + value is not null 
[info]   + parsed value = 1000000000  
[info]   + cl_type = U512  
[info]   + bytes same as  HexUtils.fromHex("0400ca9A3B")  
[info] - Deserialize PublicKey value
[info]   + value is not null 
[info]   + parsed value = 017d96B9A63abCB61c870A4F55187a0a7AC24096bdB5fc585C12A686a4D892009e  
[info]   + cl_type = PublicKey  
[info]   + bytes same as  HexUtils.fromHex("017d96B9A63abCB61c870A4F55187a0a7AC24096bdB5fc585C12A686a4D892009e")  
[info] - Deserialize byteArray32 value
[info]   + value is not null 
[info]   + parsed value = 2fe0d35b6a92e17ee8f3ee3693452d6141df5c8db8e17a1c0985572842e13385  
[info]   + cl_type = ByteArray  
[info]   + bytes same as  HexUtils.fromHex("2fe0d35b6a92e17ee8f3ee3693452d6141df5c8db8e17a1c0985572842e13385")  
[info] - Deserialize Option value
[info]   + value is not null 
[info]   + parsed value = null 
[info]   + cl_type = U64  
[info]   + bytes same as  HexUtils.fromHex("00")  
[info] - Deserialize String value
[info]   + value is not null 
[info]   + parsed value = https://caspercommunity.io 
[info]   + cl_type = String  
[info]   + bytes same as  HexUtils.fromHex("1a00000068747470733a2f2f636173706572636f6d6d756e6974792e696f")  
[info] CasperSdkTest:
[info] - RPC Call to a non existing node (http://1.2.3.4:7777/rpc) Throws an RPCIOException
[info] - Testnet Network Peers list is not empty
[info]   + Peers List size : 397 
[info] - Get state root hash with no blockHash paramter, state root hash is not empty and is 64 characters long
[info]   + state root hash : 2183d6f1315EC51D3F5b5124c54a7CFe9F7B7A5f4422aE9dc154B0a0C1FfaE1E 
[info] - Get state root hash with a blockHash parameter ,state root hash is not empty and is 64 character  long
[info]   + state root hash : 2183d6f1315EC51D3F5b5124c54a7CFe9F7B7A5f4422aE9dc154B0a0C1FfaE1E 
[info] - Get Block using Block hash parameter
[info]   + block  hash : 74dce8911A3EDf0f872dC11F0a63Ca9fE1b55b7188a9Feaaf431518bF9c508B4 
[info] - Get Block using an empty Block hash parameter, retrieves the latest known block hash
[info]   + block  hash : 0b6608B88dA36F66AF41464feafDB4c08dAb385A71a05548b9b0Fd36ac830510 
[info] - Get Block using non existing Block hash parameter, retrieves the latest known block hash
[info]   + block  hash : 0b6608B88dA36F66AF41464feafDB4c08dAb385A71a05548b9b0Fd36ac830510 
[info] - Get Block using Block height parameter
[info] - Get Block using non existing Block height  parameter
[info] - Get Deploy using a Deploy hash parameter
[info]   + deploy  header is not null 
[info]   + This deploy  has a ModuleBytes paiement  
[info]   + This deploy  has a StoredContractByHash as session 
[info] - Get Deploy using an empty Deploy hash parameter, throws RPCException with message: Invalid params 
[info] - Get Node Status
[info]   + assert node pub key is : 01cd807fb41345d8dD5A61da7991e1468173acbEE53920E4DFe0D28Cb8825AC664 
[info]   + assert network is : casper-test  
[info] - getBlockTransfers 
[info]   + assert this block contains two transfert 
[info]   + assert first transfert deploy hash is = 277AEF49321B3b19B0EDd732Cd5CFf4F2E76c1Df0260356367711aD81f4bC8FC 
[info]   + assert amount of first transfert is = 1000000000000 motes 
[info] - getAuctionInfo with a block hash , retieves current auction state
[info]   + assert  state_root_hash = current state root hash 
[info] - getAuctionInfo with empty block hash, retieves current auction state
[info]   + assert  state_root_hash = current state root hash 
[info] - getEraInfoBySwitchBlock : 2974-->2975 : 1e46B4c173dB70fDE0E867FF679ACa24e1c5Bea3C4333af94e53B4E3BC548B6B
[info]   + assert  era = 2974 
[info]   + assert  state root hash  = c1A62d5DeB74d3fEAfeCd1EEa526941edd0264895EB8E516474108D4EA4D7D21 
[info] - getEraInfoBySwitchBlock non switch bloc : a2C85FD13bba200E47c2d7c74E87F0f0c96aDcEE227877168a639Fa67d046933 , throws RPCException
[info] - getEraInfoBySwitchBlock with empty block param, throws RPCException 
[info] - getStateItem   retrieving Contract
[info]   + assert contract is not null  
[info]   + assert contract_package_hash = contract-wasm-8D1c5ab95baaa77c302232a00FE1C6cF6975ffD6430a9ECd87EC5266280BB18D 
[info]   + assert first enry point is an allowance  
[info]   + assert first arg of the first entry point is of type CLType = Key   
[info] - getStateItem   retrieving Account
[info]   + assert contract is  null  
[info]   + assert account is not null  
[info]   + assert main_purse : uref-9cC68775d07c211e44068D5dCc2cC28A67Cb582C3e239E83Bb0c3d067C4D0363-007 
[info] - getStateItem   retrieving CLValue
[info] - getStateItem with wrong parameters , throws RPCException 
[info] - getStateItem with empty parameters , throws RPCException 
[info] - getBalance   with existing account
[info]   + Assert balance = 869077209920 motes  
[info] - getBalance  with non hex key account , throws IllegalArgumentException
[info] - getBalance  with non uref key account, throws IllegalArgumentException
[info] - getDictionaryItem   
[info]   + CLValeu is not nul   
[info]   + cl_Type is String    
[info]   + CLValeu parsed =  "https://caspercommunity.io"  
[info] Run completed in 14 seconds, 540 milliseconds.
[info] Total number of tests run: 36
[info] Suites: completed 9, aborted 0
[info] Tests: succeeded 36, failed 0, canceled 0, ignored 0, pending 0
[info] All tests passed.
[success] Total time: 16 s, completed Dec 19, 2021, 7:59:22 PM
```
