
Grant Proposal | [327 - Casper C++ SDK](https://portal.devxdao.com/app/proposal/327)
------------ | -------------
Milestone | 1
Milestone Title | Alpha
OP | numlock
Reviewer | M Chad ABAHMANE

# Milestone Details
This is the first milestone of grant. 
The review will cover the first milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Base project of C++ SDK will be created and published on a GitHub repository.
- Following methods of the API will be fully implemented and will return when called by the SDK:
   * chainGetStateRootHash
   * infoGetPeers

**Acceptance criteria:**

- C++ SDK project available on a public GitHub repository
- It will be possible to connect to a Casper node and retrieve information by using the implemented methods.
- Following methods of the API fully implemented and will return when called:
   * chainGetStateRootHash
   * infoGetPeers

**Additional notes regarding submission from OP:**

SDK currently only runs on Linux systems. It will have multi platform support by the last milestone.

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/yusufketen/casper-cpp-sdk | db262e6

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of  repository : https://github.com/yusufketen/casper-cpp-sdk, reviewer was able to successfully build the source code on a Ubuntu 20.04 server using CMake version 3.20.0 

````bash
cmake -DCMAKE_BUILD_TYPE=Debug .
-- The C compiler identification is GNU 9.3.0
-- The CXX compiler identification is GNU 9.3.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CasperSDK Version: 1.0.0
-- CASPERSDK-NOTFOUND
-- Configuring done
-- Generating done
-- Build files have been written to: /home/abahmane/reviews/casper-cpp-sdk

````

````bash
make all
[ 16%] Building CXX object src/CMakeFiles/CasperSDK.dir/CasperClient.cpp.o
[ 33%] Linking CXX shared library libCasperSDK.so
[ 33%] Built target CasperSDK
[ 50%] Building CXX object test/CMakeFiles/CasperSDK_test.dir/ClientTest.cpp.o
[ 66%] Linking CXX executable CasperSDK_test
[ 66%] Built target CasperSDK_test
[ 83%] Building CXX object examples/CMakeFiles/HelloSDK.dir/HelloSDK.cpp.o
[100%] Linking CXX executable HelloSDK
[100%] Built target HelloSDK

````

## Overall Impression of usage testing

The project has sufficient and well documented instructions to successfully build the source code.
**However, the reviewer recommends detailing these instructions so that any lamba user  could install and build the project.**

Example:
Instructions showing user how to clone the project are missing:

````bash
git clone https://github.com/yusufketen/casper-cpp-sdk.git
````


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 


# Unit / Automated Testing

The project has 2 tests corresponding to the RPC calls implemented in the milestone :
* chainGetStateRootHash
* infoGetPeers

The reviewer checked that the two RPC calls have at least one positive path test.
**However, there are no negative path tests**, this is not blocking for this milestone as the project is in its very early stage.
The OP is strongly encouraged to add negative path tests for the next milestones.  
**Reviewer also recommends to document tests so that we could see the actual progress of the tests (while running) and what functions are being tested.**
The tests run successfully, without errors and produce the following output:

````bash
make test
Running tests...
Test project /home/abahmane/reviews/casper-cpp-sdk
    Start 1: CasperSDK_test
1/1 Test #1: CasperSDK_test ...................   Passed    0.96 sec

100% tests passed, 0 tests failed out of 1

Total Test time (real) =   0.96 sec
````


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes


# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project does not provide detailed documentation but README.md has sufficient usage instructions for the the 2 implemented RPC methods.
There is one Example folder with codes for doing examples.
This is acceptable since the project is its beginning.

**For next milestones, OP is encouraged to provide more documentation on how to use the SDK, along with sample codes for using critical SDK functions**


Requirement | Finding
------------ | -------------
Usage Documented | PASS with notes
Example Documented | PASS 


## Overall Conclusion on Documentation

In the reviewer's opinion, the project,  usage documentation and code-level documentation are sufficient. 

# Open Source Practices

## Licenses

The Project is correctly released under the Apache License 2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. There is also a CONTRIBUTING and a SECURITY policies.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS


# Coding Standards

## General Observations

Code is generally well-structured and readable. Comments are good enough for all classes and methods.

# Final Conclusion

The project code seems to provide the functionality described in the grant application and milestone acceptance criteria. In the reviewer's opinion, this submission should PASS. 

# Recommendation

Recommendation | PASS with notes
------------ | -------------
