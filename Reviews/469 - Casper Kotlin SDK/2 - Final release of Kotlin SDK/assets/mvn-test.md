```
muharremsalel@Muharrems-MacBook-Pro Casper-Kotlin-sdk % mvn test
[INFO] Scanning for projects...
[INFO] 
[INFO] ----------------< casper.kotlin.sdk:casper-kotlin-sdk >-----------------
[INFO] Building CasperKotlinSDK 1.0
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ casper-kotlin-sdk ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/muharremsalel/Desktop/Casper-Kotlin-sdk/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ casper-kotlin-sdk ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- kotlin-maven-plugin:1.6.10:compile (compile) @ casper-kotlin-sdk ---
[WARNING] /Users/muharremsalel/Desktop/Casper-Kotlin-sdk/src/main/kotlin/com/casper/sdk/serialization/CLParseSerialization.kt: (101, 38) Parameter 'clParse' is never used
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ casper-kotlin-sdk ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/muharremsalel/Desktop/Casper-Kotlin-sdk/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ casper-kotlin-sdk ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- kotlin-maven-plugin:1.6.10:test-compile (test-compile) @ casper-kotlin-sdk ---
[WARNING] /Users/muharremsalel/Desktop/Casper-Kotlin-sdk/src/test/kotlin/com/casper/sdk/crypto/Secp256k1HandleTest.kt: (40, 13) Variable 'CURVE' is never used
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ casper-kotlin-sdk ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.casper.sdk.crypto.Ed25519HandleTest
Error write private key to a non-exist file
Error write public key to a non-exist file
Error load private key from a wrong file format
Error load private key from a wrong file format
Error load wrong private key from a wrong path
Error load public key from a wrong file format
Error load public key from a wrong file format
Error load wrong public key from a wrong path
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.776 s - in com.casper.sdk.crypto.Ed25519HandleTest
[INFO] Running com.casper.sdk.crypto.Secp256k1HandleTest
Error write private key to a non-exist file
Error write public key to a non-exist file
Error load private key from a wrong file format
Error load private key from a wrong file format
Error load wrong private key from a wrong path
Error load public key from a wrong file format
Error load public key from a wrong file format
Error load wrong public key from a wrong path
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.139 s - in com.casper.sdk.crypto.Secp256k1HandleTest
[INFO] Running com.casper.sdk.getblock.GetBlockRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.052 s - in com.casper.sdk.getblock.GetBlockRPCTest
[INFO] Running com.casper.sdk.getpeers.GetPeersTest
First peer entry nodeId: tls:000b..65c7 and address: 136.243.187.84:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.342 s - in com.casper.sdk.getpeers.GetPeersTest
[INFO] Running com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.068 s - in com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
[INFO] Running com.casper.sdk.serialization.CLTypeSerializationTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.001 s - in com.casper.sdk.serialization.CLTypeSerializationTest
[INFO] Running com.casper.sdk.serialization.DeploySerializeHelperTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.023 s - in com.casper.sdk.serialization.DeploySerializeHelperTest
[INFO] Running com.casper.sdk.serialization.CLParseSerializationTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.007 s - in com.casper.sdk.serialization.CLParseSerializationTest
[INFO] Running com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.328 s - in com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Running com.casper.sdk.getstateroothash.GetStateRootHashTest
Error Get State Root Hash,  invalid parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.767 s - in com.casper.sdk.getstateroothash.GetStateRootHashTest
[INFO] Running com.casper.sdk.getauction.GetAuctionInfoRPCTest
Error get auction information with wrong block height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 44.115 s - in com.casper.sdk.getauction.GetAuctionInfoRPCTest
[INFO] Running com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
Error with wrong state root hash
Error wrong DictionayIdentifier parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.154 s - in com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
[INFO] Running com.casper.sdk.getstatus.GetStatusRPCTest
First peer entry node_id:  tls:000b..65c7 and address: 136.243.187.84:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.367 s - in com.casper.sdk.getstatus.GetStatusRPCTest
[INFO] Running com.casper.sdk.getitem.GetItemRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.569 s - in com.casper.sdk.getitem.GetItemRPCTest
[INFO] Running com.casper.sdk.getbalance.GetBalanceRPCTest
Error get balance with wrong state root hash
Error get balance with wrong purse uref
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.483 s - in com.casper.sdk.getbalance.GetBalanceRPCTest
[INFO] Running com.casper.sdk.putdeploy.PutDeployRPCTest
Put deploy successfull with deploy hash Ed25519:c268771803194a14ecd0a35df934705a30759d432cd319ef1095207bd9df6f12
Put deploy successfull with deploy hash Secp256k1:407b6a980fcab788048edea74335fde7d652b0875a6b2d16e8ba1db35dddf17a
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.755 s - in com.casper.sdk.putdeploy.PutDeployRPCTest
[INFO] Running com.casper.sdk.getdeploy.GetDeployRPCTest
Negative test, Error IllegalArgumentException caught
Negative test, Error IllegalArgumentException caught
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 13.213 s - in com.casper.sdk.getdeploy.GetDeployRPCTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 17, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:29 min
[INFO] Finished at: 2022-07-21T15:32:21+03:00
[INFO] ------------------------------------------------------------------------


```