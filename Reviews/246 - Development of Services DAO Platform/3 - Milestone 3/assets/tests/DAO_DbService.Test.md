```
gitpod /workspace/ServicesDAO/UnitTests/DAO_DbService.Test (main) $ dotnet test

Welcome to .NET Core 3.1!
---------------------
SDK Version: 3.1.416

Telemetry
---------
The .NET Core tools collect usage data in order to help us improve your experience. It is collected by Microsoft and shared with the community. You can opt-out of telemetry by setting the DOTNET_CLI_TELEMETRY_OPTOUT environment variable to '1' or 'true' using your favorite shell.

Read more about .NET Core CLI Tools telemetry: https://aka.ms/dotnet-cli-telemetry

----------------
Explore documentation: https://aka.ms/dotnet-docs
Report issues and find source on GitHub: https://github.com/dotnet/core
Find out what's new: https://aka.ms/dotnet-whats-new
Learn about the installed HTTPS developer cert: https://aka.ms/aspnet-core-https
Use 'dotnet --help' to see available commands or visit: https://aka.ms/dotnet-cli-docs
Write your first app: https://aka.ms/first-net-core-app
--------------------------------------------------------------------------------------
Controllers/WebsiteController.cs(182,25): warning CS0472: The result of the expression is always 'true' since a value of type 'int' is never equal to 'null' of type 'int?' [/workspace/ServicesDAO/DAO_DbService/DAO_DbService.csproj]
/usr/share/dotnet/sdk/3.1.416/Microsoft.Common.CurrentVersion.targets(2084,5): warning MSB3277: Found conflicts between different versions of "Microsoft.EntityFrameworkCore.Relational" that could not be resolved.  These reference conflicts are listed in the build log when log verbosity is set to detailed. [/workspace/ServicesDAO/UnitTests/DAO_DbService.Test/DAO_DbService.Test.csproj]
Test run for /workspace/ServicesDAO/UnitTests/DAO_DbService.Test/bin/Debug/netcoreapp3.1/DAO_DbService.Test.dll(.NETCoreApp,Version=v3.1)
Microsoft (R) Test Execution Command Line Tool Version 16.7.1
Copyright (c) Microsoft Corporation.  All rights reserved.

Starting test execution, please wait...

A total of 1 test files matched the specified pattern.

Test Run Successful.
Total tests: 14
     Passed: 14
 Total time: 29.9047 Seconds
```
