``` text
[INFO] Scanning for projects...
[INFO] 
[INFO] ------------------< io.caspercommunity:camel-casper >-------------------
[INFO] Building Camel Casper blockchaine Component 3.14.2-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-source (default) @ camel-casper ---
[INFO] Source directory: D:\Devel\casper\camel-casper\src\generated\java added.
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (default) @ camel-casper ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.7:prepare-agent (default) @ camel-casper ---
[INFO] argLine set to -javaagent:C:\\Users\\oak3\\.m2\\repository\\org\\jacoco\\org.jacoco.agent\\0.8.7\\org.jacoco.agent-0.8.7-runtime.jar=destfile=D:\\Devel\\casper\\camel-casper\\target\\jacoco.exec
[INFO] 
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ camel-casper ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 3 resources
[INFO] Copying 6 resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.9.0:compile (default-compile) @ camel-casper ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- camel-package-maven-plugin:3.14.2:generate (generate) @ camel-casper ---
[INFO] No previous run data found, generating files.
[INFO] Building index...
[INFO] Updated org/apache/camel/component/casper/CasperEndpointUriFactory.java
[INFO] Updated org/apache/camel/component/casper/CasperProducerInvokeOnHeaderFactory.java
[INFO] Validation complete
[WARNING] Cannot find markers in file D:\Devel\casper\camel-casper\src\main\docs\casper-component.adoc
[WARNING] Add the following markers
[WARNING] 	// component-configure options: START
[WARNING] 	// component-configure options: END
[WARNING] Cannot find markers in file D:\Devel\casper\camel-casper\src\main\docs\casper-component.adoc
[WARNING] Add the following markers
[WARNING] 	// component options: START
[WARNING] 	// component options: END
[WARNING] Cannot find markers in file D:\Devel\casper\camel-casper\src\main\docs\casper-component.adoc
[WARNING] Add the following markers
[WARNING] 	// endpoint options: START
[WARNING] 	// endpoint options: END
[INFO] 
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ camel-casper ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] skip non existing resourceDirectory D:\Devel\casper\camel-casper\src\test\resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.9.0:testCompile (default-testCompile) @ camel-casper ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 55 source files to D:\Devel\casper\camel-casper\target\test-classes
[INFO] /D:/Devel/casper/camel-casper/src/test/java/org/apache/camel/component/casper/CasperTestSupport.java: D:\Devel\casper\camel-casper\src\test\java\org\apache\camel\component\casper\CasperTestSupport.java uses or overrides a deprecated API.
[INFO] /D:/Devel/casper/camel-casper/src/test/java/org/apache/camel/component/casper/CasperTestSupport.java: Recompile with -Xlint:deprecation for details.
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.0:test (default-test) @ camel-casper ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running org.apache.camel.component.casper.consumer.CasperConsumerComponentTest
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.105 s - in org.apache.camel.component.casper.consumer.CasperConsumerComponentTest
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test
[                          main] KotlinDetector                 INFO  Kotlin reflection implementation not found at runtime, related features won't be available.

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:40.371  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:40.372  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:40.875  WARN 41196 --- [kground-preinit] o.s.h.c.j.Jackson2ObjectMapperBuilder    : For Jackson Kotlin classes support please add "com.fasterxml.jackson.module:jackson-module-kotlin" to the classpath
2022-03-28 14:57:42.696  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:42.732  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:42.732  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:42.751  INFO 41196 --- [           main] o.a.c.c.AprLifecycleListener             : The APR based Apache Tomcat Native library which allows optimal performance in production environments was not found on the java.library.path: [C:\Program Files\Amazon Corretto\jdk1.8.0_292\jre\bin;C:\WINDOWS\Sun\Java\bin;C:\WINDOWS\system32;C:\WINDOWS;C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\wbin;C:\PROGRA~1\AMAZON~1\jdk11.0.7_10\bin;D:\Python\Python310\Scripts\;D:\Python\Python310\;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\iCLS\;C:\Program Files\Intel\Intel(R) Management Engine Components\iCLS\;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files\NVIDIA Corporation\NVIDIA NvDLISR;C:\Program Files (x86)\NVIDIA Corporation\PhysX\Common;D:\Devel\HaxeToolkit\haxe;D:\Devel\HaxeToolkit\neko;C:\Program Files\dotnet\;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program Files (x86)\dotnet\;C:\ProgramData\chocolatey\bin;C:\Program Files\gettext-iconv\bin;C:\Program Files\Microsoft VS Code\bin;C:\Program Files\nodejs\;C:\Program Files\Go\bin;C:\Program Files (x86)\gnupg\bin;C:\Program Files\Microsoft SQL Server\150\Tools\Binn\;C:\Program Files (x86)\Gpg4win\..\GnuPG\bin;C:\Program Files\Git\cmd;;C:\Program Files\Docker\Docker\resources\bin;C:\ProgramData\DockerDesktop\version-bin;C:\Users\oak3\AppData\Local\pnpm;C:\Users\oak3\.cargo\bin;D:\Devel\apps\apache-maven\bin;D:\devel\apps\gradle\current\bin;D:\Devel\apps\java\scripts;C:\Users\oak3\AppData\Roaming\npm;D:\Devel\apps\mandrel\current\bin;C:\Program Files\JetBrains\IntelliJ IDEA 2021.3.2\bin;C:\Program Files\Microsoft Visual Studio\2022\Enterprise\VC\Tools\MSVC\14.30.30705\bin\Hostx64\x64;C:\Program Files\Microsoft Visual Studio\2022\Enterprise\VC\Auxiliary\Build\;D:\Devel\apps\mandrel\mandrel-java11-22.0.0.2-Final\bin;;D:\Devel\apps\java\jdk-11.0.2\bin;;C:\Program Files\JetBrains\PyCharm 2021.3.2\bin;;C:\Program Files\JetBrains\CLion 2021.3.3\bin;;C:\Program Files\JetBrains\DataGrip 2021.3.4\bin;;C:\Program Files\JetBrains\GoLand 2021.3.3\bin;;D:\Devel\apps\CMake\bin;.]
2022-03-28 14:57:42.893  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:42.893  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 2461 ms
2022-03-28 14:57:43.015  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:43.573  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:43.578  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 3.724 seconds (JVM running for 6.134)
2022-03-28 14:57:43.859  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:43.863  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test)
2022-03-28 14:57:43.863  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:44.472  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-28 14:57:44.475  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:44.475  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route4 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:44.475  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-4) started in 549ms (build:7ms init:37ms start:505ms)
2022-03-28 14:57:44.478  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:44.727  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:44.727  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:44.740  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 12 ms
2022-03-28 14:57:44.805  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:44.810  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:44.899  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:44.901  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:44.901  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test)
2022-03-28 14:57:44.902  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 424ms (424 millis)
2022-03-28 14:57:44.902  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:44.904  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-4) shutting down (timeout:10s)
2022-03-28 14:57:44.910  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:44.911  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
2022-03-28 14:57:44.912  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 3822 milliseconds before reconnecting...
2022-03-28 14:57:44.915  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:44.915  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route4 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:44.918  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-4) shutdown in 14ms (uptime:948ms)
2022-03-28 14:57:44.922  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 6.043 s - in org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:45.802  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:45.802  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:46.071  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:46.072  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:46.072  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:46.080  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:46.081  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 275 ms
2022-03-28 14:57:46.101  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:46.229  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:46.230  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.471 seconds (JVM running for 8.786)
2022-03-28 14:57:46.234  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:46.234  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test)
2022-03-28 14:57:46.234  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:46.254  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/deploys
2022-03-28 14:57:46.255  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:46.255  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route5 (casper://http://localhost:8080/events/deploys)
2022-03-28 14:57:46.255  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-5) started in 14ms (build:6ms init:5ms start:3ms)
2022-03-28 14:57:46.256  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:46.267  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:46.267  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:46.270  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 3 ms
2022-03-28 14:57:46.274  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:46.277  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:46.287  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:46.295  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:46.296  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test)
2022-03-28 14:57:46.296  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 39ms (39 millis)
2022-03-28 14:57:46.296  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:46.296  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-5) shutting down (timeout:10s)
2022-03-28 14:57:46.309  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:46.310  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route5 (casper://http://localhost:8080/events/deploys)
2022-03-28 14:57:46.310  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-5) shutdown in 14ms (uptime:58ms)
2022-03-28 14:57:46.311  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:46.317  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:46.317  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 3392 milliseconds before reconnecting...
2022-03-28 14:57:46.318  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.433 s - in org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_EXPIRED_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:47.246  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:47.246  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:47.497  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:47.499  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:47.499  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:47.510  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:47.510  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 259 ms
2022-03-28 14:57:47.523  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:47.662  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:47.663  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.459 seconds (JVM running for 10.219)
2022-03-28 14:57:47.665  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:47.665  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_EXPIRED_Event_Test)
2022-03-28 14:57:47.665  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:47.685  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-28 14:57:47.686  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:47.686  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route6 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:47.686  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-6) started in 15ms (build:8ms init:5ms start:2ms)
2022-03-28 14:57:47.686  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:47.691  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:47.691  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:47.694  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 3 ms
2022-03-28 14:57:47.697  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:47.707  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:47.727  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:47.727  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:47.727  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_EXPIRED_Event_Test)
2022-03-28 14:57:47.727  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 41ms (41 millis)
2022-03-28 14:57:47.727  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:47.727  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-6) shutting down (timeout:10s)
2022-03-28 14:57:47.737  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:47.738  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 4700 milliseconds before reconnecting...
2022-03-28 14:57:47.738  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:47.738  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route6 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:47.739  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
2022-03-28 14:57:47.740  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-6) shutdown in 13ms (uptime:56ms)
2022-03-28 14:57:47.743  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.439 s - in org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_EXPIRED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:48.685  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:48.686  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:48.857  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:48.859  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:48.859  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:48.870  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:48.870  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 182 ms
2022-03-28 14:57:48.883  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:48.982  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:48.983  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.333 seconds (JVM running for 11.539)
2022-03-28 14:57:48.985  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:48.985  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test)
2022-03-28 14:57:48.985  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:49.004  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-28 14:57:49.004  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:49.004  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route7 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:49.004  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-7) started in 13ms (build:6ms init:5ms start:2ms)
2022-03-28 14:57:49.005  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:49.008  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:49.008  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:49.010  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 2 ms
2022-03-28 14:57:49.012  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:49.015  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:49.024  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:49.024  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:49.024  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test)
2022-03-28 14:57:49.024  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 19ms (19 millis)
2022-03-28 14:57:49.025  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:49.025  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-7) shutting down (timeout:10s)
2022-03-28 14:57:49.026  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:49.026  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route7 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:49.027  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-7) shutdown in 1ms (uptime:24ms)
2022-03-28 14:57:49.028  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:49.036  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:49.037  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 5824 milliseconds before reconnecting...
2022-03-28 14:57:49.037  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
2022-03-28 14:57:49.782  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 8210 milliseconds before reconnecting...
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.141 s - in org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_FAULT_Event_Test
2022-03-28 14:57:49.782 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.SocketException: Connection reset
	at java.net.SocketInputStream.read(SocketInputStream.java:210) ~[?:1.8.0_292]
	at java.net.SocketInputStream.read(SocketInputStream.java:141) ~[?:1.8.0_292]
	at okio.InputStreamSource.read(JvmOkio.kt:90) ~[okio-2.5.0.jar:?]
	at okio.AsyncTimeout$source$1.read(AsyncTimeout.kt:129) ~[okio-2.5.0.jar:?]
	at okio.RealBufferedSource.indexOf(RealBufferedSource.kt:449) ~[okio-2.5.0.jar:?]
	at okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.kt:333) ~[okio-2.5.0.jar:?]
	at okhttp3.internal.http1.Http1ExchangeCodec.readHeaderLine(Http1ExchangeCodec.kt:207) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http1.Http1ExchangeCodec.readResponseHeaders(Http1ExchangeCodec.kt:178) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.Exchange.readResponseHeaders(Exchange.kt:106) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.CallServerInterceptor.intercept(CallServerInterceptor.kt:79) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:34) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.SocketException: Software caused connection abort: recv failed
		at java.net.SocketInputStream.socketRead0(Native Method) ~[?:1.8.0_292]
		at java.net.SocketInputStream.socketRead(SocketInputStream.java:116) ~[?:1.8.0_292]
		at java.net.SocketInputStream.read(SocketInputStream.java:171) ~[?:1.8.0_292]
		at java.net.SocketInputStream.read(SocketInputStream.java:141) ~[?:1.8.0_292]
		at okio.InputStreamSource.read(JvmOkio.kt:90) ~[okio-2.5.0.jar:?]
		at okio.AsyncTimeout$source$1.read(AsyncTimeout.kt:129) ~[okio-2.5.0.jar:?]
		at okio.RealBufferedSource.indexOf(RealBufferedSource.kt:449) ~[okio-2.5.0.jar:?]
		at okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.kt:333) ~[okio-2.5.0.jar:?]
		at okhttp3.internal.http1.Http1ExchangeCodec.readHeaderLine(Http1ExchangeCodec.kt:207) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http1.Http1ExchangeCodec.readResponseHeaders(Http1ExchangeCodec.kt:178) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.Exchange.readResponseHeaders(Exchange.kt:106) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.CallServerInterceptor.intercept(CallServerInterceptor.kt:79) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:34) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]


  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:49.826  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:49.826  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:49.976  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:49.978  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:49.978  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:49.988  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:49.989  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 160 ms
2022-03-28 14:57:50.008  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:50.156  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:50.156  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.358 seconds (JVM running for 12.713)
2022-03-28 14:57:50.163  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:50.164  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_FAULT_Event_Test)
2022-03-28 14:57:50.164  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:50.204  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-28 14:57:50.205  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:50.205  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route8 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:50.205  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-8) started in 28ms (build:11ms init:15ms start:2ms)
2022-03-28 14:57:50.205  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:50.209  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:50.209  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:50.212  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 3 ms
2022-03-28 14:57:50.214  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:50.219  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:50.236  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:50.237  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:50.237  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_FAULT_Event_Test)
2022-03-28 14:57:50.237  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 32ms (32 millis)
2022-03-28 14:57:50.237  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:50.237  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:50.237  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 3797 milliseconds before reconnecting...
2022-03-28 14:57:50.238  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-8) shutting down (timeout:10s)
2022-03-28 14:57:50.238  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
2022-03-28 14:57:50.242  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:50.243  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route8 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:50.243  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-8) shutdown in 5ms (uptime:40ms)
2022-03-28 14:57:50.244  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:50.284  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 7062 milliseconds before reconnecting...
2022-03-28 14:57:50.285 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.SocketException: Software caused connection abort: recv failed
	at java.net.SocketInputStream.socketRead0(Native Method) ~[?:1.8.0_292]
	at java.net.SocketInputStream.socketRead(SocketInputStream.java:116) ~[?:1.8.0_292]
	at java.net.SocketInputStream.read(SocketInputStream.java:171) ~[?:1.8.0_292]
	at java.net.SocketInputStream.read(SocketInputStream.java:141) ~[?:1.8.0_292]
	at okio.InputStreamSource.read(JvmOkio.kt:90) ~[okio-2.5.0.jar:?]
	at okio.AsyncTimeout$source$1.read(AsyncTimeout.kt:129) ~[okio-2.5.0.jar:?]
	at okio.RealBufferedSource.indexOf(RealBufferedSource.kt:449) ~[okio-2.5.0.jar:?]
	at okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.kt:333) ~[okio-2.5.0.jar:?]
	at okhttp3.internal.http1.Http1ExchangeCodec.readHeaderLine(Http1ExchangeCodec.kt:207) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http1.Http1ExchangeCodec.readResponseHeaders(Http1ExchangeCodec.kt:178) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.Exchange.readResponseHeaders(Exchange.kt:106) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.CallServerInterceptor.intercept(CallServerInterceptor.kt:79) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:34) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.SocketException: Connection reset
		at java.net.SocketInputStream.read(SocketInputStream.java:210) ~[?:1.8.0_292]
		at java.net.SocketInputStream.read(SocketInputStream.java:141) ~[?:1.8.0_292]
		at okio.InputStreamSource.read(JvmOkio.kt:90) ~[okio-2.5.0.jar:?]
		at okio.AsyncTimeout$source$1.read(AsyncTimeout.kt:129) ~[okio-2.5.0.jar:?]
		at okio.RealBufferedSource.indexOf(RealBufferedSource.kt:449) ~[okio-2.5.0.jar:?]
		at okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.kt:333) ~[okio-2.5.0.jar:?]
		at okhttp3.internal.http1.Http1ExchangeCodec.readHeaderLine(Http1ExchangeCodec.kt:207) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http1.Http1ExchangeCodec.readResponseHeaders(Http1ExchangeCodec.kt:178) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.Exchange.readResponseHeaders(Exchange.kt:106) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.CallServerInterceptor.intercept(CallServerInterceptor.kt:79) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:34) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]

[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.227 s - in org.apache.camel.component.casper.consumer.ConsumerTest_FAULT_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:51.065  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:51.065  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:51.215  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:51.216  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:51.217  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:51.227  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:51.227  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 160 ms
2022-03-28 14:57:51.237  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:51.343  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:51.343  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.307 seconds (JVM running for 13.9)
2022-03-28 14:57:51.346  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:51.346  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test)
2022-03-28 14:57:51.346  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:51.371  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/sigs
2022-03-28 14:57:51.372  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:51.372  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route9 (casper://http://localhost:8080/events/sigs)
2022-03-28 14:57:51.372  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-9) started in 16ms (build:8ms init:6ms start:2ms)
2022-03-28 14:57:51.372  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:51.380  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:51.380  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:51.382  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 2 ms
2022-03-28 14:57:51.384  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:51.385  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:51.404  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:51.404  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:51.404  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test)
2022-03-28 14:57:51.404  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 32ms (32 millis)
2022-03-28 14:57:51.404  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:51.405  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-9) shutting down (timeout:10s)
2022-03-28 14:57:51.405  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:51.405  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 3145 milliseconds before reconnecting...
2022-03-28 14:57:51.410  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
2022-03-28 14:57:51.410  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:51.410  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route9 (casper://http://localhost:8080/events/sigs)
2022-03-28 14:57:51.411  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-9) shutdown in 6ms (uptime:41ms)
2022-03-28 14:57:51.412  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.171 s - in org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-28 14:57:52.238  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 41196 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-28 14:57:52.238  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-28 14:57:52.375  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-28 14:57:52.376  INFO 41196 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-28 14:57:52.376  INFO 41196 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-28 14:57:52.383  INFO 41196 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-28 14:57:52.383  INFO 41196 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 144 ms
2022-03-28 14:57:52.395  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:52.480  INFO 41196 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-28 14:57:52.480  INFO 41196 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.27 seconds (JVM running for 15.037)
2022-03-28 14:57:52.482  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:52.482  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test)
2022-03-28 14:57:52.482  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:52.499  INFO 41196 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-28 14:57:52.500  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:52.500  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route10 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:52.500  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-10) started in 13ms (build:6ms init:5ms start:2ms)
2022-03-28 14:57:52.500  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-28 14:57:52.503  INFO 41196 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-28 14:57:52.503  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-28 14:57:52.505  INFO 41196 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 2 ms
2022-03-28 14:57:52.506  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-28 14:57:52.507  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been opened
2022-03-28 14:57:52.517  INFO 41196 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-28 14:57:52.518  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:52.518  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test)
2022-03-28 14:57:52.518  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 18ms (18 millis)
2022-03-28 14:57:52.518  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:52.518  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-10) shutting down (timeout:10s)
2022-03-28 14:57:52.521  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:52.521  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route10 (casper://http://localhost:8080/events/main)
2022-03-28 14:57:52.522  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-10) shutdown in 4ms (uptime:24ms)
2022-03-28 14:57:52.523  INFO 41196 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
2022-03-28 14:57:52.523  WARN 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-28 14:57:52.524  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 4378 milliseconds before reconnecting...
2022-03-28 14:57:52.531  INFO 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : The event stream has been closed
2022-03-28 14:57:53.338  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 8136 milliseconds before reconnecting...
2022-03-28 14:57:53.338 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.SocketException: Connection reset
	at java.net.SocketInputStream.read(SocketInputStream.java:210) ~[?:1.8.0_292]
	at java.net.SocketInputStream.read(SocketInputStream.java:141) ~[?:1.8.0_292]
	at okio.InputStreamSource.read(JvmOkio.kt:90) ~[okio-2.5.0.jar:?]
	at okio.AsyncTimeout$source$1.read(AsyncTimeout.kt:129) ~[okio-2.5.0.jar:?]
	at okio.RealBufferedSource.indexOf(RealBufferedSource.kt:449) ~[okio-2.5.0.jar:?]
	at okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.kt:333) ~[okio-2.5.0.jar:?]
	at okhttp3.internal.http1.Http1ExchangeCodec.readHeaderLine(Http1ExchangeCodec.kt:207) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http1.Http1ExchangeCodec.readResponseHeaders(Http1ExchangeCodec.kt:178) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.Exchange.readResponseHeaders(Exchange.kt:106) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.CallServerInterceptor.intercept(CallServerInterceptor.kt:79) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:34) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.SocketException: Software caused connection abort: recv failed
		at java.net.SocketInputStream.socketRead0(Native Method) ~[?:1.8.0_292]
		at java.net.SocketInputStream.socketRead(SocketInputStream.java:116) ~[?:1.8.0_292]
		at java.net.SocketInputStream.read(SocketInputStream.java:171) ~[?:1.8.0_292]
		at java.net.SocketInputStream.read(SocketInputStream.java:141) ~[?:1.8.0_292]
		at okio.InputStreamSource.read(JvmOkio.kt:90) ~[okio-2.5.0.jar:?]
		at okio.AsyncTimeout$source$1.read(AsyncTimeout.kt:129) ~[okio-2.5.0.jar:?]
		at okio.RealBufferedSource.indexOf(RealBufferedSource.kt:449) ~[okio-2.5.0.jar:?]
		at okio.RealBufferedSource.readUtf8LineStrict(RealBufferedSource.kt:333) ~[okio-2.5.0.jar:?]
		at okhttp3.internal.http1.Http1ExchangeCodec.readHeaderLine(Http1ExchangeCodec.kt:207) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http1.Http1ExchangeCodec.readResponseHeaders(Http1ExchangeCodec.kt:178) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.Exchange.readResponseHeaders(Exchange.kt:106) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.CallServerInterceptor.intercept(CallServerInterceptor.kt:79) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:34) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]

[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.139 s - in org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerComponentTest
2022-03-28 14:57:53.366 ERROR 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Error starting CamelContext (camel-11) due to exception thrown: Failed to start route route11 because of null

org.apache.camel.FailedToStartRouteException: Failed to start route route11 because of null
	at org.apache.camel.impl.engine.RouteService.warmUp(RouteService.java:123) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.InternalRouteStartupManager.doWarmUpRoutes(InternalRouteStartupManager.java:306) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.InternalRouteStartupManager.safelyStartRouteServices(InternalRouteStartupManager.java:189) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.InternalRouteStartupManager.doStartOrResumeRoutes(InternalRouteStartupManager.java:147) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.AbstractCamelContext.doStartCamel(AbstractCamelContext.java:3300) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.AbstractCamelContext.doStartContext(AbstractCamelContext.java:2952) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.AbstractCamelContext.doStart(AbstractCamelContext.java:2903) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.AbstractCamelContext.start(AbstractCamelContext.java:2587) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.DefaultCamelContext.start(DefaultCamelContext.java:253) ~[camel-core-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerComponentTest.lambda$testWithUnsuportedOperation$1(CasperProducerComponentTest.java:43) ~[test-classes/:?]
	at org.junit.Assert.assertThrows(Assert.java:1001) ~[junit-4.13.2.jar:4.13.2]
	at org.junit.Assert.assertThrows(Assert.java:981) ~[junit-4.13.2.jar:4.13.2]
	at org.apache.camel.component.casper.producer.CasperProducerComponentTest.testWithUnsuportedOperation(CasperProducerComponentTest.java:43) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]
Caused by: org.apache.camel.RuntimeCamelException: java.lang.UnsupportedOperationException: Operation 'test' not supported by casper producer
	at org.apache.camel.RuntimeCamelException.wrapRuntimeCamelException(RuntimeCamelException.java:51) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.ChildServiceSupport.start(ChildServiceSupport.java:67) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:130) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultChannel.doStart(DefaultChannel.java:126) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:116) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:130) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.doStart(Pipeline.java:221) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.processor.DelegateAsyncProcessor.doStart(DelegateAsyncProcessor.java:89) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.RouteService.startChildServices(RouteService.java:396) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.RouteService.doWarmUp(RouteService.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.RouteService.warmUp(RouteService.java:121) ~[camel-base-engine-3.14.2.jar:3.14.2]
	... 76 more
Caused by: java.lang.UnsupportedOperationException: Operation 'test' not supported by casper producer
	at org.apache.camel.component.casper.CasperEndPoint.createProducer(CasperEndPoint.java:96) ~[classes/:?]
	at org.apache.camel.support.DefaultEndpoint.createAsyncProducer(DefaultEndpoint.java:197) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.doStart(SendProcessor.java:245) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:130) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler.doStart(RedeliveryErrorHandler.java:1655) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.support.ChildServiceSupport.start(ChildServiceSupport.java:60) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:130) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultChannel.doStart(DefaultChannel.java:126) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:116) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:130) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.doStart(Pipeline.java:221) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.processor.DelegateAsyncProcessor.doStart(DelegateAsyncProcessor.java:89) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.BaseService.start(BaseService.java:119) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.support.service.ServiceHelper.startService(ServiceHelper.java:113) ~[camel-api-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.RouteService.startChildServices(RouteService.java:396) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.RouteService.doWarmUp(RouteService.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.RouteService.warmUp(RouteService.java:121) ~[camel-base-engine-3.14.2.jar:3.14.2]
	... 76 more

2022-03-28 14:57:53.369  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-11) shutting down (timeout:45s)
2022-03-28 14:57:53.369  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:53.369  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route11 (direct://start)
2022-03-28 14:57:53.370  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-11) shutdown in 1ms (uptime:5ms)
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.045 s - in org.apache.camel.component.casper.producer.CasperProducerComponentTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest
2022-03-28 14:57:53.384  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:53.384  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-28 14:57:53.385  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:53.404  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:53.404  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route13 (direct://start)
2022-03-28 14:57:53.404  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-13) started in 15ms (build:2ms init:4ms start:9ms)
2022-03-28 14:57:54.260  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.260  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-28 14:57:54.260  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 856ms (856 millis)
2022-03-28 14:57:54.260  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.260  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-13) shutting down (timeout:10s)
2022-03-28 14:57:54.261  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:54.262  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route13 (direct://start)
2022-03-28 14:57:54.262  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-13) shutdown in 2ms (uptime:867ms)
2022-03-28 14:57:54.264  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.264  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-28 14:57:54.264  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.278  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.278  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route14 (direct://start)
2022-03-28 14:57:54.278  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-14) started in 9ms (build:3ms init:4ms start:2ms)
2022-03-28 14:57:54.280 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 27C165D07AA8F96-0000000000000000 on ExchangeId: 27C165D07AA8F96-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: stateRootHash parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route14           ] [route14           ] [                                                                              ] [         0]
	...
[route14           ] [to11              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: stateRootHash parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountBalance(CasperProducer.java:410) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:20) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest.testCallWithout_STATE_ROOT_HASH_Parameter(CasperProducerWith_ACCOUNT_BALANCE_OperationTest.java:77) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:57:54.281  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.281  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-28 14:57:54.281  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 3ms (3 millis)
2022-03-28 14:57:54.281  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.281  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-14) shutting down (timeout:10s)
2022-03-28 14:57:54.283  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
stateRootHash parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]  stateroothash parameter is required   with endpoint operation account_balance
2022-03-28 14:57:54.283  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route14 (direct://start)
2022-03-28 14:57:54.283  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-14) shutdown in 2ms (uptime:7ms)
2022-03-28 14:57:54.285  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.285  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_UREF_PURSE_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-28 14:57:54.285  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.300  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.300  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route15 (direct://start)
2022-03-28 14:57:54.301  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-15) started in 11ms (build:4ms init:5ms start:2ms)
2022-03-28 14:57:54.301 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: BE34F7590ACF127-0000000000000000 on ExchangeId: BE34F7590ACF127-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: purseUref parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route15           ] [route15           ] [                                                                              ] [         0]
	...
[route15           ] [to12              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: purseUref parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountBalance(CasperProducer.java:414) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:20) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest.testCallWithout_UREF_PURSE_KEY_Parameter(CasperProducerWith_ACCOUNT_BALANCE_OperationTest.java:56) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:57:54.302  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.303  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_UREF_PURSE_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-28 14:57:54.303  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:57:54.303  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.303  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-15) shutting down (timeout:10s)
2022-03-28 14:57:54.313  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:54.313  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route15 (direct://start)
2022-03-28 14:57:54.314  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-15) shutdown in 11ms (uptime:15ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.935 s - in org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest
2022-03-28 14:57:54.318  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.318  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.318  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.344  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.345  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route16 (direct://start)
2022-03-28 14:57:54.345  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-16) started in 19ms (build:9ms init:9ms start:1ms)
2022-03-28 14:57:54.642  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.642  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.643  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 297ms (297 millis)
2022-03-28 14:57:54.643  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.643  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-16) shutting down (timeout:10s)
2022-03-28 14:57:54.644  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:54.644  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route16 (direct://start)
2022-03-28 14:57:54.644  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-16) shutdown in 1ms (uptime:300ms)
2022-03-28 14:57:54.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.657  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.657  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route17 (direct://start)
2022-03-28 14:57:54.657  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-17) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:57:54.915  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.915  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.915  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 258ms (258 millis)
2022-03-28 14:57:54.915  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.915  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-17) shutting down (timeout:10s)
2022-03-28 14:57:54.916  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:54.916  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route17 (direct://start)
2022-03-28 14:57:54.916  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-17) shutdown in 1ms (uptime:260ms)
2022-03-28 14:57:54.917  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.918  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.918  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.930  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.930  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route18 (direct://start)
2022-03-28 14:57:54.930  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-18) started in 7ms (build:3ms init:3ms start:1ms)
2022-03-28 14:57:54.931 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 1CF0BEB3CCC1F0E-0000000000000000 on ExchangeId: 1CF0BEB3CCC1F0E-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: publicKey parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route18           ] [route18           ] [                                                                              ] [         0]
	...
[route18           ] [to15              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: publicKey parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountInfo(CasperProducer.java:217) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:22) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest.testCallWithout_PUBLIC_KEY_Parameters(CasperProducerWith_ACCOUNT_INFO_OperationTest.java:61) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:57:54.932  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.932  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.932  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:57:54.932  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.932  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-18) shutting down (timeout:10s)
2022-03-28 14:57:54.933  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:54.933  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route18 (direct://start)
2022-03-28 14:57:54.933  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-18) shutdown in 1ms (uptime:4ms)
2022-03-28 14:57:54.934  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.935  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithOnly_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.935  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.946  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.946  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route19 (direct://start)
2022-03-28 14:57:54.946  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-19) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:57:54.947 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: ECBD9D264C8C2B8-0000000000000000 on ExchangeId: ECBD9D264C8C2B8-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route19           ] [route19           ] [                                                                              ] [         0]
	...
[route19           ] [to16              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountInfo(CasperProducer.java:226) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:22) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest.testCallWithOnly_PUBLIC_KEY_Parameters(CasperProducerWith_ACCOUNT_INFO_OperationTest.java:77) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:57:54.948  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.948  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithOnly_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-28 14:57:54.948  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:57:54.948  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.949  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-19) shutting down (timeout:10s)
2022-03-28 14:57:54.950  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:54.951  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route19 (direct://start)
2022-03-28 14:57:54.951  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-19) shutdown in 2ms (uptime:6ms)
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.643 s - in org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest
2022-03-28 14:57:54.954  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.954  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-28 14:57:54.954  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:54.966  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:54.966  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route20 (direct://start)
2022-03-28 14:57:54.966  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-20) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:57:57.637  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:57.637  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-28 14:57:57.637  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2s670ms (2670 millis)
2022-03-28 14:57:57.637  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:57.637  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-20) shutting down (timeout:10s)
2022-03-28 14:57:57.639  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:57.639  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route20 (direct://start)
2022-03-28 14:57:57.640  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-20) shutdown in 3ms (uptime:2s675ms)
2022-03-28 14:57:57.642  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:57.642  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-28 14:57:57.642  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:57.656  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:57.656  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route21 (direct://start)
2022-03-28 14:57:57.656  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-21) started in 9ms (build:4ms init:4ms start:1ms)
2022-03-28 14:57:58.105  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 10539 milliseconds before reconnecting...
2022-03-28 14:57:58.105 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:57:58.635  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 10926 milliseconds before reconnecting...
2022-03-28 14:57:58.635 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:57:58.738  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:58.738  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-28 14:57:58.738  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1s81ms (1081 millis)
2022-03-28 14:57:58.738  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:58.738  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-21) shutting down (timeout:10s)
2022-03-28 14:57:58.739  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:57:58.739  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route21 (direct://start)
2022-03-28 14:57:58.739  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-21) shutdown in 1ms (uptime:1s84ms)
2022-03-28 14:57:58.741  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:58.741  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-28 14:57:58.741  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:57:58.753  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:57:58.753  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route22 (direct://start)
2022-03-28 14:57:58.753  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-22) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:57:58.943  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 7327 milliseconds before reconnecting...
2022-03-28 14:57:58.943 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:58:00.067  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.068  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-28 14:58:00.068  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1s314ms (1314 millis)
2022-03-28 14:58:00.068  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.068  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-22) shutting down (timeout:10s)
2022-03-28 14:58:00.068  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:00.069  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route22 (direct://start)
2022-03-28 14:58:00.069  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-22) shutdown in 1ms (uptime:1s317ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 5.08 s - in org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest
2022-03-28 14:58:00.071  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.072  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-28 14:58:00.072  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.082  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:00.082  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route23 (direct://start)
2022-03-28 14:58:00.082  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-23) started in 6ms (build:2ms init:3ms start:1ms)
2022-03-28 14:58:00.364  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.364  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-28 14:58:00.364  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 282ms (282 millis)
2022-03-28 14:58:00.364  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.365  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-23) shutting down (timeout:10s)
2022-03-28 14:58:00.366  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:00.366  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route23 (direct://start)
2022-03-28 14:58:00.367  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-23) shutdown in 3ms (uptime:286ms)
2022-03-28 14:58:00.368  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.368  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-28 14:58:00.368  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.388  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:00.388  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route24 (direct://start)
2022-03-28 14:58:00.388  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-24) started in 16ms (build:11ms init:3ms start:2ms)
2022-03-28 14:58:00.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-28 14:58:00.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 257ms (257 millis)
2022-03-28 14:58:00.645  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.645  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-24) shutting down (timeout:10s)
2022-03-28 14:58:00.646  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:00.646  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route24 (direct://start)
2022-03-28 14:58:00.647  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-24) shutdown in 1ms (uptime:260ms)
2022-03-28 14:58:00.648  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.648  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-28 14:58:00.648  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:00.658  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:00.658  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route25 (direct://start)
2022-03-28 14:58:00.659  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-25) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:58:01.003  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 11509 milliseconds before reconnecting...
2022-03-28 14:58:01.003 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:58:01.168  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-28 14:58:01.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 509ms (509 millis)
2022-03-28 14:58:01.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.169  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-25) shutting down (timeout:10s)
2022-03-28 14:58:01.170  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:01.170  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route25 (direct://start)
2022-03-28 14:58:01.170  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-25) shutdown in 1ms (uptime:512ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.098 s - in org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest
2022-03-28 14:58:01.173  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.174  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:01.174  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.186  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:01.186  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route26 (direct://start)
2022-03-28 14:58:01.186  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-26) started in 6ms (build:3ms init:3ms start:0ms)
2022-03-28 14:58:01.441  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.441  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:01.441  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 254ms (254 millis)
2022-03-28 14:58:01.441  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.441  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-26) shutting down (timeout:10s)
2022-03-28 14:58:01.442  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:01.442  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route26 (direct://start)
2022-03-28 14:58:01.443  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-26) shutdown in 2ms (uptime:257ms)
2022-03-28 14:58:01.444  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.444  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:01.444  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.449  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 18266 milliseconds before reconnecting...
2022-03-28 14:58:01.449 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:58:01.460  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:01.460  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route27 (direct://start)
2022-03-28 14:58:01.460  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-27) started in 12ms (build:7ms init:5ms start:0ms)
2022-03-28 14:58:01.720  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.720  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:01.720  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 259ms (259 millis)
2022-03-28 14:58:01.720  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.720  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-27) shutting down (timeout:10s)
2022-03-28 14:58:01.721  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:01.721  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route27 (direct://start)
2022-03-28 14:58:01.721  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-27) shutdown in 1ms (uptime:261ms)
2022-03-28 14:58:01.722  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.723  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:01.723  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.735  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:01.735  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route28 (direct://start)
2022-03-28 14:58:01.735  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-28) started in 9ms (build:3ms init:5ms start:1ms)
2022-03-28 14:58:01.987  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.987  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:01.987  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 252ms (252 millis)
2022-03-28 14:58:01.987  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.987  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-28) shutting down (timeout:10s)
2022-03-28 14:58:01.988  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:01.988  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route28 (direct://start)
2022-03-28 14:58:01.988  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-28) shutdown in 1ms (uptime:254ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.791 s - in org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest
2022-03-28 14:58:01.991  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:01.991  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-28 14:58:01.991  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.001  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:02.002  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route29 (direct://start)
2022-03-28 14:58:02.002  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-29) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:58:02.063  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 22313 milliseconds before reconnecting...
2022-03-28 14:58:02.063 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:58:02.330 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 65020726FD115CF-0000000000000000 on ExchangeId: 65020726FD115CF-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: Cannot deserialize value of type `java.lang.String` from Object value (token `JsonToken.START_OBJECT`)
 at [Source: UNKNOWN; byte offset: #UNKNOWN] (through reference chain: com.syntifi.casper.sdk.model.deploy.DeployData["deploy"]->com.syntifi.casper.sdk.model.deploy.Deploy["session"]->com.syntifi.casper.sdk.model.deploy.executabledeploy.StoredContractByHash["args"]->java.util.ArrayList[0]->com.syntifi.casper.sdk.model.deploy.NamedArg["clValue"]->com.syntifi.casper.sdk.model.clvalue.CLValueKey["parsed"]). Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route29           ] [route29           ] [                                                                              ] [       327]
	...
[route29           ] [to26              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: Cannot deserialize value of type `java.lang.String` from Object value (token `JsonToken.START_OBJECT`)
 at [Source: UNKNOWN; byte offset: #UNKNOWN] (through reference chain: com.syntifi.casper.sdk.model.deploy.DeployData["deploy"]->com.syntifi.casper.sdk.model.deploy.Deploy["session"]->com.syntifi.casper.sdk.model.deploy.executabledeploy.StoredContractByHash["args"]->java.util.ArrayList[0]->com.syntifi.casper.sdk.model.deploy.NamedArg["clValue"]->com.syntifi.casper.sdk.model.clvalue.CLValueKey["parsed"]). Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.deploy(CasperProducer.java:129) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:30) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest.testCallWith_DEPLOY_HASH_Parameter(CasperProducerWith_DEPLOY_OperationTest.java:28) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:02.331  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.331  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-28 14:58:02.331  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 328ms (328 millis)
2022-03-28 14:58:02.331  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.331  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-29) shutting down (timeout:10s)
2022-03-28 14:58:02.332  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:02.332  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route29 (direct://start)
2022-03-28 14:58:02.332  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-29) shutdown in 1ms (uptime:331ms)
2022-03-28 14:58:02.333  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.333  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-28 14:58:02.333  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.344  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:02.344  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route30 (direct://start)
2022-03-28 14:58:02.344  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-30) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:58:02.344 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 017B7BBCD713800-0000000000000000 on ExchangeId: 017B7BBCD713800-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: deployHash parameter is required with endpoint operation DEPLOY. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route30           ] [route30           ] [                                                                              ] [         0]
	...
[route30           ] [to27              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: deployHash parameter is required with endpoint operation DEPLOY. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.deploy(CasperProducer.java:123) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:30) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest.testCallWithout_DEPLOY_HASH_Parameter(CasperProducerWith_DEPLOY_OperationTest.java:42) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:02.345  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.345  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-28 14:58:02.345  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:58:02.345  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.345  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-30) shutting down (timeout:10s)
2022-03-28 14:58:02.346  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:02.346  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route30 (direct://start)
2022-03-28 14:58:02.346  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-30) shutdown in 1ms (uptime:3ms)
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.393 s - in org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest
2022-03-28 14:58:02.348  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.349  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter_Returning_Null() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:02.349  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.360  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:02.360  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route31 (direct://start)
2022-03-28 14:58:02.360  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-31) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:02.619  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.619  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter_Returning_Null() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:02.619  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 259ms (259 millis)
2022-03-28 14:58:02.620  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.620  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-31) shutting down (timeout:10s)
2022-03-28 14:58:02.620  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:02.620  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route31 (direct://start)
2022-03-28 14:58:02.621  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-31) shutdown in 1ms (uptime:262ms)
2022-03-28 14:58:02.622  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.622  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:02.622  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:02.633  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:02.633  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route32 (direct://start)
2022-03-28 14:58:02.633  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-32) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:04.920  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:04.920  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:04.920  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2s287ms (2287 millis)
2022-03-28 14:58:04.920  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:04.920  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-32) shutting down (timeout:10s)
2022-03-28 14:58:04.921  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:04.921  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route32 (direct://start)
2022-03-28 14:58:04.921  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-32) shutdown in 1ms (uptime:2s289ms)
2022-03-28 14:58:04.922  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:04.922  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:04.922  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:04.935  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:04.935  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route33 (direct://start)
2022-03-28 14:58:04.935  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-33) started in 8ms (build:2ms init:5ms start:1ms)
2022-03-28 14:58:05.382  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.382  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:05.382  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 447ms (447 millis)
2022-03-28 14:58:05.382  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.382  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-33) shutting down (timeout:10s)
2022-03-28 14:58:05.383  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:05.383  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route33 (direct://start)
2022-03-28 14:58:05.383  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-33) shutdown in 1ms (uptime:449ms)
2022-03-28 14:58:05.384  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.384  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:05.384  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.395  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:05.395  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route34 (direct://start)
2022-03-28 14:58:05.395  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-34) started in 7ms (build:3ms init:3ms start:1ms)
2022-03-28 14:58:05.396 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: D5B5C24BF71B314-0000000000000000 on ExchangeId: D5B5C24BF71B314-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route34           ] [route34           ] [                                                                              ] [         1]
	...
[route34           ] [to31              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.eraInfo(CasperProducer.java:322) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:34) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest.testCallWithout_Parameters(CasperProducerWith_ERA_INFO_OperationTest.java:71) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:05.397  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.397  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-28 14:58:05.397  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-28 14:58:05.397  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.397  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-34) shutting down (timeout:10s)
2022-03-28 14:58:05.398  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:05.398  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route34 (direct://start)
2022-03-28 14:58:05.398  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-34) shutdown in 1ms (uptime:4ms)
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 3.044 s - in org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest
2022-03-28 14:58:05.400  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.400  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest)
2022-03-28 14:58:05.400  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.413  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:05.413  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route35 (direct://start)
2022-03-28 14:58:05.413  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-35) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:05.555  INFO 41196 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 15804 milliseconds before reconnecting...
2022-03-28 14:58:05.555 ERROR 41196 --- [rce-events-[]-0] o.a.c.c.c.CasperEventHandler             : an error occured when connecting to the event stream

java.net.ConnectException: Failed to connect to localhost/0:0:0:0:0:0:0:1:8080
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
	at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Suppressed: java.net.ConnectException: Failed to connect to localhost/127.0.0.1:8080
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:285) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connect(RealConnection.kt:195) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findConnection(ExchangeFinder.kt:249) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.findHealthyConnection(ExchangeFinder.kt:108) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ExchangeFinder.find(ExchangeFinder.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.initExchange$okhttp(RealCall.kt:245) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.ConnectInterceptor.intercept(ConnectInterceptor.kt:32) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.cache.CacheInterceptor.intercept(CacheInterceptor.kt:82) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.BridgeInterceptor.intercept(BridgeInterceptor.kt:83) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RetryAndFollowUpInterceptor.intercept(RetryAndFollowUpInterceptor.kt:76) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.http.RealInterceptorChain.proceed(RealInterceptorChain.kt:100) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.getResponseWithInterceptorChain$okhttp(RealCall.kt:197) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealCall.execute(RealCall.kt:148) ~[okhttp-4.5.0.jar:?]
		at com.launchdarkly.eventsource.EventSource.newConnectionAttempt(EventSource.java:299) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at com.launchdarkly.eventsource.EventSource.run(EventSource.java:255) ~[okhttp-eventsource-2.3.2.jar:2.3.2]
		at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149) [?:1.8.0_292]
		at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624) [?:1.8.0_292]
		at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292]
	Caused by: java.net.ConnectException: Connection refused: connect
		at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
		at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
		at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
		at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
		at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
		at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
		at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
		at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
		... 20 more
Caused by: java.net.ConnectException: Connection refused: connect
	at java.net.DualStackPlainSocketImpl.waitForConnect(Native Method) ~[?:1.8.0_292]
	at java.net.DualStackPlainSocketImpl.socketConnect(DualStackPlainSocketImpl.java:85) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206) ~[?:1.8.0_292]
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188) ~[?:1.8.0_292]
	at java.net.PlainSocketImpl.connect(PlainSocketImpl.java:172) ~[?:1.8.0_292]
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392) ~[?:1.8.0_292]
	at java.net.Socket.connect(Socket.java:607) ~[?:1.8.0_292]
	at okhttp3.internal.platform.Platform.connectSocket(Platform.kt:117) ~[okhttp-4.5.0.jar:?]
	at okhttp3.internal.connection.RealConnection.connectSocket(RealConnection.kt:283) ~[okhttp-4.5.0.jar:?]
	... 20 more

2022-03-28 14:58:05.668  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.669  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest)
2022-03-28 14:58:05.669  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 255ms (255 millis)
2022-03-28 14:58:05.669  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.669  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-35) shutting down (timeout:10s)
2022-03-28 14:58:05.669  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:05.669  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route35 (direct://start)
2022-03-28 14:58:05.670  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-35) shutdown in 1ms (uptime:258ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.235 s - in org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest
2022-03-28 14:58:05.673  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.673  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:05.673  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.685  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:05.685  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route36 (direct://start)
2022-03-28 14:58:05.685  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-36) started in 7ms (build:3ms init:4ms start:0ms)
2022-03-28 14:58:05.935  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.935  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest)
2022-03-28 14:58:05.935  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 250ms (250 millis)
2022-03-28 14:58:05.935  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.935  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-36) shutting down (timeout:10s)
2022-03-28 14:58:05.936  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:05.936  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route36 (direct://start)
2022-03-28 14:58:05.937  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-36) shutdown in 1ms (uptime:252ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.263 s - in org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest
2022-03-28 14:58:05.939  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.939  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest)
2022-03-28 14:58:05.939  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:05.950  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:05.950  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route37 (direct://start)
2022-03-28 14:58:05.950  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-37) started in 7ms (build:3ms init:4ms start:0ms)
2022-03-28 14:58:06.208  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.208  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest)
2022-03-28 14:58:06.208  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 257ms (257 millis)
2022-03-28 14:58:06.208  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.208  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-37) shutting down (timeout:10s)
2022-03-28 14:58:06.211  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.211  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route37 (direct://start)
2022-03-28 14:58:06.211  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-37) shutdown in 3ms (uptime:261ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.274 s - in org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest
2022-03-28 14:58:06.213  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.213  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest)
2022-03-28 14:58:06.213  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.225  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.225  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route38 (direct://start)
2022-03-28 14:58:06.225  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-38) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:58:06.482  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.482  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest)
2022-03-28 14:58:06.483  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 257ms (257 millis)
2022-03-28 14:58:06.483  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.483  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-38) shutting down (timeout:10s)
2022-03-28 14:58:06.488  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.488  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route38 (direct://start)
2022-03-28 14:58:06.488  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-38) shutdown in 5ms (uptime:264ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.271 s - in org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest
2022-03-28 14:58:06.491  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.491  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-28 14:58:06.491  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.503  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.503  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route39 (direct://start)
2022-03-28 14:58:06.503  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-39) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:06.503 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: D0DF7D501C3D0CD-0000000000000000 on ExchangeId: D0DF7D501C3D0CD-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route39           ] [route39           ] [                                                                              ] [         0]
	...
[route39           ] [to36              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.putDeploy(CasperProducer.java:440) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:46) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest.testCallWith_DEPLOY_Parameter(CasperProducerWith_PUT_DEPLOY_OperationTest.java:32) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:06.504  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.504  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-28 14:58:06.504  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:58:06.504  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.504  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-39) shutting down (timeout:10s)
2022-03-28 14:58:06.505  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.505  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route39 (direct://start)
2022-03-28 14:58:06.506  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-39) shutdown in 2ms (uptime:4ms)
2022-03-28 14:58:06.507  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.507  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-28 14:58:06.507  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.518  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.519  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route40 (direct://start)
2022-03-28 14:58:06.519  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-40) started in 8ms (build:2ms init:5ms start:1ms)
2022-03-28 14:58:06.519 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 1796D5375A7B159-0000000000000000 on ExchangeId: 1796D5375A7B159-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route40           ] [route40           ] [                                                                              ] [         0]
	...
[route40           ] [to37              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.putDeploy(CasperProducer.java:440) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:46) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest.testCallWithout_DEPLOY_Parameter(CasperProducerWith_PUT_DEPLOY_OperationTest.java:42) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:06.520  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.521  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-28 14:58:06.521  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:58:06.521  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.521  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-40) shutting down (timeout:10s)
2022-03-28 14:58:06.523  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.524  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route40 (direct://start)
2022-03-28 14:58:06.524  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-40) shutdown in 3ms (uptime:6ms)
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.077 s - in org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest
2022-03-28 14:58:06.526  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.526  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.527  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.539  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.539  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route41 (direct://start)
2022-03-28 14:58:06.539  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-41) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:06.542 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 2915379CCBF3B79-0000000000000000 on ExchangeId: 2915379CCBF3B79-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation DICTIONARY_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route41           ] [route41           ] [                                                                              ] [         1]
	...
[route41           ] [to38              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation DICTIONARY_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.getDictionayItem(CasperProducer.java:372) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:32) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest.testCallWithout_STATE_ROOT_HASH_Parameter(CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest.java:68) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:06.543  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.543  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.543  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 3ms (3 millis)
2022-03-28 14:58:06.543  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.544  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-41) shutting down (timeout:10s)
2022-03-28 14:58:06.544  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.544  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route41 (direct://start)
2022-03-28 14:58:06.545  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-41) shutdown in 1ms (uptime:7ms)
2022-03-28 14:58:06.547  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.547  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_All_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.547  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.560  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.560  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route42 (direct://start)
2022-03-28 14:58:06.560  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-42) started in 9ms (build:3ms init:5ms start:1ms)
2022-03-28 14:58:06.820  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.820  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_All_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.820  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 260ms (260 millis)
2022-03-28 14:58:06.820  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.821  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-42) shutting down (timeout:10s)
2022-03-28 14:58:06.821  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.821  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route42 (direct://start)
2022-03-28 14:58:06.821  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-42) shutdown in 1ms (uptime:262ms)
2022-03-28 14:58:06.823  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.823  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_SEED_UREF_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.823  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.834  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.834  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route43 (direct://start)
2022-03-28 14:58:06.834  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-43) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:58:06.834 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 0FEA71FAB67DAEC-0000000000000000 on ExchangeId: 0FEA71FAB67DAEC-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: seedUref parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route43           ] [route43           ] [                                                                              ] [         0]
	...
[route43           ] [to40              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: seedUref parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.getDictionayItem(CasperProducer.java:381) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:32) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest.testCallWithout_SEED_UREF_Parameter(CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest.java:86) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

seedUref parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]
2022-03-28 14:58:06.835  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.835  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_SEED_UREF_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.835  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:58:06.835  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.835  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-43) shutting down (timeout:10s)
2022-03-28 14:58:06.837  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.837  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route43 (direct://start)
2022-03-28 14:58:06.837  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-43) shutdown in 2ms (uptime:4ms)
2022-03-28 14:58:06.838  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.838  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_DICTIONNARY_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.838  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.849  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.849  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route44 (direct://start)
2022-03-28 14:58:06.849  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-44) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:06.850 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 183624DC438CA08-0000000000000000 on ExchangeId: 183624DC438CA08-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: dictionnary key parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route44           ] [route44           ] [                                                                              ] [         1]
	...
[route44           ] [to41              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: dictionnary key parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.getDictionayItem(CasperProducer.java:376) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:32) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest.testCallWithout_DICTIONNARY_KEY_Parameter(CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest.java:51) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:06.851  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.851  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_DICTIONNARY_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest)
2022-03-28 14:58:06.851  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-28 14:58:06.851  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.851  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-44) shutting down (timeout:10s)
2022-03-28 14:58:06.852  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:06.852  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route44 (direct://start)
2022-03-28 14:58:06.853  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-44) shutdown in 2ms (uptime:5ms)
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.329 s - in org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONARY_ITEM_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest
2022-03-28 14:58:06.855  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.855  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-28 14:58:06.855  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:06.867  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:06.867  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route45 (direct://start)
2022-03-28 14:58:06.868  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-45) started in 7ms (build:2ms init:5ms start:0ms)
2022-03-28 14:58:07.141  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.142  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-28 14:58:07.142  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 273ms (273 millis)
2022-03-28 14:58:07.142  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.142  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-45) shutting down (timeout:10s)
2022-03-28 14:58:07.142  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:07.143  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route45 (direct://start)
2022-03-28 14:58:07.143  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-45) shutdown in 1ms (uptime:276ms)
2022-03-28 14:58:07.144  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.144  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-28 14:58:07.144  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.154  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:07.154  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route46 (direct://start)
2022-03-28 14:58:07.154  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-46) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-28 14:58:07.154 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 4BB25EF023A1FC6-0000000000000000 on ExchangeId: 4BB25EF023A1FC6-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation STATE_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route46           ] [route46           ] [                                                                              ] [         0]
	...
[route46           ] [to43              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation STATE_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.storedValue(CasperProducer.java:343) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:48) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest.testCallWithout_STATE_ROOT_HASH_Parameter(CasperProducerWith_STATE_ITEM_OperationTest.java:67) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:07.155  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.155  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-28 14:58:07.155  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:58:07.155  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.155  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-46) shutting down (timeout:10s)
2022-03-28 14:58:07.156  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:07.156  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route46 (direct://start)
2022-03-28 14:58:07.156  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-46) shutdown in 1ms (uptime:3ms)
2022-03-28 14:58:07.157  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.157  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-28 14:58:07.157  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.167  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:07.167  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route47 (direct://start)
2022-03-28 14:58:07.167  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-47) started in 6ms (build:2ms init:3ms start:1ms)
2022-03-28 14:58:07.168 ERROR 41196 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: BE630B829728F26-0000000000000000 on ExchangeId: BE630B829728F26-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: key parameter is required   with endpoint operation STATE_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route47           ] [route47           ] [                                                                              ] [         0]
	...
[route47           ] [to44              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: key parameter is required   with endpoint operation STATE_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:486) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.storedValue(CasperProducer.java:347) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:48) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:193) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.2.jar:3.14.2]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest.testCallWithout_KEY_Parameter(CasperProducerWith_STATE_ITEM_OperationTest.java:50) ~[test-classes/:?]
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_292]
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_292]
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_292]
	at java.lang.reflect.Method.invoke(Method.java:498) ~[?:1.8.0_292]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.2.jar:5.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at java.util.ArrayList.forEach(ArrayList.java:1259) ~[?:1.8.0_292]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.2.jar:1.8.2]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-28 14:58:07.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-28 14:58:07.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-28 14:58:07.169  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.169  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-47) shutting down (timeout:10s)
2022-03-28 14:58:07.170  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:07.170  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route47 (direct://start)
2022-03-28 14:58:07.170  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-47) shutdown in 1ms (uptime:4ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.307 s - in org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest
2022-03-28 14:58:07.173  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.173  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-28 14:58:07.173  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.183  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:07.183  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route48 (direct://start)
2022-03-28 14:58:07.183  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-48) started in 6ms (build:2ms init:3ms start:1ms)
2022-03-28 14:58:07.442  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.442  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-28 14:58:07.442  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 259ms (259 millis)
2022-03-28 14:58:07.442  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.442  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-48) shutting down (timeout:10s)
2022-03-28 14:58:07.443  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:07.443  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route48 (direct://start)
2022-03-28 14:58:07.444  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-48) shutdown in 2ms (uptime:262ms)
2022-03-28 14:58:07.445  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.445  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-28 14:58:07.445  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.454  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:07.454  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route49 (direct://start)
2022-03-28 14:58:07.454  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-49) started in 5ms (build:2ms init:3ms start:0ms)
2022-03-28 14:58:07.707  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.707  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-28 14:58:07.707  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 252ms (252 millis)
2022-03-28 14:58:07.707  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.707  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-49) shutting down (timeout:10s)
2022-03-28 14:58:07.734  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:07.734  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route49 (direct://start)
2022-03-28 14:58:07.734  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-49) shutdown in 27ms (uptime:280ms)
2022-03-28 14:58:07.735  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.736  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-28 14:58:07.736  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:07.747  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-28 14:58:07.747  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route50 (direct://start)
2022-03-28 14:58:07.747  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-50) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-28 14:58:08.244  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:08.244  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-28 14:58:08.244  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 497ms (497 millis)
2022-03-28 14:58:08.244  INFO 41196 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-28 14:58:08.244  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-50) shutting down (timeout:10s)
2022-03-28 14:58:08.245  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-28 14:58:08.245  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route50 (direct://start)
2022-03-28 14:58:08.245  INFO 41196 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.2 (camel-50) shutdown in 1ms (uptime:499ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.035 s - in org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 50, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  36.540 s
[INFO] Finished at: 2022-03-28T14:58:08-03:00
[INFO] ------------------------------------------------------------------------
```