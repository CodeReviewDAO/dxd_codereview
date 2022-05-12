Grant Proposal | [327 - Casper C++ SDK](https://portal.devxdao.com/public-proposals/327)
------------ | -------------
Milestone | 3
Milestone Title | Final
OP | numlock
Reviewer | Gökhan Gurbetoğlu

# Milestone Details
This is the final milestone of the grant.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The following methods will be implemented:

- C++ version of CLType primitives
- C++ version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects
- ED25519/SECP256K1 key pairs  Wrappers
- PutDeploy RPC call implemented
- Refactoring C++ SDK calls to return Casper Domaine Specific Objects

**Acceptance criteria:**

- C++ version of CLType primitives
- C++ version for Casper Domain Specific Objects 
- Serialization of Casper Domain Specific Objects 
- ED25519/SECP256K1 key pairs  Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper Domaine Specific Objects

**Additional notes regarding submission from OP:**

Requirements of the last milestone is also complete.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/yusufketen/casper-cpp-sdk | 5f65ee0


# Install & Usage Testing Procedure and Findings

## Installation

Following the instructions in the README of https://github.com/yusufketen/casper-cpp-sdk, reviewer was able to successfully build the source code for this milestone for both the Debug and Release builds on Ubuntu 20.04 in a cloud environment.

### Debug Build

```sh
gitpod /workspace/casper-cpp-sdk (main) $ cmake -DCMAKE_BUILD_TYPE=Debug .
CasperSDK Version: 1.0.0
-- Configuring done
-- Generating done
-- Build files have been written to: /workspace/casper-cpp-sdk

gitpod /workspace/casper-cpp-sdk (main) $ make all
[  3%] Creating directories for 'LIBCRYPTOPP'
[  7%] No download step for 'LIBCRYPTOPP'
[ 10%] No patch step for 'LIBCRYPTOPP'
[ 14%] No configure step for 'LIBCRYPTOPP'
[ 17%] Performing build step for 'LIBCRYPTOPP'
[ 21%] No install step for 'LIBCRYPTOPP'
[ 25%] Completed 'LIBCRYPTOPP'
[ 25%] Built target LIBCRYPTOPP
[ 28%] Building CXX object src/CMakeFiles/CasperSDK.dir/CasperClient.cpp.o
[ 32%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/CLValue.cpp.o
[ 35%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/CLType.cpp.o
[ 39%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/GlobalStateKey.cpp.o
[ 42%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/URef.cpp.o
[ 46%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/ED25519Key.cpp.o
[ 50%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/Secp256k1Key.cpp.o
[ 53%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/CryptoUtil.cpp.o
[ 57%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/StringUtil.cpp.o
[ 60%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/CEP57Checksum.cpp.o
[ 64%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/CLConverter.cpp.o
[ 67%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/Deploy.cpp.o
[ 71%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/ByteSerializers/BaseByteSerializer.cpp.o
[ 75%] Linking CXX shared library libCasperSDK.so
[ 75%] Built target CasperSDK
[ 78%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/ClientTest.cpp.o
[ 82%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/RpcTest.cpp.o
[ 85%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/CLValueByteSerializerTest.cpp.o
[ 89%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/DeployItemByteSerializerTest.cpp.o
[ 92%] Linking CXX executable CasperSDK_test
[ 92%] Built target CasperSDK_test
[ 96%] Building CXX object examples/CMakeFiles/example.dir/HelloSDK.cpp.o
[100%] Linking CXX executable example
[100%] Built target example
```

### Release Build

```sh
gitpod /workspace/casper-cpp-sdk (main) $ cmake -DCMAKE_BUILD_TYPE=Release .
CasperSDK Version: 1.0.0
-- Configuring done
-- Generating done
-- Build files have been written to: /workspace/casper-cpp-sdk

gitpod /workspace/casper-cpp-sdk (main) $ make all
[  3%] Creating directories for 'LIBCRYPTOPP'
[  7%] No download step for 'LIBCRYPTOPP'
[ 10%] No patch step for 'LIBCRYPTOPP'
[ 14%] No configure step for 'LIBCRYPTOPP'
[ 17%] Performing build step for 'LIBCRYPTOPP'
ar: creating libcryptopp.a
[ 21%] No install step for 'LIBCRYPTOPP'
[ 25%] Completed 'LIBCRYPTOPP'
[ 25%] Built target LIBCRYPTOPP
[ 28%] Building CXX object src/CMakeFiles/CasperSDK.dir/CasperClient.cpp.o
[ 32%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/CLValue.cpp.o
[ 35%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/CLType.cpp.o
[ 39%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/GlobalStateKey.cpp.o
[ 42%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/URef.cpp.o
[ 46%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/ED25519Key.cpp.o
[ 50%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/Secp256k1Key.cpp.o
[ 53%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/CryptoUtil.cpp.o
[ 57%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/StringUtil.cpp.o
[ 60%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/CEP57Checksum.cpp.o
[ 64%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/CLConverter.cpp.o
[ 67%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/Deploy.cpp.o
[ 71%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/ByteSerializers/BaseByteSerializer.cpp.o
[ 75%] Linking CXX shared library libCasperSDK.so
[ 75%] Built target CasperSDK
[ 78%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/ClientTest.cpp.o
[ 82%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/RpcTest.cpp.o
[ 85%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/CLValueByteSerializerTest.cpp.o
[ 89%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/DeployItemByteSerializerTest.cpp.o
[ 92%] Linking CXX executable CasperSDK_test
[ 92%] Built target CasperSDK_test
[ 96%] Building CXX object examples/CMakeFiles/example.dir/HelloSDK.cpp.o
[100%] Linking CXX executable example
[100%] Built target example
```

## Overall Impression of usage testing

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

Unit tests FAIL for this milestone. While most unit tests are working as intended, reviewer needed to manually edit some test files that included hard coded paths to correctly point to the desired location for key pairs required for some tests. These key pairs are also needed to be manually added. The path they are in (`/test/data/KeyPair/`) does not exist initially and needs to be manually created in the filesystem. There is no information about the creation of the key pairs in the documentation either.

```bash
Summary:
  Count of all unit tests:       95
  Count of run unit tests:       95
  Count of failed unit tests:     3
  Count of skipped unit tests:    0
FAILED: 3 of 95 unit tests have failed.
```

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | N/A
Unit Tests - At least one negative path test | N/A
Unit Tests - Additional path tests | N/A

# Documentation

### Code Documentation

The code-level documentation is acceptable. It has proper formatting for its summaries and comments for both classes and methods. The descriptions of methods could be longer and more explanatory nevertheless.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

README.md includes clear information about the build and installation of the SDK.

There exists an `/example/` folder with code samples that show how to use every RPC call. How to run code samples is instructed in the README. The examples run as intended.  
A side note: The last example in the sequation aborts with messages. This is an expected outcome and not an unexpected error. Including expected results in the output would be a plus for understanding the operations better.

There is clear information about how to generate the documentation with `doxygen`. Reviewer successfully generated and was able to view the documentation after using these instructions. However, as stated in previous milestones, auto generation of documentation without manual user invocation is preferable.

**Some of the tests, however, failed due to missing key pairs as stated in Unit / Automated Testing section. There is no mention of how to create these key pairs in the documentation. A user cannot directly understand what is wrong and cannot fix the issue immediately. These either need to be automated or sufficient documentation should be provided.**

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

Coverage of code documentation is complete but not that detailed. The reverse is true for project documentation, it does not cover some key parts but covered parts are detailed and sufficient.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING and SECURITY policies. The optional Code of Conduct is not included. Pull requests and Issues are enabled on the repository and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout. Some leftover comments can be cleaned up as a suggestion.

# Final Conclusion

Source code meets the requirements and implements the functionalities stated in the grant application.

The documentation could be more detailed for setting up the SDK and its usage.

Unit tests should be fixed. In its current state, they fail. Hard coded paths should be removed and user should not have to manually add these in the source code themselves.

Since this is the final milestone, it should cover the general expectations of the project. The project needs to have multiplatform support but in its current state, only builds on Linux are supported.

Reviewer recommends that this submission should fail code review because of these reasons.

# Recommendation

Recommendation | FAIL
------------ | -------------
