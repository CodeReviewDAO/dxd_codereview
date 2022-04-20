```
$ sbt test
[info] welcome to sbt 1.6.2 (Ubuntu Java 11.0.14)
[info] loading project definition from /home/kara/casper-scala-sdk/project
[info] loading settings for project casper-scala-sdk from build.sbt ...
[info] set current project to casper-scala-sdk (in build file:/home/kara/casper-scala-sdk/)
[info] compiling 55 Scala sources to /home/kara/casper-scala-sdk/target/scala-3.0.2/classes ...
[info] compiling 34 Scala sources to /home/kara/casper-scala-sdk/target/scala-3.0.2/classes ...
[info] compiling 38 Scala sources to /home/kara/casper-scala-sdk/target/scala-3.0.2/test-classes ...
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
[info] - Test  CLPublicKey loadFromPem from a non valid file , throws IllegalArgumentException
[info] - Test new CLPublicKey with a non valid hex string  , throws NoSuchElementException
[info] HexUtilsTest:
[info] - HexUtils  toHex Test 
[info] - HexUtils  fromHex Test 
[info] - gHexUtils  fromHex Test with illegal hex litteral, throws IllegalArgumentException
[info] DeployApprovalByteSerializerTest:
[info] - Test DeployApprovalByteSerializer with a signle DeployApproval  
[info] SignatureDeserializerTest:
[info] - Deserialize CLPublicKey
[info]   + Signature is not null 
[info]   + signature.bytes  is the same as new Signature("012dbf03817a51794a8e19e0724884075e6d1fbec326b766ecfa6658b41f81290da85e23b24e88b1c8d9761185c961daee1adab0649912a6477bcd2e69bd91bd08").bytes 
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
[info] - Test serialize Empty List of CLType throws IllegalArgumentException 
[info] - Test CLValueBteSerializer with empty List CLType 
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
[info] URefDeserializerTest:
[info] - Deserialize URef
[info]   + URef is not null 
[info]   + uref.bytes  is the same as new Uref("uref-9cC68775d07c211e44068D5dCc2cC28A67Cb582C3e239E83Bb0c3d067C4D0363-007").bytes 
[info] HashSerializerTest:
[info] - Serialize CLPublicKey
[info]   + new Hash(new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e")) json serialization =  "7d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e" 
[info] DeployExecutableByteSerializerTest:
[info] - Test serialize ModuleBytes 
[info] - Test serialize storedContractByName 
[info] - Test serialize storedContractByHash 
[info] - Test serialize storedVersionedContractByHash 
[info] - Test serialize StoredVersionedContractByName 
[info] - Test serialize DeployTransfer 
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
[info]   + Load keyPair from non private pem file Throws IllegalArgumentException 
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
[info] - Test sign message with SECP256K1 keyPair 
[info]   + assert verifySignature with SECP256K1 publickey = true   
[info] - Test verifiy signature with ed25519 keyPair gives false 
[info]   + assert verifySignature on a différent message with ed25519 publickey = false   
[info] - Test verifiy signature with SECP256K1 keyPair gives false 
[info]   + assert verifySignature on a différent message with SECP256K1 publickey = false   
[info] CLValueSerializerTest:
[info] - Serialize Option value
[info]   + CLValue.Option(CLValue.String("Hello, World!")) serializes to {
[info]   "cl_type" : {
[info]     "Option" : "String"
[info]   },
[info]   "bytes" : "010d00000048656c6c6f2c20576f726c6421",
[info]   "parsed" : "Hello, World!"
[info] } 
[info] - Serialize Bool value
[info]   + CLValue.Bool(true) serializes to {
[info]   "cl_type" : "Bool",
[info]   "bytes" : "01",
[info]   "parsed" : "true"
[info] } 
[info] - Serialize String value
[info]   + CLValue.String("Hello, world!") serializes to {
[info]   "cl_type" : "String",
[info]   "bytes" : "0d00000048656c6c6f2c20776f726c6421",
[info]   "parsed" : "Hello, world!"
[info] } 
[info] - Serialize U8 value
[info]   + CLValue.U8(7) serializes to {
[info]   "cl_type" : "U8",
[info]   "bytes" : "00000000000000",
[info]   "parsed" : "7"
[info] } 
[info] - Serialize U512 value
[info]   + CLValue.U512(458745874) serializes to {
[info]   "cl_type" : "U512",
[info]   "bytes" : "0412e8571b",
[info]   "parsed" : "458745874"
[info] } 
[info] - Serialize U32 value
[info]   + CLValue.U32(45874) serializes to {
[info]   "cl_type" : "U32",
[info]   "bytes" : "32b30000",
[info]   "parsed" : "45874"
[info] } 
[info] - Serialize I32 value
[info]   + CLValue.I32(10000) serializes to {
[info]   "cl_type" : "I32",
[info]   "bytes" : "10270000",
[info]   "parsed" : "10000"
[info] } 
[info] - Serialize I64 value
[info]   + CLValue.I64(-541287) serializes to {
[info]   "cl_type" : "I64",
[info]   "bytes" : "99bdf7ffffffffff",
[info]   "parsed" : "-541287"
[info] } 
[info] - Serialize U128 value
[info]   + CLValue.U128(458745874) serializes to {
[info]   "cl_type" : "U128",
[info]   "bytes" : "04bf3d3209",
[info]   "parsed" : "154287551"
[info] } 
[info] - Serialize U256 value
[info]   + CLValue.U256(BigInt.apply("4545487556545454545454")) serializes to {
[info]   "cl_type" : "U256",
[info]   "bytes" : "0a2e1a2022a7d14f69f600",
[info]   "parsed" : "4545487556545454545454"
[info] } 
[info] - Serialize List of CLvalues
[info]   + CLValue.List(CLValue.String("abc"),CLValue.String("defg") , CLValue.String("hijklmnopq")) serializes to {
[info]   "cl_type" : {
[info]     "List" : "String"
[info]   },
[info]   "bytes" : "030000000300000061626304000000646566670a00000068696a6b6c6d6e6f7071",
[info]   "parsed" : "[\"abc\",\"defg\",\"hijklmnopq\"]"
[info] } 
[info] - Serialize Tuple1 with CLValue
[info]   + CLValue.Tuple1(CLValue.String("abcef")) serializes to {
[info]   "cl_type" : {
[info]     "Tuple1" : [
[info]       "String"
[info]     ]
[info]   },
[info]   "bytes" : "050000006162636566",
[info]   "parsed" : "[\"abcef\"]"
[info] } 
[info] - Serialize Tuple2 with CLValues
[info]   + CLValue.Tuple2(CLValue.String("abc"), CLValue.U512(2)) serializes to {
[info]   "cl_type" : {
[info]     "Tuple2" : [
[info]       "String",
[info]       "U512"
[info]     ]
[info]   },
[info]   "bytes" : "030000006162630102",
[info]   "parsed" : "[\"abc\",\"2\"]"
[info] } 
[info] - Serialize Tuple3 with CLValues
[info]   + CLValue.Tuple3(CLValue.PublicKey("01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa9") ,
[info] 
[info]     CLValue.Option(CLValue.String("abc")), CLValue.U512(2)) serializes to {
[info]   "cl_type" : {
[info]     "Tuple3" : [
[info]       "PublicKey",
[info]       {
[info]         "Option" : "String"
[info]       },
[info]       "U512"
[info]     ]
[info]   },
[info]   "bytes" : "01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa901030000006162630102",
[info]   "parsed" : "[\"01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa9\",\"abc\",\"2\"]"
[info] } 
[info] - Serialize Result with OK CLValue
[info]   + CLValue.Ok(CLValue.String("goodresult"),new CLTypeInfo (CLType.String)) serializes to {
[info]   "cl_type" : {
[info]     "Result" : {
[info]       "ok" : "String",
[info]       "err" : "String"
[info]     }
[info]   },
[info]   "bytes" : "010a000000676f6f64726573756c74",
[info]   "parsed" : "goodresult"
[info] } 
[info] - Serialize Result with Err CLValue
[info]   + CLValue.Err(CLValue.String("uh, something wnet wrong!!"),new CLTypeInfo (CLType.String)) serializes to {
[info]   "cl_type" : {
[info]     "Result" : {
[info]       "ok" : "String",
[info]       "err" : "String"
[info]     }
[info]   },
[info]   "bytes" : "001a00000075682c20736f6d657468696e6720776e65742077726f6e672121",
[info]   "parsed" : "uh, something wnet wrong!!"
[info] } 
[info] - Serialize Key CLValue
[info]   +  CLValue.Key("transfer-e330a31701205e3871cb4f7e14d3ff26074735c84b0e54b7a75f553a8405d182") serializes to {
[info]   "cl_type" : "Key",
[info]   "bytes" : "03e330a31701205e3871cb4f7e14d3ff26074735c84b0e54b7a75f553a8405d182",
[info]   "parsed" : "{\"Transfer\":\"transfer-e330a31701205e3871cb4f7e14d3ff26074735c84b0e54b7a75f553a8405d182\"}"
[info] } 
[info] - Serialize a List with Option String CLValue
[info]   + CLValue.List(CLValue.Option(CLValue.String("value1")),CLValue.Option(CLValue.String("value2")),
[info]       CLValue.OptionNone(new CLTypeInfo(CLType.String)),
[info]       CLValue.Option(CLValue.String("value4"))) serializes to {
[info]   "cl_type" : {
[info]     "List" : {
[info]       "Option" : "String"
[info]     }
[info]   },
[info]   "bytes" : "04000000010600000076616c756531010600000076616c75653200010600000076616c756534",
[info]   "parsed" : "[\"value1\",\"value2\",\"null\",\"value4\"]"
[info] } 
[info] KeyAlgorithmTest:
[info] JsonConverterTest:
[info] AccountHashDeserializerTest:
[info] - Deserialize AccountHash
[info]   + AccountHash is not null 
[info]   + account.bytes  is the same as new AccountHash("account-hash-85148dcd6c54b77e462a9acf387fb05aca953a83011db2c601716de0af1cf47c").bytes 
[info] DeployNamedArgByteSerializerTest:
[info] - Test serialize DeployNamedArg  with String CLValue
[info] - Test serialize DeployNamedArg  with U512 CLValue
[info] - Test serialize DeployNamedArg  with Bytearray CLValue
[info] - Test serialize DeployNamedArg  with CLPublicKey CLValue
[info] - Test serialize DeployNamedArg  with URef CLValue
[info] ByteUtilTest:
[info] - ByteUtils join Test 
[info] RPCResultDeserializerTest:
[info] - RPCResultDeserializer test with getPeers
[info] - RPCResultDeserializer test with getStateRootHash
[info] - RPCResultDeserializer test with getBlock
[info] - RPCResultDeserializer test with getBlockByHeight
[info] - RPCResultDeserializer test with getStatus
[info] - RPCResultDeserializer test with getBlockTransfers
[info] - RPCResultDeserializer test with getAuctionInfo
[info] - RPCResultDeserializer test with getDeploy
[info] - RPCResultDeserializer test with getEraInfoBySwitchBlock
[info] - RPCResultDeserializer test with getStateItem
[info] - RPCResultDeserializer test with getBalance
[info] - RPCResultDeserializer test with getDictionaryItem
[info] CLTypeDeserialiserTest:
[info] - Deserialize  U512 CLType
[info] - Deserialize  ByteArray CLType
[info] - Deserialize  Option CLType
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
[info] - Test ttlToMillis with a non supported TTL , Thorws IllegalArgumentException 
[info]   + TimeUtil.ttlToMillis ("3041mn") throws IllegalArgumentException 
[info] - Test MillisToTtl
[info]   + TimeUtil.MillisToTtl (1800000L)=="30m" 
[info]   + TimeUtil.MillisToTtl (5400000L)=="1h 30m" 
[info] - Test MillisToTtl with negative millis ,  Thorws IllegalArgumentException
[info]   + TimeUtil.MillisToTtl (-5L) throws IllegalArgumentException 
[info] DeployByteSerializerTest:
[info] - Test DeployByteSerializer with json deploy  
[info] TimeStampSerializerTest:
[info] DeployNamedArgSerializerTest:
[info] - DeployNamedArgSerializerTest with a single DeployNamedArg 
[info] - DeployNamedArgSerializerTest with a list of DeployNamedArg
[info] CLPublicKeySerializerTest:
[info] - Serialize CLPublicKey
[info]   + new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e") json serialization =  "017d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e" 
[info] SignatureTest:
[info] - Test Signature KeyAlgorithm = ED25519
[info] - Test Signature  decode 
[info] - Test Signature formatAsHexAccount   
[info] - Test new Signature with a non valid hex string  , throws IllegalArgumentException
[info] CLPublicKeySerializerTest:
[info] - Test serialize CLPublicKey 
[info] AccountHashTest:
[info] - Test AccountHash  decode 
[info] - Test AccountHash formatAsHexAccount   
[info] - Test new AccountHash with a non valid hex string  , throws IllegalArgumentException
[info] DeployExecutableDeserializerTest:
[info] - DeployExecutableDeserializer test ModuleBytes 
[info] - DeployExecutableDeserializer test StoredContractByHash 
[info] - DeployExecutableDeserializer test StoredContractByName 
[info] - DeployExecutableDeserializer test StoredVersionedContractByHash 
[info] - DeployExecutableDeserializer test StoredVersionedContractByName 
[info] - DeployExecutableDeserializer test Transfer 
[info] DeployHeaderByteSerializerTest:
[info] - Test serialize DeployHeader 
[info] CLPublicKeyDeserializerTest:
[info] - Deserialize CLPublicKey
[info]   + PublicKey is not null 
[info]   + pubKey.bytes  is the same as new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e").bytes 
[info] CLTypeInfoSerializerTest:
[info] - Serialize CLTypeInfo with U64
[info]   + new  CLTypeInfo(CLType.U64) json serialization =  "U64" 
[info] - Serialize CLTypeInfo with String
[info]   + new  CLTypeInfo(CLType.String) json serialization =  "String" 
[info] - Serialize CLTypeInfo with ByteArray
[info]   + new  new CLByteArrayTypeInfo(124) json serialization =  {
[info]   "ByteArray" : 124
[info] } 
[info] - Serialize CLTypeInfo with Option
[info]   + new  new CLOptionTypeInfo(new CLTypeInfo(CLType.I64)) json serialization =  {
[info]   "Option" : "I64"
[info] } 
[info] TTLSerializerTest:
[info] - Serialize CLPublicKey
[info]   + new Hash( CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e")) json serialization =  "7d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e" 
[info] URefTest:
[info] - Test Uref AccessRight
[info] - Test Uref decode 
[info] - Test format Uref  
[info] - Test new Uref with a non valid hex string  , throws IllegalArgumentException
[info] DeployExecutableSerializerTest:
[info] - DeployExecutableSerializerTest with StoredVersionedContractByName
[info] - DeployExecutableSerializerTest with StoredVersionedContractByHash
[info] - DeployExecutableSerializerTest with StoredContractByHash
[info] - DeployExecutableSerializerTest with StoredContractByName
[info] - DeployExecutableSerializerTest with DeployTransfer
[info] CasperSdkTest:
[info] - RPC Call to a non existing node (http://1.2.3.4:7777/rpc) Throws an RPCIOException
[info] - Testnet Network Peers list is not empty
[info]   + Peers List size : 498 
[info] - Get state root hash with no blockHash parameter, state root hash is not empty and is 64 characters long
[info]   + state root hash : b2e0b35a13e862c529dffd7aa5650cacea679911c7cf0ea19d56a595390c6049 
[info] - Get state root hash with a blockHash parameter ,state root hash is not empty and is 64 character  long
[info]   + state root hash : b2e0b35a13e862c529dffd7aa5650cacea679911c7cf0ea19d56a595390c6049 
[info] - Get Block using Block hash parameter
[info]   + block  hash : 74dce8911a3edf0f872dc11f0a63ca9fe1b55b7188a9feaaf431518bf9c508b4 
[info] - Get Block using an empty Block hash parameter, retrieves the latest known block hash
[info]   + block  hash : 1647e83f331b511dd199c6494703eb814df29449164373aacdd94119931faa13 
[info] - Get Block using non existing Block hash parameter, retrieves the latest known block hash
[info]   + block  hash : 1647e83f331b511dd199c6494703eb814df29449164373aacdd94119931faa13 
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
[info] - PutDeploy  : Standard Transfer 
[info] Run completed in 17 seconds, 274 milliseconds.
[info] Total number of tests run: 212
[info] Suites: completed 34, aborted 0
[info] Tests: succeeded 212, failed 0, canceled 0, ignored 0, pending 0
[info] All tests passed.
[success] Total time: 54 s, completed Mar 14, 2022, 2:02:27 AM
```

