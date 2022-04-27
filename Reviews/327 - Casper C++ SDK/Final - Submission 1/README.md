Grant Proposal | [0 - My Grant Proposal](https://portal.devxdao.com/public-proposals/0)
------------ | -------------
Milestone | 3
Milestone Title | Final Submission 1
OP | numlock
Reviewer | Gökhan Gurbetoğlu <ggurbet@gmail.com>

# Milestone Details
This is the final milestone of the grant.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

_Copy the content for this section of the milestone submission from the DxD MVPR Portal_

**Acceptance criteria:**

_Copy the content for this section of the milestone submission from the DxD MVPR Portal_

**Additional notes regarding submission from OP:**

_Copy the content for this section of the milestone submission from the DxD MVPR Portal_

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/yusufketen/casper-cpp-sdk | 9b44942


# Install & Usage Testing Procedure and Findings

## Installation

Following the instructions in the README of https://github.com/yusufketen/casper-cpp-sdk, reviewer was able to successfully build the source code with warnings for this milestone for both the Debug and Release builds on Ubuntu 20.04 in a cloud environment.

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
/workspace/casper-cpp-sdk/src/include/Types/CLValue.cpp: In member function ‘bool Casper::CLValue::operator<(const Casper::CLValue&) const’:
/workspace/casper-cpp-sdk/src/include/Types/CLValue.cpp:64:1: warning: control reaches end of non-void function [-Wreturn-type]
   64 | }
      | ^
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
/workspace/casper-cpp-sdk/src/include/Types/CLValue.cpp: In member function ‘bool Casper::CLValue::operator<(const Casper::CLValue&) const’:
/workspace/casper-cpp-sdk/src/include/Types/CLValue.cpp:64:1: warning: control reaches end of non-void function [-Wreturn-type]
   64 | }
      | ^
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
Project builds without errors | PASS with Notes
Documentation provides sufficient installation/execution instructions | PASS / FAIL / PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS / FAIL / PASS with Notes

While the project builds with a warning, the warning in question is about control reaching end of non-void function and can easily be ignored in this context since it has no effect on the build.

# Unit / Automated Testing

_Summarize the result of the unit testing / automated testing / integration testing provided in the Milestone. Feel free to include
automated test output, either as text, image or other artifact. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS / FAIL / PASS with Notes
Unit Tests - At least one negative path test | PASS / FAIL / PASS with Notes
Unit Tests - Additional path tests | PASS / FAIL / PASS with Notes

# Documentation

### Code Documentation

_Summarize the code level documentation you encountered. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Code Documented | PASS / FAIL / PASS with Notes

### Project Documentation

_Summarize the project level documentation you encountered. This covers the information provided in the README for the project, 
as well any exampled provided. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
Usage Documented | PASS / FAIL / PASS with Notes
Example Documented | PASS / FAIL / PASS with Notes

## Overall Conclusion on Documentation

_Summarize your review of the documentation in this project, including code, usage and examples_

# Open Source Practices

## Licenses

_List which Open Source license is used and note anything that's non-standard. Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS / FAIL / PASS with Notes

## Contribution Policies

_Confirm that the project contains a `CONTRIBUTING` and `SECURITY` policy, and optionally an associated `Code of Conduct` policy. Confirm
that Pull Requests and Issues are enabled on the repository and that generally the Project is set up for public participation. 
Provide a `PASS`, `FAIL`, or `PASS With Notes` for the requirements
below. In the case of `PASS With Notes`, make sure that the notes for improvement are clearly spelled out in this section._

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS / FAIL / PASS with Notes

# Coding Standards

## General Observations

_Provide any general observations about the project you want to add to your review. These can be subjective in nature as well, and do not
contribute to your recommendation to pass or fail the submission._

# Final Conclusion

_Summarize your final conclusion, and provide your motivation for your recommendation below. For example, you may say 'Reviewer recommends that this
submission should fail code review, because it does not contain an OSI-approved open source license'_

# Recommendation

Recommendation | PASS / FAIL / PASS with Notes
------------ | -------------
