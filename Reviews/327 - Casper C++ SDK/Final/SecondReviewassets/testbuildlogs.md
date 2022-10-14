# Output of cmake command

```sh
CasperSDK Version: 1.0.0
using deps from vcpkg or system
building tests
-- Configuring done
-- Generating done
-- Build files have been written to: /workspace/casper-cpp-sdk/build

```
# Output of ninja command

```sh

[1/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_eol.cxx.o
[2/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_common.cpp.o
[3/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_test.cxx.o
[4/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/CEP57Checksum.cpp.o
[5/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_read.cpp.o
[6/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/StringUtil.cpp.o
[7/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/CryptoUtil.cpp.o
[8/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_write.cpp.o
[9/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/badcert.cxx.o
[10/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/ByteSerializers/BaseByteSerializer.cpp.o
[11/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLType.cpp.o
[12/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLConverter.cpp.o
[13/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/LogConfigurator.cpp.o
[14/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/URef.cpp.o
[15/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/GlobalStateKey.cpp.o
[16/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/ED25519Key.cpp.o
[17/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/Secp256k1Key.cpp.o
[18/29] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/x509cert.cpp.o
[19/29] Linking CXX static library lib/cryptopp-pem/libcryptopp_pem.a
[20/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLValue.cpp.o
[21/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLTypeParsed.cpp.o
[22/29] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/Deploy.cpp.o
[23/29] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/DeployItemByteSerializerTest.cpp.o
[24/29] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/CLValueByteSerializerTest.cpp.o
[25/29] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/RpcTest.cpp.o
[26/29] Building CXX object test/CMakeFiles/casper_cpp_sdk_tests.dir/ClientTest.cpp.o
[27/29] Building CXX object src/CMakeFiles/casper_sdk.dir/CasperClient.cpp.o
[28/29] Linking CXX static library src/libcasper_sdk.a
[29/29] Linking CXX executable test/casper_cpp_sdk_tests

```

# Output of "./test/casper_cpp_sdk_tests" command

