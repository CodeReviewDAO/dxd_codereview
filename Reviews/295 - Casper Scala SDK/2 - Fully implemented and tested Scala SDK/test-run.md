```
Run sbt test
copying runtime jar...
[info] [launcher] getting org.scala-sbt sbt 1.5.7  (this may take some time)...
[info] [launcher] getting Scala 2.12.14 (for sbt)...
[info] Updated file /home/runner/work/casper-scala-sdk/casper-scala-sdk/project/build.properties: set sbt.version to 1.5.7
[info] welcome to sbt 1.5.7 (AdoptOpenJDK Java 11.0.11)
[info] loading project definition from /home/runner/work/casper-scala-sdk/casper-scala-sdk/project
[info] loading settings for project casper-scala-sdk from build.sbt ...
[info] set current project to casper-scala-sdk (in build file:/home/runner/work/casper-scala-sdk/casper-scala-sdk/)
[info] compiling 99 Scala sources to /home/runner/work/casper-scala-sdk/casper-scala-sdk/target/scala-3.0.2/classes ...
[info] done compiling
[info] compiling 25 Scala sources to /home/runner/work/casper-scala-sdk/casper-scala-sdk/target/scala-3.0.2/test-classes ...
[info] done compiling
[info] URefTest:
[info] - Test Uref AccessRight
[info] - Test Uref decode 
[info] - Test format Uref  
[info] - Test new Uref with a non valid hex string  , throws IllegalArgumentException
[info] DeployApprovalByteSerializerTest:
[info] - Test DeployApprovalByteSerializer with a signle DeployApproval  
[info] ByteUtilTest:
[info] JsonConverterTest:
[info] CLPublicKeySerializerTest:
[info] - Test serialize CLPublicKey 
[info] CLPublicKeyDeserializerTest:
[info] - Deserialize CLPublicKey
[info]   + PublicKey is not null 
[info]   + pubKey.bytes  is the same as new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e").bytes 
[info] DeployExecutableByteSerializerTest:
[info] - Test serialize ModuleBytes 
[info] - Test serialize storedContractByName 
[info] - Test serialize storedContractByHash 
[info] - Test serialize storedVersionedContractByHash 
[info] - Test serialize DeployTransfer 
[info] URefDeserializerTest:
[info] - Deserialize URef
[info]   + PublicKey is not null 
[info]   + uref.bytes  is the same as new Uref("uref-9cC68775d07c211e44068D5dCc2cC28A67Cb582C3e239E83Bb0c3d067C4D0363-007").bytes 
[info] CLPublicKeyTest:
[info] - Test CLPublicKey KeyAlgorithm = ED25519
[info] - Test CLPublicKey  decode 
[info] - Test CLPublicKey formatAsHexAccount   
[info] - Test new CLPublicKey with a non valid hex string  , throws IllegalArgumentException
[info] RPCResultDeserializerTest:
[info] - RPCResultDeserializer test with getPeers
[info] - RPCResultDeserializer test with getStateRootHash
[info]   + Signature is not null 
[info]   + signature.bytes  is the same as new Signature("012dbf03817a51794a8e19e0724884075e6d1fbec326b766ecfa6658b41f81290da85e23b24e88b1c8d9761185c961daee1adab0649912a6477bcd2e69bd91bd08").bytes 
[info] AccountHashDeserializerTest:
[info] - Deserialize AccountHash
[info]   + AccountHash is not null 
[info]   + account.bytes  is the same as new AccountHash("account-hash-85148dcd6c54b77e462a9acf387fb05aca953a83011db2c601716de0af1cf47c").bytes 
[info] AccountHashTest:
[info] - Test AccountHash  decode 
[info] - Test AccountHash formatAsHexAccount   
[info] - Test new AccountHash with a non valid hex string  , throws IllegalArgumentException
[info] DeployNamedArgByteSerializerTest:
[info] - Test serialize DeployNamedArg  with String CLValue
[info] - Test serialize DeployNamedArg  with U512 CLValue
[info] - Test serialize DeployNamedArg  with Bytearray CLValue
[info] - Test serialize DeployNamedArg  with CLPublicKey CLValue
[info] - Test serialize DeployNamedArg  with URef CLValue
[info] DeployHeaderByteSerializerTest:
[info] - Test serialize DeployHeader 
[info] CasperSdkTest:
[info] - RPC Call to a non existing node (http://1.2.3.4:7777/rpc) Throws an RPCIOException
[info] - Testnet Network Peers list is not empty
[info]   + Peers List size : 356 
[info] - Get state root hash with no blockHash parameter, state root hash is not empty and is 64 characters long
[info]   + state root hash : d023cc0012a2f9b37d01271fba5fd95c94882bf527eb088bb945809bc1b248e4 
[info] - Get state root hash with a blockHash parameter ,state root hash is not empty and is 64 character  long
[info]   + state root hash : d023cc0012a2f9b37d01271fba5fd95c94882bf527eb088bb945809bc1b248e4 
[info] - Get Block using Block hash parameter
[info]   + block  hash : 74dce8911a3edf0f872dc11f0a63ca9fe1b55b7188a9feaaf431518bf9c508b4 
[info] - Get Block using an empty Block hash parameter, retrieves the latest known block hash
[info]   + block  hash : 1a28e52a93ebfff1d2c885a2ea66b17d8808832eed33aacacaca9e9ed1c9fd54 
[info] - Get Block using non existing Block hash parameter, retrieves the latest known block hash
[info]   + block  hash : 1a28e52a93ebfff1d2c885a2ea66b17d8808832eed33aacacaca9e9ed1c9fd54 
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
[info]   + CLValue is not nul   
[info]   + cl_Type is String    
[info]   + CLValue parsed =  "https://caspercommunity.io"  
[info] Run completed in 16 seconds, 825 milliseconds.
[info] Total number of tests run: 128
[info] Suites: completed 23, aborted 0
[info] Tests: succeeded 128, failed 0, canceled 0, ignored 0, pending 0
[info] All tests passed.
[success] Total time: 35 s, completed Jan 7, 2022, 8:47:02 PM
```

