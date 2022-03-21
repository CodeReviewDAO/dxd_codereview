~/reviews/ori$ sudo ./mvnw package -DskipTests
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-shared ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-shared ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-shared ---
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-risk-metric ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-risk-metric ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-risk-metric ---
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-api ---
[INFO] Building jar: /home/user/reviews/ori/ori-api/target/ori-api-0.2.0-SNAPSHOT.jar
[INFO]
[INFO] --- quarkus-maven-plugin:2.7.1.Final:build (default) @ ori-api ---
[INFO] [org.hibernate.Version] HHH000412: Hibernate ORM core version 5.6.5.Final
[INFO] Loaded org.testcontainers.dockerclient.UnixSocketClientProviderStrategy from ~/.testcontainers.properties, will try it first
[INFO] Found Docker environment with local Unix socket (unix:///var/run/docker.sock)
[INFO] Docker host IP address is localhost
[INFO] Connected to docker:
  Server Version: 20.10.13
  API Version: 1.41
  Operating System: Ubuntu 20.04.3 LTS
  Total Memory: 128822 MB
[INFO] Image name substitution will be performed by: DefaultImageNameSubstitutor (composite of 'ConfigurationFileImageNameSubstitutor' and 'PrefixingImageNameSubstitutor')
[INFO] Failure when attempting to lookup auth config. Please ignore if you don't have images in an authenticated registry. Details: (dockerImageName: testcontainers/ryuk:0.3.3, configFile: /root/.docker/config.json. Falling back to docker-java default behaviour. Exception message: /root/.docker/config.json (No such file or directory)
[INFO] Ryuk started - will monitor and terminate Testcontainers containers on JVM exit
[INFO] Checking the system...
[INFO] ✔︎ Docker server version should be at least 1.6.0
[INFO] ✔︎ Docker environment should have more than 2GB free disk space
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Starting (local) container image build for jar using docker.
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Executing the following command to build docker image: 'docker build -f /home/user/reviews/ori/ori-api/src/main/docker/Dockerfile.jvm -t syntifi.com/ori/ori-api-jvm:0.2.0-SNAPSHOT /home/user/reviews/ori/ori-api'
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Sending build context to Docker daemon  42.31MB
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 1/13 : FROM registry.access.redhat.com/ubi8/ubi-minimal:8.4
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> e7685639f552
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 2/13 : ARG JAVA_PACKAGE=java-11-openjdk-headless
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Using cache
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 2e66aa4e2ec7
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 3/13 : ARG RUN_JAVA_VERSION=1.3.8
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Using cache
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 7f008c8c2303
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 4/13 : ENV LANG='en_US.UTF-8' LANGUAGE='en_US:en'
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Using cache
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 29895f94bd8f
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 5/13 : RUN microdnf install curl ca-certificates ${JAVA_PACKAGE}     && microdnf update     && microdnf clean all     && mkdir /deployments     && chown 1001 /deployments     && chmod "g+rwX" /deployments     && chown 1001:root /deployments     && curl https://repo1.maven.org/maven2/io/fabric8/run-java-sh/${RUN_JAVA_VERSION}/run-java-sh-${RUN_JAVA_VERSION}-sh.sh -o /deployments/run-java.sh     && chown 1001 /deployments/run-java.sh     && chmod 540 /deployments/run-java.sh     && echo "securerandom.source=file:/dev/urandom" >> /etc/alternatives/jre/conf/security/java.security
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Using cache
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 9434ddc80eaa
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 6/13 : ENV JAVA_OPTIONS="-Dquarkus.http.host=0.0.0.0 -Djava.util.logging.manager=org.jboss.logmanager.LogManager"
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Using cache
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 071110404335
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 7/13 : COPY --chown=1001 target/quarkus-app/lib/ /deployments/lib/
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Using cache
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> c5f6116e4577
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 8/13 : COPY --chown=1001 target/quarkus-app/*.jar /deployments/
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> bce67e4bec5f
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 9/13 : COPY --chown=1001 target/quarkus-app/app/ /deployments/app/
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 7dd41dfb9b3f
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 10/13 : COPY --chown=1001 target/quarkus-app/quarkus/ /deployments/quarkus/
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 70e88fee4da9
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 11/13 : EXPOSE 8080
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Running in 3b2155d89ad1
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Removing intermediate container 3b2155d89ad1
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 70bfe9aefd13
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 12/13 : USER 1001
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Running in 4ebc5ce1391f
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Removing intermediate container 4ebc5ce1391f
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> 30f20b469c8d
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Step 13/13 : ENTRYPOINT [ "/deployments/run-java.sh" ]
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> Running in 1d7926549bed
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Removing intermediate container 1d7926549bed
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor]  ---> eeed9e1c7129
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Successfully built eeed9e1c7129
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Successfully tagged syntifi.com/ori/ori-api-jvm:0.2.0-SNAPSHOT
[INFO] [io.quarkus.container.image.docker.deployment.DockerProcessor] Built container image syntifi.com/ori/ori-api-jvm:0.2.0-SNAPSHOT (eeed9e1c7129)

[INFO] [io.quarkus.deployment.QuarkusAugmentor] Quarkus augmentation completed in 3388ms
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-client ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-client ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-client ---
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
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-chains ---
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-chain-base ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-chain-base ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-chain-base ---
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-cspr ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-cspr ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-cspr ---
[INFO]
[INFO] >>> spring-boot-maven-plugin:2.6.3:build-image (default) > package @ ori-cspr >>>
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-cspr ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-cspr ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-cspr ---
[INFO]
[INFO] <<< spring-boot-maven-plugin:2.6.3:build-image (default) < package @ ori-cspr <<<
[INFO]
[INFO]
[INFO] --- spring-boot-maven-plugin:2.6.3:build-image (default) @ ori-cspr ---
[INFO] Building image 'syntifi.com/ori/ori-chains/ori-cspr:0.1.0-SNAPSHOT'
[INFO]
[INFO]  > Pulling builder image 'docker.io/paketobuildpacks/builder:base' 100%
[INFO]  > Pulled builder image 'paketobuildpacks/builder@sha256:f0f81da4ebb0a9ae5c67ff0bc2de3896ff1b33bb5645b9d360ac8643a908ffa1'
[INFO]  > Pulling run image 'docker.io/paketobuildpacks/run:base-cnb' 100%
[INFO]  > Pulled run image 'paketobuildpacks/run@sha256:bcab6379bf83f0657dab49f08c7da7f23a6b18145352b2e13178e35cf6bd39c1'
[INFO]  > Executing lifecycle version v0.13.5
[INFO]  > Using build cache volume 'pack-cache-ec4f3d728ef3.build'
[INFO]
[INFO]  > Running creator
[INFO]     [creator]     ===> DETECTING
[INFO]     [creator]     ======== Output: paketo-buildpacks/poetry@0.1.2 ========
[INFO]     [creator]     pyproject.toml must include [tool.poetry.dependencies.python], see https://python-poetry.org/docs/pyproject/#dependencies-and-dev-dependencies
[INFO]     [creator]     err:  paketo-buildpacks/poetry@0.1.2 (1)
[INFO]     [creator]     ======== Output: paketo-buildpacks/poetry@0.1.2 ========
[INFO]     [creator]     pyproject.toml must include [tool.poetry.dependencies.python], see https://python-poetry.org/docs/pyproject/#dependencies-and-dev-dependencies
[INFO]     [creator]     err:  paketo-buildpacks/poetry@0.1.2 (1)
[INFO]     [creator]     6 of 21 buildpacks participating
[INFO]     [creator]     paketo-buildpacks/ca-certificates   3.1.0
[INFO]     [creator]     paketo-buildpacks/bellsoft-liberica 9.2.0
[INFO]     [creator]     paketo-buildpacks/syft              1.10.0
[INFO]     [creator]     paketo-buildpacks/executable-jar    6.1.0
[INFO]     [creator]     paketo-buildpacks/dist-zip          5.2.0
[INFO]     [creator]     paketo-buildpacks/spring-boot       5.8.0
[INFO]     [creator]     ===> ANALYZING
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/ca-certificates:helper" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/bellsoft-liberica:jre" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/bellsoft-liberica:helper" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/bellsoft-liberica:java-security-properties" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/syft:syft" from cache
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/spring-boot:spring-cloud-bindings" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/spring-boot:web-application-type" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/spring-boot:helper" from app image
[INFO]     [creator]     ===> RESTORING
[INFO]     [creator]     Restoring data for "paketo-buildpacks/syft:syft" from cache
[INFO]     [creator]     ===> BUILDING
[INFO]     [creator]
[INFO]     [creator]     Paketo CA Certificates Buildpack 3.1.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/ca-certificates
[INFO]     [creator]       Launch Helper: Reusing cached layer
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]
[INFO]     [creator]     Paketo BellSoft Liberica Buildpack 9.2.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/bellsoft-liberica
[INFO]     [creator]       Build Configuration:
[INFO]     [creator]         $BP_JVM_TYPE                 JRE             the JVM type - JDK or JRE
[INFO]     [creator]         $BP_JVM_VERSION              11.*            the Java version
[INFO]     [creator]       Launch Configuration:
[INFO]     [creator]         $BPL_DEBUG_ENABLED           false           enables Java remote debugging support
[INFO]     [creator]         $BPL_DEBUG_PORT              8000            configure the remote debugging port
[INFO]     [creator]         $BPL_DEBUG_SUSPEND           false           configure whether to suspend execution until a debugger has attached
[INFO]     [creator]         $BPL_HEAP_DUMP_PATH                          write heap dumps on error to this path
[INFO]     [creator]         $BPL_JAVA_NMT_ENABLED        true            enables Java Native Memory Tracking (NMT)
[INFO]     [creator]         $BPL_JAVA_NMT_LEVEL          summary         configure level of NMT, summary or detail
[INFO]     [creator]         $BPL_JFR_ARGS                                configure custom Java Flight Recording (JFR) arguments
[INFO]     [creator]         $BPL_JFR_ENABLED             false           enables Java Flight Recording (JFR)
[INFO]     [creator]         $BPL_JMX_ENABLED             false           enables Java Management Extensions (JMX)
[INFO]     [creator]         $BPL_JMX_PORT                5000            configure the JMX port
[INFO]     [creator]         $BPL_JVM_HEAD_ROOM           0               the headroom in memory calculation
[INFO]     [creator]         $BPL_JVM_LOADED_CLASS_COUNT  35% of classes  the number of loaded classes in memory calculation
[INFO]     [creator]         $BPL_JVM_THREAD_COUNT        250             the number of threads in memory calculation
[INFO]     [creator]         $JAVA_TOOL_OPTIONS                           the JVM launch flags
[INFO]     [creator]       BellSoft Liberica JRE 11.0.14: Reusing cached layer
[INFO]     [creator]       Launch Helper: Reusing cached layer
[INFO]     [creator]       Java Security Properties: Reusing cached layer
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]
[INFO]     [creator]     Paketo Syft Buildpack 1.10.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/syft
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]
[INFO]     [creator]     Paketo Executable JAR Buildpack 6.1.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/executable-jar
[INFO]     [creator]       Class Path: Contributing to layer
[INFO]     [creator]         Writing env/CLASSPATH.delim
[INFO]     [creator]         Writing env/CLASSPATH.prepend
[INFO]     [creator]       Process types:
[INFO]     [creator]         executable-jar: java org.springframework.boot.loader.JarLauncher (direct)
[INFO]     [creator]         task:           java org.springframework.boot.loader.JarLauncher (direct)
[INFO]     [creator]         web:            java org.springframework.boot.loader.JarLauncher (direct)
[INFO]     [creator]
[INFO]     [creator]     Paketo Spring Boot Buildpack 5.8.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/spring-boot
[INFO]     [creator]       Build Configuration:
[INFO]     [creator]         $BP_SPRING_CLOUD_BINDINGS_ENABLED    true   whether to contribute Spring Boot cloud bindings support
[INFO]     [creator]       Launch Configuration:
[INFO]     [creator]         $BPL_SPRING_CLOUD_BINDINGS_DISABLED  false  whether to auto-configure Spring Boot environment properties from bindings
[INFO]     [creator]         $BPL_SPRING_CLOUD_BINDINGS_ENABLED   true   Deprecated - whether to auto-configure Spring Boot environment properties from bindings
[INFO]     [creator]       Creating slices from layers index
[INFO]     [creator]         dependencies
[INFO]     [creator]         spring-boot-loader
[INFO]     [creator]         snapshot-dependencies
[INFO]     [creator]         application
[INFO]     [creator]       Launch Helper: Reusing cached layer
[INFO]     [creator]       Spring Cloud Bindings 1.8.1: Reusing cached layer
[INFO]     [creator]       Web Application Type: Reusing cached layer
[INFO]     [creator]       4 application slices
[INFO]     [creator]       Image labels:
[INFO]     [creator]         org.springframework.boot.version
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]     ===> EXPORTING
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/ca-certificates:helper'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/bellsoft-liberica:helper'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/bellsoft-liberica:java-security-properties'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/bellsoft-liberica:jre'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/executable-jar:classpath'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/spring-boot:helper'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/spring-boot:spring-cloud-bindings'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/spring-boot:web-application-type'
[INFO]     [creator]     Reusing 5/5 app layer(s)
[INFO]     [creator]     Reusing layer 'launcher'
[INFO]     [creator]     Reusing layer 'config'
[INFO]     [creator]     Reusing layer 'process-types'
[INFO]     [creator]     Adding label 'io.buildpacks.lifecycle.metadata'
[INFO]     [creator]     Adding label 'io.buildpacks.build.metadata'
[INFO]     [creator]     Adding label 'io.buildpacks.project.metadata'
[INFO]     [creator]     Adding label 'org.springframework.boot.version'
[INFO]     [creator]     Setting default process type 'web'
[INFO]     [creator]     Saving syntifi.com/ori/ori-chains/ori-cspr:0.1.0-SNAPSHOT...
[INFO]     [creator]     *** Images (78f11981982b):
[INFO]     [creator]           syntifi.com/ori/ori-chains/ori-cspr:0.1.0-SNAPSHOT
[INFO]     [creator]     Reusing cache layer 'paketo-buildpacks/syft:syft'
[INFO]
[INFO] Successfully built image 'syntifi.com/ori/ori-chains/ori-cspr:0.1.0-SNAPSHOT'
[INFO]
[INFO] Successfully created image tag 'syntifi.com/ori/ori-chains/ori-cspr:latest'
[INFO]
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-eth ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-eth ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-eth ---
[INFO]
[INFO] >>> spring-boot-maven-plugin:2.6.3:build-image (default) > package @ ori-eth >>>
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
[INFO] Tests are skipped.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (post-unit-test) @ ori-eth ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- jacoco-maven-plugin:0.8.7:report (report) @ ori-eth ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO]
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ ori-eth ---
[INFO]
[INFO] <<< spring-boot-maven-plugin:2.6.3:build-image (default) < package @ ori-eth <<<
[INFO]
[INFO]
[INFO] --- spring-boot-maven-plugin:2.6.3:build-image (default) @ ori-eth ---
[INFO] Building image 'syntifi.com/ori/ori-chains/ori-eth:0.1.0-SNAPSHOT'
[INFO]
[INFO]  > Pulling builder image 'docker.io/paketobuildpacks/builder:base' 100%
[INFO]  > Pulled builder image 'paketobuildpacks/builder@sha256:f0f81da4ebb0a9ae5c67ff0bc2de3896ff1b33bb5645b9d360ac8643a908ffa1'
[INFO]  > Pulling run image 'docker.io/paketobuildpacks/run:base-cnb' 100%
[INFO]  > Pulled run image 'paketobuildpacks/run@sha256:bcab6379bf83f0657dab49f08c7da7f23a6b18145352b2e13178e35cf6bd39c1'
[INFO]  > Executing lifecycle version v0.13.5
[INFO]  > Using build cache volume 'pack-cache-adab780b26f8.build'
[INFO]
[INFO]  > Running creator
[INFO]     [creator]     ===> DETECTING
[INFO]     [creator]     ======== Output: paketo-buildpacks/poetry@0.1.2 ========
[INFO]     [creator]     pyproject.toml must include [tool.poetry.dependencies.python], see https://python-poetry.org/docs/pyproject/#dependencies-and-dev-dependencies
[INFO]     [creator]     err:  paketo-buildpacks/poetry@0.1.2 (1)
[INFO]     [creator]     ======== Output: paketo-buildpacks/poetry@0.1.2 ========
[INFO]     [creator]     pyproject.toml must include [tool.poetry.dependencies.python], see https://python-poetry.org/docs/pyproject/#dependencies-and-dev-dependencies
[INFO]     [creator]     err:  paketo-buildpacks/poetry@0.1.2 (1)
[INFO]     [creator]     6 of 21 buildpacks participating
[INFO]     [creator]     paketo-buildpacks/ca-certificates   3.1.0
[INFO]     [creator]     paketo-buildpacks/bellsoft-liberica 9.2.0
[INFO]     [creator]     paketo-buildpacks/syft              1.10.0
[INFO]     [creator]     paketo-buildpacks/executable-jar    6.1.0
[INFO]     [creator]     paketo-buildpacks/dist-zip          5.2.0
[INFO]     [creator]     paketo-buildpacks/spring-boot       5.8.0
[INFO]     [creator]     ===> ANALYZING
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/ca-certificates:helper" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/bellsoft-liberica:helper" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/bellsoft-liberica:java-security-properties" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/bellsoft-liberica:jre" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/syft:syft" from cache
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/spring-boot:helper" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/spring-boot:spring-cloud-bindings" from app image
[INFO]     [creator]     Restoring metadata for "paketo-buildpacks/spring-boot:web-application-type" from app image
[INFO]     [creator]     ===> RESTORING
[INFO]     [creator]     Restoring data for "paketo-buildpacks/syft:syft" from cache
[INFO]     [creator]     ===> BUILDING
[INFO]     [creator]
[INFO]     [creator]     Paketo CA Certificates Buildpack 3.1.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/ca-certificates
[INFO]     [creator]       Launch Helper: Reusing cached layer
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]
[INFO]     [creator]     Paketo BellSoft Liberica Buildpack 9.2.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/bellsoft-liberica
[INFO]     [creator]       Build Configuration:
[INFO]     [creator]         $BP_JVM_TYPE                 JRE             the JVM type - JDK or JRE
[INFO]     [creator]         $BP_JVM_VERSION              11.*            the Java version
[INFO]     [creator]       Launch Configuration:
[INFO]     [creator]         $BPL_DEBUG_ENABLED           false           enables Java remote debugging support
[INFO]     [creator]         $BPL_DEBUG_PORT              8000            configure the remote debugging port
[INFO]     [creator]         $BPL_DEBUG_SUSPEND           false           configure whether to suspend execution until a debugger has attached
[INFO]     [creator]         $BPL_HEAP_DUMP_PATH                          write heap dumps on error to this path
[INFO]     [creator]         $BPL_JAVA_NMT_ENABLED        true            enables Java Native Memory Tracking (NMT)
[INFO]     [creator]         $BPL_JAVA_NMT_LEVEL          summary         configure level of NMT, summary or detail
[INFO]     [creator]         $BPL_JFR_ARGS                                configure custom Java Flight Recording (JFR) arguments
[INFO]     [creator]         $BPL_JFR_ENABLED             false           enables Java Flight Recording (JFR)
[INFO]     [creator]         $BPL_JMX_ENABLED             false           enables Java Management Extensions (JMX)
[INFO]     [creator]         $BPL_JMX_PORT                5000            configure the JMX port
[INFO]     [creator]         $BPL_JVM_HEAD_ROOM           0               the headroom in memory calculation
[INFO]     [creator]         $BPL_JVM_LOADED_CLASS_COUNT  35% of classes  the number of loaded classes in memory calculation
[INFO]     [creator]         $BPL_JVM_THREAD_COUNT        250             the number of threads in memory calculation
[INFO]     [creator]         $JAVA_TOOL_OPTIONS                           the JVM launch flags
[INFO]     [creator]       BellSoft Liberica JRE 11.0.14: Reusing cached layer
[INFO]     [creator]       Launch Helper: Reusing cached layer
[INFO]     [creator]       Java Security Properties: Reusing cached layer
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]
[INFO]     [creator]     Paketo Syft Buildpack 1.10.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/syft
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]
[INFO]     [creator]     Paketo Executable JAR Buildpack 6.1.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/executable-jar
[INFO]     [creator]       Class Path: Contributing to layer
[INFO]     [creator]         Writing env/CLASSPATH.delim
[INFO]     [creator]         Writing env/CLASSPATH.prepend
[INFO]     [creator]       Process types:
[INFO]     [creator]         executable-jar: java org.springframework.boot.loader.JarLauncher (direct)
[INFO]     [creator]         task:           java org.springframework.boot.loader.JarLauncher (direct)
[INFO]     [creator]         web:            java org.springframework.boot.loader.JarLauncher (direct)
[INFO]     [creator]
[INFO]     [creator]     Paketo Spring Boot Buildpack 5.8.0
[INFO]     [creator]       https://github.com/paketo-buildpacks/spring-boot
[INFO]     [creator]       Build Configuration:
[INFO]     [creator]         $BP_SPRING_CLOUD_BINDINGS_ENABLED    true   whether to contribute Spring Boot cloud bindings support
[INFO]     [creator]       Launch Configuration:
[INFO]     [creator]         $BPL_SPRING_CLOUD_BINDINGS_DISABLED  false  whether to auto-configure Spring Boot environment properties from bindings
[INFO]     [creator]         $BPL_SPRING_CLOUD_BINDINGS_ENABLED   true   Deprecated - whether to auto-configure Spring Boot environment properties from bindings
[INFO]     [creator]       Creating slices from layers index
[INFO]     [creator]         dependencies
[INFO]     [creator]         spring-boot-loader
[INFO]     [creator]         snapshot-dependencies
[INFO]     [creator]         application
[INFO]     [creator]       Launch Helper: Reusing cached layer
[INFO]     [creator]       Spring Cloud Bindings 1.8.1: Reusing cached layer
[INFO]     [creator]       Web Application Type: Reusing cached layer
[INFO]     [creator]       4 application slices
[INFO]     [creator]       Image labels:
[INFO]     [creator]         org.springframework.boot.version
[INFO]     [creator]     Warning: BOM table is deprecated in this buildpack api version, though it remains supported for backwards compatibility. Buildpack authors should write BOM information to <layer>.sbom.<ext>, launch.sbom.<ext>, or build.sbom.<ext>.
[INFO]     [creator]     ===> EXPORTING
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/ca-certificates:helper'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/bellsoft-liberica:helper'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/bellsoft-liberica:java-security-properties'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/bellsoft-liberica:jre'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/executable-jar:classpath'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/spring-boot:helper'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/spring-boot:spring-cloud-bindings'
[INFO]     [creator]     Reusing layer 'paketo-buildpacks/spring-boot:web-application-type'
[INFO]     [creator]     Reusing 5/5 app layer(s)
[INFO]     [creator]     Reusing layer 'launcher'
[INFO]     [creator]     Reusing layer 'config'
[INFO]     [creator]     Reusing layer 'process-types'
[INFO]     [creator]     Adding label 'io.buildpacks.lifecycle.metadata'
[INFO]     [creator]     Adding label 'io.buildpacks.build.metadata'
[INFO]     [creator]     Adding label 'io.buildpacks.project.metadata'
[INFO]     [creator]     Adding label 'org.springframework.boot.version'
[INFO]     [creator]     Setting default process type 'web'
[INFO]     [creator]     Saving syntifi.com/ori/ori-chains/ori-eth:0.1.0-SNAPSHOT...
[INFO]     [creator]     *** Images (13a7d9a6639e):
[INFO]     [creator]           syntifi.com/ori/ori-chains/ori-eth:0.1.0-SNAPSHOT
[INFO]     [creator]     Reusing cache layer 'paketo-buildpacks/syft:syft'
[INFO]
[INFO] Successfully built image 'syntifi.com/ori/ori-chains/ori-eth:0.1.0-SNAPSHOT'
[INFO]
[INFO] Successfully created image tag 'syntifi.com/ori/ori-chains/ori-eth:latest'
[INFO]
[INFO]
[INFO] --------------------< com.syntifi.ori:ori-frontend >--------------------
[INFO] Building ori-frontend 0.1.0-SNAPSHOT                             [10/11]
[INFO] --------------------------------[ pom ]---------------------------------
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
[INFO] --- exec-maven-plugin:3.0.0:exec (docker-build) @ ori-dashboard ---
Sending build context to Docker daemon  123.4kB
Step 1/8 : FROM apache/superset
 ---> 580d5b31cb0f
Step 2/8 : USER superset
 ---> Using cache
 ---> 2cd898e5245d
Step 3/8 : WORKDIR /app
 ---> Using cache
 ---> 1e34969bedd4
Step 4/8 : COPY --chown=1001 resources ./docker/
 ---> Using cache
 ---> 529376f8a0d1
Step 5/8 : RUN cp ./docker/config/superset_config.py ./pythonpath/
 ---> Using cache
 ---> a30ffb0a87c4
Step 6/8 : RUN cp ./docker/data/logo.png ./superset/static/assets/images/
 ---> Using cache
 ---> 245a1c1e6a31
Step 7/8 : RUN cp ./docker/data/icon.png ./superset/static/assets/images/
 ---> Using cache
 ---> 50756a413818
Step 8/8 : CMD ["sh", "./docker/entrypoint.sh"]
 ---> Using cache
 ---> 327ef9b6a97d
Successfully built 327ef9b6a97d
Successfully tagged syntifi.com/ori/ori-dashboard:0.1.0-SNAPSHOT
Successfully tagged syntifi.com/ori/ori-dashboard:latest
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO]
[INFO] com.syntifi.ori:ori 0.2.0-SNAPSHOT ................. SUCCESS [  0.002 s]
[INFO] ori-shared 0.1.0-SNAPSHOT .......................... SUCCESS [  0.384 s]
[INFO] ori-risk-metric 0.1.0-SNAPSHOT ..................... SUCCESS [  0.062 s]
[INFO] ori-api 0.2.0-SNAPSHOT ............................. SUCCESS [  5.360 s]
[INFO] ori-client 0.1.0-SNAPSHOT .......................... SUCCESS [  0.035 s]
[INFO] ori-chains 0.1.0-SNAPSHOT .......................... SUCCESS [  0.030 s]
[INFO] ori-chain-base 0.1.0-SNAPSHOT ...................... SUCCESS [  0.026 s]
[INFO] ori-cspr 0.1.0-SNAPSHOT ............................ SUCCESS [  5.262 s]
[INFO] ori-eth 0.1.0-SNAPSHOT ............................. SUCCESS [  5.211 s]
[INFO] ori-frontend 0.1.0-SNAPSHOT ........................ SUCCESS [ 22.765 s]
[INFO] ori-dashboard 0.1.0-SNAPSHOT ....................... SUCCESS [  0.106 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  39.865 s
[INFO] Finished at: 2022-03-19T15:49:57+01:00
[INFO] ------------------------------------------------------------------------