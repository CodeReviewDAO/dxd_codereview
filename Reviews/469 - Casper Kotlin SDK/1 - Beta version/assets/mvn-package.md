```
yusuf@Yusuf-MacBook-Pro Casper-Kotlin-sdk % mvn package
[INFO] Scanning for projects...
[INFO] 
[INFO] -------------------------< me.hien:consoleApp >-------------------------
[INFO] Building consoleApp 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ consoleApp ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ consoleApp ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- kotlin-maven-plugin:1.5.10:compile (compile) @ consoleApp ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ consoleApp ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ consoleApp ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- kotlin-maven-plugin:1.5.10:test-compile (test-compile) @ consoleApp ---
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ consoleApp ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.casper.sdk.getblock.GetBlockRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 5.148 s - in com.casper.sdk.getblock.GetBlockRPCTest
[INFO] Running com.casper.sdk.getpeers.GetPeersTest
First peer entry nodeId: tls:0097..b253 and address: 18.163.249.168:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.509 s - in com.casper.sdk.getpeers.GetPeersTest
[INFO] Running com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.016 s - in com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
[INFO] Running com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.677 s - in com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Running com.casper.sdk.getstateroothash.GetStateRootHashTest
Error Get State Root Hash,  invalid parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.033 s - in com.casper.sdk.getstateroothash.GetStateRootHashTest
[INFO] Running com.casper.sdk.getauction.GetAuctionInfoRPCTest
Error get auction information with wrong block height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 24.233 s - in com.casper.sdk.getauction.GetAuctionInfoRPCTest
[INFO] Running com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
Error with wrong state root hash
Error wrong DictionayIdentifier parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 3.125 s - in com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
[INFO] Running com.casper.sdk.getstatus.GetStatusRPCTest
First peer entry node_id:  tls:0097..b253 and address: 18.163.249.168:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.552 s - in com.casper.sdk.getstatus.GetStatusRPCTest
[INFO] Running com.casper.sdk.getitem.GetItemRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 13.342 s - in com.casper.sdk.getitem.GetItemRPCTest
[INFO] Running com.casper.sdk.getbalance.GetBalanceRPCTest
Error get balance with wrong state root hash
Error get balance with wrong purse uref
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.374 s - in com.casper.sdk.getbalance.GetBalanceRPCTest
[INFO] Running com.casper.sdk.getdeploy.GetDeployRPCTest
Error IllegalArgumentException caught
Error IllegalArgumentException caught
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 4.907 s - in com.casper.sdk.getdeploy.GetDeployRPCTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 11, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ consoleApp ---
[INFO] Building jar: /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/target/consoleApp-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:53 min
[INFO] Finished at: 2022-05-04T16:18:20+03:00
[INFO] ------------------------------------------------------------------------
```
