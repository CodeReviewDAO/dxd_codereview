# Output of the cmake command

```sh

CasperSDK Version: 1.0.0
using deps from vcpkg or system
building tests
building examples
-- Configuring done
-- Generating done
-- Build files have been written to: /workspace/casper-cpp-sdk/build

```

# Output of the ninja command

```sh

[1/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_eol.cxx.o
[2/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_common.cpp.o
[3/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_test.cxx.o
[4/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/CryptoUtil.cpp.o
[5/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_read.cpp.o
[6/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/badcert.cxx.o
[7/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/StringUtil.cpp.o
[8/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_write.cpp.o
[9/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/CEP57Checksum.cpp.o
[10/31] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/x509cert.cpp.o
[11/31] Linking CXX static library lib/cryptopp-pem/libcryptopp_pem.a
[12/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/URef.cpp.o
[13/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/LogConfigurator.cpp.o
[14/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/GlobalStateKey.cpp.o
[15/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/Secp256k1Key.cpp.o
[16/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/ED25519Key.cpp.o
[17/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLType.cpp.o
[18/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/ByteSerializers/BaseByteSerializer.cpp.o
[19/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLConverter.cpp.o
[20/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLValue.cpp.o
[21/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLTypeParsed.cpp.o
[22/31] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/Deploy.cpp.o
[23/31] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/DeployItemByteSerializerTest.cpp.o
[24/31] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/RpcTest.cpp.o
[25/31] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/CLValueByteSerializerTest.cpp.o
[26/31] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/ClientTest.cpp.o
[27/31] Building CXX object examples/CMakeFiles/example.dir/HelloSDK.cpp.o
[28/31] Building CXX object src/CMakeFiles/casper_sdk.dir/CasperClient.cpp.o
[29/31] Linking CXX static library src/libcasper_sdk.a
[30/31] Linking CXX executable examples/example
[31/31] Linking CXX executable test/casper_cpp_sdk_tests

```

# Output of the ninja install command

```sh

[0/1] Install the project...
-- Install configuration: "Release"
-- Up-to-date: /workspace/casper-cpp-sdk/include
-- Installing: /workspace/casper-cpp-sdk/include/Algorithm
-- Installing: /workspace/casper-cpp-sdk/include/Algorithm/Join.hpp
-- Installing: /workspace/casper-cpp-sdk/include/Base.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/BaseByteSerializer.cpp
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/BaseByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/CLValueByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/DeployApprovalByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/DeployByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/ExecutableDeployItemByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/GlobalStateKeyByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/ByteSerializers/NamedArgByteSerializer.h
-- Installing: /workspace/casper-cpp-sdk/include/CasperClient.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/Connection
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/Connection/HttpLibConnector.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/Connection/httplib.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetAuctionInfoResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetBalanceResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetBlockResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetBlockTransfersResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetDeployResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetDictionaryItemResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetEraInfoResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetItemResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetStateRootHashResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/GetStatusResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/InfoGetPeersResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/PutDeployResult.h
-- Installing: /workspace/casper-cpp-sdk/include/JsonRpc/ResultTypes/RpcResult.h
-- Installing: /workspace/casper-cpp-sdk/include/Types
-- Installing: /workspace/casper-cpp-sdk/include/Types/AccessRights.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Account.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/AuctionState.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Bid.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Block.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/BlockInfo.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLConverter.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLConverter.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLType.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLType.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLTypeParsed.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLTypeParsed.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLValue.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/CLValue.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Configuration.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Contract.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ContractPackage.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Delegator.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Deploy.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/Deploy.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/DeployApproval.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/DeployHeader.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/DeployInfo.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ED25519Key.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/ED25519Key.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/EntryPoint.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/EraEnd.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/EraInfo.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/EraSummary.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/EraValidators.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ExecutableDeployItem.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ExecutionEffect.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ExecutionResult.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/GlobalStateKey.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/GlobalStateKey.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/KeyAlgo.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/KeyPair.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ModuleBytes.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/NamedArg.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/NamedKey.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/NextUpgrade.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Operation.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Peer.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/PublicKey.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Secp256k1Key.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/Secp256k1Key.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/SeigniorageAllocation.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Signature.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/StoredContractByHash.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/StoredContractByName.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/StoredValue.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/StoredVersionedContractByHash.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/StoredVersionedContractByName.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Transfer.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/TransferDeployItem.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/Transform.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/TransformEntry.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/URef.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Types/URef.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/UnbondingPurse.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ValidatorBid.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ValidatorChanges.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/ValidatorWeight.h
-- Installing: /workspace/casper-cpp-sdk/include/Types/VestingSchedule.h
-- Installing: /workspace/casper-cpp-sdk/include/Utils
-- Installing: /workspace/casper-cpp-sdk/include/Utils/CEP57Checksum.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Utils/CEP57Checksum.h
-- Installing: /workspace/casper-cpp-sdk/include/Utils/CryptoUtil.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Utils/CryptoUtil.h
-- Installing: /workspace/casper-cpp-sdk/include/Utils/File.h
-- Installing: /workspace/casper-cpp-sdk/include/Utils/LogConfigurator.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Utils/LogConfigurator.h
-- Installing: /workspace/casper-cpp-sdk/include/Utils/StringUtil.cpp
-- Installing: /workspace/casper-cpp-sdk/include/Utils/StringUtil.h
-- Installing: /workspace/casper-cpp-sdk/libs/libcasper_sdk.a

```
