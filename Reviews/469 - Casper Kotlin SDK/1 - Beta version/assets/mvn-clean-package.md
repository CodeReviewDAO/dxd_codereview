```
yusuf@Yusuf-MacBook-Pro ~ % mvn -v
Apache Maven 3.8.5 (3599d3414f046de2324203b78ddcf9b5e4388aa0)
Maven home: /usr/local/Cellar/maven/3.8.5/libexec
Java version: 18.0.1, vendor: Homebrew, runtime: /usr/local/Cellar/openjdk/18.0.1/libexec/openjdk.jdk/Contents/Home
Default locale: en_TR, platform encoding: UTF-8
OS name: "mac os x", version: "12.3", arch: "x86_64", family: "mac"
yusuf@Yusuf-MacBook-Pro kotlin-sdk % git clone https://github.com/tqhuy2018/Casper-Kotlin-sdk
Cloning into 'Casper-Kotlin-sdk'...
remote: Enumerating objects: 1784, done.
remote: Total 1784 (delta 0), reused 0 (delta 0), pack-reused 1784
Receiving objects: 100% (1784/1784), 278.35 KiB | 1.68 MiB/s, done.
Resolving deltas: 100% (758/758), done.
yusuf@Yusuf-MacBook-Pro kotlin-sdk % cd Casper-Kotlin-sdk 
yusuf@Yusuf-MacBook-Pro Casper-Kotlin-sdk % ls
CONTRIBUTING.md	LICENSE		SECURITY.md	pom.xml		target
Docs		README.md	consoleApp.iml	src
yusuf@Yusuf-MacBook-Pro Casper-Kotlin-sdk % mvn clean package
[INFO] Scanning for projects...
[INFO] 
[INFO] -------------------------< me.hien:consoleApp >-------------------------
[INFO] Building consoleApp 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-clean-plugin/2.5/maven-clean-plugin-2.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-clean-plugin/2.5/maven-clean-plugin-2.5.pom (3.9 kB at 10 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/22/maven-plugins-22.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/22/maven-plugins-22.pom (13 kB at 303 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-clean-plugin/2.5/maven-clean-plugin-2.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-clean-plugin/2.5/maven-clean-plugin-2.5.jar (25 kB at 503 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.pom (8.1 kB at 219 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/23/maven-plugins-23.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/23/maven-plugins-23.pom (9.2 kB at 242 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.jar (30 kB at 579 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.1/maven-compiler-plugin-3.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.1/maven-compiler-plugin-3.1.pom (10 kB at 232 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.1/maven-compiler-plugin-3.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.1/maven-compiler-plugin-3.1.jar (43 kB at 976 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-maven-plugin/1.5.10/kotlin-maven-plugin-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-maven-plugin/1.5.10/kotlin-maven-plugin-1.5.10.pom (5.9 kB at 38 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-project/1.5.10/kotlin-project-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-project/1.5.10/kotlin-project-1.5.10.pom (10 kB at 274 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-maven-plugin/1.5.10/kotlin-maven-plugin-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-maven-plugin/1.5.10/kotlin-maven-plugin-1.5.10.jar (80 kB at 466 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/2.4/maven-jar-plugin-2.4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/2.4/maven-jar-plugin-2.4.pom (5.8 kB at 154 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/2.4/maven-jar-plugin-2.4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/2.4/maven-jar-plugin-2.4.jar (34 kB at 920 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/net/jemzart/jsonkraken/1.2.0/jsonkraken-1.2.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/net/jemzart/jsonkraken/1.2.0/jsonkraken-1.2.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/net/jemzart/jsonkraken/1.2.0/jsonkraken-1.2.0.pom (1.6 kB at 5.8 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.3.21/kotlin-stdlib-jdk8-1.3.21.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.3.21/kotlin-stdlib-jdk8-1.3.21.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.3.21/kotlin-stdlib-jdk8-1.3.21.pom (1.8 kB at 56 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.3.21/kotlin-stdlib-1.3.21.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.3.21/kotlin-stdlib-1.3.21.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.3.21/kotlin-stdlib-1.3.21.pom (1.8 kB at 12 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.3.21/kotlin-stdlib-common-1.3.21.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.3.21/kotlin-stdlib-common-1.3.21.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.3.21/kotlin-stdlib-common-1.3.21.pom (1.6 kB at 50 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/annotations/13.0/annotations-13.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/annotations/13.0/annotations-13.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/annotations/13.0/annotations-13.0.pom (4.9 kB at 149 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.3.21/kotlin-stdlib-jdk7-1.3.21.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.3.21/kotlin-stdlib-jdk7-1.3.21.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.3.21/kotlin-stdlib-jdk7-1.3.21.pom (1.6 kB at 50 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-test-junit5/1.5.10/kotlin-test-junit5-1.5.10.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test-junit5/1.5.10/kotlin-test-junit5-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test-junit5/1.5.10/kotlin-test-junit5-1.5.10.pom (2.1 kB at 14 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-test/1.5.10/kotlin-test-1.5.10.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test/1.5.10/kotlin-test-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test/1.5.10/kotlin-test-1.5.10.pom (1.7 kB at 54 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.5.10/kotlin-stdlib-1.5.10.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.5.10/kotlin-stdlib-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.5.10/kotlin-stdlib-1.5.10.pom (1.6 kB at 50 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.5.10/kotlin-stdlib-common-1.5.10.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.5.10/kotlin-stdlib-common-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.5.10/kotlin-stdlib-common-1.5.10.pom (1.2 kB at 37 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/jupiter/junit-jupiter-api/5.6.0/junit-jupiter-api-5.6.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-api/5.6.0/junit-jupiter-api-5.6.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-api/5.6.0/junit-jupiter-api-5.6.0.pom (3.2 kB at 97 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/junit-bom/5.6.0/junit-bom-5.6.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/junit-bom/5.6.0/junit-bom-5.6.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/junit-bom/5.6.0/junit-bom-5.6.0.pom (4.9 kB at 150 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/platform/junit-platform-commons/1.6.0/junit-platform-commons-1.6.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.6.0/junit-platform-commons-1.6.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.6.0/junit-platform-commons-1.6.0.pom (2.8 kB at 63 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/jupiter/junit-jupiter-engine/5.6.0/junit-jupiter-engine-5.6.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-engine/5.6.0/junit-jupiter-engine-5.6.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-engine/5.6.0/junit-jupiter-engine-5.6.0.pom (3.2 kB at 71 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/platform/junit-platform-engine/1.6.0/junit-platform-engine-1.6.0.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.6.0/junit-platform-engine-1.6.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.6.0/junit-platform-engine-1.6.0.pom (3.2 kB at 61 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.5.10/kotlin-stdlib-jdk8-1.5.10.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.5.10/kotlin-stdlib-jdk8-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.5.10/kotlin-stdlib-jdk8-1.5.10.pom (1.6 kB at 29 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.5.10/kotlin-stdlib-jdk7-1.5.10.pom
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.5.10/kotlin-stdlib-jdk7-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.5.10/kotlin-stdlib-jdk7-1.5.10.pom (1.4 kB at 31 kB/s)
Downloading from mavenCentral: https: //repo1.maven.org/maven2/net/jemzart/jsonkraken/1.2.0/jsonkraken-1.2.0.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-test-junit5/1.5.10/kotlin-test-junit5-1.5.10.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-test/1.5.10/kotlin-test-1.5.10.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/jupiter/junit-jupiter-api/5.6.0/junit-jupiter-api-5.6.0.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/platform/junit-platform-commons/1.6.0/junit-platform-commons-1.6.0.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/jupiter/junit-jupiter-engine/5.6.0/junit-jupiter-engine-5.6.0.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/junit/platform/junit-platform-engine/1.6.0/junit-platform-engine-1.6.0.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.5.10/kotlin-stdlib-1.5.10.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/annotations/13.0/annotations-13.0.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.5.10/kotlin-stdlib-common-1.5.10.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.5.10/kotlin-stdlib-jdk8-1.5.10.jar
Downloading from mavenCentral: https: //repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.5.10/kotlin-stdlib-jdk7-1.5.10.jar
Downloading from central: https://repo.maven.apache.org/maven2/net/jemzart/jsonkraken/1.2.0/jsonkraken-1.2.0.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test-junit5/1.5.10/kotlin-test-junit5-1.5.10.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test/1.5.10/kotlin-test-1.5.10.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-api/5.6.0/junit-jupiter-api-5.6.0.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.6.0/junit-platform-commons-1.6.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test-junit5/1.5.10/kotlin-test-junit5-1.5.10.jar (5.1 kB at 61 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-engine/5.6.0/junit-jupiter-engine-5.6.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-api/5.6.0/junit-jupiter-api-5.6.0.jar (154 kB at 647 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-commons/1.6.0/junit-platform-commons-1.6.0.jar (97 kB at 404 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.5.10/kotlin-stdlib-jdk8-1.5.10.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.6.0/junit-platform-engine-1.6.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.5.10/kotlin-stdlib-jdk8-1.5.10.jar (16 kB at 58 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.5.10/kotlin-stdlib-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/jupiter/junit-jupiter-engine/5.6.0/junit-jupiter-engine-5.6.0.jar (209 kB at 719 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/annotations/13.0/annotations-13.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/annotations/13.0/annotations-13.0.jar (18 kB at 53 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.5.10/kotlin-stdlib-common-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/platform/junit-platform-engine/1.6.0/junit-platform-engine-1.6.0.jar (174 kB at 497 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.5.10/kotlin-stdlib-jdk7-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-test/1.5.10/kotlin-test-1.5.10.jar (134 kB at 356 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/net/jemzart/jsonkraken/1.2.0/jsonkraken-1.2.0.jar (55 kB at 146 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.5.10/kotlin-stdlib-jdk7-1.5.10.jar (23 kB at 58 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.5.10/kotlin-stdlib-common-1.5.10.jar (197 kB at 448 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.5.10/kotlin-stdlib-1.5.10.jar (1.5 MB at 2.6 MB/s)
[INFO] 
[INFO] --- maven-clean-plugin:2.5:clean (default-clean) @ consoleApp ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.6/maven-plugin-api-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.6/maven-plugin-api-2.0.6.pom (1.5 kB at 45 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.6/maven-plugin-api-2.0.6.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0/plexus-utils-3.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.6/maven-plugin-api-2.0.6.jar (13 kB at 390 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0/plexus-utils-3.0.jar (226 kB at 4.3 MB/s)
[INFO] Deleting /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/target
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ consoleApp ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.6/maven-project-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.6/maven-project-2.0.6.pom (2.6 kB at 85 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.6/maven-settings-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.6/maven-settings-2.0.6.pom (2.0 kB at 67 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.6/maven-profile-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.6/maven-profile-2.0.6.pom (2.0 kB at 51 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.6/maven-artifact-manager-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.6/maven-artifact-manager-2.0.6.pom (2.6 kB at 87 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.6/maven-repository-metadata-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.6/maven-repository-metadata-2.0.6.pom (1.9 kB at 58 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.6/maven-plugin-registry-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.6/maven-plugin-registry-2.0.6.pom (1.9 kB at 56 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.pom (6.7 kB at 231 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.pom (1.9 kB at 68 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.0.6/maven-reporting-api-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.0.6/maven-reporting-api-2.0.6.pom (1.8 kB at 60 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting/2.0.6/maven-reporting-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting/2.0.6/maven-reporting-2.0.6.pom (1.4 kB at 50 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.0-alpha-7/doxia-sink-api-1.0-alpha-7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.0-alpha-7/doxia-sink-api-1.0-alpha-7.pom (424 B at 14 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia/1.0-alpha-7/doxia-1.0-alpha-7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia/1.0-alpha-7/doxia-1.0-alpha-7.pom (3.9 kB at 140 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.pom (1.7 kB at 57 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/commons-cli/commons-cli/1.0/commons-cli-1.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/commons-cli/commons-cli/1.0/commons-cli-1.0.pom (2.1 kB at 73 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.pom (2.0 kB at 61 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interactivity-api/1.0-alpha-4/plexus-interactivity-api-1.0-alpha-4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interactivity-api/1.0-alpha-4/plexus-interactivity-api-1.0-alpha-4.pom (7.1 kB at 253 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.pom (1.3 kB at 45 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.pom (5.8 kB at 193 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/17/maven-shared-components-17.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/17/maven-shared-components-17.pom (8.7 kB at 256 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.12/plexus-interpolation-1.12.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.12/plexus-interpolation-1.12.pom (889 B at 30 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.pom (2.9 kB at 51 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/10/spice-parent-10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/10/spice-parent-10.pom (3.0 kB at 100 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/3/forge-parent-3.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/3/forge-parent-3.pom (5.0 kB at 168 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.6/maven-profile-2.0.6.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.6/maven-artifact-manager-2.0.6.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.6/maven-plugin-registry-2.0.6.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.6/maven-project-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.6/maven-profile-2.0.6.jar (35 kB at 641 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.6/maven-plugin-registry-2.0.6.jar (29 kB at 425 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.0.6/maven-reporting-api-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.6/maven-artifact-manager-2.0.6.jar (57 kB at 744 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.0-alpha-7/doxia-sink-api-1.0-alpha-7.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.6/maven-project-2.0.6.jar (116 kB at 1.3 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.6/maven-repository-metadata-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.jar (152 kB at 1.6 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.jar (21 kB at 196 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.0-alpha-7/doxia-sink-api-1.0-alpha-7.jar (5.9 kB at 55 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/commons-cli/commons-cli/1.0/commons-cli-1.0.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.0.6/maven-reporting-api-2.0.6.jar (9.9 kB at 88 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interactivity-api/1.0-alpha-4/plexus-interactivity-api-1.0-alpha-4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.6/maven-repository-metadata-2.0.6.jar (24 kB at 191 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.6/maven-artifact-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.jar (14 kB at 101 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.6/maven-settings-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interactivity-api/1.0-alpha-4/plexus-interactivity-api-1.0-alpha-4.jar (13 kB at 92 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.6/maven-model-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.jar (37 kB at 253 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/commons-cli/commons-cli/1.0/commons-cli-1.0.jar (30 kB at 203 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.5/plexus-utils-2.0.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.6/maven-artifact-2.0.6.jar (87 kB at 520 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.6/maven-settings-2.0.6.jar (49 kB at 287 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.jar (10 kB at 56 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.13/plexus-interpolation-1.13.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.6/maven-model-2.0.6.jar (86 kB at 450 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.jar (6.8 kB at 34 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.jar (43 kB at 213 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.5/plexus-utils-2.0.5.jar (223 kB at 1.1 MB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.13/plexus-interpolation-1.13.jar (61 kB at 279 kB/s)
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ consoleApp ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.9/maven-plugin-api-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.9/maven-plugin-api-2.0.9.pom (1.5 kB at 52 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/2.0.9/maven-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/2.0.9/maven-2.0.9.pom (19 kB at 652 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/8/maven-parent-8.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/8/maven-parent-8.pom (24 kB at 832 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.9/maven-artifact-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.9/maven-artifact-2.0.9.pom (1.6 kB at 54 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.1/plexus-utils-1.5.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.1/plexus-utils-1.5.1.pom (2.3 kB at 85 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.9/maven-core-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.9/maven-core-2.0.9.pom (7.8 kB at 278 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.9/maven-settings-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.9/maven-settings-2.0.9.pom (2.1 kB at 74 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.9/maven-model-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.9/maven-model-2.0.9.pom (3.1 kB at 90 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.9/maven-plugin-parameter-documenter-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.9/maven-plugin-parameter-documenter-2.0.9.pom (2.0 kB at 65 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.9/maven-profile-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.9/maven-profile-2.0.9.pom (2.0 kB at 73 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.9/maven-repository-metadata-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.9/maven-repository-metadata-2.0.9.pom (1.9 kB at 68 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.9/maven-error-diagnostics-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.9/maven-error-diagnostics-2.0.9.pom (1.7 kB at 60 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.9/maven-project-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.9/maven-project-2.0.9.pom (2.7 kB at 73 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.9/maven-artifact-manager-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.9/maven-artifact-manager-2.0.9.pom (2.7 kB at 93 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.9/maven-plugin-registry-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.9/maven-plugin-registry-2.0.9.pom (2.0 kB at 73 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.9/maven-plugin-descriptor-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.9/maven-plugin-descriptor-2.0.9.pom (2.1 kB at 74 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.9/maven-monitor-2.0.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.9/maven-monitor-2.0.9.pom (1.3 kB at 48 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/1.0/maven-toolchain-1.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/1.0/maven-toolchain-1.0.pom (3.4 kB at 90 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.2/plexus-compiler-api-2.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.2/plexus-compiler-api-2.2.pom (865 B at 22 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler/2.2/plexus-compiler-2.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler/2.2/plexus-compiler-2.2.pom (3.6 kB at 98 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.8/plexus-utils-3.0.8.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.8/plexus-utils-3.0.8.pom (3.1 kB at 101 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/3.2/plexus-3.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/3.2/plexus-3.2.pom (19 kB at 646 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.2/plexus-compiler-manager-2.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.2/plexus-compiler-manager-2.2.pom (690 B at 24 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.2/plexus-compiler-javac-2.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.2/plexus-compiler-javac-2.2.pom (769 B at 23 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compilers/2.2/plexus-compilers-2.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compilers/2.2/plexus-compilers-2.2.pom (1.2 kB at 44 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-container-default/1.5.5/plexus-container-default-1.5.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-container-default/1.5.5/plexus-container-default-1.5.5.pom (2.8 kB at 74 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.2/plexus-classworlds-2.2.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.2/plexus-classworlds-2.2.2.pom (4.0 kB at 122 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/xbean/xbean-reflect/3.4/xbean-reflect-3.4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/xbean/xbean-reflect/3.4/xbean-reflect-3.4.pom (2.8 kB at 69 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/xbean/xbean/3.4/xbean-3.4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/xbean/xbean/3.4/xbean-3.4.pom (19 kB at 488 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging-api/1.1/commons-logging-api-1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging-api/1.1/commons-logging-api-1.1.pom (5.3 kB at 184 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/com/google/collections/google-collections/1.0/google-collections-1.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/com/google/collections/google-collections/1.0/google-collections-1.0.pom (2.5 kB at 83 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/com/google/google/1/google-1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/com/google/google/1/google-1.pom (1.6 kB at 40 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/3.8.2/junit-3.8.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/3.8.2/junit-3.8.2.pom (747 B at 27 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.9/maven-plugin-api-2.0.9.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.9/maven-artifact-2.0.9.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.1/plexus-utils-1.5.1.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.9/maven-core-2.0.9.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.9/maven-settings-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.9/maven-artifact-2.0.9.jar (89 kB at 1.9 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.9/maven-plugin-parameter-documenter-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.9/maven-plugin-api-2.0.9.jar (13 kB at 280 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.9/maven-profile-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.9/maven-plugin-parameter-documenter-2.0.9.jar (21 kB at 278 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.9/maven-model-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.9/maven-core-2.0.9.jar (160 kB at 2.0 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.9/maven-repository-metadata-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.9/maven-profile-2.0.9.jar (35 kB at 442 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.9/maven-error-diagnostics-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.1/plexus-utils-1.5.1.jar (211 kB at 2.3 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.9/maven-project-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.9/maven-error-diagnostics-2.0.9.jar (14 kB at 122 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.9/maven-plugin-registry-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.9/maven-model-2.0.9.jar (87 kB at 759 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.9/maven-plugin-descriptor-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.9/maven-repository-metadata-2.0.9.jar (25 kB at 210 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.9/maven-artifact-manager-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.9/maven-project-2.0.9.jar (122 kB at 923 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.9/maven-monitor-2.0.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.9/maven-plugin-registry-2.0.9.jar (29 kB at 205 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/1.0/maven-toolchain-1.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.9/maven-plugin-descriptor-2.0.9.jar (37 kB at 255 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/0.1/maven-shared-utils-0.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.9/maven-artifact-manager-2.0.9.jar (58 kB at 376 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.2/plexus-compiler-api-2.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.9/maven-monitor-2.0.9.jar (10 kB at 63 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.2/plexus-compiler-manager-2.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/1.0/maven-toolchain-1.0.jar (33 kB at 189 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.2/plexus-compiler-javac-2.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.2/plexus-compiler-api-2.2.jar (25 kB at 135 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-container-default/1.5.5/plexus-container-default-1.5.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/0.1/maven-shared-utils-0.1.jar (155 kB at 822 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.2/plexus-classworlds-2.2.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.2/plexus-compiler-manager-2.2.jar (4.6 kB at 24 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/xbean/xbean-reflect/3.4/xbean-reflect-3.4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.2/plexus-compiler-javac-2.2.jar (19 kB at 93 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/log4j/log4j/1.2.12/log4j-1.2.12.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.2/plexus-classworlds-2.2.2.jar (46 kB at 203 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging-api/1.1/commons-logging-api-1.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/xbean/xbean-reflect/3.4/xbean-reflect-3.4.jar (134 kB at 562 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/com/google/collections/google-collections/1.0/google-collections-1.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-container-default/1.5.5/plexus-container-default-1.5.5.jar (217 kB at 881 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/3.8.2/junit-3.8.2.jar
Downloaded from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging-api/1.1/commons-logging-api-1.1.jar (45 kB at 170 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/log4j/log4j/1.2.12/log4j-1.2.12.jar (358 kB at 1.3 MB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/3.8.2/junit-3.8.2.jar (121 kB at 422 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.9/maven-settings-2.0.9.jar (49 kB at 159 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/com/google/collections/google-collections/1.0/google-collections-1.0.jar (640 kB at 2.0 MB/s)
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- kotlin-maven-plugin:1.5.10:compile (compile) @ consoleApp ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0.5/maven-core-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0.5/maven-core-3.0.5.pom (5.5 kB at 195 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0.5/maven-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0.5/maven-3.0.5.pom (22 kB at 773 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.5/maven-model-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.5/maven-model-3.0.5.pom (3.8 kB at 131 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.6/plexus-utils-2.0.6.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.6/plexus-utils-2.0.6.pom (2.9 kB at 107 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0.5/maven-settings-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0.5/maven-settings-3.0.5.pom (1.8 kB at 68 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0.5/maven-settings-builder-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0.5/maven-settings-builder-3.0.5.pom (2.3 kB at 84 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0.5/maven-repository-metadata-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0.5/maven-repository-metadata-3.0.5.pom (1.9 kB at 65 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0.5/maven-artifact-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0.5/maven-artifact-3.0.5.pom (1.6 kB at 58 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0.5/maven-plugin-api-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0.5/maven-plugin-api-3.0.5.pom (2.7 kB at 99 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/2.3.0/sisu-inject-plexus-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/2.3.0/sisu-inject-plexus-2.3.0.pom (6.1 kB at 212 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-plexus/2.3.0/guice-plexus-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-plexus/2.3.0/guice-plexus-2.3.0.pom (3.8 kB at 136 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-bean/2.3.0/guice-bean-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-bean/2.3.0/guice-bean-2.3.0.pom (3.0 kB at 108 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/containers/2.3.0/containers-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/containers/2.3.0/containers-2.3.0.pom (1.2 kB at 41 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject/2.3.0/sisu-inject-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject/2.3.0/sisu-inject-2.3.0.pom (3.2 kB at 116 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-parent/2.3.0/sisu-parent-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-parent/2.3.0/sisu-parent-2.3.0.pom (11 kB at 379 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/2.3.0/sisu-inject-bean-2.3.0.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/2.3.0/sisu-inject-bean-2.3.0.pom (7.1 kB at 237 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guava/0.9.9/sisu-guava-0.9.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guava/0.9.9/sisu-guava-0.9.9.pom (1.1 kB at 39 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guava-parent/0.9.9/guava-parent-0.9.9.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guava-parent/0.9.9/guava-parent-0.9.9.pom (11 kB at 408 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0.5/maven-model-builder-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0.5/maven-model-builder-3.0.5.pom (2.5 kB at 88 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0.5/maven-aether-provider-3.0.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0.5/maven-aether-provider-3.0.5.pom (2.8 kB at 101 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.pom (1.4 kB at 51 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether/1.13.1/aether-1.13.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether/1.13.1/aether-1.13.1.pom (10 kB at 375 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.13.1/aether-spi-1.13.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.13.1/aether-spi-1.13.1.pom (1.4 kB at 52 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.13.1/aether-util-1.13.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.13.1/aether-util-1.13.1.pom (1.7 kB at 66 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.13.1/aether-impl-1.13.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.13.1/aether-impl-1.13.1.pom (2.5 kB at 95 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.4/maven-plugin-annotations-3.4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.4/maven-plugin-annotations-3.4.pom (1.6 kB at 54 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-tools/3.4/maven-plugin-tools-3.4.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-tools/3.4/maven-plugin-tools-3.4.pom (14 kB at 503 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-compiler/1.5.10/kotlin-compiler-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-compiler/1.5.10/kotlin-compiler-1.5.10.pom (1.9 kB at 59 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-script-runtime/1.5.10/kotlin-script-runtime-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-script-runtime/1.5.10/kotlin-script-runtime-1.5.10.pom (1.2 kB at 20 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-reflect/1.5.10/kotlin-reflect-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-reflect/1.5.10/kotlin-reflect-1.5.10.pom (1.4 kB at 25 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/intellij/deps/trove4j/1.0.20181211/trove4j-1.0.20181211.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/intellij/deps/trove4j/1.0.20181211/trove4j-1.0.20181211.pom (1.4 kB at 31 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler/1.5.10/kotlin-scripting-compiler-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler/1.5.10/kotlin-scripting-compiler-1.5.10.pom (2.4 kB at 8.7 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-common/1.5.10/kotlin-scripting-common-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-common/1.5.10/kotlin-scripting-common-1.5.10.pom (1.6 kB at 56 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlinx/kotlinx-coroutines-core/1.3.8/kotlinx-coroutines-core-1.3.8.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlinx/kotlinx-coroutines-core/1.3.8/kotlinx-coroutines-core-1.3.8.pom (1.5 kB at 55 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.3.71/kotlin-stdlib-1.3.71.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib/1.3.71/kotlin-stdlib-1.3.71.pom (1.8 kB at 63 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.3.71/kotlin-stdlib-common-1.3.71.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-stdlib-common/1.3.71/kotlin-stdlib-common-1.3.71.pom (1.6 kB at 55 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-js/1.5.10/kotlin-scripting-js-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-js/1.5.10/kotlin-scripting-js-1.5.10.pom (1.4 kB at 45 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-klib/1.5.10/kotlin-util-klib-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-klib/1.5.10/kotlin-util-klib-1.5.10.pom (1.6 kB at 10 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-io/1.5.10/kotlin-util-io-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-io/1.5.10/kotlin-util-io-1.5.10.pom (1.4 kB at 49 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-jvm/1.5.10/kotlin-scripting-jvm-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-jvm/1.5.10/kotlin-scripting-jvm-1.5.10.pom (1.8 kB at 61 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler-impl/1.5.10/kotlin-scripting-compiler-impl-1.5.10.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler-impl/1.5.10/kotlin-scripting-compiler-impl-1.5.10.pom (2.2 kB at 71 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.5.1/maven-compiler-plugin-3.5.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.5.1/maven-compiler-plugin-3.5.1.pom (10 kB at 327 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/28/maven-plugins-28.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/28/maven-plugins-28.pom (12 kB at 446 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.2.1/maven-reporting-api-2.2.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.2.1/maven-reporting-api-2.2.1.pom (1.9 kB at 62 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting/2.2.1/maven-reporting-2.2.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting/2.2.1/maven-reporting-2.2.1.pom (1.4 kB at 50 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.1/doxia-sink-api-1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.1/doxia-sink-api-1.1.pom (2.0 kB at 76 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia/1.1/doxia-1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia/1.1/doxia-1.1.pom (15 kB at 542 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-logging-api/1.1/doxia-logging-api-1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-logging-api/1.1/doxia-logging-api-1.1.pom (1.6 kB at 54 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/commons-cli/commons-cli/1.2/commons-cli-1.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/commons-cli/commons-cli/1.2/commons-cli-1.2.pom (8.0 kB at 275 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/11/commons-parent-11.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/11/commons-parent-11.pom (25 kB at 850 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.7/plexus-compiler-api-2.7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.7/plexus-compiler-api-2.7.pom (891 B at 30 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler/2.7/plexus-compiler-2.7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler/2.7/plexus-compiler-2.7.pom (4.9 kB at 159 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.7/plexus-compiler-manager-2.7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.7/plexus-compiler-manager-2.7.pom (711 B at 21 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.7/plexus-compiler-javac-2.7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.7/plexus-compiler-javac-2.7.pom (792 B at 27 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compilers/2.7/plexus-compilers-2.7.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compilers/2.7/plexus-compilers-2.7.pom (1.4 kB at 42 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0.5/maven-core-3.0.5.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.5/maven-model-3.0.5.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0.5/maven-settings-3.0.5.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0.5/maven-settings-builder-3.0.5.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0.5/maven-repository-metadata-3.0.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0.5/maven-settings-3.0.5.jar (47 kB at 1.3 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0.5/maven-artifact-3.0.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0.5/maven-settings-builder-3.0.5.jar (41 kB at 1.0 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0.5/maven-model-builder-3.0.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0.5/maven-repository-metadata-3.0.5.jar (30 kB at 684 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0.5/maven-aether-provider-3.0.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0.5/maven-artifact-3.0.5.jar (52 kB at 840 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.13.1/aether-spi-1.13.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0.5/maven-core-3.0.5.jar (559 kB at 6.8 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.13.1/aether-impl-1.13.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0.5/maven-aether-provider-3.0.5.jar (57 kB at 796 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.5/maven-model-3.0.5.jar (164 kB at 1.9 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.13.1/aether-util-1.13.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0.5/maven-model-builder-3.0.5.jar (151 kB at 2.0 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/2.3.0/sisu-inject-plexus-2.3.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.13.1/aether-spi-1.13.1.jar (15 kB at 166 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/2.3.0/sisu-inject-bean-2.3.0.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.13.1/aether-impl-1.13.1.jar (130 kB at 1.1 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guava/0.9.9/sisu-guava-0.9.9.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.jar (90 kB at 747 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.6/plexus-utils-2.0.6.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.13.1/aether-util-1.13.1.jar (130 kB at 1.1 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.4/plexus-classworlds-2.4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/2.3.0/sisu-inject-plexus-2.3.0.jar (204 kB at 1.6 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0.5/maven-plugin-api-3.0.5.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/2.3.0/sisu-inject-bean-2.3.0.jar (289 kB at 1.9 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.4/maven-plugin-annotations-3.4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.4/plexus-classworlds-2.4.jar (47 kB at 294 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-compiler/1.5.10/kotlin-compiler-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0.5/maven-plugin-api-3.0.5.jar (49 kB at 287 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-script-runtime/1.5.10/kotlin-script-runtime-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.6/plexus-utils-2.0.6.jar (223 kB at 1.3 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-reflect/1.5.10/kotlin-reflect-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugin-tools/maven-plugin-annotations/3.4/maven-plugin-annotations-3.4.jar (14 kB at 79 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/intellij/deps/trove4j/1.0.20181211/trove4j-1.0.20181211.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/intellij/deps/trove4j/1.0.20181211/trove4j-1.0.20181211.jar (573 kB at 1.9 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler/1.5.10/kotlin-scripting-compiler-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-script-runtime/1.5.10/kotlin-script-runtime-1.5.10.jar (42 kB at 125 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-common/1.5.10/kotlin-scripting-common-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guava/0.9.9/sisu-guava-0.9.9.jar (1.5 MB at 4.0 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlinx/kotlinx-coroutines-core/1.3.8/kotlinx-coroutines-core-1.3.8.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-reflect/1.5.10/kotlin-reflect-1.5.10.jar (3.0 MB at 6.2 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-js/1.5.10/kotlin-scripting-js-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler/1.5.10/kotlin-scripting-compiler-1.5.10.jar (403 kB at 806 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-klib/1.5.10/kotlin-util-klib-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-common/1.5.10/kotlin-scripting-common-1.5.10.jar (219 kB at 436 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-io/1.5.10/kotlin-util-io-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-io/1.5.10/kotlin-util-io-1.5.10.jar (48 kB at 89 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-jvm/1.5.10/kotlin-scripting-jvm-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-jvm/1.5.10/kotlin-scripting-jvm-1.5.10.jar (195 kB at 334 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler-impl/1.5.10/kotlin-scripting-compiler-impl-1.5.10.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlinx/kotlinx-coroutines-core/1.3.8/kotlinx-coroutines-core-1.3.8.jar (1.7 MB at 2.8 MB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.5.1/maven-compiler-plugin-3.5.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-compiler-impl/1.5.10/kotlin-scripting-compiler-impl-1.5.10.jar (310 kB at 485 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.4/commons-io-2.4.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.5.1/maven-compiler-plugin-3.5.1.jar (50 kB at 77 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.7/plexus-compiler-api-2.7.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-util-klib/1.5.10/kotlin-util-klib-1.5.10.jar (245 kB at 362 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.7/plexus-compiler-manager-2.7.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.7/plexus-compiler-api-2.7.jar (26 kB at 37 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.7/plexus-compiler-javac-2.7.jar
Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.4/commons-io-2.4.jar (185 kB at 268 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.7/plexus-compiler-manager-2.7.jar (4.7 kB at 6.6 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.7/plexus-compiler-javac-2.7.jar (19 kB at 27 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-scripting-js/1.5.10/kotlin-scripting-js-1.5.10.jar (7.8 kB at 10 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/jetbrains/kotlin/kotlin-compiler/1.5.10/kotlin-compiler-1.5.10.jar (48 MB at 28 MB/s)
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
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 4.028 s - in com.casper.sdk.getblock.GetBlockRPCTest
[INFO] Running com.casper.sdk.getpeers.GetPeersTest
First peer entry nodeId: tls:0097..b253 and address: 18.163.249.168:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.541 s - in com.casper.sdk.getpeers.GetPeersTest
[INFO] Running com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
Error get block with too big height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.036 s - in com.casper.sdk.getblocktransfer.GetBlockTransferRPCTest
[INFO] Running com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.671 s - in com.casper.sdk.era.GetEraBySwitchBlockRPCTest
[INFO] Running com.casper.sdk.getstateroothash.GetStateRootHashTest
Error Get State Root Hash,  invalid parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.008 s - in com.casper.sdk.getstateroothash.GetStateRootHashTest
[INFO] Running com.casper.sdk.getauction.GetAuctionInfoRPCTest
Error get auction information with wrong block height
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 19.065 s - in com.casper.sdk.getauction.GetAuctionInfoRPCTest
[INFO] Running com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
Error with wrong state root hash
Error wrong DictionayIdentifier parameter
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 3.128 s - in com.casper.sdk.getdictionary.GetDictionaryItemRPCTest
[INFO] Running com.casper.sdk.getstatus.GetStatusRPCTest
First peer entry node_id:  tls:0097..b253 and address: 18.163.249.168:35000
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.529 s - in com.casper.sdk.getstatus.GetStatusRPCTest
[INFO] Running com.casper.sdk.getitem.GetItemRPCTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 4.311 s - in com.casper.sdk.getitem.GetItemRPCTest
[INFO] Running com.casper.sdk.getbalance.GetBalanceRPCTest
Error get balance with wrong state root hash
Error get balance with wrong purse uref
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.323 s - in com.casper.sdk.getbalance.GetBalanceRPCTest
[INFO] Running com.casper.sdk.getdeploy.GetDeployRPCTest
Error IllegalArgumentException caught
Error IllegalArgumentException caught
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 4.833 s - in com.casper.sdk.getdeploy.GetDeployRPCTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 11, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ consoleApp ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/2.5/maven-archiver-2.5.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/2.5/maven-archiver-2.5.pom (4.5 kB at 146 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/2.1/plexus-archiver-2.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/2.1/plexus-archiver-2.1.pom (2.8 kB at 97 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/2.0.2/plexus-io-2.0.2.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/2.0.2/plexus-io-2.0.2.pom (1.7 kB at 27 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.pom (1.0 kB at 25 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/2.5/maven-archiver-2.5.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/2.1/plexus-archiver-2.1.jar
Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/2.0.2/plexus-io-2.0.2.jar
Downloading from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.1/commons-lang-2.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/2.5/maven-archiver-2.5.jar (22 kB at 79 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.jar (60 kB at 214 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/2.0.2/plexus-io-2.0.2.jar (58 kB at 161 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/2.1/plexus-archiver-2.1.jar (184 kB at 439 kB/s)
Downloaded from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.1/commons-lang-2.1.jar (208 kB at 490 kB/s)
[INFO] Building jar: /Users/yusuf/kotlin-sdk/Casper-Kotlin-sdk/target/consoleApp-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:29 min
[INFO] Finished at: 2022-05-04T16:14:19+03:00
[INFO] ------------------------------------------------------------------------
```
