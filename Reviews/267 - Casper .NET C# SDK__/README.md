Grant Proposal | [267 - Casper .NET C# SDK](https://portal.devxdao.com/public-proposals/267)
------------ | -------------
Milestone | 1
Milestone Title | Alpha Version
OP | Michael Steuer | MAKE
Reviewer | Robert Carbone <codereview@robertcarbone.com>

# Milestone Details
This is the first milestone of grant. 
The reveiw will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Scaffolding of C# SDK project, public on GitHub, 
and able to connect to a Casper Node and execute and return response for at least 1 method

**Acceptance criteria:**

- C# SDK project is available on public GitHub repository
- When instantiated, can connect to a Casper node
- When connected, it can make at least 1 method call and return a response

**Additional notes regarding submission from OP:**


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-net-sdk 

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-net-sdk, the reviewer was able to successfully install the library. Only a small hiccup when the reviewer had to figure out the .Net 5.0 was needed. The reviewer was also able to successfully build the source code for this milestone by using the build script furnished in the root and readme of the repository. 

## Overall Impression of usage testing

The code was very well laid out and pretty printed for easy reading. Things were aligned nicely and it was easy to understand what was happening in the libraries as everything was also named very appropriatly. In this milestone usage testing is not part of the requirement. 
Still things look to be on a promising track for future milestones where this criteria is more mission critical. 

Requirement | Finding
------------ | -------------

                           C# SDK project is available on public GitHub repository | PASS
                                   When instantiated, can connect to a Casper node | PASS
          When connected, it can make at least 1 method call and return a response | PASS
                                                     Project builds without errors | PASS
             Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
                                                      Can connect to a Casper node | PASS

# Unit / Automated Testing

Project contains 41 unit tests that can be executed from the console. 
The reviewer has observed that all tests run successfully without errors. 

Requirement | Finding
------------ | -------------
Unit Tests - Sufficeint | PASS

# Documentation

### Code Documentation

Code Documentation was acceptable for this stage of the project. 

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Project Documentation was acceptable for this stage of the project. 

Requirement | Finding
------------ | -------------
  Usage Documented | PASS


## Overall Conclusion on Documentation


# Open Source Practices

## Licenses

The Project is released under the MIT License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Sufficient for the current state of the project. 

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is fantastically well-structured and readable. The project has been committed to GitHub and all 41 unit tests pass. 

# Final Conclusion

The project meets the functionality described in the grant application and milestone acceptance criteria. 
With the only note being that net5.0 should be a mentioned prequisite, and the fact this this is an exceedingly easy fix,
the submission does not meet the plurity requirement to bring it down to the level of pass with note(s). :)
Resounding PASS.

# Recommendation

Recommendation | PASS
------------ | -------------




TESTS
------------------------------------------------------------------
Microsoft (R) Build Engine version 17.0.0+c9eb9dd64 for .NET
Copyright (C) Microsoft Corporation. All rights reserved.

  Determining projects to restore...
  All projects are up-to-date for restore.
  NetCasperSDK -> C:\Users\r\workspace\casper-net-sdk\build\NetCasperSDK.dll
  NetCasperTest -> C:\Users\r\workspace\casper-net-sdk\build\NetCasperTest.dll
  NetCasperSDK -> C:\Users\r\workspace\casper-net-sdk\build\NetCasperSDK.dll

Build succeeded.
    0 Warning(s)
    0 Error(s)

Time Elapsed 00:00:00.42


Determining projects to restore...
  All projects are up-to-date for restore.
  NetCasperSDK -> C:\Users\r\workspace\casper-net-sdk\NetCasperSDK\bin\Debug\net5.0\NetCasperSDK.dll
  NetCasperTest -> C:\Users\r\workspace\casper-net-sdk\NetCasperTest\bin\Debug\net5.0\NetCasperTest.dll
Test run for C:\Users\r\workspace\casper-net-sdk\NetCasperTest\bin\Debug\net5.0\NetCasperTest.dll (.NETCoreApp,Version=v5.0)
Microsoft (R) Test Execution Command Line Tool Version 17.0.0
Copyright (c) Microsoft Corporation.  All rights reserved.

Starting test execution, please wait...
A total of 1 test files matched the specified pattern.

Passed!  - Failed:     0, Passed:    41, Skipped:     0, Total:    41, Duration: 1 s - NetCasperTest.dll (net5.0)
