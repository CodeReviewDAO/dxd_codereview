```
hep-abaelm:crypto-keys reviewer$ ./mvnw package
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 58727  100 58727    0     0  42787      0  0:00:01  0:00:01 --:--:-- 42991
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] com.syntifi.crypto:crypto-keys                                     [pom]
[INFO] crypto-key-common                                                  [jar]
[INFO] crypto-key-ed25519                                                 [jar]
[INFO] crypto-key-secp256k1                                               [jar]
[INFO] 
[INFO] -------------------< com.syntifi.crypto:crypto-keys >-------------------
[INFO] Building com.syntifi.crypto:crypto-keys 0.3.0-SNAPSHOT             [1/4]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-keys ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/p35862/reviews/crypto-keys/target/jacoco.exec
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ crypto-keys ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ crypto-keys ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] ----------------< com.syntifi.crypto:crypto-key-common >----------------
[INFO] Building crypto-key-common 0.3.0-SNAPSHOT                          [2/4]
[INFO] --------------------------------[ jar ]---------------------------------
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/2.22.2/maven-surefire-plugin-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/2.22.2/maven-surefire-plugin-2.22.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire/2.22.2/surefire-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire/2.22.2/surefire-2.22.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/33/maven-parent-33.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/33/maven-parent-33.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/2.22.2/maven-surefire-plugin-2.22.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/2.22.2/maven-surefire-plugin-2.22.2.jar (0 B at 0 B/s)
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-key-common ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/p35862/reviews/crypto-keys/crypto-key-common/target/jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ crypto-key-common ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ crypto-key-common ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 8 source files to /Users/reviewer/reviews/crypto-keys/crypto-key-common/target/classes
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ crypto-key-common ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ crypto-key-common ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /Users/reviewer/reviews/crypto-keys/crypto-key-common/target/test-classes
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ crypto-key-common ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/2.22.2/maven-surefire-common-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/2.22.2/maven-surefire-common-2.22.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.5.2/maven-plugin-annotations-3.5.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.5.2/maven-plugin-annotations-3.5.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-tools/3.5.2/maven-plugin-tools-3.5.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-tools/3.5.2/maven-plugin-tools-3.5.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/31/maven-parent-31.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/31/maven-parent-31.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/2.22.2/surefire-api-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/2.22.2/surefire-api-2.22.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/2.22.2/surefire-logger-api-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/2.22.2/surefire-logger-api-2.22.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/2.22.2/surefire-booter-2.22.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/2.22.2/surefire-booter-2.22.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/0.9.10/plexus-languages-0.9.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/0.9.10/plexus-languages-0.9.10.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M8/qdox-2.0-M8.pom
Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M8/qdox-2.0-M8.pom (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/2.22.2/maven-surefire-common-2.22.2.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.5.2/maven-plugin-annotations-3.5.2.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/2.22.2/surefire-api-2.22.2.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/2.22.2/surefire-logger-api-2.22.2.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/2.22.2/surefire-booter-2.22.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/2.22.2/maven-surefire-common-2.22.2.jar (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.jar (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.jar (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M8/qdox-2.0-M8.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/2.22.2/surefire-logger-api-2.22.2.jar (0 B at 0 B/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.5.2/maven-plugin-annotations-3.5.2.jar (0 B at 0 B/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/2.22.2/surefire-api-2.22.2.jar (0 B at 0 B/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/2.22.2/surefire-booter-2.22.2.jar (0 B at 0 B/s)
Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M8/qdox-2.0-M8.jar (0 B at 0 B/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/opentest4j/opentest4j/1.1.1/opentest4j-1.1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/opentest4j/opentest4j/1.1.1/opentest4j-1.1.1.pom (0 B at 0 B/s)
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.crypto.key.encdec.Base58Test
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.035 s - in com.syntifi.crypto.key.encdec.Base58Test
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
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ crypto-key-common ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-common/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-common' with 6 classes
[INFO] 
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ crypto-key-common ---
[INFO] Building jar: /Users/reviewer/reviews/crypto-keys/crypto-key-common/target/crypto-key-common-0.3.0-SNAPSHOT.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.2:test-jar (default) @ crypto-key-common ---
[INFO] Building jar: /Users/reviewer/reviews/crypto-keys/crypto-key-common/target/crypto-key-common-0.3.0-SNAPSHOT-tests.jar
[INFO] 
[INFO] ---------------< com.syntifi.crypto:crypto-key-ed25519 >----------------
[INFO] Building crypto-key-ed25519 0.3.0-SNAPSHOT                         [3/4]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-key-ed25519 ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/p35862/reviews/crypto-keys/crypto-key-ed25519/target/jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ crypto-key-ed25519 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ crypto-key-ed25519 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /Users/reviewer/reviews/crypto-keys/crypto-key-ed25519/target/classes
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ crypto-key-ed25519 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 3 resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ crypto-key-ed25519 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /Users/reviewer/reviews/crypto-keys/crypto-key-ed25519/target/test-classes
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ crypto-key-ed25519 ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.crypto.key.Ed25519PublicKeyTests
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.734 s - in com.syntifi.crypto.key.Ed25519PublicKeyTests
[INFO] Running com.syntifi.crypto.key.Ed25519PrivateKeyTests
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.013 s - in com.syntifi.crypto.key.Ed25519PrivateKeyTests
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
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ crypto-key-ed25519 ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-ed25519/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-ed25519' with 2 classes
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ crypto-key-ed25519 ---
[INFO] Building jar: /Users/p35862/reviews/crypto-keys/crypto-key-ed25519/target/crypto-key-ed25519-0.3.0-SNAPSHOT.jar
[INFO] 
[INFO] --------------< com.syntifi.crypto:crypto-key-secp256k1 >---------------
[INFO] Building crypto-key-secp256k1 0.3.0-SNAPSHOT                       [4/4]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ crypto-key-secp256k1 ---
[INFO] argLine set to -javaagent:/Users/reviewer/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/Users/p35862/reviews/crypto-keys/crypto-key-secp256k1/target/jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ crypto-key-secp256k1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ crypto-key-secp256k1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/classes
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ crypto-key-secp256k1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 3 resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ crypto-key-secp256k1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/test-classes
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ crypto-key-secp256k1 ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.crypto.key.Secp256k1PrivateKeyTests
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.722 s - in com.syntifi.crypto.key.Secp256k1PrivateKeyTests
[INFO] Running com.syntifi.crypto.key.Secp256k1PublicKeyTests
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.006 s - in com.syntifi.crypto.key.Secp256k1PublicKeyTests
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 7, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ crypto-key-secp256k1 ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-secp256k1' with 2 classes
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ crypto-key-secp256k1 ---
[INFO] Loading execution data file /Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/jacoco.exec
[INFO] Analyzed bundle 'crypto-key-secp256k1' with 2 classes
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ crypto-key-secp256k1 ---
[INFO] Building jar: /Users/reviewer/reviews/crypto-keys/crypto-key-secp256k1/target/crypto-key-secp256k1-0.3.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary for com.syntifi.crypto:crypto-keys 0.3.0-SNAPSHOT:
[INFO] 
[INFO] com.syntifi.crypto:crypto-keys ..................... SUCCESS [  0.383 s]
[INFO] crypto-key-common .................................. SUCCESS [  4.504 s]
[INFO] crypto-key-ed25519 ................................. SUCCESS [  3.061 s]
[INFO] crypto-key-secp256k1 ............................... SUCCESS [  3.031 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  11.068 s
[INFO] Finished at: 2022-04-20T12:19:06+02:00
[INFO] ------------------------------------------------------------------------

```