```bash
~/reviews/ori$ sudo ./mvnw test
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO]
[INFO] com.syntifi.ori:ori                                                [pom]
[INFO] ori-shared                                                         [jar]
[INFO] ori-risk-metric                                                    [jar]
[INFO] ori-api                                                            [jar]
[INFO] ori-client                                                         [jar]
[INFO] ori-chains                                                         [pom]
[INFO] ori-chain-base                                                     [jar]
[INFO] ori-cspr                                                           [jar]
[INFO] ori-eth                                                            [jar]
[INFO] ori-frontend                                                       [pom]
[INFO] ori-dashboard                                                      [pom]
[INFO]
[INFO] ------------------------< com.syntifi.ori:ori >-------------------------
[INFO] Building com.syntifi.ori:ori 0.2.0-SNAPSHOT                       [1/11]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] ---------------------< com.syntifi.ori:ori-shared >---------------------
[INFO] Building ori-shared 0.1.0-SNAPSHOT                                [2/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-shared ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-shared/target/jacoco.exec
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-shared ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-shared ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-shared ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-shared ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-shared ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.ori.dto.BlockDTOTest
Mar 21, 2022 10:57:08 AM org.hibernate.validator.internal.util.Version <clinit>
INFO: HV000001: Hibernate Validator 6.2.1.Final
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.535 s - in com.syntifi.ori.dto.BlockDTOTest
[INFO] Running com.syntifi.ori.dto.AccountDTOTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.006 s - in com.syntifi.ori.dto.AccountDTOTest
[INFO] Running com.syntifi.ori.dto.AMLRulesDTOTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.004 s - in com.syntifi.ori.dto.AMLRulesDTOTest
[INFO] Running com.syntifi.ori.dto.TransactionDTOTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.005 s - in com.syntifi.ori.dto.TransactionDTOTest
[INFO] Running com.syntifi.ori.dto.TokenDTOTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.004 s - in com.syntifi.ori.dto.TokenDTOTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 6, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-shared ---
[INFO] Loading execution data file /home/user/reviews/ori/ori-shared/target/jacoco.exec
[INFO] Analyzed bundle 'ori-shared' with 1 classes
[INFO]
[INFO] ------------------< com.syntifi.ori:ori-risk-metric >-------------------
[INFO] Building ori-risk-metric 0.1.0-SNAPSHOT                           [3/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-risk-metric ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-risk-metric/target/jacoco.exec
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-risk-metric ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-risk-metric ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-risk-metric ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-risk-metric ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-risk-metric ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.ori.RiskMetricsTest
log4j:WARN No appenders could be found for logger (org.jboss.logging).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.255 s - in com.syntifi.ori.RiskMetricsTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-risk-metric ---
[INFO] Loading execution data file /home/user/reviews/ori/ori-risk-metric/target/jacoco.exec
[INFO] Analyzed bundle 'ori-risk-metric' with 1 classes
[INFO]
[INFO] ----------------------< com.syntifi.ori:ori-api >-----------------------
[INFO] Building ori-api 0.2.0-SNAPSHOT                                   [4/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-api ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 2 resources
[INFO] Copying 9 resources to frontend
[INFO]
[INFO] --- quarkus-maven-plugin:2.7.1.Final:generate-code (default) @ ori-api ---
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-api ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- quarkus-maven-plugin:2.7.1.Final:generate-code-tests (default) @ ori-api ---
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-api ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-api ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-api ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.ori.repository.AccountRespositoryTest
2022-03-21 10:57:13,959 INFO  [org.jbo.threads] (main) JBoss Threads version 3.4.2.Final
2022-03-21 10:57:14,649 WARN  [io.qua.dep.ste.ClassTransformingBuildStep] (build-24) Cannot transform io.smallrye.context.Jdk12CompletionStageWrapper as its containing application archive could not be found.
2022-03-21 10:57:14,657 WARN  [io.qua.dep.ste.ClassTransformingBuildStep] (build-24) Cannot transform io.smallrye.context.Jdk12CompletableFutureWrapper as its containing application archive could not be found.
2022-03-21 10:57:16,219 INFO  [io.quarkus] (main) Quarkus 2.7.1.Final on JVM started in 2.667s. Listening on: http://localhost:8083
2022-03-21 10:57:16,220 INFO  [io.quarkus] (main) Profile test activated.
2022-03-21 10:57:16,220 INFO  [io.quarkus] (main) Installed features: [agroal, cdi, hibernate-orm, hibernate-orm-panache, hibernate-validator, jacoco, jdbc-h2, jdbc-postgresql, narayana-jta, resteasy, resteasy-jackson, smallrye-context-propagation, smallrye-openapi, swagger-ui, vertx]
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 4.756 s - in com.syntifi.ori.repository.AccountRespositoryTest
[INFO] Running com.syntifi.ori.repository.BlockRespositoryTest
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.036 s - in com.syntifi.ori.repository.BlockRespositoryTest
[INFO] Running com.syntifi.ori.repository.TokenRespositoryTest
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.024 s - in com.syntifi.ori.repository.TokenRespositoryTest
[INFO] Running com.syntifi.ori.repository.TransactionRepositoryTest
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.057 s - in com.syntifi.ori.repository.TransactionRepositoryTest
[INFO] Running com.syntifi.ori.rest.AccountRestAPITest
[INFO] Tests run: 7, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.184 s - in com.syntifi.ori.rest.AccountRestAPITest
[INFO] Running com.syntifi.ori.rest.BlockRestAPITest
[INFO] Tests run: 11, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.4 s - in com.syntifi.ori.rest.BlockRestAPITest
[INFO] Running com.syntifi.ori.rest.TokenRestAPITest
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.117 s - in com.syntifi.ori.rest.TokenRestAPITest
[INFO] Running com.syntifi.ori.rest.TransactionMonitorRestAPITest
[INFO] Tests run: 11, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.335 s - in com.syntifi.ori.rest.TransactionMonitorRestAPITest
[INFO] Running com.syntifi.ori.rest.TransactionRestAPITest
[INFO] Tests run: 16, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.402 s - in com.syntifi.ori.rest.TransactionRestAPITest
[INFO] Running com.syntifi.ori.service.AMLServiceTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.004 s - in com.syntifi.ori.service.AMLServiceTest
[INFO] Running com.syntifi.ori.service.TransactionServiceTest
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.013 s - in com.syntifi.ori.service.TransactionServiceTest
[INFO] Running com.syntifi.ori.model.AccountTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.115 s - in com.syntifi.ori.model.AccountTest
[INFO] Running com.syntifi.ori.model.BlockTest
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.011 s - in com.syntifi.ori.model.BlockTest
[INFO] Running com.syntifi.ori.model.TokenTest
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.006 s - in com.syntifi.ori.model.TokenTest
[INFO] Running com.syntifi.ori.model.TransactionTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.005 s - in com.syntifi.ori.model.TransactionTest
2022-03-21 10:57:19,532 INFO  [io.quarkus] (main) Quarkus stopped in 0.039s
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 84, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] ---------------------< com.syntifi.ori:ori-client >---------------------
[INFO] Building ori-client 0.1.0-SNAPSHOT                                [5/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-client ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-client/target/jacoco.exec
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-client ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-client ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-client ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-client ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-client ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 0, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-client ---
[INFO] Loading execution data file /home/user/reviews/ori/ori-client/target/jacoco.exec
[INFO] Analyzed bundle 'ori-client' with 2 classes
[INFO]
[INFO] ---------------------< com.syntifi.ori:ori-chains >---------------------
[INFO] Building ori-chains 0.1.0-SNAPSHOT                                [6/11]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-chains ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-chains/target/jacoco.exec
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-chains ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] ---------------< com.syntifi.ori.chains:ori-chain-base >----------------
[INFO] Building ori-chain-base 0.1.0-SNAPSHOT                            [7/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-chain-base ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-chains/ori-chain-base/target/jacoco.exec
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-chain-base ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-chain-base ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-chain-base ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-chain-base ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-chain-base ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.ori.chains.base.reader.MockChainReaderTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 6.762 s - in com.syntifi.ori.chains.base.reader.MockChainReaderTest
[INFO] Running com.syntifi.ori.chains.base.writer.OriWriterTest
[INFO] Tests run: 6, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 12.102 s - in com.syntifi.ori.chains.base.writer.OriWriterTest
[INFO] Running com.syntifi.ori.chains.base.processor.MockChainProcessorTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.03 s - in com.syntifi.ori.chains.base.processor.MockChainProcessorTest
[INFO] Running com.syntifi.ori.chains.base.MockChainCrawlerJobTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.112 s - in com.syntifi.ori.chains.base.MockChainCrawlerJobTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 9, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-chain-base ---
[INFO] Loading execution data file /home/user/reviews/ori/ori-chains/ori-chain-base/target/jacoco.exec
[INFO] Analyzed bundle 'ori-chain-base' with 17 classes
[INFO]
[INFO] ------------------< com.syntifi.ori.chains:ori-cspr >-------------------
[INFO] Building ori-cspr 0.1.0-SNAPSHOT                                  [8/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-cspr ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-chains/ori-cspr/target/jacoco.exec
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-cspr ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-cspr ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-cspr ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 9 resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-cspr ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-cspr ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.ori.chains.cspr.reader.CsprChainReaderTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.972 s - in com.syntifi.ori.chains.cspr.reader.CsprChainReaderTest
[INFO] Running com.syntifi.ori.chains.cspr.CsprChainCrawlerJobTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.093 s - in com.syntifi.ori.chains.cspr.CsprChainCrawlerJobTest
[INFO] Running com.syntifi.ori.chains.cspr.processor.CsprChainProcessorTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.025 s - in com.syntifi.ori.chains.cspr.processor.CsprChainProcessorTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-cspr ---
[INFO] Loading execution data file /home/user/reviews/ori/ori-chains/ori-cspr/target/jacoco.exec
[INFO] Analyzed bundle 'ori-cspr' with 5 classes
[INFO]
[INFO] -------------------< com.syntifi.ori.chains:ori-eth >-------------------
[INFO] Building ori-eth 0.1.0-SNAPSHOT                                   [9/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-eth ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-chains/ori-eth/target/jacoco.exec
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ ori-eth ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ ori-eth ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ ori-eth ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 12 resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ ori-eth ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ ori-eth ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.syntifi.ori.chains.eth.reader.EthChainReaderTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 3.456 s - in com.syntifi.ori.chains.eth.reader.EthChainReaderTest
[INFO] Running com.syntifi.ori.chains.eth.EthChainCrawlerJobTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.102 s - in com.syntifi.ori.chains.eth.EthChainCrawlerJobTest
[INFO] Running com.syntifi.ori.chains.eth.processor.EthChainProcessorTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.011 s - in com.syntifi.ori.chains.eth.processor.EthChainProcessorTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-eth ---
[INFO] Loading execution data file /home/user/reviews/ori/ori-chains/ori-eth/target/jacoco.exec
[INFO] Analyzed bundle 'ori-eth' with 5 classes
[INFO]
[INFO] --------------------< com.syntifi.ori:ori-frontend >--------------------
[INFO] Building ori-frontend 0.1.0-SNAPSHOT                             [10/11]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] --- exec-maven-plugin:3.0.0:exec (npm-install) @ ori-frontend ---

up to date, audited 2234 packages in 5s

212 packages are looking for funding
  run `npm fund` for details

17 moderate severity vulnerabilities

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
[INFO]
[INFO] --- exec-maven-plugin:3.0.0:exec (npm-build) @ ori-frontend ---

> frontend@0.1.0 build
> react-scripts build

Creating an optimized production build...
Compiled with warnings.

Failed to parse source map from '/home/user/reviews/ori/ori-frontend/src/css/vis-network.css.map' file: Error: ENOENT: no such file or directory, open '/home/user/reviews/ori/ori-frontend/src/css/vis-network.css.map'

Search for the keywords to learn more about each warning.
To ignore, add // eslint-disable-next-line to the line before.

File sizes after gzip:

  487.98 kB  build/static/js/main.2b1021f1.js
  30.78 kB   build/static/css/main.9b26f175.css

The project was built assuming it is hosted at /.
You can control this with the homepage field in your package.json.

The build folder is ready to be deployed.
You may serve it with a static server:

  npm install -g serve
  serve -s build

Find out more about deployment here:

  https://cra.link/deployment

[INFO]
[INFO] -------------------< com.syntifi.ori:ori-dashboard >--------------------
[INFO] Building ori-dashboard 0.1.0-SNAPSHOT                            [11/11]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO]
[INFO] com.syntifi.ori:ori 0.2.0-SNAPSHOT ................. SUCCESS [  0.001 s]
[INFO] ori-shared 0.1.0-SNAPSHOT .......................... SUCCESS [  1.649 s]
[INFO] ori-risk-metric 0.1.0-SNAPSHOT ..................... SUCCESS [  0.910 s]
[INFO] ori-api 0.2.0-SNAPSHOT ............................. SUCCESS [  9.980 s]
[INFO] ori-client 0.1.0-SNAPSHOT .......................... SUCCESS [  0.624 s]
[INFO] ori-chains 0.1.0-SNAPSHOT .......................... SUCCESS [  0.029 s]
[INFO] ori-chain-base 0.1.0-SNAPSHOT ...................... SUCCESS [ 23.936 s]
[INFO] ori-cspr 0.1.0-SNAPSHOT ............................ SUCCESS [  3.991 s]
[INFO] ori-eth 0.1.0-SNAPSHOT ............................. SUCCESS [  4.552 s]
[INFO] ori-frontend 0.1.0-SNAPSHOT ........................ SUCCESS [ 25.364 s]
[INFO] ori-dashboard 0.1.0-SNAPSHOT ....................... SUCCESS [  0.001 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:11 min
[INFO] Finished at: 2022-03-21T10:58:18+01:00
[INFO] ------------------------------------------------------------------------
```
