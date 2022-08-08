``` text
[INFO] Scanning for projects...
[INFO] 
[INFO] ------------------< io.caspercommunity:camel-casper >-------------------
[INFO] Building Camel Casper blockchaine Component 3.14.1-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-source (default) @ camel-casper ---
[INFO] Source directory: D:\Devel\casper\camel-casper\src\generated\java added.
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (default) @ camel-casper ---
[INFO] 
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ camel-casper ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 2 resources
[INFO] Copying 6 resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.9.0:compile (default-compile) @ camel-casper ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- camel-package-maven-plugin:3.14.1:generate (generate) @ camel-casper ---
[INFO] Stale files detected, re-generating.
[INFO] Stale files detected, re-generating index.
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
[INFO] Compiling 53 source files to D:\Devel\casper\camel-casper\target\test-classes
[INFO] /D:/Devel/casper/camel-casper/src/test/java/org/apache/camel/component/casper/CasperTestSupport.java: D:\Devel\casper\camel-casper\src\test\java\org\apache\camel\component\casper\CasperTestSupport.java uses or overrides a deprecated API.
[INFO] /D:/Devel/casper/camel-casper/src/test/java/org/apache/camel/component/casper/CasperTestSupport.java: Recompile with -Xlint:deprecation for details.
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.0:test (default-test) @ camel-casper ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test
[                          main] KotlinDetector                 INFO  Kotlin reflection implementation not found at runtime, related features won't be available.

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-03 11:52:28.659  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 23592 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-03 11:52:28.660  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-03 11:52:28.926  WARN 23592 --- [kground-preinit] o.s.h.c.j.Jackson2ObjectMapperBuilder    : For Jackson Kotlin classes support please add "com.fasterxml.jackson.module:jackson-module-kotlin" to the classpath
2022-03-03 11:52:30.969  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-03 11:52:31.009  INFO 23592 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-03 11:52:31.011  INFO 23592 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-03 11:52:31.024  INFO 23592 --- [           main] o.a.c.c.AprLifecycleListener             : The APR based Apache Tomcat Native library which allows optimal performance in production environments was not found on the java.library.path: [C:\Program Files\Amazon Corretto\jdk11.0.7_10\bin;C:\WINDOWS\Sun\Java\bin;C:\WINDOWS\system32;C:\WINDOWS;C:\PROGRA~1\AMAZON~1\jdk11.0.7_10\bin;C:\Python39\Scripts\;C:\Python39\;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\iCLS\;C:\Program Files\Intel\Intel(R) Management Engine Components\iCLS\;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files\NVIDIA Corporation\NVIDIA NvDLISR;C:\Program Files (x86)\NVIDIA Corporation\PhysX\Common;D:\Devel\HaxeToolkit\haxe;D:\Devel\HaxeToolkit\neko;C:\Program Files\dotnet\;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program Files (x86)\dotnet\;C:\ProgramData\chocolatey\bin;C:\Program Files\gettext-iconv\bin;C:\Program Files\Microsoft VS Code\bin;C:\Program Files\nodejs\;C:\Program Files\Go\bin;C:\Program Files (x86)\gnupg\bin;C:\Program Files\Microsoft SQL Server\150\Tools\Binn\;C:\Program Files (x86)\Gpg4win\..\GnuPG\bin;C:\Program Files\Git\cmd;C:\Program Files\Docker\Docker\resources\bin;C:\ProgramData\DockerDesktop\version-bin;D:\Devel\apps\apache-maven\bin;D:\devel\apps\gradle\current\bin;D:\Devel\apps\java\scripts;C:\Users\oak3\AppData\Roaming\npm;D:\Devel\apps\mandrel\current\bin;C:\Program Files\JetBrains\IntelliJ IDEA 2021.3.2\bin;C:\Program Files\Microsoft Visual Studio\2022\Enterprise\VC\Tools\MSVC\14.30.30705\bin\Hostx64\x64;C:\Program Files\Microsoft Visual Studio\2022\Enterprise\VC\Auxiliary\Build\;D:\Devel\apps\mandrel\mandrel-java11-22.0.0.2-Final\bin;C:\PROGRA~1\AMAZON~1\jdk1.8.0_252\bin;;.]
2022-03-03 11:52:31.232  INFO 23592 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-03 11:52:31.232  INFO 23592 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 2525 ms
2022-03-03 11:52:31.336  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:31.765  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-03 11:52:31.768  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 3.64 seconds (JVM running for 5.066)
2022-03-03 11:52:32.155  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:32.157  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test)
2022-03-03 11:52:32.157  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:32.801  INFO 23592 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-03 11:52:32.805  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:32.805  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route1 (casper://http://localhost:8080/events/main)
2022-03-03 11:52:32.805  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-1) started in 470ms (build:55ms init:96ms start:319ms)
2022-03-03 11:52:32.810  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-03 11:52:32.896  INFO 23592 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-03 11:52:32.896  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-03 11:52:32.904  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 8 ms
2022-03-03 11:52:32.953  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-03 11:52:33.013  WARN 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-03 11:52:33.014  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 4245 milliseconds before reconnecting...
2022-03-03 11:52:33.023  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-03 11:52:33.025  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:33.025  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test)
2022-03-03 11:52:33.025  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 216ms (216 millis)
2022-03-03 11:52:33.025  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:33.028  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-1) shutting down (timeout:10s)
2022-03-03 11:52:33.034  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:33.034  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route1 (casper://http://localhost:8080/events/main)
2022-03-03 11:52:33.036  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-1) shutdown in 8ms (uptime:550ms)
2022-03-03 11:52:33.043  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 6.422 s - in org.apache.camel.component.casper.consumer.ConsumerTest_BLOCK_ADDED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-03 11:52:34.013  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 23592 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-03 11:52:34.014  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-03 11:52:34.242  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-03 11:52:34.247  INFO 23592 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-03 11:52:34.249  INFO 23592 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-03 11:52:34.312  INFO 23592 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-03 11:52:34.312  INFO 23592 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 296 ms
2022-03-03 11:52:34.326  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:34.445  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-03 11:52:34.446  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.499 seconds (JVM running for 7.744)
2022-03-03 11:52:34.448  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:34.448  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test)
2022-03-03 11:52:34.448  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:34.464  INFO 23592 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/deploys
2022-03-03 11:52:34.465  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:34.465  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route2 (casper://http://localhost:8080/events/deploys)
2022-03-03 11:52:34.465  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-2) started in 12ms (build:3ms init:6ms start:3ms)
2022-03-03 11:52:34.466  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-03 11:52:34.468  INFO 23592 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-03 11:52:34.469  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-03 11:52:34.473  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 4 ms
2022-03-03 11:52:34.475  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-03 11:52:34.481  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-03 11:52:34.482  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:34.482  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test)
2022-03-03 11:52:34.482  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 16ms (16 millis)
2022-03-03 11:52:34.482  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:34.482  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-2) shutting down (timeout:10s)
2022-03-03 11:52:34.486  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:34.487  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route2 (casper://http://localhost:8080/events/deploys)
2022-03-03 11:52:34.487  WARN 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-03 11:52:34.488  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 3544 milliseconds before reconnecting...
2022-03-03 11:52:34.494  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-2) shutdown in 7ms (uptime:27ms)
2022-03-03 11:52:34.495  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.445 s - in org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_ACCEPTED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-03 11:52:35.479  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 23592 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-03 11:52:35.479  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-03 11:52:35.625  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-03 11:52:35.626  INFO 23592 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-03 11:52:35.626  INFO 23592 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-03 11:52:35.662  INFO 23592 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-03 11:52:35.662  INFO 23592 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 180 ms
2022-03-03 11:52:35.675  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:35.803  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-03 11:52:35.803  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.362 seconds (JVM running for 9.101)
2022-03-03 11:52:35.806  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:35.806  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test)
2022-03-03 11:52:35.806  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:35.817  INFO 23592 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/main
2022-03-03 11:52:35.818  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:35.818  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route3 (casper://http://localhost:8080/events/main)
2022-03-03 11:52:35.818  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-3) started in 9ms (build:3ms init:4ms start:2ms)
2022-03-03 11:52:35.819  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-03 11:52:35.821  INFO 23592 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-03 11:52:35.821  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-03 11:52:35.824  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 2 ms
2022-03-03 11:52:35.835  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-03 11:52:35.850  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-03 11:52:35.851  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:35.851  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test)
2022-03-03 11:52:35.851  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 33ms (33 millis)
2022-03-03 11:52:35.851  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:35.851  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-3) shutting down (timeout:10s)
2022-03-03 11:52:35.852  WARN 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-03 11:52:35.852  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 4797 milliseconds before reconnecting...
2022-03-03 11:52:35.854  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:35.854  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route3 (casper://http://localhost:8080/events/main)
2022-03-03 11:52:35.854  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-3) shutdown in 3ms (uptime:38ms)
2022-03-03 11:52:35.857  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.337 s - in org.apache.camel.component.casper.consumer.ConsumerTest_DEPLOY_PROCESSED_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-03 11:52:36.820  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 23592 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-03 11:52:36.821  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-03 11:52:36.984  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-03 11:52:36.985  INFO 23592 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-03 11:52:36.985  INFO 23592 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-03 11:52:37.021  INFO 23592 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-03 11:52:37.021  INFO 23592 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 197 ms
2022-03-03 11:52:37.035  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:37.152  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-03 11:52:37.153  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.363 seconds (JVM running for 10.451)
2022-03-03 11:52:37.157  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:37.157  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test)
2022-03-03 11:52:37.157  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:37.176  INFO 23592 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/sigs
2022-03-03 11:52:37.177  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:37.177  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route4 (casper://http://localhost:8080/events/sigs)
2022-03-03 11:52:37.177  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-4) started in 15ms (build:5ms init:6ms start:4ms)
2022-03-03 11:52:37.177  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-03 11:52:37.179  INFO 23592 --- [nio-8080-exec-3] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-03 11:52:37.180  INFO 23592 --- [nio-8080-exec-3] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-03 11:52:37.182  INFO 23592 --- [nio-8080-exec-3] o.s.w.s.DispatcherServlet                : Completed initialization in 2 ms
2022-03-03 11:52:37.186  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-03 11:52:37.197  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-03 11:52:37.197  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:37.197  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test)
2022-03-03 11:52:37.198  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 20ms (20 millis)
2022-03-03 11:52:37.198  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:37.198  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-4) shutting down (timeout:10s)
2022-03-03 11:52:37.201  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:37.201  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route4 (casper://http://localhost:8080/events/sigs)
2022-03-03 11:52:37.202  WARN 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-03 11:52:37.203  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 3081 milliseconds before reconnecting...
2022-03-03 11:52:37.204  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-4) shutdown in 4ms (uptime:29ms)
2022-03-03 11:52:37.205  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:38.176  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 8895 milliseconds before reconnecting...
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.389 s - in org.apache.camel.component.casper.consumer.ConsumerTest_FINALITY_SIGNATURE_Event_Test
[INFO] Running org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.1.2.RELEASE)

2022-03-03 11:52:38.214  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Starting SpringAsyncTestApplication on OAKDESK with PID 23592 (started by oak3 in D:\Devel\casper\camel-casper)
2022-03-03 11:52:38.215  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : No active profile set, falling back to default profiles: default
2022-03-03 11:52:38.406  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat initialized with port(s): 8080 (http)
2022-03-03 11:52:38.408  INFO 23592 --- [           main] o.a.c.c.StandardService                  : Starting service [Tomcat]
2022-03-03 11:52:38.408  INFO 23592 --- [           main] o.a.c.c.StandardEngine                   : Starting Servlet engine: [Apache Tomcat/9.0.14]
2022-03-03 11:52:38.451  INFO 23592 --- [           main] o.a.c.c.C.[.[.[/]                        : Initializing Spring embedded WebApplicationContext
2022-03-03 11:52:38.452  INFO 23592 --- [           main] o.s.w.c.ContextLoader                    : Root WebApplicationContext: initialization completed in 236 ms
2022-03-03 11:52:38.464  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Initializing ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:38.574  INFO 23592 --- [           main] o.s.b.w.e.t.TomcatWebServer              : Tomcat started on port(s): 8080 (http) with context path ''
2022-03-03 11:52:38.575  INFO 23592 --- [           main] o.a.c.c.c.c.s.SpringAsyncTestApplication : Started SpringAsyncTestApplication in 0.389 seconds (JVM running for 11.873)
2022-03-03 11:52:38.577  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:38.577  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test)
2022-03-03 11:52:38.577  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:38.608  INFO 23592 --- [           main] c.l.e.EventSource                        : Starting EventSource client using URI: http://localhost:8080/events/sigs
2022-03-03 11:52:38.613  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:38.613  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route5 (casper://http://localhost:8080/events/sigs)
2022-03-03 11:52:38.613  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-5) started in 24ms (build:4ms init:14ms start:6ms)
2022-03-03 11:52:38.613  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://result is satisfied
2022-03-03 11:52:38.622  INFO 23592 --- [nio-8080-exec-1] o.a.c.c.C.[.[.[/]                        : Initializing Spring DispatcherServlet 'dispatcherServlet'
2022-03-03 11:52:38.622  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Initializing Servlet 'dispatcherServlet'
2022-03-03 11:52:38.627  INFO 23592 --- [nio-8080-exec-1] o.s.w.s.DispatcherServlet                : Completed initialization in 5 ms
2022-03-03 11:52:38.631  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connected to EventSource stream.
2022-03-03 11:52:38.655  INFO 23592 --- [           main] o.a.c.c.m.MockEndpoint                   : Asserting: mock://error is satisfied
2022-03-03 11:52:38.656  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:38.656  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testEvent() (org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test)
2022-03-03 11:52:38.656  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 43ms (43 millis)
2022-03-03 11:52:38.656  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:38.656  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-5) shutting down (timeout:10s)
2022-03-03 11:52:38.668  WARN 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Connection unexpectedly closed
2022-03-03 11:52:38.669  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 4099 milliseconds before reconnecting...
2022-03-03 11:52:38.669  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:38.669  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route5 (casper://http://localhost:8080/events/sigs)
2022-03-03 11:52:38.670  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-5) shutdown in 14ms (uptime:63ms)
2022-03-03 11:52:38.673  INFO 23592 --- [           main] o.s.s.c.ThreadPoolTaskExecutor           : Shutting down ExecutorService 'mvcTaskExecutor'
2022-03-03 11:52:38.679  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 7823 milliseconds before reconnecting...
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.388 s - in org.apache.camel.component.casper.consumer.ConsumerTest_STEP_Event_Test
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest
2022-03-03 11:52:39.585  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:39.585  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-03 11:52:39.585  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:39.617  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:39.617  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route6 (direct://start)
2022-03-03 11:52:39.617  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-6) started in 23ms (build:8ms init:7ms start:8ms)
2022-03-03 11:52:40.506  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.506  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-03 11:52:40.506  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 889ms (889 millis)
2022-03-03 11:52:40.506  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.506  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-6) shutting down (timeout:10s)
2022-03-03 11:52:40.507  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:40.507  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route6 (direct://start)
2022-03-03 11:52:40.508  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-6) shutdown in 1ms (uptime:898ms)
2022-03-03 11:52:40.509  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.509  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-03 11:52:40.509  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.520  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:40.521  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route7 (direct://start)
2022-03-03 11:52:40.521  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-7) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:40.523 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 36F94E4BCD5DFFF-0000000000000000 on ExchangeId: 36F94E4BCD5DFFF-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: stateRootHash parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route7            ] [route7            ] [                                                                              ] [         2]
	...
[route7            ] [to7               ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: stateRootHash parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountBalance(CasperProducer.java:441) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:20) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest.testCallWithout_STATE_ROOT_HASH_Parameter(CasperProducerWith_ACCOUNT_BALANCE_OperationTest.java:83) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:40.531  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.531  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-03 11:52:40.531  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 10ms (10 millis)
2022-03-03 11:52:40.531  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.532  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-7) shutting down (timeout:10s)
2022-03-03 11:52:40.532  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:40.532  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route7 (direct://start)
2022-03-03 11:52:40.533  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-7) shutdown in 1ms (uptime:13ms)
2022-03-03 11:52:40.534  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.534  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_UREF_PURSE_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-03 11:52:40.534  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.551  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:40.551  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route8 (direct://start)
2022-03-03 11:52:40.551  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-8) started in 10ms (build:3ms init:5ms start:2ms)
2022-03-03 11:52:40.552 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 189CD8377835B0D-0000000000000000 on ExchangeId: 189CD8377835B0D-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: purseUref parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]
stateRootHash parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]  stateroothash parameter is required   with endpoint operation account_balance

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route8            ] [route8            ] [                                                                              ] [         0]
	...
[route8            ] [to8               ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: purseUref parameter is required   with endpoint operation ACCOUNT_BALANCE. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountBalance(CasperProducer.java:447) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:20) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest.testCallWithout_UREF_PURSE_KEY_Parameter(CasperProducerWith_ACCOUNT_BALANCE_OperationTest.java:58) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:40.553  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.553  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_UREF_PURSE_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest)
2022-03-03 11:52:40.553  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-03 11:52:40.553  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.553  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-8) shutting down (timeout:10s)
2022-03-03 11:52:40.554  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:40.554  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route8 (direct://start)
2022-03-03 11:52:40.555  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-8) shutdown in 1ms (uptime:6ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.041 s - in org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_BALANCE_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest
2022-03-03 11:52:40.558  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.558  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:40.558  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.578  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:40.578  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route9 (direct://start)
2022-03-03 11:52:40.579  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-9) started in 12ms (build:3ms init:7ms start:2ms)
2022-03-03 11:52:40.880  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.881  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:40.881  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 301ms (301 millis)
2022-03-03 11:52:40.881  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.881  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-9) shutting down (timeout:10s)
2022-03-03 11:52:40.882  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:40.882  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route9 (direct://start)
2022-03-03 11:52:40.883  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-9) shutdown in 2ms (uptime:306ms)
2022-03-03 11:52:40.884  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.884  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:40.885  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:40.898  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:40.898  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route10 (direct://start)
2022-03-03 11:52:40.898  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-10) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:41.189  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.189  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:41.189  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 287ms (287 millis)
2022-03-03 11:52:41.189  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.189  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-10) shutting down (timeout:10s)
2022-03-03 11:52:41.198  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:41.198  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route10 (direct://start)
2022-03-03 11:52:41.199  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-10) shutdown in 10ms (uptime:302ms)
2022-03-03 11:52:41.201  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.201  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:41.201  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.214  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:41.214  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route11 (direct://start)
2022-03-03 11:52:41.214  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-11) started in 7ms (build:3ms init:4ms start:0ms)
2022-03-03 11:52:41.215 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 1F023F26FE3F824-0000000000000000 on ExchangeId: 1F023F26FE3F824-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: publicKey parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route11           ] [route11           ] [                                                                              ] [         0]
	...
[route11           ] [to11              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: publicKey parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountInfo(CasperProducer.java:224) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:22) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest.testCallWithout_PUBLIC_KEY_Parameters(CasperProducerWith_ACCOUNT_INFO_OperationTest.java:73) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:41.217  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.217  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:41.217  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-03 11:52:41.217  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.218  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-11) shutting down (timeout:10s)
2022-03-03 11:52:41.225  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:41.225  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route11 (direct://start)
2022-03-03 11:52:41.225  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-11) shutdown in 7ms (uptime:11ms)
2022-03-03 11:52:41.227  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.227  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithOnly_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:41.227  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.250  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:41.250  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route12 (direct://start)
2022-03-03 11:52:41.250  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-12) started in 15ms (build:4ms init:10ms start:1ms)
2022-03-03 11:52:41.252 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: B80DC2382F38A38-0000000000000000 on ExchangeId: B80DC2382F38A38-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route12           ] [route12           ] [                                                                              ] [         0]
	...
[route12           ] [to12              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.accountInfo(CasperProducer.java:236) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:22) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest.testCallWithOnly_PUBLIC_KEY_Parameters(CasperProducerWith_ACCOUNT_INFO_OperationTest.java:96) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:41.253  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.253  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithOnly_PUBLIC_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest)
2022-03-03 11:52:41.254  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-03 11:52:41.254  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.254  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-12) shutting down (timeout:10s)
2022-03-03 11:52:41.255  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:41.255  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route12 (direct://start)
2022-03-03 11:52:41.256  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-12) shutdown in 1ms (uptime:6ms)
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.667 s - in org.apache.camel.component.casper.producer.CasperProducerWith_ACCOUNT_INFO_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest
2022-03-03 11:52:41.259  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.259  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-03 11:52:41.259  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:41.279  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:41.279  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route13 (direct://start)
2022-03-03 11:52:41.279  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-13) started in 10ms (build:5ms init:4ms start:1ms)
2022-03-03 11:52:44.054  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:44.054  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-03 11:52:44.055  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2s775ms (2775 millis)
2022-03-03 11:52:44.055  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:44.055  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-13) shutting down (timeout:10s)
2022-03-03 11:52:44.058  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:44.058  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route13 (direct://start)
2022-03-03 11:52:44.059  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-13) shutdown in 4ms (uptime:2s781ms)
2022-03-03 11:52:44.061  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:44.061  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-03 11:52:44.061  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:44.073  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:44.073  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route14 (direct://start)
2022-03-03 11:52:44.073  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-14) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-03 11:52:44.327  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 9935 milliseconds before reconnecting...
2022-03-03 11:52:44.731  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 6562 milliseconds before reconnecting...
2022-03-03 11:52:45.212  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:45.212  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-03 11:52:45.213  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1s139ms (1139 millis)
2022-03-03 11:52:45.213  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:45.213  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-14) shutting down (timeout:10s)
2022-03-03 11:52:45.214  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:45.214  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route14 (direct://start)
2022-03-03 11:52:45.214  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-14) shutdown in 1ms (uptime:1s142ms)
2022-03-03 11:52:45.216  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:45.216  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-03 11:52:45.216  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:45.227  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:45.227  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route15 (direct://start)
2022-03-03 11:52:45.227  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-15) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:46.818  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 10680 milliseconds before reconnecting...
2022-03-03 11:52:46.866  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:46.867  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest)
2022-03-03 11:52:46.867  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1s639ms (1639 millis)
2022-03-03 11:52:46.867  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:46.867  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-15) shutting down (timeout:10s)
2022-03-03 11:52:46.867  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:46.868  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route15 (direct://start)
2022-03-03 11:52:46.868  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-15) shutdown in 1ms (uptime:1s642ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 5.536 s - in org.apache.camel.component.casper.producer.CasperProducerWith_AUCTION_INFO_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest
2022-03-03 11:52:46.871  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:46.871  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-03 11:52:46.871  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:46.886  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:46.886  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route16 (direct://start)
2022-03-03 11:52:46.888  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-16) started in 9ms (build:4ms init:4ms start:1ms)
2022-03-03 11:52:47.190  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.190  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-03 11:52:47.190  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 302ms (302 millis)
2022-03-03 11:52:47.190  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.190  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-16) shutting down (timeout:10s)
2022-03-03 11:52:47.193  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:47.193  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route16 (direct://start)
2022-03-03 11:52:47.193  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-16) shutdown in 3ms (uptime:308ms)
2022-03-03 11:52:47.196  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.196  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-03 11:52:47.196  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.209  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:47.210  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route17 (direct://start)
2022-03-03 11:52:47.210  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-17) started in 10ms (build:3ms init:5ms start:2ms)
2022-03-03 11:52:47.495  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.495  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-03 11:52:47.495  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 285ms (285 millis)
2022-03-03 11:52:47.495  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.495  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-17) shutting down (timeout:10s)
2022-03-03 11:52:47.499  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:47.499  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route17 (direct://start)
2022-03-03 11:52:47.500  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-17) shutdown in 5ms (uptime:292ms)
2022-03-03 11:52:47.502  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.502  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-03 11:52:47.502  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:47.517  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:47.517  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route18 (direct://start)
2022-03-03 11:52:47.518  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-18) started in 12ms (build:6ms init:4ms start:2ms)
2022-03-03 11:52:48.070  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.070  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest)
2022-03-03 11:52:48.070  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 552ms (552 millis)
2022-03-03 11:52:48.070  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.070  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-18) shutting down (timeout:10s)
2022-03-03 11:52:48.072  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:48.072  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route18 (direct://start)
2022-03-03 11:52:48.072  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-18) shutdown in 2ms (uptime:556ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.198 s - in org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest
2022-03-03 11:52:48.074  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.075  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:48.075  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.086  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:48.086  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route19 (direct://start)
2022-03-03 11:52:48.086  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-19) started in 7ms (build:2ms init:4ms start:1ms)
2022-03-03 11:52:48.360  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.360  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:48.360  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 274ms (274 millis)
2022-03-03 11:52:48.360  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.360  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-19) shutting down (timeout:10s)
2022-03-03 11:52:48.362  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:48.363  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route19 (direct://start)
2022-03-03 11:52:48.363  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-19) shutdown in 3ms (uptime:278ms)
2022-03-03 11:52:48.364  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.364  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:48.364  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.374  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:48.374  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route20 (direct://start)
2022-03-03 11:52:48.374  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-20) started in 7ms (build:3ms init:3ms start:1ms)
2022-03-03 11:52:48.659  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.659  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:48.659  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 285ms (285 millis)
2022-03-03 11:52:48.659  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.659  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-20) shutting down (timeout:10s)
2022-03-03 11:52:48.663  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:48.663  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route20 (direct://start)
2022-03-03 11:52:48.663  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-20) shutdown in 4ms (uptime:290ms)
2022-03-03 11:52:48.665  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.665  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:48.665  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.677  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:48.677  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route21 (direct://start)
2022-03-03 11:52:48.677  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-21) started in 8ms (build:3ms init:3ms start:2ms)
2022-03-03 11:52:48.950  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.950  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:48.950  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 273ms (273 millis)
2022-03-03 11:52:48.950  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.950  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-21) shutting down (timeout:10s)
2022-03-03 11:52:48.951  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:48.951  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route21 (direct://start)
2022-03-03 11:52:48.952  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-21) shutdown in 2ms (uptime:277ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.876 s - in org.apache.camel.component.casper.producer.CasperProducerWith_BLOCK_TRANSFERS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest
2022-03-03 11:52:48.954  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.955  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-03 11:52:48.955  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:48.967  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:48.967  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route22 (direct://start)
2022-03-03 11:52:48.967  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-22) started in 6ms (build:2ms init:3ms start:1ms)
2022-03-03 11:52:49.299 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 33BB409CB933E12-0000000000000000 on ExchangeId: 33BB409CB933E12-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: Cannot deserialize value of type `java.lang.String` from Object value (token `JsonToken.START_OBJECT`)
 at [Source: UNKNOWN; byte offset: #UNKNOWN] (through reference chain: com.syntifi.casper.sdk.model.deploy.DeployData["deploy"]->com.syntifi.casper.sdk.model.deploy.Deploy["session"]->com.syntifi.casper.sdk.model.deploy.executabledeploy.StoredContractByHash["args"]->java.util.ArrayList[0]->com.syntifi.casper.sdk.model.deploy.NamedArg["clValue"]->com.syntifi.casper.sdk.model.clvalue.CLValueKey["parsed"]). Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route22           ] [route22           ] [                                                                              ] [       332]
	...
[route22           ] [to22              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: Cannot deserialize value of type `java.lang.String` from Object value (token `JsonToken.START_OBJECT`)
 at [Source: UNKNOWN; byte offset: #UNKNOWN] (through reference chain: com.syntifi.casper.sdk.model.deploy.DeployData["deploy"]->com.syntifi.casper.sdk.model.deploy.Deploy["session"]->com.syntifi.casper.sdk.model.deploy.executabledeploy.StoredContractByHash["args"]->java.util.ArrayList[0]->com.syntifi.casper.sdk.model.deploy.NamedArg["clValue"]->com.syntifi.casper.sdk.model.clvalue.CLValueKey["parsed"]). Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.deploy(CasperProducer.java:136) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:30) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest.testCallWith_DEPLOY_HASH_Parameter(CasperProducerWith_DEPLOY_OperationTest.java:38) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:49.300  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.300  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-03 11:52:49.300  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 333ms (333 millis)
2022-03-03 11:52:49.300  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.301  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-22) shutting down (timeout:10s)
2022-03-03 11:52:49.304  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:49.304  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route22 (direct://start)
2022-03-03 11:52:49.304  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-22) shutdown in 3ms (uptime:338ms)
2022-03-03 11:52:49.306  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.306  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-03 11:52:49.306  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.324  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:49.324  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route23 (direct://start)
2022-03-03 11:52:49.324  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-23) started in 12ms (build:2ms init:7ms start:3ms)
2022-03-03 11:52:49.325 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: C397622ED7B66E7-0000000000000000 on ExchangeId: C397622ED7B66E7-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: deployHash parameter is required with endpoint operation DEPLOY. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route23           ] [route23           ] [                                                                              ] [         0]
	...
[route23           ] [to23              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: deployHash parameter is required with endpoint operation DEPLOY. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.deploy(CasperProducer.java:127) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:30) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest.testCallWithout_DEPLOY_HASH_Parameter(CasperProducerWith_DEPLOY_OperationTest.java:53) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:49.326  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.326  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest)
2022-03-03 11:52:49.326  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-03 11:52:49.327  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.327  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-23) shutting down (timeout:10s)
2022-03-03 11:52:49.328  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:49.328  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route23 (direct://start)
2022-03-03 11:52:49.328  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-23) shutdown in 1ms (uptime:7ms)
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.435 s - in org.apache.camel.component.casper.producer.CasperProducerWith_DEPLOY_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest
2022-03-03 11:52:49.334  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.334  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter_Returning_Null() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:49.334  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.346  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:49.346  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route24 (direct://start)
2022-03-03 11:52:49.346  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-24) started in 9ms (build:3ms init:4ms start:2ms)
2022-03-03 11:52:49.629  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.629  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter_Returning_Null() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:49.629  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 281ms (281 millis)
2022-03-03 11:52:49.629  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.629  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-24) shutting down (timeout:10s)
2022-03-03 11:52:49.632  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:49.632  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route24 (direct://start)
2022-03-03 11:52:49.633  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-24) shutdown in 3ms (uptime:289ms)
2022-03-03 11:52:49.634  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.634  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:49.634  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:49.649  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:49.649  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route25 (direct://start)
2022-03-03 11:52:49.649  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-25) started in 11ms (build:5ms init:5ms start:1ms)
2022-03-03 11:52:50.368  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:50.368  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:50.368  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 719ms (719 millis)
2022-03-03 11:52:50.368  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:50.368  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-25) shutting down (timeout:10s)
2022-03-03 11:52:50.370  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:50.370  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route25 (direct://start)
2022-03-03 11:52:50.370  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-25) shutdown in 2ms (uptime:722ms)
2022-03-03 11:52:50.372  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:50.372  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:50.372  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:50.388  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:50.388  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route26 (direct://start)
2022-03-03 11:52:50.388  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-26) started in 12ms (build:3ms init:8ms start:1ms)
2022-03-03 11:52:50.583  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 15641 milliseconds before reconnecting...
2022-03-03 11:52:51.101  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.101  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:51.101  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 713ms (713 millis)
2022-03-03 11:52:51.101  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.101  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-26) shutting down (timeout:10s)
2022-03-03 11:52:51.108  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:51.108  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route26 (direct://start)
2022-03-03 11:52:51.110  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-26) shutdown in 7ms (uptime:721ms)
2022-03-03 11:52:51.111  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.112  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:51.112  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.124  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:51.124  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route27 (direct://start)
2022-03-03 11:52:51.124  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-27) started in 7ms (build:3ms init:3ms start:1ms)
2022-03-03 11:52:51.124 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 3E80532D2AEA31F-0000000000000000 on ExchangeId: 3E80532D2AEA31F-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route27           ] [route27           ] [                                                                              ] [         0]
	...
[route27           ] [to27              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: Either blockHeight or BlockHash parameter is required  with endpoint operation ACCOUNT_INFO. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.eraInfo(CasperProducer.java:335) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:34) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest.testCallWithout_Parameters(CasperProducerWith_ERA_INFO_OperationTest.java:78) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:51.125  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.126  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest)
2022-03-03 11:52:51.126  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-03 11:52:51.126  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.126  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-27) shutting down (timeout:10s)
2022-03-03 11:52:51.126  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:51.126  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route27 (direct://start)
2022-03-03 11:52:51.127  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-27) shutdown in 1ms (uptime:4ms)
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.775 s - in org.apache.camel.component.casper.producer.CasperProducerWith_ERA_INFO_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest
2022-03-03 11:52:51.129  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.129  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest)
2022-03-03 11:52:51.129  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.141  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:51.141  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route28 (direct://start)
2022-03-03 11:52:51.141  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-28) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:51.159  INFO 23592 --- [rce-stream-[]-0] c.l.e.EventSource                        : Waiting 20136 milliseconds before reconnecting...
2022-03-03 11:52:51.418  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.419  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_DEPLOY_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest)
2022-03-03 11:52:51.419  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 277ms (277 millis)
2022-03-03 11:52:51.419  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.419  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-28) shutting down (timeout:10s)
2022-03-03 11:52:51.420  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:51.420  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route28 (direct://start)
2022-03-03 11:52:51.421  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-28) shutdown in 2ms (uptime:281ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.219 s - in org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest
2022-03-03 11:52:51.423  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.423  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:51.423  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.434  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:51.434  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route29 (direct://start)
2022-03-03 11:52:51.434  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-29) started in 6ms (build:3ms init:2ms start:1ms)
2022-03-03 11:52:51.709  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.710  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest)
2022-03-03 11:52:51.710  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 275ms (275 millis)
2022-03-03 11:52:51.710  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.710  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-29) shutting down (timeout:10s)
2022-03-03 11:52:51.711  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:51.711  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route29 (direct://start)
2022-03-03 11:52:51.711  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-29) shutdown in 1ms (uptime:278ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.29 s - in org.apache.camel.component.casper.producer.CasperProducerWith_LAST_BLOCK_TRANSFERS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest
2022-03-03 11:52:51.715  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.715  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest)
2022-03-03 11:52:51.715  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:51.726  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:51.726  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route30 (direct://start)
2022-03-03 11:52:51.726  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-30) started in 8ms (build:3ms init:3ms start:2ms)
2022-03-03 11:52:52.003  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.003  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest)
2022-03-03 11:52:52.003  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 277ms (277 millis)
2022-03-03 11:52:52.003  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.003  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-30) shutting down (timeout:10s)
2022-03-03 11:52:52.005  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.005  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route30 (direct://start)
2022-03-03 11:52:52.006  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-30) shutdown in 3ms (uptime:282ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.287 s - in org.apache.camel.component.casper.producer.CasperProducerWith_NETWORK_PEERS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest
2022-03-03 11:52:52.008  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.008  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest)
2022-03-03 11:52:52.008  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.019  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.019  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route31 (direct://start)
2022-03-03 11:52:52.019  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-31) started in 7ms (build:3ms init:3ms start:1ms)
2022-03-03 11:52:52.302  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.302  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCall() (org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest)
2022-03-03 11:52:52.302  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 283ms (283 millis)
2022-03-03 11:52:52.302  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.302  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-31) shutting down (timeout:10s)
2022-03-03 11:52:52.304  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.304  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route31 (direct://start)
2022-03-03 11:52:52.305  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-31) shutdown in 3ms (uptime:287ms)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.271 s - in org.apache.camel.component.casper.producer.CasperProducerWith_NODE_STATUS_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest
2022-03-03 11:52:52.307  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.307  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-03 11:52:52.307  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.320  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.320  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route32 (direct://start)
2022-03-03 11:52:52.320  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-32) started in 8ms (build:2ms init:4ms start:2ms)
2022-03-03 11:52:52.320 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 7AFF75920AFE46C-0000000000000000 on ExchangeId: 7AFF75920AFE46C-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route32           ] [route32           ] [                                                                              ] [         0]
	...
[route32           ] [to32              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.putDeploy(CasperProducer.java:475) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:46) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest.testCallWith_DEPLOY_Parameter(CasperProducerWith_PUT_DEPLOY_OperationTest.java:39) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:52.321  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.321  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-03 11:52:52.321  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-03 11:52:52.321  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.321  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-32) shutting down (timeout:10s)
2022-03-03 11:52:52.323  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.323  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route32 (direct://start)
2022-03-03 11:52:52.324  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-32) shutdown in 3ms (uptime:6ms)
2022-03-03 11:52:52.325  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.325  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-03 11:52:52.325  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.338  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.339  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route33 (direct://start)
2022-03-03 11:52:52.339  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-33) started in 10ms (build:3ms init:5ms start:2ms)
2022-03-03 11:52:52.341 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 086F359C865CD63-0000000000000000 on ExchangeId: 086F359C865CD63-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route33           ] [route33           ] [                                                                              ] [         0]
	...
[route33           ] [to33              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: deloy parameter is required   with endpoint operation PUT_DEPLOY. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.putDeploy(CasperProducer.java:475) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:46) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest.testCallWithout_DEPLOY_Parameter(CasperProducerWith_PUT_DEPLOY_OperationTest.java:54) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:52.342  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.342  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_DEPLOY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest)
2022-03-03 11:52:52.342  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-03 11:52:52.342  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.342  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-33) shutting down (timeout:10s)
2022-03-03 11:52:52.344  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.344  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route33 (direct://start)
2022-03-03 11:52:52.344  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-33) shutdown in 2ms (uptime:7ms)
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.11 s - in org.apache.camel.component.casper.producer.CasperProducerWith_PUT_DEPLOY_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest
2022-03-03 11:52:52.348  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.348  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.348  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.370  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.370  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route34 (direct://start)
2022-03-03 11:52:52.370  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-34) started in 16ms (build:10ms init:5ms start:1ms)
2022-03-03 11:52:52.371 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: B083F57559F153C-0000000000000000 on ExchangeId: B083F57559F153C-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation DICTIONARY_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route34           ] [route34           ] [                                                                              ] [         1]
	...
[route34           ] [to34              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation DICTIONARY_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.getDictionayItem(CasperProducer.java:397) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:32) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest.testCallWithout_STATE_ROOT_HASH_Parameter(CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest.java:88) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:52.373  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.373  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.373  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 3ms (3 millis)
2022-03-03 11:52:52.373  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.373  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-34) shutting down (timeout:10s)
2022-03-03 11:52:52.374  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.374  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route34 (direct://start)
2022-03-03 11:52:52.374  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-34) shutdown in 1ms (uptime:5ms)
2022-03-03 11:52:52.376  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.376  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_All_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.376  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.389  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.389  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route35 (direct://start)
2022-03-03 11:52:52.389  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-35) started in 6ms (build:2ms init:3ms start:1ms)
2022-03-03 11:52:52.667  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.667  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_All_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.667  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 278ms (278 millis)
2022-03-03 11:52:52.667  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.667  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-35) shutting down (timeout:10s)
2022-03-03 11:52:52.670  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.670  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route35 (direct://start)
2022-03-03 11:52:52.670  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-35) shutdown in 3ms (uptime:282ms)
2022-03-03 11:52:52.671  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.671  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_SEED_UREF_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.671  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.686  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.686  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route36 (direct://start)
2022-03-03 11:52:52.686  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-36) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:52.687 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 65F9C50483DF4FC-0000000000000000 on ExchangeId: 65F9C50483DF4FC-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: seedUref parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route36           ] [route36           ] [                                                                              ] [         0]
	...
[route36           ] [to36              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: seedUref parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.getDictionayItem(CasperProducer.java:409) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:32) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest.testCallWithout_SEED_UREF_Parameter(CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest.java:111) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
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
2022-03-03 11:52:52.688  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.688  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_SEED_UREF_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.688  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 2ms (2 millis)
2022-03-03 11:52:52.688  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.688  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-36) shutting down (timeout:10s)
2022-03-03 11:52:52.689  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.689  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route36 (direct://start)
2022-03-03 11:52:52.689  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-36) shutdown in 1ms (uptime:4ms)
2022-03-03 11:52:52.690  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.690  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_DICTIONNARY_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.690  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.703  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.703  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route37 (direct://start)
2022-03-03 11:52:52.703  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-37) started in 9ms (build:3ms init:4ms start:2ms)
2022-03-03 11:52:52.703 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 4AB59A44357C6F1-0000000000000000 on ExchangeId: 4AB59A44357C6F1-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: dictionnary key parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route37           ] [route37           ] [                                                                              ] [         0]
	...
[route37           ] [to37              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: dictionnary key parameter is required   with endpoint operation DICTIONARY_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.getDictionayItem(CasperProducer.java:403) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:32) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest.testCallWithout_DICTIONNARY_KEY_Parameter(CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest.java:67) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:52.704  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.704  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_DICTIONNARY_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest)
2022-03-03 11:52:52.704  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-03 11:52:52.704  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.704  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-37) shutting down (timeout:10s)
2022-03-03 11:52:52.705  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:52.705  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route37 (direct://start)
2022-03-03 11:52:52.705  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-37) shutdown in 1ms (uptime:4ms)
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.337 s - in org.apache.camel.component.casper.producer.CasperProducerWith_STATE_DICTIONNARY_ITEM_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest
2022-03-03 11:52:52.707  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.707  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-03 11:52:52.707  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:52.722  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:52.722  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route38 (direct://start)
2022-03-03 11:52:52.722  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-38) started in 9ms (build:2ms init:6ms start:1ms)
2022-03-03 11:52:53.011  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.012  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_STATE_ROOT_HASH_KEY_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-03 11:52:53.012  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 289ms (289 millis)
2022-03-03 11:52:53.012  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.012  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-38) shutting down (timeout:10s)
2022-03-03 11:52:53.013  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:53.013  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route38 (direct://start)
2022-03-03 11:52:53.014  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-38) shutdown in 2ms (uptime:293ms)
2022-03-03 11:52:53.015  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.015  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-03 11:52:53.015  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.026  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:53.026  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route39 (direct://start)
2022-03-03 11:52:53.026  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-39) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:53.026 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 6C172F3A088F54B-0000000000000000 on ExchangeId: 6C172F3A088F54B-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation STATE_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route39           ] [route39           ] [                                                                              ] [         0]
	...
[route39           ] [to39              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: stateRootHash parameter is required  with endpoint operation STATE_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.storedValue(CasperProducer.java:360) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:48) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest.testCallWithout_STATE_ROOT_HASH_Parameter(CasperProducerWith_STATE_ITEM_OperationTest.java:76) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:53.027  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.027  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_STATE_ROOT_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-03 11:52:53.027  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 1ms (1 millis)
2022-03-03 11:52:53.028  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.028  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-39) shutting down (timeout:10s)
2022-03-03 11:52:53.028  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:53.029  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route39 (direct://start)
2022-03-03 11:52:53.029  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-39) shutdown in 1ms (uptime:4ms)
2022-03-03 11:52:53.031  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.031  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-03 11:52:53.032  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.048  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:53.049  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route40 (direct://start)
2022-03-03 11:52:53.049  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-40) started in 10ms (build:4ms init:4ms start:2ms)
2022-03-03 11:52:53.049 ERROR 23592 --- [           main] o.a.c.p.e.DefaultErrorHandler            : Failed delivery for (MessageId: 96598900D906A93-0000000000000000 on ExchangeId: 96598900D906A93-0000000000000000). Exhausted after delivery attempt: 1 caught: org.apache.camel.CamelExchangeException: key parameter is required   with endpoint operation STATE_ITEM. Exchange[]

Message History (complete message history is disabled)
---------------------------------------------------------------------------------------------------------------------------------------
RouteId              ProcessorId          Processor                                                                        Elapsed (ms)
[route40           ] [route40           ] [                                                                              ] [         0]
	...
[route40           ] [to40              ] [casper:http://65.108.1.10:7777                                                ] [         0]

Stacktrace
---------------------------------------------------------------------------------------------------------------------------------------


org.apache.camel.CamelExchangeException: key parameter is required   with endpoint operation STATE_ITEM. Exchange[]
	at org.apache.camel.component.casper.CasperProducer.handleError(CasperProducer.java:524) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducer.storedValue(CasperProducer.java:366) ~[classes/:?]
	at org.apache.camel.component.casper.CasperProducerInvokeOnHeaderFactory.invoke(CasperProducerInvokeOnHeaderFactory.java:48) ~[classes/:?]
	at org.apache.camel.support.HeaderSelectorProducer.process(HeaderSelectorProducer.java:181) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.SendProcessor.process(SendProcessor.java:172) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.errorhandler.RedeliveryErrorHandler$SimpleTask.run(RedeliveryErrorHandler.java:471) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor$Worker.schedule(DefaultReactiveExecutor.java:187) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultReactiveExecutor.scheduleMain(DefaultReactiveExecutor.java:64) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.processor.Pipeline.process(Pipeline.java:184) ~[camel-core-processor-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.CamelInternalProcessor.process(CamelInternalProcessor.java:398) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.direct.DirectProducer.process(DirectProducer.java:96) ~[camel-direct-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:217) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor$1.process(SharedCamelInternalProcessor.java:111) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultAsyncProcessorAwaitManager.process(DefaultAsyncProcessorAwaitManager.java:83) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.SharedCamelInternalProcessor.process(SharedCamelInternalProcessor.java:108) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.support.cache.DefaultProducerCache.send(DefaultProducerCache.java:199) ~[camel-support-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:176) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:148) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.impl.engine.DefaultProducerTemplate.send(DefaultProducerTemplate.java:462) ~[camel-base-engine-3.14.1.jar:3.14.1]
	at org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest.testCallWithout_KEY_Parameter(CasperProducerWith_STATE_ITEM_OperationTest.java:56) ~[test-classes/:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:?]
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?]
	at java.lang.reflect.Method.invoke(Method.java:566) ~[?:?]
	at org.junit.platform.commons.util.ReflectionUtils.invokeMethod(ReflectionUtils.java:725) ~[junit-platform-commons-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.execution.MethodInvocation.proceed(MethodInvocation.java:60) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$ValidatingInvocation.proceed(InvocationInterceptorChain.java:131) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.intercept(TimeoutExtension.java:149) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestableMethod(TimeoutExtension.java:140) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.extension.TimeoutExtension.interceptTestMethod(TimeoutExtension.java:84) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker$ReflectiveInterceptorCall.lambda$ofVoidMethod$0(ExecutableInvoker.java:115) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.lambda$invoke$0(ExecutableInvoker.java:105) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain$InterceptedInvocation.proceed(InvocationInterceptorChain.java:106) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.proceed(InvocationInterceptorChain.java:64) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.chainAndInvoke(InvocationInterceptorChain.java:45) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.InvocationInterceptorChain.invoke(InvocationInterceptorChain.java:37) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:104) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.execution.ExecutableInvoker.invoke(ExecutableInvoker.java:98) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.lambda$invokeTestMethod$7(TestMethodTestDescriptor.java:214) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.invokeTestMethod(TestMethodTestDescriptor.java:210) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:135) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.jupiter.engine.descriptor.TestMethodTestDescriptor.execute(TestMethodTestDescriptor.java:66) ~[junit-jupiter-engine-5.8.1.jar:5.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:151) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at java.util.ArrayList.forEach(ArrayList.java:1540) ~[?:?]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.invokeAll(SameThreadHierarchicalTestExecutorService.java:41) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$6(NodeTestTask.java:155) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$8(NodeTestTask.java:141) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.Node.around(Node.java:137) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.lambda$executeRecursively$9(NodeTestTask.java:139) ~[junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.ThrowableCollector.execute(ThrowableCollector.java:73) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.executeRecursively(NodeTestTask.java:138) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.NodeTestTask.execute(NodeTestTask.java:95) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.SameThreadHierarchicalTestExecutorService.submit(SameThreadHierarchicalTestExecutorService.java:35) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestExecutor.execute(HierarchicalTestExecutor.java:57) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.engine.support.hierarchical.HierarchicalTestEngine.execute(HierarchicalTestEngine.java:54) [junit-platform-engine-1.8.1.jar:1.8.1]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:170) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:154) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.junit.platform.launcher.core.DefaultLauncher.execute(DefaultLauncher.java:90) [junit-platform-launcher-1.2.0.jar:1.2.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invokeAllTests(JUnitPlatformProvider.java:142) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.junitplatform.JUnitPlatformProvider.invoke(JUnitPlatformProvider.java:117) [surefire-junit-platform-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.invokeProviderInSameClassLoader(ForkedBooter.java:383) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:344) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:125) [surefire-booter-2.22.0.jar:2.22.0]
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:417) [surefire-booter-2.22.0.jar:2.22.0]

2022-03-03 11:52:53.052  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.052  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_KEY_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest)
2022-03-03 11:52:53.052  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 3ms (3 millis)
2022-03-03 11:52:53.052  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.052  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-40) shutting down (timeout:10s)
2022-03-03 11:52:53.053  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:53.053  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route40 (direct://start)
2022-03-03 11:52:53.053  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-40) shutdown in 1ms (uptime:6ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.344 s - in org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ITEM_OperationTest
[INFO] Running org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest
2022-03-03 11:52:53.055  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.056  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-03 11:52:53.056  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.069  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:53.069  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route41 (direct://start)
2022-03-03 11:52:53.069  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-41) started in 9ms (build:2ms init:6ms start:1ms)
2022-03-03 11:52:53.353  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.353  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HASH_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-03 11:52:53.353  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 284ms (284 millis)
2022-03-03 11:52:53.353  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.354  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-41) shutting down (timeout:10s)
2022-03-03 11:52:53.354  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:53.354  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route41 (direct://start)
2022-03-03 11:52:53.355  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-41) shutdown in 2ms (uptime:287ms)
2022-03-03 11:52:53.356  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.356  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-03 11:52:53.356  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.367  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:53.367  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route42 (direct://start)
2022-03-03 11:52:53.367  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-42) started in 8ms (build:3ms init:4ms start:1ms)
2022-03-03 11:52:53.640  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.640  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWith_BLOCK_HEIGHT_Parameter() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-03 11:52:53.640  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 273ms (273 millis)
2022-03-03 11:52:53.640  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.640  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-42) shutting down (timeout:10s)
2022-03-03 11:52:53.641  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:53.641  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route42 (direct://start)
2022-03-03 11:52:53.642  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-42) shutdown in 2ms (uptime:276ms)
2022-03-03 11:52:53.643  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.643  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-03 11:52:53.643  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:53.659  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes startup (total:1 started:1)
2022-03-03 11:52:53.659  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Started route43 (direct://start)
2022-03-03 11:52:53.659  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-43) started in 10ms (build:2ms init:5ms start:3ms)
2022-03-03 11:52:54.205  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:54.205  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Testing done: testCallWithout_Parameters() (org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest)
2022-03-03 11:52:54.205  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : Took: 546ms (546 millis)
2022-03-03 11:52:54.205  INFO 23592 --- [           main] o.a.c.t.j.CamelTestSupport               : ********************************************************************************
2022-03-03 11:52:54.205  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-43) shutting down (timeout:10s)
2022-03-03 11:52:54.206  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Routes stopped (total:1 stopped:1)
2022-03-03 11:52:54.206  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           :     Stopped route43 (direct://start)
2022-03-03 11:52:54.206  INFO 23592 --- [           main] o.a.c.i.e.AbstractCamelContext           : Apache Camel 3.14.1 (camel-43) shutdown in 1ms (uptime:550ms)
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 1.088 s - in org.apache.camel.component.casper.producer.CasperProducerWith_STATE_ROOT_HASH_OperationTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 43, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  36.535 s
[INFO] Finished at: 2022-03-03T11:52:54-03:00
[INFO] ------------------------------------------------------------------------

Process finished with exit code 0
```