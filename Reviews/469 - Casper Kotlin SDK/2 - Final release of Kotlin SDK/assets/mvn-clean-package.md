```
muharremsalel@Muharrems-MacBook-Pro Casper-Kotlin-sdk % mvn clean package
[INFO] Scanning for projects...
[INFO] 
[INFO] ----------------< casper.kotlin.sdk:casper-kotlin-sdk >-----------------
[INFO] Building CasperKotlinSDK 1.0
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-clean-plugin:2.5:clean (default-clean) @ casper-kotlin-sdk ---
[INFO] Deleting /Users/muharremsalel/Desktop/Casper-Kotlin-sdk/target
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
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.656 s - in com.casper.sdk.crypto.Ed25519HandleTest
[INFO] Running com.casper.sdk.crypto.Secp256k1HandleTest
Error write private key to a non-exist file
Error write public key to a non-exist file
Error load private key from a wrong file format
Error load private key from a wrong file format
Error load wrong private key from a wrong path
Error load public key from a wrong file format
Error load public key from a wrong file format
Error load wrong public key from a wrong path
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.121 s - in com.casper.sdk.crypto.Secp256k1HandleTest
[INFO] Running com.casper.sdk.getblock.GetBlockRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.829 s - in com.casper.sdk.getblock.GetBlockRPCTest
[INFO] Running com.casper.sdk.getpeers.GetPeersTest
First peer entry nodeId: tls:000b..65c7 and address: 136.243.187.84:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.462 s - in com.casper.sdk.getpeers.GetPeersTest
[INFO] Running com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.775 s - in com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
[INFO] Running com.casper.sdk.serialization.CLTypeSerializationTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.001 s - in com.casper.sdk.serialization.CLTypeSerializationTest
[INFO] Running com.casper.sdk.serialization.DeploySerializeHelperTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.02 s - in com.casper.sdk.serialization.DeploySerializeHelperTest
[INFO] Running com.casper.sdk.serialization.CLParseSerializationTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.006 s - in com.casper.sdk.serialization.CLParseSerializationTest
[INFO] Running com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.209 s - in com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Running com.casper.sdk.getstateroothash.GetStateRootHashTest
Error Get State Root Hash,  invalid parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.772 s - in com.casper.sdk.getstateroothash.GetStateRootHashTest
[INFO] Running com.casper.sdk.getauction.GetAuctionInfoRPCTest
Error get auction information with wrong block height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 41.809 s - in com.casper.sdk.getauction.GetAuctionInfoRPCTest
[INFO] Running com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
Error with wrong state root hash
Error wrong DictionayIdentifier parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.357 s - in com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
[INFO] Running com.casper.sdk.getstatus.GetStatusRPCTest
First peer entry node_id:  tls:000b..65c7 and address: 136.243.187.84:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.364 s - in com.casper.sdk.getstatus.GetStatusRPCTest
[INFO] Running com.casper.sdk.getitem.GetItemRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.422 s - in com.casper.sdk.getitem.GetItemRPCTest
[INFO] Running com.casper.sdk.getbalance.GetBalanceRPCTest
Error get balance with wrong state root hash
Error get balance with wrong purse uref
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.456 s - in com.casper.sdk.getbalance.GetBalanceRPCTest
[INFO] Running com.casper.sdk.putdeploy.PutDeployRPCTest
Put deploy successfull with deploy hash Ed25519:3043b7ae05a70c09790dce5134609790c45f13cd9d7f9cba114aec7ee8add166
Put deploy successfull with deploy hash Secp256k1:ef4b5aef043177bfb3d02ddfacc104c2ed0570b2c41df9658ff0bc316568a4bc
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.61 s - in com.casper.sdk.putdeploy.PutDeployRPCTest
[INFO] Running com.casper.sdk.getdeploy.GetDeployRPCTest
Negative test, Error IllegalArgumentException caught
Negative test, Error IllegalArgumentException caught
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 12.221 s - in com.casper.sdk.getdeploy.GetDeployRPCTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 17, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ casper-kotlin-sdk ---
[INFO] Building jar: /Users/muharremsalel/Desktop/Casper-Kotlin-sdk/target/casper-kotlin-sdk-1.0.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:25 min
[INFO] Finished at: 2022-07-21T15:39:40+03:00
[INFO] ------------------------------------------------------------------------
```