```
yusuf@ubuntu:~/crdao/ServicesDAO_VotingEngine$ ls
CONTRIBUTING.md  DAO_ReputationService  DAO_VotingEngine  docker-compose.override.yml  docker-compose.yml  Helpers  LICENSE  README.md  SECURITY.md  ServicesDAO_VotingEngine.sln  UnitTests
yusuf@ubuntu:~/crdao/ServicesDAO_VotingEngine$ docker compose up
[+] Running 0/2
 ⠿ dao_votingengine Error                                                                                                                                                                                                                           2.8s
 ⠿ dao_reputationservice Error                                                                                                                                                                                                                      2.9s
Sending build context to Docker daemon  848.5kB
Step 1/18 : FROM mcr.microsoft.com/dotnet/aspnet:3.1 AS base
 ---> 131e5408266f
Step 2/18 : WORKDIR /app
 ---> Using cache
 ---> 9b6816c77943
Step 3/18 : EXPOSE 80
 ---> Using cache
 ---> 5f5e8e0cb4d6
Step 4/18 : EXPOSE 443
 ---> Using cache
 ---> f5279272cd68
Step 5/18 : FROM mcr.microsoft.com/dotnet/sdk:3.1 AS build
 ---> 9e061f4e4e4c
Step 6/18 : WORKDIR /src
 ---> Using cache
 ---> dd8567e83b1d
Step 7/18 : COPY ["DAO_ReputationService/DAO_ReputationService.csproj", "DAO_ReputationService/"]
 ---> Using cache
 ---> fab0297b70ef
Step 8/18 : COPY ["Helpers/Helpers.csproj", "Helpers/"]
 ---> Using cache
 ---> db8690be7810
Step 9/18 : RUN dotnet restore "DAO_ReputationService/DAO_ReputationService.csproj"
 ---> Running in 533ede6a5b82
  Determining projects to restore...
  Restored /src/Helpers/Helpers.csproj (in 30.15 sec).
  Restored /src/DAO_ReputationService/DAO_ReputationService.csproj (in 30.15 sec).
Removing intermediate container 533ede6a5b82
 ---> 49797b5bd312
Step 10/18 : COPY . .
 ---> 8f2cc5659b10
Step 11/18 : WORKDIR "/src/DAO_ReputationService"
 ---> Running in 852fe41829e3
Removing intermediate container 852fe41829e3
 ---> 7479a5e851bf
Step 12/18 : RUN dotnet build "DAO_ReputationService.csproj" -c Release -o /app/build
 ---> Running in 8161f09938f1
Microsoft (R) Build Engine version 16.7.2+b60ddb6f4 for .NET
Copyright (C) Microsoft Corporation. All rights reserved.

  Determining projects to restore...
  All projects are up-to-date for restore.
  Helpers -> /app/build/Helpers.dll
  DAO_ReputationService -> /app/build/DAO_ReputationService.dll

Build succeeded.
    0 Warning(s)
    0 Error(s)

Time Elapsed 00:00:01.69
Removing intermediate container 8161f09938f1
 ---> 9fb7f35c2b6f
Step 13/18 : FROM build AS publish
 ---> 9fb7f35c2b6f
Step 14/18 : RUN dotnet publish "DAO_ReputationService.csproj" -c Release -o /app/publish
 ---> Running in 79c1497d9eec
Microsoft (R) Build Engine version 16.7.2+b60ddb6f4 for .NET
Copyright (C) Microsoft Corporation. All rights reserved.

  Determining projects to restore...
  All projects are up-to-date for restore.
  Helpers -> /src/Helpers/bin/Release/netcoreapp3.1/Helpers.dll
  DAO_ReputationService -> /src/DAO_ReputationService/bin/Release/netcoreapp3.1/DAO_ReputationService.dll
  DAO_ReputationService -> /app/publish/
Removing intermediate container 79c1497d9eec
 ---> aef843b64729
Step 15/18 : FROM base AS final
 ---> f5279272cd68
Step 16/18 : WORKDIR /app
 ---> Using cache
 ---> 3afcb592ccf8
Step 17/18 : COPY --from=publish /app/publish .
 ---> 1b31c6035fa2
Step 18/18 : ENTRYPOINT ["dotnet", "DAO_ReputationService.dll"]
 ---> Running in ef4603b4af36
Removing intermediate container ef4603b4af36
 ---> fa5ac2a6705a
Successfully built fa5ac2a6705a
Successfully tagged daoreputationservice:latest
Sending build context to Docker daemon  848.5kB
Step 1/17 : FROM mcr.microsoft.com/dotnet/aspnet:3.1 AS base
 ---> 131e5408266f
Step 2/17 : WORKDIR /app
 ---> Using cache
 ---> 9b6816c77943
Step 3/17 : EXPOSE 80
 ---> Using cache
 ---> 5f5e8e0cb4d6
Step 4/17 : EXPOSE 443
 ---> Using cache
 ---> f5279272cd68
Step 5/17 : FROM mcr.microsoft.com/dotnet/sdk:3.1 AS build
 ---> 9e061f4e4e4c
Step 6/17 : WORKDIR /src
 ---> Using cache
 ---> dd8567e83b1d
Step 7/17 : COPY ["DAO_VotingEngine/DAO_VotingEngine.csproj", "DAO_VotingEngine/"]
 ---> 41c611ae9528
Step 8/17 : RUN dotnet restore "DAO_VotingEngine/DAO_VotingEngine.csproj"
 ---> Running in 284493efbe0e
  Determining projects to restore...
  Skipping project "/src/Helpers/Helpers.csproj" because it was not found.
  Skipping project "/src/Helpers/Helpers.csproj" because it was not found.
  Restored /src/DAO_VotingEngine/DAO_VotingEngine.csproj (in 28.14 sec).
Removing intermediate container 284493efbe0e
 ---> aad1e6ed39f1
Step 9/17 : COPY . .
 ---> cfbec57d1d74
Step 10/17 : WORKDIR "/src/DAO_VotingEngine"
 ---> Running in 823dd17f3b46
Removing intermediate container 823dd17f3b46
 ---> 6b3161e9b029
Step 11/17 : RUN dotnet build "DAO_VotingEngine.csproj" -c Release -o /app/build
 ---> Running in fe0663983d75
Microsoft (R) Build Engine version 16.7.2+b60ddb6f4 for .NET
Copyright (C) Microsoft Corporation. All rights reserved.

  Determining projects to restore...
  Restored /src/DAO_VotingEngine/DAO_VotingEngine.csproj (in 12.66 sec).
  Restored /src/Helpers/Helpers.csproj (in 12.66 sec).
  Helpers -> /app/build/Helpers.dll
  DAO_VotingEngine -> /app/build/DAO_VotingEngine.dll

Build succeeded.
    0 Warning(s)
    0 Error(s)

Time Elapsed 00:00:14.23
Removing intermediate container fe0663983d75
 ---> bb18be28a3f4
Step 12/17 : FROM build AS publish
 ---> bb18be28a3f4
Step 13/17 : RUN dotnet publish "DAO_VotingEngine.csproj" -c Release -o /app/publish
 ---> Running in 37745ba3113a
Microsoft (R) Build Engine version 16.7.2+b60ddb6f4 for .NET
Copyright (C) Microsoft Corporation. All rights reserved.

  Determining projects to restore...
  All projects are up-to-date for restore.
  Helpers -> /src/Helpers/bin/Release/netcoreapp3.1/Helpers.dll
  DAO_VotingEngine -> /src/DAO_VotingEngine/bin/Release/netcoreapp3.1/DAO_VotingEngine.dll
  DAO_VotingEngine -> /app/publish/
Removing intermediate container 37745ba3113a
 ---> 43ceb7c2b4bf
Step 14/17 : FROM base AS final
 ---> f5279272cd68
Step 15/17 : WORKDIR /app
 ---> Using cache
 ---> 3afcb592ccf8
Step 16/17 : COPY --from=publish /app/publish .
 ---> e50aa851241a
Step 17/17 : ENTRYPOINT ["dotnet", "DAO_VotingEngine.dll"]
 ---> Running in 3a45f430aae6
Removing intermediate container 3a45f430aae6
 ---> 28a9a1c631d9
Successfully built 28a9a1c631d9
Successfully tagged daovotingengine:latest
[+] Running 6/6
 ⠿ Volume "servicesdao_votingengine_reputation_datafiles"      Created                                                                                                                                                                              0.0s
 ⠿ Volume "servicesdao_votingengine_vote_datafiles"            Created                                                                                                                                                                              0.0s
 ⠿ Container servicesdao_votingengine-dao_votingengine-1       Created                                                                                                                                                                              0.0s
 ⠿ Container servicesdao_votingengine-dao_reputationservice-1  Created                                                                                                                                                                              0.0s
 ⠿ Container servicesdao_votingengine-dao_votedb-1             Created                                                                                                                                                                              0.0s
 ⠿ Container servicesdao_votingengine-dao_reputationdb-1       Created                                                                                                                                                                              0.0s
Attaching to servicesdao_votingengine-dao_reputationdb-1, servicesdao_votingengine-dao_reputationservice-1, servicesdao_votingengine-dao_votedb-1, servicesdao_votingengine-dao_votingengine-1
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Initializing database files
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:31.990331Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:31+00:00 [Note] [Entrypoint]: Initializing database files
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.004771Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.164058Z 0 [Warning] InnoDB: New log files created, LSN=45790
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.164047Z 0 [Warning] InnoDB: New log files created, LSN=45790
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.192653Z 0 [Warning] InnoDB: Creating foreign key constraint system tables.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.192628Z 0 [Warning] InnoDB: Creating foreign key constraint system tables.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.246568Z 0 [Warning] No existing UUID has been found, so we assume that this is the first time that this server has been started. Generating a new UUID: 4a2ce764-c3b9-11ec-b2f2-0242ac120004.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.246568Z 0 [Warning] No existing UUID has been found, so we assume that this is the first time that this server has been started. Generating a new UUID: 4a2ce764-c3b9-11ec-9acf-0242ac120005.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.247466Z 0 [Warning] Gtid table is not ready to be used. Table 'mysql.gtid_executed' cannot be opened.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.247486Z 0 [Warning] Gtid table is not ready to be used. Table 'mysql.gtid_executed' cannot be opened.
servicesdao_votingengine-dao_reputationservice-1  | crit: Microsoft.AspNetCore.Hosting.Diagnostics[6]
servicesdao_votingengine-dao_reputationservice-1  |       Application startup exception
servicesdao_votingengine-dao_reputationservice-1  | System.InvalidOperationException: An exception has been raised that is likely due to a transient failure. Consider enabling transient error resiliency by adding 'EnableRetryOnFailure()' to the 'UseMySql' call.
servicesdao_votingengine-dao_reputationservice-1  |  ---> MySql.Data.MySqlClient.MySqlException (0x80004005): Unable to connect to any of the specified MySQL hosts.
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.AggregateException: One or more errors occurred. (Connection refused 172.18.0.5:3306)
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.Net.Internals.SocketExceptionFactory+ExtendedSocketException (111): Connection refused 172.18.0.5:3306
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.MultipleAddressConnectCallback(IAsyncResult result)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.<>c.<ConnectAsync>b__28_1(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.TaskFactory`1.FromAsyncCoreLogic(IAsyncResult iar, Func`2 endFunction, Action`1 endAction, Task`1 promise, Boolean requiresSynchronization)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetTcpStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Create(MySqlConnectionStringBuilder settings)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.CreateNewPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.TryToGetDriver()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlConnection.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.<>c__DisplayClass18_0.<Exists>b__0(DateTime giveUp)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.<>c__DisplayClass12_0`2.<Execute>b__0(DbContext c, TState s)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation, Func`2 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists(Boolean retryOnNotExists)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.HistoryRepository.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.Internal.Migrator.Migrate(String targetMigration)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.RelationalDatabaseFacadeExtensions.Migrate(DatabaseFacade databaseFacade)
servicesdao_votingengine-dao_reputationservice-1  |    at DAO_ReputationService.Startup.Configure(IApplicationBuilder app, IWebHostEnvironment env) in /src/DAO_ReputationService/Startup.cs:line 112
servicesdao_votingengine-dao_reputationservice-1  |    at System.RuntimeMethodHandle.InvokeMethod(Object target, Object[] arguments, Signature sig, Boolean constructor, Boolean wrapExceptions)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Reflection.RuntimeMethodInfo.Invoke(Object obj, BindingFlags invokeAttr, Binder binder, Object[] parameters, CultureInfo culture)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.Invoke(Object instance, IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.<>c__DisplayClass4_0.<Build>b__0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostBuilder.<>c__DisplayClass13_0.<UseStartup>b__2(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Mvc.Filters.MiddlewareFilterBuilderStartupFilter.<>c__DisplayClass0_0.<Configure>g__MiddlewareFilterBuilder|0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.HostFilteringStartupFilter.<>c__DisplayClass0_0.<Configure>b__0(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostService.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  | Unhandled exception. System.InvalidOperationException: An exception has been raised that is likely due to a transient failure. Consider enabling transient error resiliency by adding 'EnableRetryOnFailure()' to the 'UseMySql' call.
servicesdao_votingengine-dao_reputationservice-1  |  ---> MySql.Data.MySqlClient.MySqlException (0x80004005): Unable to connect to any of the specified MySQL hosts.
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.AggregateException: One or more errors occurred. (Connection refused 172.18.0.5:3306)
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.Net.Internals.SocketExceptionFactory+ExtendedSocketException (111): Connection refused 172.18.0.5:3306
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.MultipleAddressConnectCallback(IAsyncResult result)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.<>c.<ConnectAsync>b__28_1(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.TaskFactory`1.FromAsyncCoreLogic(IAsyncResult iar, Func`2 endFunction, Action`1 endAction, Task`1 promise, Boolean requiresSynchronization)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetTcpStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Create(MySqlConnectionStringBuilder settings)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.CreateNewPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.TryToGetDriver()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlConnection.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.<>c__DisplayClass18_0.<Exists>b__0(DateTime giveUp)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.<>c__DisplayClass12_0`2.<Execute>b__0(DbContext c, TState s)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation, Func`2 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists(Boolean retryOnNotExists)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.HistoryRepository.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.Internal.Migrator.Migrate(String targetMigration)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.RelationalDatabaseFacadeExtensions.Migrate(DatabaseFacade databaseFacade)
servicesdao_votingengine-dao_reputationservice-1  |    at DAO_ReputationService.Startup.Configure(IApplicationBuilder app, IWebHostEnvironment env) in /src/DAO_ReputationService/Startup.cs:line 112
servicesdao_votingengine-dao_reputationservice-1  |    at System.RuntimeMethodHandle.InvokeMethod(Object target, Object[] arguments, Signature sig, Boolean constructor, Boolean wrapExceptions)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Reflection.RuntimeMethodInfo.Invoke(Object obj, BindingFlags invokeAttr, Binder binder, Object[] parameters, CultureInfo culture)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.Invoke(Object instance, IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.<>c__DisplayClass4_0.<Build>b__0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostBuilder.<>c__DisplayClass13_0.<UseStartup>b__2(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Mvc.Filters.MiddlewareFilterBuilderStartupFilter.<>c__DisplayClass0_0.<Configure>g__MiddlewareFilterBuilder|0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.HostFilteringStartupFilter.<>c__DisplayClass0_0.<Configure>b__0(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostService.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.Internal.Host.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.RunAsync(IHost host, CancellationToken token)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.RunAsync(IHost host, CancellationToken token)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.Run(IHost host)
servicesdao_votingengine-dao_reputationservice-1  |    at DAO_ReputationService.Program.Main(String[] args) in /src/DAO_ReputationService/Program.cs:line 32
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.576394Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.576413Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.576657Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao_votingengine-dao_votingengine-1       | crit: Microsoft.AspNetCore.Hosting.Diagnostics[6]
servicesdao_votingengine-dao_votingengine-1       |       Application startup exception
servicesdao_votingengine-dao_votingengine-1       | System.InvalidOperationException: An exception has been raised that is likely due to a transient failure. Consider enabling transient error resiliency by adding 'EnableRetryOnFailure()' to the 'UseMySql' call.
servicesdao_votingengine-dao_votingengine-1       |  ---> MySql.Data.MySqlClient.MySqlException (0x80004005): Unable to connect to any of the specified MySQL hosts.
servicesdao_votingengine-dao_votingengine-1       |  ---> System.AggregateException: One or more errors occurred. (Connection refused 172.18.0.4:3306)
servicesdao_votingengine-dao_votingengine-1       |  ---> System.Net.Internals.SocketExceptionFactory+ExtendedSocketException (111): Connection refused 172.18.0.4:3306
servicesdao_votingengine-dao_votingengine-1       |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_votingengine-1       | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_votingengine-1       |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.MultipleAddressConnectCallback(IAsyncResult result)
servicesdao_votingengine-dao_votingengine-1       | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_votingengine-1       |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.TcpClient.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.TcpClient.<>c.<ConnectAsync>b__28_1(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Threading.Tasks.TaskFactory`1.FromAsyncCoreLogic(IAsyncResult iar, Func`2 endFunction, Action`1 endAction, Task`1 promise, Boolean requiresSynchronization)
servicesdao_votingengine-dao_votingengine-1       |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_votingengine-1       |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
servicesdao_votingengine-dao_votingengine-1       |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.Common.StreamCreator.GetTcpStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.Common.StreamCreator.GetStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.Driver.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.Driver.Create(MySqlConnectionStringBuilder settings)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.CreateNewPooledConnection()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.GetPooledConnection()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.TryToGetDriver()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.GetConnection()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlConnection.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.<>c__DisplayClass18_0.<Exists>b__0(DateTime giveUp)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.<>c__DisplayClass12_0`2.<Execute>b__0(DbContext c, TState s)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_votingengine-1       |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation, Func`2 verifySucceeded)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists(Boolean retryOnNotExists)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists()
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.Migrations.HistoryRepository.Exists()
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.Migrations.Internal.Migrator.Migrate(String targetMigration)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.RelationalDatabaseFacadeExtensions.Migrate(DatabaseFacade databaseFacade)
servicesdao_votingengine-dao_votingengine-1       |    at DAO_VotingEngine.Startup.Configure(IApplicationBuilder app, IWebHostEnvironment env) in /src/DAO_VotingEngine/Startup.cs:line 109
servicesdao_votingengine-dao_votingengine-1       |    at System.RuntimeMethodHandle.InvokeMethod(Object target, Object[] arguments, Signature sig, Boolean constructor, Boolean wrapExceptions)
servicesdao_votingengine-dao_votingengine-1       |    at System.Reflection.RuntimeMethodInfo.Invoke(Object obj, BindingFlags invokeAttr, Binder binder, Object[] parameters, CultureInfo culture)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.Invoke(Object instance, IApplicationBuilder builder)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.<>c__DisplayClass4_0.<Build>b__0(IApplicationBuilder builder)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.GenericWebHostBuilder.<>c__DisplayClass13_0.<UseStartup>b__2(IApplicationBuilder app)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Mvc.Filters.MiddlewareFilterBuilderStartupFilter.<>c__DisplayClass0_0.<Configure>g__MiddlewareFilterBuilder|0(IApplicationBuilder builder)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.HostFilteringStartupFilter.<>c__DisplayClass0_0.<Configure>b__0(IApplicationBuilder app)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.GenericWebHostService.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_votingengine-1       | Unhandled exception. System.InvalidOperationException: An exception has been raised that is likely due to a transient failure. Consider enabling transient error resiliency by adding 'EnableRetryOnFailure()' to the 'UseMySql' call.
servicesdao_votingengine-dao_votingengine-1       |  ---> MySql.Data.MySqlClient.MySqlException (0x80004005): Unable to connect to any of the specified MySQL hosts.
servicesdao_votingengine-dao_votingengine-1       |  ---> System.AggregateException: One or more errors occurred. (Connection refused 172.18.0.4:3306)
servicesdao_votingengine-dao_votingengine-1       |  ---> System.Net.Internals.SocketExceptionFactory+ExtendedSocketException (111): Connection refused 172.18.0.4:3306
servicesdao_votingengine-dao_votingengine-1       |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_votingengine-1       | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_votingengine-1       |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.MultipleAddressConnectCallback(IAsyncResult result)
servicesdao_votingengine-dao_votingengine-1       | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_votingengine-1       |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.TcpClient.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Net.Sockets.TcpClient.<>c.<ConnectAsync>b__28_1(IAsyncResult asyncResult)
servicesdao_votingengine-dao_votingengine-1       |    at System.Threading.Tasks.TaskFactory`1.FromAsyncCoreLogic(IAsyncResult iar, Func`2 endFunction, Action`1 endAction, Task`1 promise, Boolean requiresSynchronization)
servicesdao_votingengine-dao_votingengine-1       |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_votingengine-1       |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
servicesdao_votingengine-dao_votingengine-1       |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.Common.StreamCreator.GetTcpStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.Common.StreamCreator.GetStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.Driver.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.Driver.Create(MySqlConnectionStringBuilder settings)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.CreateNewPooledConnection()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.GetPooledConnection()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.TryToGetDriver()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlPool.GetConnection()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.Data.MySqlClient.MySqlConnection.Open()
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.<>c__DisplayClass18_0.<Exists>b__0(DateTime giveUp)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.<>c__DisplayClass12_0`2.<Execute>b__0(DbContext c, TState s)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_votingengine-1       |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation, Func`2 verifySucceeded)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists(Boolean retryOnNotExists)
servicesdao_votingengine-dao_votingengine-1       |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists()
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.Migrations.HistoryRepository.Exists()
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.Migrations.Internal.Migrator.Migrate(String targetMigration)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.EntityFrameworkCore.RelationalDatabaseFacadeExtensions.Migrate(DatabaseFacade databaseFacade)
servicesdao_votingengine-dao_votingengine-1       |    at DAO_VotingEngine.Startup.Configure(IApplicationBuilder app, IWebHostEnvironment env) in /src/DAO_VotingEngine/Startup.cs:line 109
servicesdao_votingengine-dao_votingengine-1       |    at System.RuntimeMethodHandle.InvokeMethod(Object target, Object[] arguments, Signature sig, Boolean constructor, Boolean wrapExceptions)
servicesdao_votingengine-dao_votingengine-1       |    at System.Reflection.RuntimeMethodInfo.Invoke(Object obj, BindingFlags invokeAttr, Binder binder, Object[] parameters, CultureInfo culture)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.Invoke(Object instance, IApplicationBuilder builder)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.<>c__DisplayClass4_0.<Build>b__0(IApplicationBuilder builder)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.GenericWebHostBuilder.<>c__DisplayClass13_0.<UseStartup>b__2(IApplicationBuilder app)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Mvc.Filters.MiddlewareFilterBuilderStartupFilter.<>c__DisplayClass0_0.<Configure>g__MiddlewareFilterBuilder|0(IApplicationBuilder builder)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.HostFilteringStartupFilter.<>c__DisplayClass0_0.<Configure>b__0(IApplicationBuilder app)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.AspNetCore.Hosting.GenericWebHostService.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.Extensions.Hosting.Internal.Host.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.RunAsync(IHost host, CancellationToken token)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.RunAsync(IHost host, CancellationToken token)
servicesdao_votingengine-dao_votingengine-1       |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.Run(IHost host)
servicesdao_votingengine-dao_votingengine-1       |    at DAO_VotingEngine.Program.Main(String[] args) in /src/DAO_VotingEngine/Program.cs:line 34
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.696532Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.696560Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.696804Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:32.727537Z 1 [Warning] root@localhost is created with an empty password ! Please consider switching off the --initialize-insecure option.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:32.776225Z 1 [Warning] root@localhost is created with an empty password ! Please consider switching off the --initialize-insecure option.
servicesdao_votingengine-dao_reputationservice-1 exited with code 139
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:34+00:00 [Note] [Entrypoint]: Database files initialized
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:34+00:00 [Note] [Entrypoint]: Starting temporary server
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:34+00:00 [Note] [Entrypoint]: Waiting for server startup
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:34+00:00 [Note] [Entrypoint]: Database files initialized
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:34+00:00 [Note] [Entrypoint]: Starting temporary server
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:34+00:00 [Note] [Entrypoint]: Waiting for server startup
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.041248Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.042457Z 0 [Note] mysqld (mysqld 5.7.37) starting as process 78 ...
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044501Z 0 [Note] InnoDB: PUNCH HOLE support available
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044515Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044516Z 0 [Note] InnoDB: Uses event mutexes
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044517Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044518Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044520Z 0 [Note] InnoDB: Using Linux native AIO
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044731Z 0 [Note] InnoDB: Number of pools: 1
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.044816Z 0 [Note] InnoDB: Using CPU crc32 instructions
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.046016Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.050378Z 0 [Note] InnoDB: Completed initialization of buffer pool
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.052137Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.052096Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.053294Z 0 [Note] mysqld (mysqld 5.7.37) starting as process 79 ...
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.054951Z 0 [Note] InnoDB: PUNCH HOLE support available
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055007Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055018Z 0 [Note] InnoDB: Uses event mutexes
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055025Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055032Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055040Z 0 [Note] InnoDB: Using Linux native AIO
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055169Z 0 [Note] InnoDB: Number of pools: 1
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.055267Z 0 [Note] InnoDB: Using CPU crc32 instructions
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.056279Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.060443Z 0 [Note] InnoDB: Completed initialization of buffer pool
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.061758Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.063703Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.068010Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.068039Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.073354Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.082919Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.083033Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.083209Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.083675Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.083694Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.084057Z 0 [Note] InnoDB: Waiting for purge to start
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.096094Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.096652Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.096696Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.097372Z 0 [Note] InnoDB: 5.7.37 started; log sequence number 2749976
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.097720Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.098148Z 0 [Note] Plugin 'FEDERATED' is disabled.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.098843Z 0 [Note] InnoDB: Buffer pool(s) load completed at 220424 10:28:35
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.102279Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.102324Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.102334Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.102341Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.103338Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.103384Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.104464Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.108533Z 0 [Note] Event Scheduler: Loaded 0 events
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:35.108848Z 0 [Note] mysqld: ready for connections.
servicesdao_votingengine-dao_reputationdb-1       | Version: '5.7.37'  socket: '/var/run/mysqld/mysqld.sock'  port: 0  MySQL Community Server (GPL)
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.134384Z 0 [Note] InnoDB: 5.7.37 started; log sequence number 2749976
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.134765Z 0 [Note] Plugin 'FEDERATED' is disabled.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.135051Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.136019Z 0 [Note] InnoDB: Buffer pool(s) load completed at 220424 10:28:35
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.138875Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.138908Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.138911Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.138912Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.139294Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.139330Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.140411Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.144978Z 0 [Note] Event Scheduler: Loaded 0 events
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:35.145325Z 0 [Note] mysqld: ready for connections.
servicesdao_votingengine-dao_votedb-1             | Version: '5.7.37'  socket: '/var/run/mysqld/mysqld.sock'  port: 0  MySQL Community Server (GPL)
servicesdao_votingengine-dao_reputationservice-1  | crit: Microsoft.AspNetCore.Hosting.Diagnostics[6]
servicesdao_votingengine-dao_reputationservice-1  |       Application startup exception
servicesdao_votingengine-dao_reputationservice-1  | System.InvalidOperationException: An exception has been raised that is likely due to a transient failure. Consider enabling transient error resiliency by adding 'EnableRetryOnFailure()' to the 'UseMySql' call.
servicesdao_votingengine-dao_reputationservice-1  |  ---> MySql.Data.MySqlClient.MySqlException (0x80004005): Unable to connect to any of the specified MySQL hosts.
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.AggregateException: One or more errors occurred. (Connection refused 172.18.0.5:3306)
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.Net.Internals.SocketExceptionFactory+ExtendedSocketException (111): Connection refused 172.18.0.5:3306
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.MultipleAddressConnectCallback(IAsyncResult result)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.<>c.<ConnectAsync>b__28_1(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.TaskFactory`1.FromAsyncCoreLogic(IAsyncResult iar, Func`2 endFunction, Action`1 endAction, Task`1 promise, Boolean requiresSynchronization)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetTcpStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Create(MySqlConnectionStringBuilder settings)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.CreateNewPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.TryToGetDriver()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlConnection.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.<>c__DisplayClass18_0.<Exists>b__0(DateTime giveUp)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.<>c__DisplayClass12_0`2.<Execute>b__0(DbContext c, TState s)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation, Func`2 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists(Boolean retryOnNotExists)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.HistoryRepository.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.Internal.Migrator.Migrate(String targetMigration)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.RelationalDatabaseFacadeExtensions.Migrate(DatabaseFacade databaseFacade)
servicesdao_votingengine-dao_reputationservice-1  |    at DAO_ReputationService.Startup.Configure(IApplicationBuilder app, IWebHostEnvironment env) in /src/DAO_ReputationService/Startup.cs:line 112
servicesdao_votingengine-dao_reputationservice-1  |    at System.RuntimeMethodHandle.InvokeMethod(Object target, Object[] arguments, Signature sig, Boolean constructor, Boolean wrapExceptions)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Reflection.RuntimeMethodInfo.Invoke(Object obj, BindingFlags invokeAttr, Binder binder, Object[] parameters, CultureInfo culture)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.Invoke(Object instance, IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.<>c__DisplayClass4_0.<Build>b__0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostBuilder.<>c__DisplayClass13_0.<UseStartup>b__2(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Mvc.Filters.MiddlewareFilterBuilderStartupFilter.<>c__DisplayClass0_0.<Configure>g__MiddlewareFilterBuilder|0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.HostFilteringStartupFilter.<>c__DisplayClass0_0.<Configure>b__0(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostService.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  | Unhandled exception. System.InvalidOperationException: An exception has been raised that is likely due to a transient failure. Consider enabling transient error resiliency by adding 'EnableRetryOnFailure()' to the 'UseMySql' call.
servicesdao_votingengine-dao_reputationservice-1  |  ---> MySql.Data.MySqlClient.MySqlException (0x80004005): Unable to connect to any of the specified MySQL hosts.
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.AggregateException: One or more errors occurred. (Connection refused 172.18.0.5:3306)
servicesdao_votingengine-dao_reputationservice-1  |  ---> System.Net.Internals.SocketExceptionFactory+ExtendedSocketException (111): Connection refused 172.18.0.5:3306
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.DoMultipleAddressConnectCallback(Object result, MultipleAddressConnectAsyncResult context)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.MultipleAddressConnectCallback(IAsyncResult result)
servicesdao_votingengine-dao_reputationservice-1  | --- End of stack trace from previous location where exception was thrown ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw(Exception source)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.Socket.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.EndConnect(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Net.Sockets.TcpClient.<>c.<ConnectAsync>b__28_1(IAsyncResult asyncResult)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.TaskFactory`1.FromAsyncCoreLogic(IAsyncResult iar, Func`2 endFunction, Action`1 endAction, Task`1 promise, Boolean requiresSynchronization)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetTcpStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.Common.StreamCreator.GetStream(MySqlConnectionStringBuilder settings, MyNetworkStream& networkStream)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.NativeDriver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.Driver.Create(MySqlConnectionStringBuilder settings)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.CreateNewPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetPooledConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.TryToGetDriver()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlPool.GetConnection()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.Data.MySqlClient.MySqlConnection.Open()
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.<>c__DisplayClass18_0.<Exists>b__0(DateTime giveUp)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.<>c__DisplayClass12_0`2.<Execute>b__0(DbContext c, TState s)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    --- End of inner exception stack trace ---
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.Storage.Internal.MySQLExecutionStrategy.Execute[TState,TResult](TState state, Func`3 operation, Func`3 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation, Func`2 verifySucceeded)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.ExecutionStrategyExtensions.Execute[TState,TResult](IExecutionStrategy strategy, TState state, Func`2 operation)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists(Boolean retryOnNotExists)
servicesdao_votingengine-dao_reputationservice-1  |    at MySql.EntityFrameworkCore.MySQLDatabaseCreator.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.HistoryRepository.Exists()
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.Migrations.Internal.Migrator.Migrate(String targetMigration)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.EntityFrameworkCore.RelationalDatabaseFacadeExtensions.Migrate(DatabaseFacade databaseFacade)
servicesdao_votingengine-dao_reputationservice-1  |    at DAO_ReputationService.Startup.Configure(IApplicationBuilder app, IWebHostEnvironment env) in /src/DAO_ReputationService/Startup.cs:line 112
servicesdao_votingengine-dao_reputationservice-1  |    at System.RuntimeMethodHandle.InvokeMethod(Object target, Object[] arguments, Signature sig, Boolean constructor, Boolean wrapExceptions)
servicesdao_votingengine-dao_reputationservice-1  |    at System.Reflection.RuntimeMethodInfo.Invoke(Object obj, BindingFlags invokeAttr, Binder binder, Object[] parameters, CultureInfo culture)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.Invoke(Object instance, IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.ConfigureBuilder.<>c__DisplayClass4_0.<Build>b__0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostBuilder.<>c__DisplayClass13_0.<UseStartup>b__2(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Mvc.Filters.MiddlewareFilterBuilderStartupFilter.<>c__DisplayClass0_0.<Configure>g__MiddlewareFilterBuilder|0(IApplicationBuilder builder)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.HostFilteringStartupFilter.<>c__DisplayClass0_0.<Configure>b__0(IApplicationBuilder app)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.AspNetCore.Hosting.GenericWebHostService.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.Internal.Host.StartAsync(CancellationToken cancellationToken)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.RunAsync(IHost host, CancellationToken token)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.RunAsync(IHost host, CancellationToken token)
servicesdao_votingengine-dao_reputationservice-1  |    at Microsoft.Extensions.Hosting.HostingAbstractionsHostExtensions.Run(IHost host)
servicesdao_votingengine-dao_reputationservice-1  |    at DAO_ReputationService.Program.Main(String[] args) in /src/DAO_ReputationService/Program.cs:line 32
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:35+00:00 [Note] [Entrypoint]: Temporary server started.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:35+00:00 [Note] [Entrypoint]: Temporary server started.
servicesdao_votingengine-dao_votedb-1             | Warning: Unable to load '/usr/share/zoneinfo/iso3166.tab' as time zone. Skipping it.
servicesdao_votingengine-dao_votedb-1             | Warning: Unable to load '/usr/share/zoneinfo/leap-seconds.list' as time zone. Skipping it.
servicesdao_votingengine-dao_reputationdb-1       | Warning: Unable to load '/usr/share/zoneinfo/iso3166.tab' as time zone. Skipping it.
servicesdao_votingengine-dao_reputationdb-1       | Warning: Unable to load '/usr/share/zoneinfo/leap-seconds.list' as time zone. Skipping it.
servicesdao_votingengine-dao_votedb-1             | Warning: Unable to load '/usr/share/zoneinfo/zone.tab' as time zone. Skipping it.
servicesdao_votingengine-dao_votedb-1             | Warning: Unable to load '/usr/share/zoneinfo/zone1970.tab' as time zone. Skipping it.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:36+00:00 [Note] [Entrypoint]: Creating database daovotedb
servicesdao_votingengine-dao_votedb-1             | 
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:36+00:00 [Note] [Entrypoint]: Stopping temporary server
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.944609Z 0 [Note] Giving 0 client threads a chance to die gracefully
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.944638Z 0 [Note] Shutting down slave threads
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.944641Z 0 [Note] Forcefully disconnecting 0 remaining clients
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.944645Z 0 [Note] Event Scheduler: Purging the queue. 0 events
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.944690Z 0 [Note] Binlog end
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945173Z 0 [Note] Shutting down plugin 'ngram'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945189Z 0 [Note] Shutting down plugin 'partition'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945192Z 0 [Note] Shutting down plugin 'BLACKHOLE'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945193Z 0 [Note] Shutting down plugin 'ARCHIVE'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945194Z 0 [Note] Shutting down plugin 'PERFORMANCE_SCHEMA'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945216Z 0 [Note] Shutting down plugin 'MRG_MYISAM'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945218Z 0 [Note] Shutting down plugin 'MyISAM'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945222Z 0 [Note] Shutting down plugin 'INNODB_SYS_VIRTUAL'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945223Z 0 [Note] Shutting down plugin 'INNODB_SYS_DATAFILES'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945224Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLESPACES'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945225Z 0 [Note] Shutting down plugin 'INNODB_SYS_FOREIGN_COLS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945225Z 0 [Note] Shutting down plugin 'INNODB_SYS_FOREIGN'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945226Z 0 [Note] Shutting down plugin 'INNODB_SYS_FIELDS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945227Z 0 [Note] Shutting down plugin 'INNODB_SYS_COLUMNS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945227Z 0 [Note] Shutting down plugin 'INNODB_SYS_INDEXES'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945228Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLESTATS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945228Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLES'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945229Z 0 [Note] Shutting down plugin 'INNODB_FT_INDEX_TABLE'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945230Z 0 [Note] Shutting down plugin 'INNODB_FT_INDEX_CACHE'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945230Z 0 [Note] Shutting down plugin 'INNODB_FT_CONFIG'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945231Z 0 [Note] Shutting down plugin 'INNODB_FT_BEING_DELETED'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945386Z 0 [Note] Shutting down plugin 'INNODB_FT_DELETED'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945396Z 0 [Note] Shutting down plugin 'INNODB_FT_DEFAULT_STOPWORD'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945420Z 0 [Note] Shutting down plugin 'INNODB_METRICS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945421Z 0 [Note] Shutting down plugin 'INNODB_TEMP_TABLE_INFO'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945422Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_POOL_STATS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945422Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_PAGE_LRU'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945423Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_PAGE'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945424Z 0 [Note] Shutting down plugin 'INNODB_CMP_PER_INDEX_RESET'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945424Z 0 [Note] Shutting down plugin 'INNODB_CMP_PER_INDEX'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945425Z 0 [Note] Shutting down plugin 'INNODB_CMPMEM_RESET'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945426Z 0 [Note] Shutting down plugin 'INNODB_CMPMEM'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945426Z 0 [Note] Shutting down plugin 'INNODB_CMP_RESET'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945427Z 0 [Note] Shutting down plugin 'INNODB_CMP'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945428Z 0 [Note] Shutting down plugin 'INNODB_LOCK_WAITS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945428Z 0 [Note] Shutting down plugin 'INNODB_LOCKS'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945429Z 0 [Note] Shutting down plugin 'INNODB_TRX'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945430Z 0 [Note] Shutting down plugin 'InnoDB'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945613Z 0 [Note] InnoDB: FTS optimize thread exiting.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:36.945865Z 0 [Note] InnoDB: Starting shutdown...
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.047069Z 0 [Note] InnoDB: Dumping buffer pool(s) to /var/lib/mysql/ib_buffer_pool
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.047305Z 0 [Note] InnoDB: Buffer pool(s) dump completed at 220424 10:28:37
servicesdao_votingengine-dao_reputationdb-1       | Warning: Unable to load '/usr/share/zoneinfo/zone.tab' as time zone. Skipping it.
servicesdao_votingengine-dao_reputationdb-1       | Warning: Unable to load '/usr/share/zoneinfo/zone1970.tab' as time zone. Skipping it.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:37+00:00 [Note] [Entrypoint]: Creating database daoreputationdb
servicesdao_votingengine-dao_reputationdb-1       | 
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:37+00:00 [Note] [Entrypoint]: Stopping temporary server
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280134Z 0 [Note] Giving 0 client threads a chance to die gracefully
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280185Z 0 [Note] Shutting down slave threads
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280198Z 0 [Note] Forcefully disconnecting 0 remaining clients
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280207Z 0 [Note] Event Scheduler: Purging the queue. 0 events
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280268Z 0 [Note] Binlog end
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280871Z 0 [Note] Shutting down plugin 'ngram'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280889Z 0 [Note] Shutting down plugin 'partition'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280891Z 0 [Note] Shutting down plugin 'BLACKHOLE'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280894Z 0 [Note] Shutting down plugin 'ARCHIVE'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280894Z 0 [Note] Shutting down plugin 'PERFORMANCE_SCHEMA'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280919Z 0 [Note] Shutting down plugin 'MRG_MYISAM'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280921Z 0 [Note] Shutting down plugin 'MyISAM'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280925Z 0 [Note] Shutting down plugin 'INNODB_SYS_VIRTUAL'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280926Z 0 [Note] Shutting down plugin 'INNODB_SYS_DATAFILES'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280927Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLESPACES'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280928Z 0 [Note] Shutting down plugin 'INNODB_SYS_FOREIGN_COLS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280929Z 0 [Note] Shutting down plugin 'INNODB_SYS_FOREIGN'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280930Z 0 [Note] Shutting down plugin 'INNODB_SYS_FIELDS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280931Z 0 [Note] Shutting down plugin 'INNODB_SYS_COLUMNS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280931Z 0 [Note] Shutting down plugin 'INNODB_SYS_INDEXES'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280932Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLESTATS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280933Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLES'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280934Z 0 [Note] Shutting down plugin 'INNODB_FT_INDEX_TABLE'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280935Z 0 [Note] Shutting down plugin 'INNODB_FT_INDEX_CACHE'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280935Z 0 [Note] Shutting down plugin 'INNODB_FT_CONFIG'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280936Z 0 [Note] Shutting down plugin 'INNODB_FT_BEING_DELETED'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280937Z 0 [Note] Shutting down plugin 'INNODB_FT_DELETED'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280938Z 0 [Note] Shutting down plugin 'INNODB_FT_DEFAULT_STOPWORD'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280939Z 0 [Note] Shutting down plugin 'INNODB_METRICS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280940Z 0 [Note] Shutting down plugin 'INNODB_TEMP_TABLE_INFO'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280940Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_POOL_STATS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280941Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_PAGE_LRU'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280942Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_PAGE'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280943Z 0 [Note] Shutting down plugin 'INNODB_CMP_PER_INDEX_RESET'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280944Z 0 [Note] Shutting down plugin 'INNODB_CMP_PER_INDEX'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280945Z 0 [Note] Shutting down plugin 'INNODB_CMPMEM_RESET'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280945Z 0 [Note] Shutting down plugin 'INNODB_CMPMEM'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280946Z 0 [Note] Shutting down plugin 'INNODB_CMP_RESET'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280947Z 0 [Note] Shutting down plugin 'INNODB_CMP'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280947Z 0 [Note] Shutting down plugin 'INNODB_LOCK_WAITS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280948Z 0 [Note] Shutting down plugin 'INNODB_LOCKS'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280949Z 0 [Note] Shutting down plugin 'INNODB_TRX'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.280950Z 0 [Note] Shutting down plugin 'InnoDB'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.281104Z 0 [Note] InnoDB: FTS optimize thread exiting.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.281238Z 0 [Note] InnoDB: Starting shutdown...
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.382489Z 0 [Note] InnoDB: Dumping buffer pool(s) to /var/lib/mysql/ib_buffer_pool
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:37.382772Z 0 [Note] InnoDB: Buffer pool(s) dump completed at 220424 10:28:37
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.954242Z 0 [Note] InnoDB: Shutdown completed; log sequence number 12659904
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.955419Z 0 [Note] InnoDB: Removed temporary tablespace data file: "ibtmp1"
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.955459Z 0 [Note] Shutting down plugin 'MEMORY'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.955463Z 0 [Note] Shutting down plugin 'CSV'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.955466Z 0 [Note] Shutting down plugin 'sha256_password'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.955467Z 0 [Note] Shutting down plugin 'mysql_native_password'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.955749Z 0 [Note] Shutting down plugin 'binlog'
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:37.956666Z 0 [Note] mysqld: Shutdown complete
servicesdao_votingengine-dao_votedb-1             | 
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:38+00:00 [Note] [Entrypoint]: Temporary server stopped
servicesdao_votingengine-dao_votedb-1             | 
servicesdao_votingengine-dao_votedb-1             | 2022-04-24 10:28:38+00:00 [Note] [Entrypoint]: MySQL init process done. Ready for start up.
servicesdao_votingengine-dao_votedb-1             | 
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.994627Z 0 [Note] InnoDB: Shutdown completed; log sequence number 12659904
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.995635Z 0 [Note] InnoDB: Removed temporary tablespace data file: "ibtmp1"
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.995663Z 0 [Note] Shutting down plugin 'MEMORY'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.995667Z 0 [Note] Shutting down plugin 'CSV'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.995669Z 0 [Note] Shutting down plugin 'sha256_password'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.995670Z 0 [Note] Shutting down plugin 'mysql_native_password'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.995751Z 0 [Note] Shutting down plugin 'binlog'
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:38.996685Z 0 [Note] mysqld: Shutdown complete
servicesdao_votingengine-dao_reputationdb-1       | 
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.110990Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.112127Z 0 [Note] mysqld (mysqld 5.7.37) starting as process 1 ...
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113694Z 0 [Note] InnoDB: PUNCH HOLE support available
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113718Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113721Z 0 [Note] InnoDB: Uses event mutexes
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113722Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113723Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113724Z 0 [Note] InnoDB: Using Linux native AIO
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113841Z 0 [Note] InnoDB: Number of pools: 1
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.113910Z 0 [Note] InnoDB: Using CPU crc32 instructions
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.114772Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.118580Z 0 [Note] InnoDB: Completed initialization of buffer pool
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.119905Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.132274Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.140104Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.140148Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.150619Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.150937Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.150957Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.151286Z 0 [Note] InnoDB: Waiting for purge to start
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.201707Z 0 [Note] InnoDB: 5.7.37 started; log sequence number 12659904
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.201945Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.202013Z 0 [Note] Plugin 'FEDERATED' is disabled.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.204107Z 0 [Note] InnoDB: Buffer pool(s) load completed at 220424 10:28:39
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205344Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205369Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205373Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205374Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205666Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205709Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.205961Z 0 [Note] Server hostname (bind-address): '*'; port: 3306
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.206000Z 0 [Note] IPv6 is available.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.206007Z 0 [Note]   - '::' resolves to '::';
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.206015Z 0 [Note] Server socket created on IP: '::'.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.206756Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.210782Z 0 [Note] Event Scheduler: Loaded 0 events
servicesdao_votingengine-dao_votedb-1             | 2022-04-24T10:28:39.211027Z 0 [Note] mysqld: ready for connections.
servicesdao_votingengine-dao_votedb-1             | Version: '5.7.37'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:39+00:00 [Note] [Entrypoint]: Temporary server stopped
servicesdao_votingengine-dao_reputationdb-1       | 
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24 10:28:39+00:00 [Note] [Entrypoint]: MySQL init process done. Ready for start up.
servicesdao_votingengine-dao_reputationdb-1       | 
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.450313Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.451218Z 0 [Note] mysqld (mysqld 5.7.37) starting as process 1 ...
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452804Z 0 [Note] InnoDB: PUNCH HOLE support available
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452828Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452830Z 0 [Note] InnoDB: Uses event mutexes
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452832Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452833Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452834Z 0 [Note] InnoDB: Using Linux native AIO
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.452939Z 0 [Note] InnoDB: Number of pools: 1
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.453087Z 0 [Note] InnoDB: Using CPU crc32 instructions
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.453966Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.457715Z 0 [Note] InnoDB: Completed initialization of buffer pool
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.458930Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.470842Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.477808Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.477852Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.487933Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.488331Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.488345Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.488683Z 0 [Note] InnoDB: Waiting for purge to start
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.539212Z 0 [Note] InnoDB: 5.7.37 started; log sequence number 12659904
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.539358Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.539477Z 0 [Note] Plugin 'FEDERATED' is disabled.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.541786Z 0 [Note] InnoDB: Buffer pool(s) load completed at 220424 10:28:39
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543127Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543132Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543134Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543135Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543654Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543686Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.543982Z 0 [Note] Server hostname (bind-address): '*'; port: 3306
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.544014Z 0 [Note] IPv6 is available.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.544019Z 0 [Note]   - '::' resolves to '::';
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.544027Z 0 [Note] Server socket created on IP: '::'.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.544845Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.548991Z 0 [Note] Event Scheduler: Loaded 0 events
servicesdao_votingengine-dao_reputationdb-1       | 2022-04-24T10:28:39.549261Z 0 [Note] mysqld: ready for connections.
servicesdao_votingengine-dao_reputationdb-1       | Version: '5.7.37'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)
servicesdao_votingengine-dao_votingengine-1 exited with code 139
servicesdao_votingengine-dao_votingengine-1       | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_votingengine-1       |       Now listening on: http://[::]:80
servicesdao_votingengine-dao_votingengine-1       | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_votingengine-1       |       Application started. Press Ctrl+C to shut down.
servicesdao_votingengine-dao_votingengine-1       | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_votingengine-1       |       Hosting environment: Development
servicesdao_votingengine-dao_votingengine-1       | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_votingengine-1       |       Content root path: /app
servicesdao_votingengine-dao_reputationservice-1 exited with code 139
servicesdao_votingengine-dao_reputationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_reputationservice-1  |       Now listening on: http://[::]:80
servicesdao_votingengine-dao_reputationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_reputationservice-1  |       Application started. Press Ctrl+C to shut down.
servicesdao_votingengine-dao_reputationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_reputationservice-1  |       Hosting environment: Development
servicesdao_votingengine-dao_reputationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao_votingengine-dao_reputationservice-1  |       Content root path: /app

```
