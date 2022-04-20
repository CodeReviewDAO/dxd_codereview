```
hep-abaelm:crypto-keys reviewer$ mvn test
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] com.syntifi.crypto:crypto-keys
[INFO] crypto-key-common
[INFO] crypto-key-ed25519
[INFO] crypto-key-secp256k1
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building com.syntifi.crypto:crypto-keys 0.3.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-keys ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/reviewer/reviews/crypto-keys/target/jacoco.exec
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ crypto-keys ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building crypto-key-common 0.3.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-key-common ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/reviewer/reviews/crypto-keys/crypto-key-common/target/jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ crypto-key-common ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ crypto-key-common ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ crypto-key-common ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ crypto-key-common ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ crypto-key-common ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.crypto.key.encdec.Base58Test
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.04 s - in com.syntifi.crypto.key.encdec.Base58Test
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ crypto-key-common ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-common/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-common' with 6 classes
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building crypto-key-ed25519 0.3.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-key-ed25519 ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/reviewer/reviews/crypto-keys/crypto-key-ed25519/target/jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ crypto-key-ed25519 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ crypto-key-ed25519 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ crypto-key-ed25519 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 3 resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ crypto-key-ed25519 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ crypto-key-ed25519 ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.crypto.key.Ed25519PublicKeyTests
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.707 s - in com.syntifi.crypto.key.Ed25519PublicKeyTests
[INFO] Running com.syntifi.crypto.key.Ed25519PrivateKeyTests
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.017 s - in com.syntifi.crypto.key.Ed25519PrivateKeyTests
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 7, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ crypto-key-ed25519 ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-ed25519/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-ed25519' with 2 classes
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building crypto-key-secp256k1 0.3.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-key-secp256k1 ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ crypto-key-secp256k1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ crypto-key-secp256k1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ crypto-key-secp256k1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 3 resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ crypto-key-secp256k1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ crypto-key-secp256k1 ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.crypto.key.Secp256k1PrivateKeyTests
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.732 s - in com.syntifi.crypto.key.Secp256k1PrivateKeyTests
[INFO] Running com.syntifi.crypto.key.Secp256k1PublicKeyTests
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.005 s - in com.syntifi.crypto.key.Secp256k1PublicKeyTests
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 7, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ crypto-key-secp256k1 ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-secp256k1' with 2 classes
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO] 
[INFO] com.syntifi.crypto:crypto-keys ..................... SUCCESS [  0.381 s]
[INFO] crypto-key-common .................................. SUCCESS [  2.201 s]
[INFO] crypto-key-ed25519 ................................. SUCCESS [  2.006 s]
[INFO] crypto-key-secp256k1 ............................... SUCCESS [  2.012 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 6.684 s
[INFO] Finished at: 2022-04-20T12:38:23+02:00
[INFO] Final Memory: 12M/203M
[INFO] ------------------------------------------------------------------------
```
