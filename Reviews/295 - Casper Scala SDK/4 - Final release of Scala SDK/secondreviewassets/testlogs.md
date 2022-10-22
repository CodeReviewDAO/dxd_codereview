# Output of the "sbt test" command

```sh

Picked up JAVA_TOOL_OPTIONS:  -Xmx3489m
[info] welcome to sbt 1.7.2 (Temurin Java 1.8.0_345)
[info] loading project definition from /workspace/casper-scala-sdk/project
[info] loading settings for project casper-scala-sdk from build.sbt ...
[info] set current project to casper-scala-sdk (in build file:/workspace/casper-scala-sdk/)
[info] compiling 107 Scala sources to /workspace/casper-scala-sdk/target/scala-3.1.3/classes ...
[warn] -- Warning: /workspace/casper-scala-sdk/src/main/scala/com/casper/sdk/domain/deploy/Deploy.scala:72:3 
[warn] 72 |   Blake2b256.hash(Try(builder.addAll(serializer.toBytes(payment).get).addAll(serializer.toBytes(session).get)).toOption.get.result())
[warn]    |   ^
[warn]    |   Line is indented too far to the left, or a `}` is missing
[warn] -- [E029] Pattern Match Exhaustivity Warning: /workspace/casper-scala-sdk/src/main/scala/com/casper/sdk/serialization/cltypes/CLValueByteSerializer.scala:32:83 
[warn] 32 |  def CLTypesToBytes(builder: ArrayBuilder.ofByte, innerType: CLTypeInfo): Unit =  innerType match {
[warn]    |                                                                                   ^^^^^^^^^
[warn]    |match may not be exhaustive.
[warn]    |
[warn]    |It would fail on pattern case: cltypes.CLTypeInfo(Option), cltypes.CLTypeInfo(List), cltypes.CLTypeInfo(ByteArray), cltypes.CLTypeInfo(Result), cltypes.CLTypeInfo(Map), cltypes.CLTypeInfo(Tuple1)
[warn]    |(More unmatched cases are elided)
[warn]    |
[warn]    | longer explanation available when compiling with `-explain`
[warn] two warnings found
[info] done compiling
[info] compiling 35 Scala sources to /workspace/casper-scala-sdk/target/scala-3.1.3/test-classes ...
[info] done compiling
01d9bf2148748a85c89da5aad8ee0b0fc2d105fd39d41a4c796536354f0ae2900ca647f0a88301000040771b000000000001000000000000004811966d37fe5674a8af4001884ea0d9042d1c06668da0c963769c3a01ebd08f0100000001010101010101010101010101010101010101010101010101010101010101010e0000006361737065722d6578616d706c65[info] TimeStampSerializerTest:
[info] ByteUtilTest:
[info] - ByteUtils join Test 
[info] DeployApprovalByteSerializerTest:
[info] - Test DeployApprovalByteSerializer with a signle DeployApproval  
[info] TTLSerializerTest:
[info] - Serialize CLPublicKey
[info]   + new Hash( CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e")) json serialization =  "7d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e" 
[info] DeployByteSerializerTest:
[info] - Test DeployByteSerializer with json deploy  
[info] CLTypeInfoSerializerTest:
[info] - Serialize CLTypeInfo with U64
[info]   + new  CLTypeInfo(CLType.U64) json serialization =  "U64" 
[info] - Serialize CLTypeInfo with String
[info]   + new  CLTypeInfo(CLType.String) json serialization =  "String" 
[info] - Serialize CLTypeInfo with ByteArray
[info]   + new  new CLByteArrayTypeInfo(124) json serialization =  {"ByteArray":124} 
[info] - Serialize CLTypeInfo with Option
[info]   + new  new CLOptionTypeInfo(new CLTypeInfo(CLType.I64)) json serialization =  {"Option":"I64"} 
[info] CLValueDeSerializerTest:
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
[info]   + cl_type = Option  
[info]   + inner cltype = U64  
[info]   + bytes same as  HexUtils.fromHex("00")  
[info] - Deserialize String value
[info]   + value is not null 
[info]   + parsed value = https://caspercommunity.io 
[info]   + cl_type = String  
[info]   + bytes same as  HexUtils.fromHex("1a00000068747470733a2f2f636173706572636f6d6d756e6974792e696f")  
[info] DeployExecutableByteSerializerTest:
[info] - Test serialize ModuleBytes 
[info] - Test serialize storedContractByName 
[info] - Test serialize storedContractByHash 
[info] - Test serialize storedVersionedContractByHash 
[info] - Test serialize StoredVersionedContractByName 
[info] - Test serialize DeployTransfer 
[info] DeployNamedArgByteSerializerTest:
[info] - Test serialize DeployNamedArg  with String CLValue
[info] - Test serialize DeployNamedArg  with U512 CLValue
[info] - Test serialize DeployNamedArg  with Bytearray CLValue
[info] - Test serialize DeployNamedArg  with CLPublicKey CLValue
[info] - Test serialize DeployNamedArg  with URef CLValue
[info] DeployExecutableSerializerTest:
[info] - DeployExecutableSerializerTest with StoredContractByHash
[info] - DeployExecutableSerializerTest with StoredVersionedContractByHash
[info] - DeployExecutableSerializerTest with StoredVersionedContractByName
[info] - DeployExecutableSerializerTest with StoredContractByName
[info] - DeployExecutableSerializerTest with Transfer
[info] DeployExecutableDeserializerTest:
[info] - DeployExecutableDeserializer test ModuleBytes 
[info] - DeployExecutableDeserializer test StoredContractByName 
[info] - DeployExecutableDeserializer test StoredVersionedContractByHash 
[info] - DeployExecutableDeserializer test StoredVersionedContractByName 
[info] - DeployExecutableDeserializer test Transfer 
[info] CLValueByteSerializerTest:
[info] - Test  serialize data with true Bool CLValue 
[info] - Test CLValueByteSerializer with true Bool CLType 
[info] - Test serialize data  Unit CLType 
[info] - Test CLValueByteSerializer with Unit CLType 
[info] - Test serialize data  U8 CLType 
[info] - Test CLValueByteSerializer with U8 CLType 
[info] - Test serialize data String CLType 
[info] - Test CLValueByteSerializer with String CLType 
[info] - Test serialize data  I32 CLType 
[info] - Test CLValueByteSerializer with I32 CLType 
[info] - Test serialize data  U32 CLType 
[info] - Test CLValueByteSerializer with U32 CLType 
[info] - Test serialize data  I64 CLType 
[info] - Test CLValueByteSerializer with I64 CLType 
[info] - Test serialize data  U64 CLType 
[info] - Test CLValueByteSerializer with U64 CLType 
[info] - Test serialize data  U128 CLType 
[info] - Test CLValueByteSerializer with U128 CLType 
[info] - Test serialize data  U256 CLType 
[info] - Test CLValueByteSerializer with U256 CLType 
[info] - Test serialize data  U512 CLType 
[info] - Test CLValueByteSerializer with U512 CLType 
[info] - Test serialize data None Option CLType 
[info] - Test CLValueByteSerializer with None Option CLType 
[info] - Test serialize data  Option CLType 
[info] - Test CLValueByteSerializer with  Option CLType 
[info] - Test serialize Empty List of CLType return None 
[info] - Test serialize non empty List of CLType 
[info] - Test CLValueBteSerializer with non empty List of CLType 
[info] - Test serialize Ok Result CLType 
[info] - Test CLValueBteSerializer with Ok Result CLType 
[info] - Test serialize Err Result CLType 
[info] - Test CLValueBteSerializer with Err Result CLType 
[info] - Test serialize Tuple1  CLType 
[info] - Test CLValueBteSerializer with Tuple1 CLType 
[info] - Test serialize Tuple2  CLType 
[info] - Test CLValueBteSerializer with Tuple2 CLType 
[info] - Test serialize Tuple3  CLType 
[info] - Test CLValueBteSerializer with Tuple3 CLType 
[info] - Test serialize ByteArray  CLType 
[info] - Test CLValueBteSerializer with ByteArray CLType 
[info] - CLTypesToBytes Test with String CLType
[info] - CLTypesToBytes Test with U64 CLType
[info] - CLTypesToBytes Test with U128 CLType
[info] - CLTypesToBytes Test with U256 CLType
[info] - CLTypesToBytes Test with U512 CLType
[info] - CLTypesToBytes Test with I32 CLType
[info] - CLTypesToBytes Test with Bool CLType
[info] - CLTypesToBytes Test with Unit CLType
[info] - CLTypesToBytes Test with PublicKey CLType
[info] - CLTypesToBytes Test with Uref CLType
[info] - CLTypesToBytes Test with CLByteArrayTypeInfo 
[info] - CLTypesToBytes Test with CLOptionTypeInfo 
[info] - CLTypesToBytes Test with CLTuple1TypeInfo 
[info] - CLTypesToBytes Test with CLTuple2TypeInfo 
[info] - CLTypesToBytes Test with CLTuple3TypeInfo 
[info] - CLTypesToBytes Test with CCListTypeInfo 
[info] - CLTypesToBytes Test with CLResultTypeInfo 
[info] CLTypeDeserialiserTest:
[info] - Deserialize  U512 CLType
[info] - Deserialize  ByteArray CLType
[info] - Deserialize  Option CLType
[info] KeyAlgorithmTest:
[info] DeployHeaderByteSerializerTest:
[info] - Test serialize DeployHeader 
[info] SignatureTest:
[info] - Test Signature KeyAlgorithm = ED25519
[info] - Test Signature  decode 
[info] - Test Signature formatAsHexAccount   
[info] - Test new Signature with a non valid hex string  gives None
[info] CLValueSerializerTest:
[info] - Serialize Option value
[info]   + CLValue.Option(CLValue.String("Hello, World!")) serializes to {"cl_type":{"Option":"String"},"bytes":"010d00000048656c6c6f2c20576f726c6421","parsed":"Hello, World!"} 
[info] - Serialize Bool value
[info]   + CLValue.Bool(true) serializes to {"cl_type":"Bool","bytes":"01","parsed":"true"} 
[info] - Serialize String value
[info]   + CLValue.String("Hello, world!") serializes to {"cl_type":"String","bytes":"0d00000048656c6c6f2c20776f726c6421","parsed":"Hello, world!"} 
[info] - Serialize U8 value
[info]   + CLValue.U8(7) serializes to {"cl_type":"U8","bytes":"00000000000000","parsed":"7"} 
[info] - Serialize U512 value
[info]   + CLValue.U512(458745874) serializes to {"cl_type":"U512","bytes":"0412e8571b","parsed":"458745874"} 
[info] - Serialize U32 value
[info]   + CLValue.U32(45874) serializes to {"cl_type":"U32","bytes":"32b30000","parsed":"45874"} 
[info] - Serialize I32 value
[info]   + CLValue.I32(10000) serializes to {"cl_type":"I32","bytes":"10270000","parsed":"10000"} 
[info] - Serialize I64 value
[info]   + CLValue.I64(-541287) serializes to {"cl_type":"I64","bytes":"99bdf7ffffffffff","parsed":"-541287"} 
[info] - Serialize U128 value
[info]   + CLValue.U128(458745874) serializes to {"cl_type":"U128","bytes":"04bf3d3209","parsed":"154287551"} 
[info] - Serialize U256 value
[info]   + CLValue.U256(BigInt.apply("4545487556545454545454")) serializes to {"cl_type":"U256","bytes":"092e1a2022a7d14f69f6","parsed":"4545487556545454545454"} 
[info] - Serialize List of CLvalues
[info]   + CLValue.List(CLValue.String("abc"),CLValue.String("defg") , CLValue.String("hijklmnopq")) serializes to {"cl_type":{"List":"String"},"bytes":"030000000300000061626304000000646566670a00000068696a6b6c6d6e6f7071","parsed":"[\"abc\",\"defg\",\"hijklmnopq\"]"} 
[info] - Serialize Tuple1 with CLValue
[info]   + CLValue.Tuple1(CLValue.String("abcef")) serializes to {"cl_type":{"Tuple1":["String"]},"bytes":"050000006162636566","parsed":"[\"abcef\"]"} 
[info] - Serialize Tuple2 with CLValues
[info]   + CLValue.Tuple2(CLValue.String("abc"), CLValue.U512(2)) serializes to {"cl_type":{"Tuple2":["String","U512"]},"bytes":"030000006162630102","parsed":"[\"abc\",\"2\"]"} 
[info] - Serialize Tuple3 with CLValues
[info]   + CLValue.Tuple3(CLValue.PublicKey("01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa9") ,
[info] 
[info]     CLValue.Option(CLValue.String("abc")), CLValue.U512(2)) serializes to {"cl_type":{"Tuple3":["PublicKey",{"Option":"String"},"U512"]},"bytes":"01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa901030000006162630102","parsed":"[\"01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa9\",\"abc\",\"2\"]"} 
[info] - Serialize Result with OK CLValue
[info]   + CLValue.Ok(CLValue.String("goodresult"),new CLTypeInfo (CLType.String)) serializes to {"cl_type":{"Result":{"ok":"String","err":"String"}},"bytes":"010a000000676f6f64726573756c74","parsed":"goodresult"} 
[info] - Serialize Result with Err CLValue
[info]   + CLValue.Err(CLValue.String("uh, something went wrong!!"),new CLTypeInfo (CLType.String)) serializes to {"cl_type":{"Result":{"ok":"String","err":"String"}},"bytes":"001a00000075682c20736f6d657468696e672077656e742077726f6e672121","parsed":"uh, something went wrong!!"} 
[info] - Serialize a List with Option String CLValue
[info]   + CLValue.List(CLValue.Option(CLValue.String("value1")),CLValue.Option(CLValue.String("value2")),
[info]       CLValue.OptionNone(new CLTypeInfo(CLType.String)),
[info]       CLValue.Option(CLValue.String("value4"))) serializes to {"cl_type":{"List":{"Option":"String"}},"bytes":"04000000010600000076616c756531010600000076616c75653200010600000076616c756534","parsed":"[\"value1\",\"value2\",\"null\",\"value4\"]"} 
[info] AccountHashDeserializerTest:
[info] - Deserialize AccountHash
[info]   + AccountHash is not null 
[info]   + account.bytes  is the same as new AccountHash("account-hash-85148dcd6c54b77e462a9acf387fb05aca953a83011db2c601716de0af1cf47c").bytes 
[info] DeployNamedArgSerializerTest:
[info] - DeployNamedArgSerializerTest with a single DeployNamedArg 
[info] - DeployNamedArgSerializerTest with a list of DeployNamedArg
[info] CLPublicKeyTest:
[info] - Test CLPublicKey from byets contructor
[info] - Test CLPublicKey KeyAlgorithm = ED25519
[info] - Test  ED25519 CLPublicKey  decode 
[info] - Test ED25519 CLPublicKey formatAsHexAccount   
[info] - Test CLPublicKey KeyAlgorithm = SECP256K1
[info] - Test SECP256K1 CLPublicKey  decode 
[info] - Test SECP256K1 CLPublicKey formatAsHexAccount   
[info] - Test ED25519 CLPublicKey toPem String   
[info] - Test SECP256K1 CLPublicKey toPem String   
[info] - Test ED25519 CLPublicKey loadFromPem    
[info] - Test SECP256K1 CLPublicKey loadFromPem    
[info] - Test  CLPublicKey loadFromPem from a non valid file  gives None
[info] - Test new CLPublicKey with a non valid hex string   gives None
[info] HexUtilsTest:
[info] - HexUtils  toHex Test 
[info] - HexUtils  fromHex Test 
[info] - HexUtils  fromHex Test with illegal hex litteral give None
[info] URefDeserializerTest:
[info] - Deserialize URef
[info]   + URef is not null 
[info]   + uref.bytes  is the same as new Uref("uref-9cC68775d07c211e44068D5dCc2cC28A67Cb582C3e239E83Bb0c3d067C4D0363-007").bytes 
[info] KeyPairTest:
[info] - Test Load keyPair from ed25519 private pem file
[info]   + assert publickey is not null 
[info]   + assert private key is not null 
[info]   + assert privateKey is of Ed25519PrivateKeyParameters   
[info]   + assert CLPublickey key is not null 
[info]   + assert Algorithm is  ED25519 
[info]   + assert  cLPublicKey hex = 0127a89db4e0806e568a5b0646594bd5d0abe0cf695a63357bd066f412e92bd68e 
[info] - Test Load keyPair from secp256k1 private pem file
[info]   + assert publickey is not null 
[info]   + assert private key is not null 
[info]   + assert privateKey is of ECPrivateKeyParameters   
[info]   + assert CLPublickey key is not null 
[info]   + assert Algorithm is  SECP256K1 
[info]   + assert SECP256K1 key length is  33 
[info]   + assert  cLPublicKey hex = 0127a89db4e0806e568a5b0646594bd5d0abe0cf695a63357bd066f412e92bd68e 
[info] - Test Load keyPair from non private pem file
[info]   + Load keyPair from non private pem give None Keypair Option 
[info] - Test create ed25519 keyPair 
[info]   + assert publickey is not null 
[info]   + assert private key is not null 
[info]   + assert privateKey is of Ed25519PrivateKeyParameters   
[info]   + assert CLPublickey key is not null 
[info] - Test create secp256k1 keyPair 
[info]   + assert publickey is not null 
[info]   + assert private key is not null 
[info]   + assert privateKey is of ECPrivateKeyParameters   
[info]   + assert CLPublickey key is not null 
[info] - Test publicKeyToPem from a  ed25519 keyPair 
[info] - Test privateKeyToPem from a ed25519 keyPair 
[info] - Test publicKeyToPem from a secp256k1 keyPair 
[info] - Test privateKeyToPem from a secp256k1 keyPair 
[info] - Test sign message with ED25519 keyPair 
[info]   + assert ED25519 signature length is 64   
[info]   + assert verifySignature  ED25519 publickey= true   
[info] - Test verifiy signature with ed25519 keyPair gives false 
[info]   + assert verifySignature on a différent message with ed25519 publickey = false   
[info] - Test verifiy signature with SECP256K1 keyPair gives false 
[info]   + assert verifySignature on a différent message with SECP256K1 publickey = false   
[info] SignatureDeserializerTest:
[info] - Deserialize Signature
[info]   + Signature is not null 
[info]   + signature.bytes  is the same as new Signature("012dbf03817a51794a8e19e0724884075e6d1fbec326b766ecfa6658b41f81290da85e23b24e88b1c8d9761185c961daee1adab0649912a6477bcd2e69bd91bd08").bytes 
[info] AccountHashTest:
[info] - Test AccountHash  decode 
[info] - Test AccountHash formatAsHexAccount   
[info] - Test new AccountHash with a non valid hex string  , throws IllegalArgumentException
[info] TimeUtilTest:
[info] - Test ToEpochMs 
[info]   + TimeUtil.ToEpochMs("2020-11-17T00:39:24.072Z") == 1605573564072L 
[info] - Test ToEpochMs with a wrong timestamp, throws NoSuchElementException 
[info]   + TimeUtil.ToEpochMs("202011-17T00:39:24.072Z") throws NoSuchElementException 
[info] - Test timeStampString from millis
[info]   + TimeUtil.timeStampString(1605573564072L)=="2020-11-17T00:39:24.072Z" 
[info] - Test ttlToMillis 
[info]   + TimeUtil.ttlToMillis ("30m") ==1800000L 
[info]   + TimeUtil.ttlToMillis ("30m") ==1800000L 
[info] - Test ttlToMillis with a non supported TTL gives None String Option 
[info]   + TimeUtil.ttlToMillis ("3041mn") gives None String Option 
[info] - Test MillisToTtl
[info]   + TimeUtil.MillisToTtl (1800000L)=="30m" 
[info]   + TimeUtil.MillisToTtl (5400000L)=="1h 30m" 
[info] - Test MillisToTtl with negative millis ,  gives None String Option
[info]   + TimeUtil.MillisToTtl (-5L) gives None String Option  
[info] CLPublicKeySerializerTest:
[info] - Serialize CLPublicKey
[info]   + new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e") json serialization =  "017d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e" 
[info] HashSerializerTest:
[info] - Serialize CLPublicKey
[info]   + new Hash(new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e")) json serialization =  "7d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e" 
[info] CLPublicKeyByteSerializerTest:
[info] - Test serialize CLPublicKey 
[info] CLPublicKeyDeserializerTest:
[info] - Deserialize CLPublicKey
[info]   + PublicKey is not null 
[info]   + pubKey.bytes  is the same as new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e").bytes 
[info] URefTest:
[info] - Test Uref AccessRight
[info] - Test Uref decode 
[info] - Test format Uref  
[info] - Test new Uref with a non valid hex string 
[info] - Test new Uref with a non uref string 
[info] CasperSdkTest:
[info] RPC Call to a non existing node (http://1.2.3.4:7777/rpc)
[info] - should fail
[info] getPeers
[info] - should succeed
[info]   + Peers List size : 2194 
[info] getStateRootHash with empty parameter
[info] - should succeed
[info]   + state root hash : Success(StateRootHashResult(1.4.8,5b18d4f888ce1afa10d645f8758b8182c568b9bc85de8d65a53e0a247e7c58cd)) 
[info] Get state root hash with a blockHash parameter
[info] - should succeed
[info]   + state root hash : Success(StateRootHashResult(1.4.8,5b18d4f888ce1afa10d645f8758b8182c568b9bc85de8d65a53e0a247e7c58cd)) 
[info] Get Block using Block hash parameter
[info] - should succeed
[info]   + block  hash : 74dce8911a3edf0f872dc11f0a63ca9fe1b55b7188a9feaaf431518bf9c508b4 
[info] GetBlock using Block hash parameter
[info] - should retrieve the latest known block hash
[info]   + block  hash : ee1101feefbd1bfd0f43503dccd9e074d73b4331feed4cce4916a09cd51772a5 
[info] GetBlock using non existing Block hash parameter
[info] - should succeed and retrieves the latest known block hash
[info]   + block  hash : ee1101feefbd1bfd0f43503dccd9e074d73b4331feed4cce4916a09cd51772a5 
[info] GetBlock  using Block height parameter
[info] - should succeed
[info]   + block  hash : 2aca74cf33f6ace634ed82ac88e597d55920ff1de8e596dd77d9558736ef570d 
[info] GetBlock using non existing height parameter
[info] - should fail
[info] GetDeploy using a Deploy hash parameter
[info] - should succeed
[info]   + deploy  header is not null 
[info]   + This deploy  has a ModuleBytes payment  
[info]   + This deploy  has a StoredContractByHash as session 
[info] GetDeploy using an empty parameter
[info] - should fail
[info] GetStatus
[info] - should succeed
[info]   + assert node pub key is : 017d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e 
[info]   + assert network is : casper-test  
[info] getBlockTransfers
[info] - should succeed
[info]   + assert this block contains two transfers 
[info]   + assert first transfer deploy hash is = 277AEF49321B3b19B0EDd732Cd5CFf4F2E76c1Df0260356367711aD81f4bC8FC 
[info]   + assert amount of first transfer is = 1000000000000 motes 
[info] GetAuctionInfo with a block hash identifier
[info] - should succeed and retrieves an auction state at era 2974
[info]   + assert  state_root_hash = aef184ba371bf4efefbbfeb9334cc9d721f5c6fe2aa3e32c87ef4fa0ab864ad9 
[info]   + assert  era = 2974 
[info] GetAuctionInfo with a block height identifier
[info] - should succeed and retrieves an auction state at era 2974
[info]   + assert  state_root_hash = aef184ba371bf4efefbbfeb9334cc9d721f5c6fe2aa3e32c87ef4fa0ab864ad9 
[info]   + assert  era = 2974 
[info] GetAuctionInfo with empty block hash
[info] - should succeed and retrieves current auction state
[info]   + assert  state_root_hash = current state root hash 
[info] GetEraInfoBySwitchBlock : 2974-->2975 with blockHash: 1e46B4c173dB70fDE0E867FF679ACa24e1c5Bea3C4333af94e53B4E3BC548B6B
[info] - should succeed
[info]   + assert  era = 2974 
[info]   + assert  state root hash  = c1A62d5DeB74d3fEAfeCd1EEa526941edd0264895EB8E516474108D4EA4D7D21 
[info] GetEraInfoBySwitchBlock with a non switch block : a2C85FD13bba200E47c2d7c74E87F0f0c96aDcEE227877168a639Fa67d046933
[info] - should retrieve a null result
[info]   + assert  era_summary = null 
[info] GetEraInfoBySwitchBlock with an empty switch bloc
[info] - should retrieve a null result
[info]   + assert  era_summary = null 
[info] queryGlobalState with stateRoothash=30cE5146268305AeeFdCC05a5f7bE7aa6dAF187937Eed9BB55Af90e1D49B7956h,key= hash-4dd10a0b2a7672e8ec964144634ddabb91504fe50b8461bac23584423318887d
[info] - should succeed and retieves a Contract
[info]   + assert block Header is null  
[info]   + assert contract is not null  
[info]   + assert contract_package_hash = contract-wasm-8D1c5ab95baaa77c302232a00FE1C6cF6975ffD6430a9ECd87EC5266280BB18D 
[info]   + assert first enry point is an allowance  
[info]   + assert first arg of the first entry point is of type CLType = Key   
[info] queryGlobalState with stateRoothash=30cE5146268305AeeFdCC05a5f7bE7aa6dAF187937Eed9BB55Af90e1D49B7956h,key=account-hash-46dE97966cfc2F00C326e654baD000AB7a5E26bEBc316EF4D74715335cF32A88
[info] - should succeed and retieves an Account
[info]   + assert contract is  null  
[info]   + assert account is not null  
[info]   + assert main_purse : uref-9cC68775d07c211e44068D5dCc2cC28A67Cb582C3e239E83Bb0c3d067C4D0363-007 
[info] getStateItem   retrieving CLValue
[info] - should succeed
[info] queryGlobalState with wrong parameters
[info] - should fail
[info] GetBalance with an existing account
[info] - should succeed
[info]   + Assert balance = 869077209920 motes  
[info] GetBalance with  non hex key account
[info] - should fail
[info] GetBalance with non uref key account
[info] - should fail
[info] getAccountInfo with Block Hash  identifier
[info] - should succed
[info] GetDictionaryItem with itemKey=a8261377ef9cf8e741dd6858801c71e38c9322e66355586549b75ab24bdd73f2
[info] - should succeed
[info]   + CLValue is not nul   
[info]   + cl_Type is String    
[info]   + CLValue parsed =  "https://caspercommunity.io"  
[info] PutDeploy with aStandard Transfer
[info] - should succeed
[info] Run completed in 17 seconds, 419 milliseconds.
[info] Total number of tests run: 198
[info] Suites: completed 32, aborted 0
[info] Tests: succeeded 198, failed 0, canceled 0, ignored 0, pending 0
[info] All tests passed.
[success] Total time: 93 s (01:33), completed Oct 21, 2022 7:53:04 AM

```