```sh

Test CLValue_ByteSer_Bool_Test...               bool false: 010000000000
bool true: 010000000100
optional false: 0200000001000d00
optional true: 0200000001010d00
optional none: 01000000000d00
[ OK ]
Test CLValue_ByteSer_I32_Test...                i32: 04000000f6ffffff01
optional i32: 0500000001f6ffffff0d01
optional none i32: 01000000000d01
[ OK ]
Test CLValue_ByteSer_I64_Test...                i64: 08000000f0ffffffffffffff02
optional i64: 0900000001f0ffffffffffffff0d02
optional none i64: 01000000000d02
[ OK ]
Test CLValue_ByteSer_U8_Test...                 u8: 010000000003
u8_2: 010000007f03
optional u8: 0200000001ff0d03
optional none u8: 01000000000d03
[ OK ]
Test CLValue_ByteSer_U32_Test...                u32: 04000000ffffffff04
optional u32: 0500000001000000000d04
optional none u32: 01000000000d04
[ OK ]
Test CLValue_ByteSer_U64_Test...                u64: 08000000ffffffffffffffff05
optional u64: 090000000101000000000000000d05
optional none u64: 01000000000d05
[ OK ]
Test CLValue_ByteSer_U128_Test...               u128: 0900000008ffffffffffffffff06
u128_2: 120000000110feffffffffffffffffffffffffffffff0d06
optional none u128: 01000000000d06
[ OK ]
Test CLValue_ByteSer_U256_Test...               u256: 0900000008ffffffffffffffff07
u256_b_val_2: 115792089237316195423570985008687907853269984665640564039457584007913129639935
optional u256: 2200000001207fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff0d07
optional none u256: 01000000000d07
[ OK ]
Test CLValue_ByteSer_U512_Test...               u512: 0900000008ffffffffffffffff08
u512 expected: 0900000008ffffffffffffffff08
optional u512: 4200000001407fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff0d08
optional u512 expected: 4200000001407fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff0d08
optional u512 none: 01000000000d08
[ OK ]
Test CLValue_ByteSer_Unit_Test...               unit: 0000000009
optional unit: 01000000010d09
optional none unit: 01000000000d09
[ OK ]
Test CLValue_ByteSer_String_Test...             string: 120000000e00000048656c6c6f2c20436173706572210a
optional string: 13000000010e00000048656c6c6f2c20436173706572210d0a
optional empty string: 0500000001000000000d0a
optional none string: 01000000000d0a
[ OK ]
Test CLValue_ByteSer_URef_Test...               uref: 21000000000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f070c
optional uref: 2200000001000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f070d0c
optional none uref: 01000000000d0c
[ OK ]
Test CLValue_ByteSer_Key_Test...                account hash key: 2100000000989ca079a5e446071866331468ab949483162588d57ec13ba6bb051f1e15f8b70b
optional account hash key: 220000000100989ca079a5e446071866331468ab949483162588d57ec13ba6bb051f1e15f8b70d0b
optional none account hash key: 01000000000d0b
[ OK ]
Test CLValue_ByteSer_PublicKey_Test...          public key: 2100000001381b36cd07ad85348607ffe0fa3a2d033ea941d14763358ebeace9c8ad3cb77116
optional public key: 220000000101381b36cd07ad85348607ffe0fa3a2d033ea941d14763358ebeace9c8ad3cb7710d16
optional none public key: 01000000000d16
[ OK ]
Test CLValue_ByteSer_List_Test...               list cltype switch
list cltype switch end
list: 1400000004000000010000000200000003000000040000000e04
list cltype switch
list cltype switch end
optional list: 150000000104000000010000000200000003000000040000000d0e04
list cltype switch
list cltype switch end
optional none list: 01000000000d0e04
list cltype switch
list cltype switch end
empty list: 04000000000000000e0b
[ OK ]
Test CLValue_ByteSer_ByteArray_Test...          byte array: 0800000001020304050607080f08000000
optional byte array: 090000000101020304050607080d0f08000000
optional none byte array: 01000000000d0f20000000
[ OK ]
Test CLValue_ByteSer_Result_Test...             result ok: 0200000001ff10030a
optional result ok: 030000000101ff0d10030a
result ok_2: 010000000110090a
result err: 0b00000000060000004572726f722110090a
optional result err: 0c0000000100060000004572726f72210d10090a
optional none result err: 01000000000d10030a
[ OK ]
Test CLValue_ByteSer_Map_Test...                map size2
map: 1c00000002000000040000006b65793101000000040000006b65793202000000110a04
optional map: 1d0000000102000000040000006b65793101000000040000006b657932020000000d110a04
optional none map: 01000000000d110a04
empty map: 0400000000000000110a0b
[ OK ]
Test CLValue_ByteSer_Tuple1_Test...             tuple1: 04000000110000001204
tuple1 str: 09000000050000004142434445120a
optional tuple1: 0a000000010500000041424344450d120a
optional none tuple1: 01000000000d120a
[ OK ]
Test CLValue_ByteSer_Tuple2_Test...             tuple2: 08000000110000007f000000130404
tuple2 str: 0d0000007f00000005000000414243444513040a
optional tuple2: 0e000000017f0000000500000041424344450d13040a
optional none tuple2: 01000000000d13040a
[ OK ]
Test CLValue_ByteSer_Tuple3_Test...             tuple3: 0c000000110000007f0000001100000014040404
tuple3 str: 110000007f0000000500000041424344457f00000014040a04
optional tuple3: 12000000017f0000000500000041424344457f0000000d14040a04
optional none tuple3: 01000000000d14040a04
[ OK ]
Test CLValue_ByteSer_Any_Test...                [ OK ]
Test ModuleBytes serialize...                   module bytes: 00000000000100000006000000616d6f756e740300000002e80308
[ OK ]
Test StoredContractByHashSerialization...       stored contract by hash: 0101020304010203040102030401020304010203040102030401020304010203040b000000636f756e7465725f696e6300000000
[ OK ]
Test StoredContractByNameSerialization...       stored contract by name: 0207000000636f756e7465720b000000636f756e7465725f696e6300000000
[ OK ]
Test StoredVersionedContractByHashSerialization... stored versioned contract by hash: 03010203040102030401020304010203040102030401020304010203040102030401010000000b000000636f756e7465725f696e6300000000
[ OK ]
Test StoredVersionedContractByNameSerialization... stored versioned contract: 0407000000636f756e746572010f0000000b000000636f756e7465725f696e6300000000
[ OK ]
Test TransferDeployItemSerialization...         transfer item: 050300000006000000616d6f756e74060000000500d6117e030806000000746172676574200000007cfcb2fbdd0e747cabd0f8fe4d743179a764a8d7174ea6f0dfdb0c41fe1348b40f20000000020000006964090000000139300000000000000d05
[ OK ]
Test ED25519 Key Test...                        
[2022-10-12 07:55:15.493] [error] [ED25519Key.cpp:31] File /workspace/casper-cpp-sdk/build/test/data/cpp_sdk_test_secret_key.pem is not a valid ED25519 private key
ed_key.getPrivateKeyStr(): 
ed_key.getPublicKeyStr(): 
in test verify: false
[ OK ]
Test PublicKey Load fromFile...                 
private key: c18453a7598d0c2a8bacf18a7fb1a3897285e6ad7305fc1991c216b124c1bf06
public key: 035724e2530c5c8f298ba41fe1cafa28294ab7b04d4f1ade025a4a268138570b3a
signature: 821aea8b9b9e8ec3bc6fe7ff3bf54c036e1ec7455b5846c2775ada0cba7b1bf48b9b2c3d87b3e4b8a826044a326536bdc744038d6c729169967b434fe98a552d
Verification: true
[ OK ]
Test getAccountHash checks internal PublicKey to AccountHash converter... lower_case_account_hash: account-hash-998c5FD4E7B568Bedd78e05555c83C61893Dc5d8546ce0BEc8B30E1c570f21aA
[ OK ]
Test toLower checks internal lower case converter... [ OK ]
Test gsk test...                                
key_bytes: 33
001b2d1D9069d21f916aB58be305C816B8f5258177d9cF29EeE33728c4e934F094

key_bytes: 33
0196053169B397360449b4de964200bE449594Ca93f252153f0a679b804e214A54

key_bytes: 34
02e48935c79E96C490c01e1E8800dE5Ec5F4A857A57dB0DcFfED1e1E2b5d29b5E407
[ OK ]
Test infoGetPeers checks node list size...      [ OK ]
Test chainGetStateRootHash using Block height parameter... [ OK ]
Test chainGetStateRootHash using invalid Block height parameter... [ OK ]
Test chainGetStateRootHash using Block hash parameter... [ OK ]
Test chainGetStateRootHash using empty Block hash parameter ... [ OK ]
Test infoGetDeploy using Deploy hash parameter... [ OK ]
Test infoGetDeploy using invalid Deploy hash parameter... [ OK ]
Test infoGetStatus compares with a reference value... [ OK ]
Test chainGetBlockTransfers using Block hash parameter... [ OK ]
Test chainGetBlock using Block hash parameter... [ OK ]
Test chainGetEraInfoBySwitchBlock using Block hash parameter ... [ OK ]
Test stateGetItem using state root hash and key parameters ... [ OK ]
Test stateGetItem using invalid state root hash and key parameters ... [ OK ]
Test stateGetDictionaryItem using state root hash and dictionary key  parameters ... [ OK ]
Test stateGetBalance compares with a reference value... [ OK ]
Test stateGetBalance using invalid URef and state root hash parameters ... [ OK ]
Test stateGetAuctionInfo using Block hash parameter (may take a while)... [ OK ]
Test PutDeploy RPC Call with a Stored Contract by Name... sig bytes while loop
{
  "approvals": [
    {
      "signature": "020fa69c0cA1E3920Ac2Eb2356af5413275bbfE85b9DBb9E37763bD108928d549b09A6D73ee9cE98a51076A5b866eFFacbE7D50d82aa5c195754ebC9062a495C63",
      "signer": "02035724e2530c5c8f298ba41fe1cAfa28294Ab7b04d4F1ade025a4a268138570B3A"
    }
  ],
  "hash": "f674ae60c2af7d340e8d9acc31cf85f4f52c5800622ecbf188392d30b8549668",
  "header": {
    "account": "02035724e2530c5c8f298ba41fe1cAfa28294Ab7b04d4F1ade025a4a268138570B3A",
    "body_hash": "f67fafa5cb1425ef8819c236d0cfbe1a144a59c7a909a1c85543e3084b7b2e53",
    "chain_name": "casper-test",
    "dependencies": [],
    "gas_price": 1,
    "timestamp": "2022-10-12T07:55:17.712Z",
    "ttl": "30m"
  },
  "payment": {
    "ModuleBytes": {
      "args": [
        [
          "amount",
          {
            "bytes": "0500d6117e03",
            "cl_type": "U512",
            "parsed": "15000000000"
          }
        ]
      ],
      "module_bytes": ""
    }
  },
  "session": {
    "StoredContractByName": {
      "args": [
        [
          "target",
          {
            "bytes": "0203297ebdcc8cb840e6e5ffb427420ec754ac35364c502f4ac58b0ffea799e57f11",
            "cl_type": {
              "ByteArray": 34
            },
            "parsed": "0203297ebdcc8cb840e6e5ffb427420ec754ac35364c502f4ac58b0ffea799e57f11"
          }
        ],
        [
          "amount",
          {
            "bytes": "0500e8764817",
            "cl_type": "U512",
            "parsed": "100000000000"
          }
        ]
      ],
      "entry_point": "call_faucet",
      "name": "faucet"
    }
  }
}
deploy id: f674ae60c2af7d340e8d9acc31cf85f4f52c5800622ecbf188392d30b8549668
[ OK ]
Test PutDeploy RPC Call with a Transfer...      sig bytes while loop
sig bytes while loop
sig bytes while loop
{
  "approvals": [
    {
      "signature": "02197f2D8f9c2020225B8fB15AeeF03FF539D2Aaa5118936F65CFabC0DF7f4801D59cF3Deaa4d611a6FF13752667816C48647C5EEc5B67378384ed28F9c95f4209",
      "signer": "02035724e2530c5c8f298ba41fe1cAfa28294Ab7b04d4F1ade025a4a268138570B3A"
    }
  ],
  "hash": "f102dd94b0933c1effc753e1bfad73757eb358d9a8b52b86b6c49171557fcc22",
  "header": {
    "account": "02035724e2530c5c8f298ba41fe1cAfa28294Ab7b04d4F1ade025a4a268138570B3A",
    "body_hash": "4a52154eceb5fbf37a265e1a0e5cecac6066a093d7db396ecb7a170966495976",
    "chain_name": "casper-test",
    "dependencies": [],
    "gas_price": 1,
    "timestamp": "2022-10-12T07:55:17.794Z",
    "ttl": "30m"
  },
  "payment": {
    "ModuleBytes": {
      "args": [
        [
          "amount",
          {
            "bytes": "0400ca9a3b",
            "cl_type": "U512",
            "parsed": "1000000000"
          }
        ]
      ],
      "module_bytes": ""
    }
  },
  "session": {
    "Transfer": {
      "args": [
        [
          "amount",
          {
            "bytes": "044d9d9da9",
            "cl_type": "U512",
            "parsed": "2845678925"
          }
        ],
        [
          "target",
          {
            "bytes": "b383c7cc23d18bc1b42406a1b2d29fc8dba86425197b6f553d7fd61375b5e446",
            "cl_type": {
              "ByteArray": 32
            },
            "parsed": "b383c7cc23d18bc1b42406a1b2d29fc8dba86425197b6f553d7fd61375b5e446"
          }
        ],
        [
          "id",
          {
            "bytes": "0179df0d8648700000",
            "cl_type": {
              "Option": "U64"
            },
            "parsed": 123456789012345
          }
        ]
      ]
    }
  }
}
deploy id: f102dd94b0933c1effc753e1bfad73757eb358d9a8b52b86b6c49171557fcc22
[ OK ]
Test PutDeploy RPC Call with a Stored Contract by Hash... sig bytes while loop
sig bytes while loop
sig bytes while loop
{
  "approvals": [
    {
      "signature": "028aa01cBE127e0a5665cEd25BD2Ec17D9897E7711adff39CBEafBDd1976Ef21620a4134d34d52c7986B5DE33210E11c9EC8E39eCa47744Be42f6f203483621C11",
      "signer": "02035724e2530c5c8f298ba41fe1cAfa28294Ab7b04d4F1ade025a4a268138570B3A"
    }
  ],
  "hash": "af4c93a4e7b3f19b4a08be3ed1a8a03f640f982159db801c61a8cdede6fa9693",
  "header": {
    "account": "02035724e2530c5c8f298ba41fe1cAfa28294Ab7b04d4F1ade025a4a268138570B3A",
    "body_hash": "de2d11652516fbddf1d232ff33e1c647be63c208934c77b52577caa98c4f4d70",
    "chain_name": "casper-test",
    "dependencies": [],
    "gas_price": 1,
    "timestamp": "2022-10-12T07:55:17.886Z",
    "ttl": "30m"
  },
  "payment": {
    "ModuleBytes": {
      "args": [
        [
          "amount",
          {
            "bytes": "0500f2052a01",
            "cl_type": "U512",
            "parsed": "5000000000"
          }
        ]
      ],
      "module_bytes": ""
    }
  },
  "session": {
    "StoredContractByHash": {
      "args": [
        [
          "receipient_publickey",
          {
            "bytes": "42000000303166323866313639646164313733313561303364313565313661613933643533343233303361653131663135633638616164666461623364663331623066636266",
            "cl_type": "String",
            "parsed": "01f28f169dad17315a03d15e16aa93d5342303ae11f15c68aadfdab3df31b0fcbf"
          }
        ],
        [
          "bsc_transaction_hash",
          {
            "bytes": "42000000307864366537663561613536316530363963333835643066363361336338646335353031663633643336313663333631373439653565666162393737366661333365",
            "cl_type": "String",
            "parsed": "0xd6e7f5aa561e069c385d0f63a3c8dc5501f63d3616c361749e5efab9776fa33e"
          }
        ],
        [
          "amount",
          {
            "bytes": "0500e571dd07",
            "cl_type": "U512",
            "parsed": "33780000000"
          }
        ]
      ],
      "entry_point": "unlock_cspr",
      "hash": "e3523602448b6085b861890b1c214181e2c1a7bdd2b23424b1941d1301256517"
    }
  }
}
deploy id: af4c93a4e7b3f19b4a08be3ed1a8a03f640f982159db801c61a8cdede6fa9693
[ OK ]
Test CLType...                                  json: {"Map":{"key":"String","value":{"List":"PublicKey"}}}
final json: {"Map":{"key":"String","value":{"List":"PublicKey"}}}
[ OK ]
Test CLType json...                             [ OK ]
Test CLType List<String>...                     json: {"List":"String"}
final json: {"List":"String"}
[ OK ]
Test CLValue parsed...                          
{
  "bytes": "06da6662305f01",
  "cl_type": "U512",
  "parsed": "1508345276122"
}

{
  "bytes": "06da6662305f01",
  "cl_type": "U512",
  "parsed": "1508345276122"
}
[ OK ]
Test CLType Tuple1...                           json: {"Tuple1":["Unit"]}
final json: {"Tuple1":["Unit"]}
[ OK ]
Test CLType Tuple2...                           json: {"Tuple2":["Bool","I32"]}
final json: {"Tuple2":["Bool","I32"]}
[ OK ]
Test CLType Tuple2 recursive...                 json: {"Tuple2":["U256",{"List":"Any"}]}
final json: {"Tuple2":["U256",{"List":"Any"}]}
[ OK ]
Test CLType Tuple3...                           json: {"Tuple3":["I32","String",{"Option":"U512"}]}
final json: {"Tuple3":["I32","String",{"Option":"U512"}]}
[ OK ]
Test CLType Option...                           json: {"Option":"Bool"}
final json: {"Option":"Bool"}
[ OK ]
Test CLType Option recursive...                 json: {"Option":{"List":{"Map":{"key":"U64","value":"U8"}}}}
final json: {"Option":{"List":{"Map":{"key":"U64","value":"U8"}}}}
[ OK ]
Test CLValue using Bool expected false...       /workspace/casper-cpp-sdk/test

{
  "bytes": "00",
  "cl_type": "Bool",
  "parsed": false
}

{
  "bytes": "00",
  "cl_type": "Bool",
  "parsed": false
}
[ OK ]
Test CLValue using Bool expected true...        /workspace/casper-cpp-sdk/test

{
  "bytes": "01",
  "cl_type": "Bool",
  "parsed": true
}

{
  "bytes": "01",
  "cl_type": "Bool",
  "parsed": true
}
[ OK ]
Test CLValue using I32...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "10270000",
  "cl_type": "I32",
  "parsed": 10000
}

{
  "bytes": "10270000",
  "cl_type": "I32",
  "parsed": 10000
}
[ OK ]
Test CLValue using I64...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "99bdf7ffffffffff",
  "cl_type": "I64",
  "parsed": -541287
}

{
  "bytes": "99bdf7ffffffffff",
  "cl_type": "I64",
  "parsed": -541287
}
[ OK ]
Test CLValue using U8...                        /workspace/casper-cpp-sdk/test

{
  "bytes": "00000000000000",
  "cl_type": "U8",
  "parsed": 7
}

{
  "bytes": "00000000000000",
  "cl_type": "U8",
  "parsed": 7
}
[ OK ]
Test CLValue using U32...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "32b30000",
  "cl_type": "U32",
  "parsed": 45874
}

{
  "bytes": "32b30000",
  "cl_type": "U32",
  "parsed": 45874
}
[ OK ]
Test CLValue using U64...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "a9f0826881010000",
  "cl_type": "U64",
  "parsed": 1655315820713
}

{
  "bytes": "a9f0826881010000",
  "cl_type": "U64",
  "parsed": 1655315820713
}
[ OK ]
Test CLValue using U128...                      /workspace/casper-cpp-sdk/test

{
  "bytes": "04bf3d3209",
  "cl_type": "U128",
  "parsed": "154287551"
}

{
  "bytes": "04bf3d3209",
  "cl_type": "U128",
  "parsed": "154287551"
}
[ OK ]
Test CLValue using U256...                      /workspace/casper-cpp-sdk/test

{
  "bytes": "092e1a2022a7d14f69f6",
  "cl_type": "U256",
  "parsed": "4545487556545454545454"
}

{
  "bytes": "092e1a2022a7d14f69f6",
  "cl_type": "U256",
  "parsed": "4545487556545454545454"
}
[ OK ]
Test CLValue using U256-2...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "20ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
  "cl_type": "U256",
  "parsed": "115792089237316195423570985008687907853269984665640564039457584007913129639935"
}

{
  "bytes": "20ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
  "cl_type": "U256",
  "parsed": "115792089237316195423570985008687907853269984665640564039457584007913129639935"
}
[ OK ]
Test CLValue using U512...                      /workspace/casper-cpp-sdk/test

{
  "bytes": "0412e8571b",
  "cl_type": "U512",
  "parsed": "458745874"
}

{
  "bytes": "0412e8571b",
  "cl_type": "U512",
  "parsed": "458745874"
}
[ OK ]
Test CLValue using U512-0...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "00",
  "cl_type": "U512",
  "parsed": "0"
}

{
  "bytes": "00",
  "cl_type": "U512",
  "parsed": "0"
}
[ OK ]
Test CLValue using Unit...                      /workspace/casper-cpp-sdk/test

{
  "bytes": "",
  "cl_type": "Unit",
  "parsed": null
}

{
  "bytes": "",
  "cl_type": "Unit",
  "parsed": null
}
[ OK ]
Test CLValue using String...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "0d00000048656c6c6f2c20776f726c6421",
  "cl_type": "String",
  "parsed": "Hello, world!"
}

{
  "bytes": "0d00000048656c6c6f2c20776f726c6421",
  "cl_type": "String",
  "parsed": "Hello, world!"
}
[ OK ]
Test CLValue using URef...                      /workspace/casper-cpp-sdk/test

{
  "bytes": "c27f301c04ea62c7610d9a3a6c220dc7101bea61b827d559fa7763d7b570148507",
  "cl_type": "URef",
  "parsed": "uref-c27f301c04ea62c7610d9a3a6c220dc7101bea61b827d559fa7763d7b5701485-007"
}

{
  "bytes": "c27f301c04ea62c7610d9a3a6c220dc7101bea61b827d559fa7763d7b570148507",
  "cl_type": "URef",
  "parsed": "uref-c27f301c04ea62c7610d9a3a6c220dc7101bea61b827d559fa7763d7b5701485-007"
}
[ OK ]
Test CLValue using Key...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "03e330a31701205e3871cb4f7e14d3ff26074735c84b0e54b7a75f553a8405d182",
  "cl_type": "Key",
  "parsed": {
    "Transfer": "transfer-e330a31701205e3871cb4f7e14d3ff26074735c84b0e54b7a75f553a8405d182"
  }
}

{
  "bytes": "03e330a31701205e3871cb4f7e14d3ff26074735c84b0e54b7a75f553a8405d182",
  "cl_type": "Key",
  "parsed": {
    "Transfer": "transfer-E330a31701205E3871cb4f7e14D3FF26074735C84b0E54B7A75F553a8405d182"
  }
}
[ OK ]
Test CLValue using PublicKey...                 /workspace/casper-cpp-sdk/test

{
  "bytes": "020201bfe26b36896d840975023089c8ec3b91d7e9db4cbfeef2b827c6f0ce8afd97",
  "cl_type": "PublicKey",
  "parsed": "020201bfe26b36896d840975023089c8ec3b91d7e9db4cbfeef2b827c6f0ce8afd97"
}

{
  "bytes": "020201bfe26b36896d840975023089c8ec3b91d7e9db4cbfeef2b827c6f0ce8afd97",
  "cl_type": "PublicKey",
  "parsed": "020201BfE26b36896d840975023089C8ec3b91d7E9DB4cBFeef2B827c6f0CE8afd97"
}
[ OK ]
Test CLValue using Option...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "010d00000048656c6c6f2c20576f726c6421",
  "cl_type": {
    "Option": "String"
  },
  "parsed": "Hello, World!"
}

CLTypeRVA from_json 3


{
  "bytes": "010d00000048656c6c6f2c20576f726c6421",
  "cl_type": {
    "Option": "String"
  },
  "parsed": "Hello, World!"
}
[ OK ]
Test CLValue using Option<List<Key>> = NULL...  /workspace/casper-cpp-sdk/test

{
  "bytes": "00",
  "cl_type": {
    "Option": {
      "List": "Key"
    }
  },
  "parsed": null
}

CLTypeRVA from_json 3


{
  "bytes": "00",
  "cl_type": {
    "Option": {
      "List": "Key"
    }
  },
  "parsed": null
}
[ OK ]
Test CLValue using Option<U64> = NULL...        /workspace/casper-cpp-sdk/test

{
  "bytes": "00",
  "cl_type": {
    "Option": "U64"
  },
  "parsed": null
}

CLTypeRVA from_json 3


{
  "bytes": "00",
  "cl_type": {
    "Option": "U64"
  },
  "parsed": null
}
[ OK ]
Test CLValue using Option<U64>...               /workspace/casper-cpp-sdk/test

{
  "bytes": "011fe0963d80010000",
  "cl_type": {
    "Option": "U64"
  },
  "parsed": 1650300739615
}

CLTypeRVA from_json 3


{
  "bytes": "011fe0963d80010000",
  "cl_type": {
    "Option": "U64"
  },
  "parsed": 1650300739615
}
[ OK ]
Test CLValue using List...                      /workspace/casper-cpp-sdk/test

{
  "bytes": "030000000300000061626304000000646566670a00000068696a6b6c6d6e6f7071",
  "cl_type": {
    "List": "String"
  },
  "parsed": [
    "abc",
    "defg",
    "hijklmnopq"
  ]
}

CLTypeRVA from_json 3


{
  "bytes": "030000000300000061626304000000646566670a00000068696a6b6c6d6e6f7071",
  "cl_type": {
    "List": "String"
  },
  "parsed": [
    "abc",
    "defg",
    "hijklmnopq"
  ]
}
[ OK ]
Test CLValue using List<ByteArray:32>...        /workspace/casper-cpp-sdk/test

{
  "bytes": "04000000f64291132b63043e56ca7ab3bd83d87008f5c317d22b07061f14199d37648d9d577d1b93dde787f48507353a1aa4195019a8fc2273559a556a83de33c97ae290120e8e62826ab59f378b6ac96b1df67f0e084c18d5275ee9c6ae68c8ada0713b45f3aa6ce2a450dd5a4f2cc4cc9054aded66de6b6cfc4ad977e7251cf94b649b",
  "cl_type": {
    "List": {
      "ByteArray": 32
    }
  },
  "parsed": [
    "f64291132b63043e56ca7ab3bd83d87008f5c317d22b07061f14199d37648d9d",
    "577d1b93dde787f48507353a1aa4195019a8fc2273559a556a83de33c97ae290",
    "120e8e62826ab59f378b6ac96b1df67f0e084c18d5275ee9c6ae68c8ada0713b",
    "45f3aa6ce2a450dd5a4f2cc4cc9054aded66de6b6cfc4ad977e7251cf94b649b"
  ]
}

CLTypeRVA from_json 3


{
  "bytes": "04000000f64291132b63043e56ca7ab3bd83d87008f5c317d22b07061f14199d37648d9d577d1b93dde787f48507353a1aa4195019a8fc2273559a556a83de33c97ae290120e8e62826ab59f378b6ac96b1df67f0e084c18d5275ee9c6ae68c8ada0713b45f3aa6ce2a450dd5a4f2cc4cc9054aded66de6b6cfc4ad977e7251cf94b649b",
  "cl_type": {
    "List": {
      "ByteArray": 32
    }
  },
  "parsed": [
    "f64291132b63043e56ca7ab3bd83d87008f5c317d22b07061f14199d37648d9d",
    "577d1b93dde787f48507353a1aa4195019a8fc2273559a556a83de33c97ae290",
    "120e8e62826ab59f378b6ac96b1df67f0e084c18d5275ee9c6ae68c8ada0713b",
    "45f3aa6ce2a450dd5a4f2cc4cc9054aded66de6b6cfc4ad977e7251cf94b649b"
  ]
}
[ OK ]
Test CLValue using List<Option<String>>...      /workspace/casper-cpp-sdk/test

{
  "bytes": "04000000010600000076616c756531010600000076616c75653200010600000076616c756534",
  "cl_type": {
    "List": {
      "Option": "String"
    }
  },
  "parsed": [
    "value1",
    "value2",
    "null",
    "value4"
  ]
}

CLTypeRVA from_json 3


CLTypeRVA from_json 3


CLTypeRVA from_json 3


CLTypeRVA from_json 3


CLTypeRVA from_json 3


{
  "bytes": "04000000010600000076616c756531010600000076616c75653200010600000076616c756534",
  "cl_type": {
    "List": {
      "Option": "String"
    }
  },
  "parsed": [
    "value1",
    "value2",
    "null",
    "value4"
  ]
}
[ OK ]
Test CLValue using List<U8>...                  /workspace/casper-cpp-sdk/test

{
  "bytes": "0400000001010100",
  "cl_type": {
    "List": "U8"
  },
  "parsed": [
    1,
    1,
    1,
    0
  ]
}

CLTypeRVA from_json 3


{
  "bytes": "0400000001010100",
  "cl_type": {
    "List": "U8"
  },
  "parsed": [
    1,
    1,
    1,
    0
  ]
}
[ OK ]
Test CLValue using List<U256>...                /workspace/casper-cpp-sdk/test

{
  "bytes": "010000000108",
  "cl_type": {
    "List": "U256"
  },
  "parsed": [
    "8"
  ]
}

CLTypeRVA from_json 3


{
  "bytes": "010000000108",
  "cl_type": {
    "List": "U256"
  },
  "parsed": [
    "8"
  ]
}
[ OK ]
Test CLValue using ByteArray...                 /workspace/casper-cpp-sdk/test

{
  "bytes": "a1d74503458cbc18bd50b205faf9e5ce31439a2a146cbf7efa30c6514728d37e",
  "cl_type": {
    "ByteArray": 32
  },
  "parsed": "a1d74503458cbc18bd50b205faf9e5ce31439a2a146cbf7efa30c6514728d37e"
}

{
  "bytes": "a1d74503458cbc18bd50b205faf9e5ce31439a2a146cbf7efa30c6514728d37e",
  "cl_type": {
    "ByteArray": 32
  },
  "parsed": "a1d74503458cbc18bd50b205faf9e5ce31439a2a146cbf7efa30c6514728d37e"
}
[ OK ]
Test CLValue using Map...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "0500000015000000636f6e74726163745f7061636b6167655f6861736840000000303365336530396232386463346434316134353037623338303733653761313634316265636330623430653739626562373237333364326662303232646566610a0000006576656e745f747970650e00000065726332305f7472616e736665720400000066726f6d4e0000004b65793a3a4163636f756e7428303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030302902000000746f4e0000004b65793a3a4163636f756e742832383266616262383761303537643939313933373737303232336465393861653836663665363532613035303832356161313936646664346634383030323965290500000076616c756515000000313030303030303030303030303030303030303030",
  "cl_type": {
    "Map": {
      "key": "String",
      "value": "String"
    }
  },
  "parsed": [
    {
      "key": "contract_package_hash",
      "value": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa"
    },
    {
      "key": "event_type",
      "value": "erc20_transfer"
    },
    {
      "key": "from",
      "value": "Key::Account(0000000000000000000000000000000000000000000000000000000000000000)"
    },
    {
      "key": "to",
      "value": "Key::Account(282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e)"
    },
    {
      "key": "value",
      "value": "100000000000000000000"
    }
  ]
}

{
  "bytes": "0500000015000000636f6e74726163745f7061636b6167655f6861736840000000303365336530396232386463346434316134353037623338303733653761313634316265636330623430653739626562373237333364326662303232646566610a0000006576656e745f747970650e00000065726332305f7472616e736665720400000066726f6d4e0000004b65793a3a4163636f756e7428303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030303030302902000000746f4e0000004b65793a3a4163636f756e742832383266616262383761303537643939313933373737303232336465393861653836663665363532613035303832356161313936646664346634383030323965290500000076616c756515000000313030303030303030303030303030303030303030",
  "cl_type": {
    "Map": {
      "key": "String",
      "value": "String"
    }
  },
  "parsed": [
    {
      "key": "contract_package_hash",
      "value": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa"
    },
    {
      "key": "event_type",
      "value": "erc20_transfer"
    },
    {
      "key": "from",
      "value": "Key::Account(0000000000000000000000000000000000000000000000000000000000000000)"
    },
    {
      "key": "to",
      "value": "Key::Account(282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e)"
    },
    {
      "key": "value",
      "value": "100000000000000000000"
    }
  ]
}
[ OK ]
Test CLValue using Tuple1...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "050000006162636566",
  "cl_type": {
    "Tuple1": [
      "String"
    ]
  },
  "parsed": [
    "abcef"
  ]
}

{
  "bytes": "050000006162636566",
  "cl_type": {
    "Tuple1": [
      "String"
    ]
  },
  "parsed": [
    "abcef"
  ]
}
[ OK ]
Test CLValue using Tuple2...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "030000006162630102",
  "cl_type": {
    "Tuple2": [
      "String",
      "U512"
    ]
  },
  "parsed": [
    "abc",
    "2"
  ]
}

{
  "bytes": "030000006162630102",
  "cl_type": {
    "Tuple2": [
      "String",
      "U512"
    ]
  },
  "parsed": [
    "abc",
    "2"
  ]
}
[ OK ]
Test CLValue using Tuple3...                    /workspace/casper-cpp-sdk/test

{
  "bytes": "01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa901030000006162630102",
  "cl_type": {
    "Tuple3": [
      "PublicKey",
      {
        "Option": "String"
      },
      "U512"
    ]
  },
  "parsed": [
    "01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa9",
    "abc",
    "2"
  ]
}

CLTypeRVA from_json 3


{
  "bytes": "01a018bf278f32fdb7b06226071ce399713ace78a28d43a346055060a660ba7aa901030000006162630102",
  "cl_type": {
    "Tuple3": [
      "PublicKey",
      {
        "Option": "String"
      },
      "U512"
    ]
  },
  "parsed": [
    "01a018bf278F32fdb7B06226071Ce399713acE78a28D43A346055060a660Ba7AA9",
    "abc",
    "2"
  ]
}
[ OK ]
Test CLValue using Any...                       /workspace/casper-cpp-sdk/test

{
  "bytes": "99040000040000001bab414e1bab414e4000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234400000006661623731643331313833633963376464633538323534343535363539313738303563623131386436313234626332663936316265626534303534366165613701400000003536343263653333613665336438666337316666366465633837396339386332356533383463666432353262343766623734356563363964346134656661343201400000003839643961666163326330616530366231386339383431316435653964306332326330326436363930366435623734316132303730653362626465313034613606000000706c61796564014000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234c15ccb6fc15ccb6f4000000035363432636533336136653364386663373166663664656338373963393863323565333834636664323532623437666237343565633639643461346566613432400000006132356631376666633432616637323532646136386161393063383732333465623966643937373636356432373836326237303337633063383739386264636601400000006165343761393235363434326132313361353561323334313462613132346665623262643531663334353762336334316138353331643631643832376237623401400000003963653638643236316530303162353239326161313335356665303534313835343561393835353435383736646433366630303836633637353337363830326106000000706c61796564014000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234ebeb0797ebeb07974000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234400000003265306236323133616334313964373832343866343433316136623661643136636533373431343034396564326362356438653936376635646263643332663200000900000063616e63656c6c656400d2cc9fa0d2cc9fa04000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234400000003839663866656366623532323433613763366161393031613738333162663864313530623232393634613765336130356663653132336637616561333035383101400000003536343263653333613665336438666337316666366465633837396339386332356533383463666432353262343766623734356563363964346134656661343201400000006135396530623433646338376666306437613737646435376535616332636433303362636330356632343232373065626639323861613231363739613961353904000000746965640011041414040a0a130d0a0d0a130a0d0a200000005bfa005126f0b6a7aaef5a8575a05154518b265e4ea11f3036e5bb6daebca9b7050000006d6f766573",
  "cl_type": "Any",
  "parsed": null
}

{
  "bytes": "99040000040000001bab414e1bab414e4000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234400000006661623731643331313833633963376464633538323534343535363539313738303563623131386436313234626332663936316265626534303534366165613701400000003536343263653333613665336438666337316666366465633837396339386332356533383463666432353262343766623734356563363964346134656661343201400000003839643961666163326330616530366231386339383431316435653964306332326330326436363930366435623734316132303730653362626465313034613606000000706c61796564014000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234c15ccb6fc15ccb6f4000000035363432636533336136653364386663373166663664656338373963393863323565333834636664323532623437666237343565633639643461346566613432400000006132356631376666633432616637323532646136386161393063383732333465623966643937373636356432373836326237303337633063383739386264636601400000006165343761393235363434326132313361353561323334313462613132346665623262643531663334353762336334316138353331643631643832376237623401400000003963653638643236316530303162353239326161313335356665303534313835343561393835353435383736646433366630303836633637353337363830326106000000706c61796564014000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234ebeb0797ebeb07974000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234400000003265306236323133616334313964373832343866343433316136623661643136636533373431343034396564326362356438653936376635646263643332663200000900000063616e63656c6c656400d2cc9fa0d2cc9fa04000000061653437613932353634343261323133613535613233343134626131323466656232626435316633343537623363343161383533316436316438323762376234400000003839663866656366623532323433613763366161393031613738333162663864313530623232393634613765336130356663653132336637616561333035383101400000003536343263653333613665336438666337316666366465633837396339386332356533383463666432353262343766623734356563363964346134656661343201400000006135396530623433646338376666306437613737646435376535616332636433303362636330356632343232373065626639323861613231363739613961353904000000746965640011041414040a0a130d0a0d0a130a0d0a200000005bfa005126f0b6a7aaef5a8575a05154518b265e4ea11f3036e5bb6daebca9b7050000006d6f766573",
  "cl_type": "Any",
  "parsed": null
}
[ OK ]
SUCCESS: All unit tests have passed.

```
