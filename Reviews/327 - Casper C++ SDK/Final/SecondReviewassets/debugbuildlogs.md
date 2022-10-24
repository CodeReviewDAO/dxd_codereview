# Output of Debug vcpkg cmake command

```sh

-- The C compiler identification is GNU 9.4.0
-- The CXX compiler identification is GNU 9.4.0
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
using deps from vcpkg or system
-- Found Boost: /workspace/casper-cpp-sdk/vcpkg-bin-lin-casper-cpp-sdk/01/installed/x64-linux/include (found suitable version "1.79.0", minimum required is "1.75.0")  
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Failed
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Found OpenSSL: /workspace/casper-cpp-sdk/vcpkg-bin-lin-casper-cpp-sdk/01/installed/x64-linux/debug/lib/libcrypto.a (found version "3.0.5")  
-- Found CryptoPP: optimized;/workspace/casper-cpp-sdk/vcpkg-bin-lin-casper-cpp-sdk/01/installed/x64-linux/lib/libcryptopp.a;debug;/workspace/casper-cpp-sdk/vcpkg-bin-lin-casper-cpp-sdk/01/installed/x64-linux/debug/lib/libcryptopp.a  
-- Configuring done
-- Generating done
-- Build files have been written to: /workspace/casper-cpp-sdk/build

```

# Output of Debug "cmake --build ." command

```sh

[1/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_eol.cxx.o
[2/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_common.cpp.o
[3/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/StringUtil.cpp.o
[4/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_test.cxx.o
[5/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/CEP57Checksum.cpp.o
[6/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/CryptoUtil.cpp.o
[7/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_write.cpp.o
[8/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/pem_read.cpp.o
[9/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/badcert.cxx.o
[10/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/URef.cpp.o
[11/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Utils/LogConfigurator.cpp.o
[12/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/GlobalStateKey.cpp.o
[13/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/ED25519Key.cpp.o
[14/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLType.cpp.o
[15/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/ByteSerializers/BaseByteSerializer.cpp.o
[16/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/Secp256k1Key.cpp.o
[17/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLConverter.cpp.o
[18/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLTypeParsed.cpp.o
[19/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/CLValue.cpp.o
[20/24] Building CXX object lib/cryptopp-pem/CMakeFiles/cryptopp_pem.dir/cryptopp/x509cert.cpp.o
[21/24] Linking CXX static library lib/cryptopp-pem/libcryptopp_pem.a
[22/24] Building CXX object src/CMakeFiles/casper_sdk.dir/include/Types/Deploy.cpp.o
[23/24] Building CXX object src/CMakeFiles/casper_sdk.dir/CasperClient.cpp.o
[24/24] Linking CXX static library src/libcasper_sdk.a

```


