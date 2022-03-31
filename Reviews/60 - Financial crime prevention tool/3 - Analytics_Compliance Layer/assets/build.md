~/reviews/ori$ sudo ./mvnw clean compile

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
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori ---
[INFO]
[INFO] ---------------------< com.syntifi.ori:ori-shared >---------------------
[INFO] Building ori-shared 0.1.0-SNAPSHOT                                [2/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-shared ---
[INFO] Deleting /home/user/reviews/ori/ori-shared/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 6 source files to /home/user/reviews/ori/ori-shared/target/classes
[INFO]
[INFO] ------------------< com.syntifi.ori:ori-risk-metric >-------------------
[INFO] Building ori-risk-metric 0.1.0-SNAPSHOT                           [3/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-risk-metric ---
[INFO] Deleting /home/user/reviews/ori/ori-risk-metric/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /home/user/reviews/ori/ori-risk-metric/target/classes
[INFO]
[INFO] ----------------------< com.syntifi.ori:ori-api >-----------------------
[INFO] Building ori-api 0.2.0-SNAPSHOT                                   [4/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-api ---
[INFO] Deleting /home/user/reviews/ori/ori-api/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 30 source files to /home/user/reviews/ori/ori-api/target/classes
[INFO]
[INFO] ---------------------< com.syntifi.ori:ori-client >---------------------
[INFO] Building ori-client 0.1.0-SNAPSHOT                                [5/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-client ---
[INFO] Deleting /home/user/reviews/ori/ori-client/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 3 source files to /home/user/reviews/ori/ori-client/target/classes
[INFO]
[INFO] ---------------------< com.syntifi.ori:ori-chains >---------------------
[INFO] Building ori-chains 0.1.0-SNAPSHOT                                [6/11]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-chains ---
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (prepare-agent) @ ori-chains ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.7/org.jacoco.agent-0.8.7-runtime.jar=destfile=/home/user/reviews/ori/ori-chains/target/jacoco.exec
[INFO]
[INFO] ---------------< com.syntifi.ori.chains:ori-chain-base >----------------
[INFO] Building ori-chain-base 0.1.0-SNAPSHOT                            [7/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-chain-base ---
[INFO] Deleting /home/user/reviews/ori/ori-chains/ori-chain-base/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 16 source files to /home/user/reviews/ori/ori-chains/ori-chain-base/target/classes
[INFO]
[INFO] ------------------< com.syntifi.ori.chains:ori-cspr >-------------------
[INFO] Building ori-cspr 0.1.0-SNAPSHOT                                  [8/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-cspr ---
[INFO] Deleting /home/user/reviews/ori/ori-chains/ori-cspr/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 6 source files to /home/user/reviews/ori/ori-chains/ori-cspr/target/classes
[INFO]
[INFO] -------------------< com.syntifi.ori.chains:ori-eth >-------------------
[INFO] Building ori-eth 0.1.0-SNAPSHOT                                   [9/11]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-eth ---
[INFO] Deleting /home/user/reviews/ori/ori-chains/ori-eth/target
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
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 6 source files to /home/user/reviews/ori/ori-chains/ori-eth/target/classes
[INFO]
[INFO] --------------------< com.syntifi.ori:ori-frontend >--------------------
[INFO] Building ori-frontend 0.1.0-SNAPSHOT                             [10/11]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-frontend ---
[INFO]
[INFO] --- exec-maven-plugin:3.0.0:exec (npm-install) @ ori-frontend ---

up to date, audited 2234 packages in 2s

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
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ ori-dashboard ---
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO]
[INFO] com.syntifi.ori:ori 0.2.0-SNAPSHOT ................. SUCCESS [  0.041 s]
[INFO] ori-shared 0.1.0-SNAPSHOT .......................... SUCCESS [  0.970 s]
[INFO] ori-risk-metric 0.1.0-SNAPSHOT ..................... SUCCESS [  0.263 s]
[INFO] ori-api 0.2.0-SNAPSHOT ............................. SUCCESS [  1.741 s]
[INFO] ori-client 0.1.0-SNAPSHOT .......................... SUCCESS [  0.245 s]
[INFO] ori-chains 0.1.0-SNAPSHOT .......................... SUCCESS [  0.025 s]
[INFO] ori-chain-base 0.1.0-SNAPSHOT ...................... SUCCESS [  0.476 s]
[INFO] ori-cspr 0.1.0-SNAPSHOT ............................ SUCCESS [  0.250 s]
[INFO] ori-eth 0.1.0-SNAPSHOT ............................. SUCCESS [  0.260 s]
[INFO] ori-frontend 0.1.0-SNAPSHOT ........................ SUCCESS [ 22.674 s]
[INFO] ori-dashboard 0.1.0-SNAPSHOT ....................... SUCCESS [  0.002 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  27.553 s
[INFO] Finished at: 2022-03-19T15:43:35+01:00
[INFO] ------------------------------------------------------------------------
