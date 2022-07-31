```
muharremsalel@Muharrems-MacBook-Pro Desktop % git clone https://github.com/tqhuy2018/Casper-Kotlin-sdk.git
Cloning into 'Casper-Kotlin-sdk'...
remote: Enumerating objects: 3485, done.
remote: Counting objects: 100% (738/738), done.
remote: Compressing objects: 100% (328/328), done.
remote: Total 3485 (delta 296), reused 704 (delta 276), pack-reused 2747
Receiving objects: 100% (3485/3485), 577.36 KiB | 1.50 MiB/s, done.
Resolving deltas: 100% (1463/1463), done.
muharremsalel@Muharrems-MacBook-Pro Desktop % cd Casper-Kotlin-sdk 
muharremsalel@Muharrems-MacBook-Pro Casper-Kotlin-sdk % mvn -v
Apache Maven 3.8.6 (84538c9988a25aec085021c365c560670ad80f63)
Maven home: /Users/muharremsalel/Downloads/apache-maven-3.8.6
Java version: 18.0.2, vendor: Oracle Corporation, runtime: /Library/Java/JavaVirtualMachines/jdk-18.0.2.jdk/Contents/Home
Default locale: en_TR, platform encoding: UTF-8
OS name: "mac os x", version: "12.0.1", arch: "x86_64", family: "mac"
muharremsalel@Muharrems-MacBook-Pro Casper-Kotlin-sdk % mvn package
[INFO] Scanning for projects...
[INFO] 
[INFO] ----------------< casper.kotlin.sdk:casper-kotlin-sdk >-----------------
[INFO] Building CasperKotlinSDK 1.0
[INFO] --------------------------------[ jar ]---------------------------------
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcjmail-jdk15on/1.70/bcjmail-jdk15on-1.70.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcjmail-jdk15on/1.70/bcjmail-jdk15on-1.70.pom (2.2 kB at 2.9 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcutil-jdk15on/1.70/bcutil-jdk15on-1.70.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcutil-jdk15on/1.70/bcutil-jdk15on-1.70.pom (1.3 kB at 5.6 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcpkix-jdk15on/1.70/bcpkix-jdk15on-1.70.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcpkix-jdk15on/1.70/bcpkix-jdk15on-1.70.pom (1.6 kB at 8.7 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/jakarta/mail/jakarta.mail-api/maven-metadata.xml
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/maven-metadata.xml
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/maven-metadata.xml (832 B at 6.6 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/jakarta/mail/jakarta.mail-api/maven-metadata.xml (832 B at 1.5 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.0.0/jakarta.mail-api-2.0.0.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.0.0/jakarta.mail-api-2.0.0.pom (5.5 kB at 46 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/com/sun/mail/all/2.0.0/all-2.0.0.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/com/sun/mail/all/2.0.0/all-2.0.0.pom (22 kB at 152 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/eclipse/ee4j/project/1.0.6/project-1.0.6.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/eclipse/ee4j/project/1.0.6/project-1.0.6.pom (13 kB at 65 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.0.1/jakarta.mail-api-2.0.1.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.0.1/jakarta.mail-api-2.0.1.pom (6.4 kB at 50 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/com/sun/mail/all/2.0.1/all-2.0.1.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/com/sun/mail/all/2.0.1/all-2.0.1.pom (24 kB at 165 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0-RC1/jakarta.mail-api-2.1.0-RC1.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0-RC1/jakarta.mail-api-2.1.0-RC1.pom (20 kB at 67 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/eclipse/ee4j/project/1.0.7/project-1.0.7.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/eclipse/ee4j/project/1.0.7/project-1.0.7.pom (14 kB at 103 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0-RC1/jakarta.activation-api-2.1.0-RC1.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0-RC1/jakarta.activation-api-2.1.0-RC1.pom (20 kB at 115 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0-RC2/jakarta.mail-api-2.1.0-RC2.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0-RC2/jakarta.mail-api-2.1.0-RC2.pom (21 kB at 89 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0-RC2/jakarta.activation-api-2.1.0-RC2.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0-RC2/jakarta.activation-api-2.1.0-RC2.pom (18 kB at 72 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0/jakarta.mail-api-2.1.0.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0/jakarta.mail-api-2.1.0.pom (20 kB at 37 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0/jakarta.activation-api-2.1.0.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0/jakarta.activation-api-2.1.0.pom (18 kB at 35 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/maven-metadata.xml
Downloading from central: https://repo.maven.apache.org/maven2/jakarta/activation/jakarta.activation-api/maven-metadata.xml
Downloaded from central: https://repo.maven.apache.org/maven2/jakarta/activation/jakarta.activation-api/maven-metadata.xml (646 B at 1.2 kB/s)
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/maven-metadata.xml (646 B at 1.2 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.0.0/jakarta.activation-api-2.0.0.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.0.0/jakarta.activation-api-2.0.0.pom (5.3 kB at 9.5 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/com/sun/activation/all/2.0.0/all-2.0.0.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/com/sun/activation/all/2.0.0/all-2.0.0.pom (17 kB at 8.7 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.0.1/jakarta.activation-api-2.0.1.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.0.1/jakarta.activation-api-2.0.1.pom (6.8 kB at 30 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/com/sun/activation/all/2.0.1/all-2.0.1.pom
Downloaded from mavenCentral: https://repo1.maven.org/maven2/com/sun/activation/all/2.0.1/all-2.0.1.pom (23 kB at 102 kB/s)
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcjmail-jdk15on/1.70/bcjmail-jdk15on-1.70.jar
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcutil-jdk15on/1.70/bcutil-jdk15on-1.70.jar
Downloading from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcpkix-jdk15on/1.70/bcpkix-jdk15on-1.70.jar
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0/jakarta.mail-api-2.1.0.jar
Downloading from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0/jakarta.activation-api-2.1.0.jar
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/activation/jakarta.activation-api/2.1.0/jakarta.activation-api-2.1.0.jar (63 kB at 106 kB/s)
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcjmail-jdk15on/1.70/bcjmail-jdk15on-1.70.jar (113 kB at 183 kB/s)
Downloaded from mavenCentral: https://repo1.maven.org/maven2/jakarta/mail/jakarta.mail-api/2.1.0/jakarta.mail-api-2.1.0.jar (236 kB at 154 kB/s)
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcutil-jdk15on/1.70/bcutil-jdk15on-1.70.jar (483 kB at 182 kB/s)
Downloaded from mavenCentral: https://repo1.maven.org/maven2/org/bouncycastle/bcpkix-jdk15on/1.70/bcpkix-jdk15on-1.70.jar (964 kB at 279 kB/s)
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
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit-platform/2.22.2/surefire-junit-platform-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit-platform/2.22.2/surefire-junit-platform-2.22.2.pom (7.0 kB at 39 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/2.22.2/surefire-providers-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/2.22.2/surefire-providers-2.22.2.pom (2.5 kB at 6.7 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-launcher/1.3.1/junit-platform-launcher-1.3.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-launcher/1.3.1/junit-platform-launcher-1.3.1.pom (2.2 kB at 18 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apiguardian/apiguardian-api/1.0.0/apiguardian-api-1.0.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apiguardian/apiguardian-api/1.0.0/apiguardian-api-1.0.0.pom (1.2 kB at 7.8 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.3.1/junit-platform-engine-1.3.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.3.1/junit-platform-engine-1.3.1.pom (2.4 kB at 21 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.3.1/junit-platform-commons-1.3.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.3.1/junit-platform-commons-1.3.1.pom (2.0 kB at 13 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/opentest4j/opentest4j/1.1.1/opentest4j-1.1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/opentest4j/opentest4j/1.1.1/opentest4j-1.1.1.pom (1.7 kB at 12 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apiguardian/apiguardian-api/1.0.0/apiguardian-api-1.0.0.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit-platform/2.22.2/surefire-junit-platform-2.22.2.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-launcher/1.3.1/junit-platform-launcher-1.3.1.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.3.1/junit-platform-commons-1.3.1.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.3.1/junit-platform-engine-1.3.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apiguardian/apiguardian-api/1.0.0/apiguardian-api-1.0.0.jar (2.2 kB at 7.3 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/opentest4j/opentest4j/1.1.1/opentest4j-1.1.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.3.1/junit-platform-commons-1.3.1.jar (78 kB at 179 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/opentest4j/opentest4j/1.1.1/opentest4j-1.1.1.jar (7.1 kB at 52 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit-platform/2.22.2/surefire-junit-platform-2.22.2.jar (66 kB at 152 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-launcher/1.3.1/junit-platform-launcher-1.3.1.jar (95 kB at 208 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.3.1/junit-platform-engine-1.3.1.jar (135 kB at 246 kB/s)
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
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.726 s - in com.casper.sdk.crypto.Ed25519HandleTest
[INFO] Running com.casper.sdk.crypto.Secp256k1HandleTest
Error write private key to a non-exist file
Error write public key to a non-exist file
Error load private key from a wrong file format
Error load private key from a wrong file format
Error load wrong private key from a wrong path
Error load public key from a wrong file format
Error load public key from a wrong file format
Error load wrong public key from a wrong path
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.183 s - in com.casper.sdk.crypto.Secp256k1HandleTest
[INFO] Running com.casper.sdk.getblock.GetBlockRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.454 s - in com.casper.sdk.getblock.GetBlockRPCTest
[INFO] Running com.casper.sdk.getpeers.GetPeersTest
First peer entry nodeId: tls:000b..65c7 and address: 136.243.187.84:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.344 s - in com.casper.sdk.getpeers.GetPeersTest
[INFO] Running com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.955 s - in com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
[INFO] Running com.casper.sdk.serialization.CLTypeSerializationTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.001 s - in com.casper.sdk.serialization.CLTypeSerializationTest
[INFO] Running com.casper.sdk.serialization.DeploySerializeHelperTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.022 s - in com.casper.sdk.serialization.DeploySerializeHelperTest
[INFO] Running com.casper.sdk.serialization.CLParseSerializationTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.006 s - in com.casper.sdk.serialization.CLParseSerializationTest
[INFO] Running com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.434 s - in com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Running com.casper.sdk.getstateroothash.GetStateRootHashTest
Error Get State Root Hash,  invalid parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.778 s - in com.casper.sdk.getstateroothash.GetStateRootHashTest
[INFO] Running com.casper.sdk.getauction.GetAuctionInfoRPCTest
Error get auction information with wrong block height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 58.471 s - in com.casper.sdk.getauction.GetAuctionInfoRPCTest
[INFO] Running com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
Error with wrong state root hash
Error wrong DictionayIdentifier parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.639 s - in com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
[INFO] Running com.casper.sdk.getstatus.GetStatusRPCTest
First peer entry node_id:  tls:000b..65c7 and address: 136.243.187.84:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.341 s - in com.casper.sdk.getstatus.GetStatusRPCTest
[INFO] Running com.casper.sdk.getitem.GetItemRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.176 s - in com.casper.sdk.getitem.GetItemRPCTest
[INFO] Running com.casper.sdk.getbalance.GetBalanceRPCTest
Error get balance with wrong state root hash
Error get balance with wrong purse uref
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.114 s - in com.casper.sdk.getbalance.GetBalanceRPCTest
[INFO] Running com.casper.sdk.putdeploy.PutDeployRPCTest
Put deploy successfull with deploy hash Ed25519:a1a76d40f799d14fcaf8e32b0a74215f73c2452bef6d49e65b15f8292cd509ef
Put deploy successfull with deploy hash Secp256k1:650ce35c7db7cdfcad3c5680db35cb3e8d3aff096789b62b45900301d1ebfe7e
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.093 s - in com.casper.sdk.putdeploy.PutDeployRPCTest
[INFO] Running com.casper.sdk.getdeploy.GetDeployRPCTest
Negative test, Error IllegalArgumentException caught
Negative test, Error IllegalArgumentException caught
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 18.483 s - in com.casper.sdk.getdeploy.GetDeployRPCTest
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
[INFO] Total time:  02:06 min
[INFO] Finished at: 2022-07-21T15:27:46+03:00
[INFO] ------------------------------------------------------------------------


```


