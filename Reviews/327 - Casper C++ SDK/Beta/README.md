
Grant Proposal | [327 - Casper C++ SDK](https://portal.devxdao.com/app/proposal/327)
------------ | -------------
Milestone | 2
Milestone Title | Beta
OP | numlock
Reviewer | M Chad ABAHMANE

# Milestone Details
This is the second milestone of the grant. 
The review will cover the second milestone criterias set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone**

The following RPC methods will be fully implemented in the C++ SDK:
* infoGetDeploy
* infoGetStatus
* chainGetBlockTransfers
* chainGetBlock
* chainGetEraInfoBySwitchBlock
* stateGetItem
* stateGetDictionaryItem
* stateGetBalance
* stateGetAuctionInfo

These methods will return JSON arrays.

- Unit tests will be implemented.
- The SDK will be fully documented.

**Acceptance criterias**
- Following methods of the SDK are fully functional and returning data when called:
  * infoGetDeploy
  * infoGetStatus
  * chainGetBlockTransfers
  * chainGetBlock
  * chainGetEraInfoBySwitchBlock
  * stateGetItem
  * stateGetDictionaryItem
  * stateGetBalance
  * stateGetAuctionInfo

- All unit tests are available and passing.
- Documentation are available for all critical classes and methods.

**Additional notes regarding submission from OP:**

SDK currently only runs on Linux systems. It will have multi platform support during the maintenance period.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/yusufketen/casper-cpp-sdk | ff216e9

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of  repository : https://github.com/yusufketen/casper-cpp-sdk, the 
reviewer was able to successfully build the source code on a Rocky 8 linux server using CMake version 3.20.2.

````bash
[reviewer@rocky8-mae-vm casper-cpp-sdk]$ cmake -DCMAKE_BUILD_TYPE=Debug .
-- The C compiler identification is GNU 8.5.0
-- The CXX compiler identification is GNU 8.5.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CasperSDK Version: 1.0.0
-- Configuring done
-- Generating done
-- Build files have been written to: /home/reviewer/dxd/reviews/casper-cpp-sdk

````

````bash
[reviewer@rocky8-mae-vm casper-cpp-sdk]$ make all
[  5%] Creating directories for 'LIBCRYPTOPP'
[ 11%] No download step for 'LIBCRYPTOPP'
[ 16%] No patch step for 'LIBCRYPTOPP'
[ 22%] No configure step for 'LIBCRYPTOPP'
[ 27%] Performing build step for 'LIBCRYPTOPP'
ar: création de libcryptopp.a
[ 33%] No install step for 'LIBCRYPTOPP'
[ 38%] Completed 'LIBCRYPTOPP'
[ 38%] Built target LIBCRYPTOPP
[ 44%] Building CXX object src/CMakeFiles/CasperSDK.dir/CasperClient.cpp.o
[ 50%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/GlobalStateKey.cpp.o
[ 55%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Types/URef.cpp.o
[ 61%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/CryptoUtil.cpp.o
[ 66%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/StringUtil.cpp.o
[ 72%] Building CXX object src/CMakeFiles/CasperSDK.dir/include/Utils/CEP57Checksum.cpp.o
[ 77%] Linking CXX shared library libCasperSDK.so
[ 77%] Built target CasperSDK
[ 83%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/ClientTest.cpp.o
[ 88%] Linking CXX executable CasperSDK_test
[ 88%] Built target CasperSDK_test
[ 94%] Building CXX object examples/CMakeFiles/example.dir/HelloSDK.cpp.o
[100%] Linking CXX executable example
[100%] Built target example

````

## Overall Impression of usage testing

In the reviewer's opinion, the instructions for building the project are clear and sufficiently documented.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 


# Unit / Automated Testing

The project has 19 unit tests corresponding to the RPC calls implemented in the milestone :

* infoGetDeploy
* infoGetStatus
* chainGetBlockTransfers
* chainGetBlock
* chainGetEraInfoBySwitchBlock
* stateGetItem
* stateGetDictionaryItem
* stateGetBalance
* stateGetAuctionInfo

The reviewer checked that the all these RPC calls have at least one positive path test.

There are also many negative path tests.

The tests run successfully, without errors and produce the following output:

````bash
[reviewer@rocky8-mae-vm casper-cpp-sdk]$ ./test/CasperSDK_test
Test infoGetPeers checks node list size...      [ OK ]
Test chainGetStateRootHash using Block height parameter... [ OK ]
Test chainGetStateRootHash using invalid Block height parameter... [ OK ]
Test chainGetStateRootHash using Block hash parameter... [ OK ]
Test chainGetStateRootHash using empty Block hash parameter... [ OK ]
Test infoGetDeploy using Deploy hash parameter... [ OK ]
Test infoGetDeploy using invalid Deploy hash parameter... [ OK ]
Test infoGetStatus compares with a reference value... [ OK ]
Test chainGetBlockTransfers using Block hash parameter... [ OK ]
Test chainGetBlock using Block hash parameter... [ OK ]
Test chainGetEraInfoBySwitchBlock using Block hash parameter... [ OK ]
Test stateGetItem using state root hash and key parameters... [ OK ]
Test stateGetItem using invalid state root hash and key parameters... [ OK ]
Test stateGetDictionaryItem using state root hash and dictionary key parameters... [ OK ]
Test stateGetBalance compares with a reference value... [ OK ]
Test stateGetBalance using invalid URef and state root hash parameters... [ OK ]
Test stateGetAuctionInfo using Block hash parameter (may take a while)... [ OK ]
Test toLower checks internal lower case converter... [ OK ]
Test getAccountHash checks internal PublicKey to AccountHash converter... [ OK ]
SUCCESS: All unit tests have passed.

````


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 


# Documentation

### Code Documentation

The reviewer has observed that the project has acceptable code-level documentation with properly formatted summaries and comments on the critical classes and methods.
Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project does not provide detailed documentation but README.md has sufficient usage instructions on how to use the SDK. 
There is one Example folder with codes samples on how to use every RPC call.
The reviewer could run the examples using this command line:

```bash
./examples/example
```

The reviewer noticed that one example fails to run and gives the following error :

```bash
terminate called after throwing an instance of 'std::runtime_error'
  what():  Invalid CLTypeInfo
Aborted (core dumped)
```
**The OP is encouraged to correct the example codes for the next milestone**

The OP also provides instructions for generating the documentation:

```bash
cd docs
doxygen Doxyfile
The documentation will be available in the "docs/html/index.html" file.
```
The reviewer was able to execute this command to generate and then access the documentation.

**However, the reviewer recommends to the OP to set up an automatic generation of the SDK documentation  (using github plugins).**

**A small effort has been made to improve the documentation of the project, but this remains insufficient.**

**For next milestones, OP is encouraged to provide more documentation on how to use the SDK, along with sample codes for using critical SDK functions**


Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS  with Notes


## Overall Conclusion on Documentation

In the reviewer's opinion, the project usage and code-level documentation are sufficient. 

# Open Source Practices

## Licenses

The Project is correctly released under the Apache License 2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. There is also a CONTRIBUTING and a SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is generally well-structured and readable. Comments are good enough for all classes and methods.

# Final Conclusion

The project code seems to provide the functionality described in the grant application and milestone acceptance criteria.
**In the last review, the reviewer highlighted the low level of general documentation of the project. A small improvement is to be noted for this milestone but the project is generally poorly documented**
**For the next milestones, The reviewer encourages the op to provide richer documentation on how to use the SDK and its functions.** 

In the reviewer's opinion, this submission should PASS with Notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
