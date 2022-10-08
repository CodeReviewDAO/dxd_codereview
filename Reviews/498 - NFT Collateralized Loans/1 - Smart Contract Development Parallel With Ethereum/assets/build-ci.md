```
make build-contract-liquid-factory && make build-contract-liquid-helper && make build-contract-liquid-locker && make copy-wasm-file-js-client && make generate-key && make build-jsclients
make[1]: Entering directory '/home/circleci/project'
cargo build --release -p liquid-factory -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
    Updating crates.io index
 Downloading crates ...
  Downloaded borsh-schema-derive-internal v0.8.2
  Downloaded ahash v0.4.7
  Downloaded sha2 v0.8.2
  Downloaded subtle v1.0.0
  Downloaded renvm-sig v0.1.1
  Downloaded wee_alloc v0.4.5
  Downloaded strsim v0.9.3
  Downloaded borsh-derive-internal v0.8.2
  Downloaded crypto-mac v0.7.0
  Downloaded casperlabs-erc20 v0.2.3
  Downloaded hmac v0.7.1
  Downloaded keccak v0.1.2
  Downloaded cryptoxide v0.3.6
  Downloaded derive_builder v0.9.0
  Downloaded casper-contract v1.4.4
  Downloaded hashbrown v0.9.1
  Downloaded darling_macro v0.10.2
  Downloaded proc-macro-crate v0.1.5
  Downloaded arrayref v0.3.6
  Downloaded opaque-debug v0.2.3
  Downloaded tiny-keccak v2.0.2
  Downloaded generic-array v0.12.4
  Downloaded rustc-hex v2.1.0
  Downloaded getrandom v0.1.16
  Downloaded fake-simd v0.1.2
  Downloaded memory_units v0.4.0
  Downloaded darling_core v0.10.2
  Downloaded sha3 v0.9.1
  Downloaded digest v0.8.1
  Downloaded hmac-drbg v0.2.0
  Downloaded byte-tools v0.3.1
  Downloaded block-padding v0.2.1
  Downloaded darling v0.10.2
  Downloaded libsecp256k1 v0.3.5
  Downloaded ident_case v1.0.1
  Downloaded derive_builder_core v0.9.0
  Downloaded borsh-derive v0.8.2
  Downloaded casperlabs-contract-utils v0.1.4
  Downloaded casperlabs-cep47 v0.2.1
  Downloaded casper_types_derive v0.1.0
  Downloaded borsh v0.8.2
  Downloaded block-padding v0.1.5
  Downloaded block-buffer v0.7.3
   Compiling proc-macro2 v1.0.43
   Compiling unicode-ident v1.0.4
   Compiling quote v1.0.21
   Compiling syn v1.0.99
   Compiling typenum v1.15.0
   Compiling version_check v0.9.4
   Compiling autocfg v1.1.0
   Compiling cfg-if v1.0.0
   Compiling getrandom v0.1.16
   Compiling subtle v2.4.1
   Compiling serde_derive v1.0.144
   Compiling serde v1.0.144
   Compiling unicode-xid v0.2.4
   Compiling byteorder v1.4.3
   Compiling radium v0.3.0
   Compiling crunchy v0.2.2
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling opaque-debug v0.3.0
   Compiling ppv-lite86 v0.2.16
   Compiling block-padding v0.2.1
   Compiling serde_json v1.0.85
   Compiling ryu v1.0.11
   Compiling wee_alloc v0.4.5
   Compiling static_assertions v1.1.0
   Compiling hex v0.4.3
   Compiling itoa v1.0.3
   Compiling rand_core v0.6.4
   Compiling hex_fmt v0.3.0
   Compiling memory_units v0.4.0
   Compiling ident_case v1.0.1
   Compiling fnv v1.0.7
   Compiling base64 v0.13.0
   Compiling strsim v0.9.3
   Compiling cfg-if v0.1.10
   Compiling base16 v0.2.1
   Compiling bitflags v1.3.2
   Compiling subtle v1.0.0
   Compiling byte-tools v0.3.1
   Compiling ahash v0.4.7
   Compiling opaque-debug v0.2.3
   Compiling fake-simd v0.1.2
   Compiling tiny-keccak v2.0.2
   Compiling derive_builder v0.9.0
   Compiling thiserror v1.0.35
   Compiling cryptoxide v0.3.6
   Compiling arrayref v0.3.6
   Compiling keccak v0.1.2
   Compiling rustc-hex v2.1.0
   Compiling rand v0.8.5
   Compiling block-padding v0.1.5
   Compiling hashbrown v0.9.1
   Compiling num-traits v0.2.15
   Compiling num-integer v0.1.45
   Compiling num-bigint v0.4.3
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling generic-array v0.14.6
   Compiling uint v0.9.3
   Compiling rand_core v0.5.1
   Compiling bitvec v0.18.5
   Compiling rand_chacha v0.2.2
   Compiling rand v0.7.3
   Compiling generic-array v0.12.4
   Compiling digest v0.8.1
   Compiling crypto-mac v0.7.0
   Compiling block-buffer v0.7.3
   Compiling hmac v0.7.1
   Compiling sha2 v0.8.2
   Compiling digest v0.9.0
   Compiling block-buffer v0.9.0
   Compiling crypto-mac v0.10.1
   Compiling crypto-mac v0.8.0
   Compiling hmac-drbg v0.2.0
   Compiling signature v1.2.2
   Compiling hmac v0.10.1
   Compiling blake2 v0.9.2
   Compiling sha2 v0.9.9
   Compiling sha3 v0.9.1
   Compiling ed25519 v1.2.0
   Compiling libsecp256k1 v0.3.5
   Compiling num-complex v0.4.2
   Compiling ff v0.8.0
   Compiling group v0.8.0
   Compiling num v0.4.0
   Compiling synstructure v0.12.6
   Compiling darling_core v0.10.2
   Compiling borsh-schema-derive-internal v0.8.2
   Compiling borsh-derive-internal v0.8.2
   Compiling zeroize_derive v1.3.2
   Compiling num-derive v0.3.3
   Compiling casper_types_derive v0.1.0
   Compiling thiserror-impl v1.0.35
   Compiling darling_macro v0.10.2
   Compiling zeroize v1.3.0
   Compiling elliptic-curve v0.8.5
   Compiling curve25519-dalek v3.2.1
   Compiling ecdsa v0.10.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling darling v0.10.2
   Compiling derive_builder_core v0.9.0
   Compiling serde_bytes v0.11.7
   Compiling toml v0.5.9
   Compiling casper-types v1.5.0
   Compiling proc-macro-crate v0.1.5
   Compiling borsh-derive v0.8.2
   Compiling borsh v0.8.2
   Compiling renvm-sig v0.1.1
   Compiling casper-contract v1.4.4
   Compiling casperlabs-contract-utils v0.1.4
   Compiling common v0.2.0 (/home/circleci/project/Contracts/common)
   Compiling liquid-base-crate v0.2.0 (/home/circleci/project/Contracts/liquid-base-crate)
   Compiling liquid-transfer-crate v0.2.0 (/home/circleci/project/Contracts/liquid-transfer-crate)
   Compiling casperlabs-cep47 v0.2.1
   Compiling casperlabs-erc20 v0.2.3
   Compiling liquid-helper-crate v0.2.0 (/home/circleci/project/Contracts/liquid-helper/liquid-helper-crate)
   Compiling liquid-locker-crate v0.2.0 (/home/circleci/project/Contracts/liquid-locker/liquid-locker-crate)
warning: unnecessary parentheses around method argument
   --> Contracts/liquid-locker/liquid-locker-crate/src/liquid_locker.rs:216:21
    |
216 |                     (prepay_amount
    |                     ^
217 |                         .checked_div(epoch_payback)
218 |                         .unwrap_or_revert_with(Error::LiquidLockerDivision0)),
    |                                                                             ^
    |
    = note: `#[warn(unused_parens)]` on by default
help: remove these parentheses
    |
216 ~                     prepay_amount
217 |                         .checked_div(epoch_payback)
218 ~                         .unwrap_or_revert_with(Error::LiquidLockerDivision0),
    |

   Compiling liquid-factory-crate v0.2.0 (/home/circleci/project/Contracts/liquid-factory/liquid-factory-crate)
warning: `liquid-locker-crate` (lib) generated 1 warning
   Compiling cep47 v0.2.0 (/home/circleci/project/Contracts/mock-cep47)
   Compiling liquid-factory v0.2.0 (/home/circleci/project/Contracts/liquid-factory/liquid-factory)
   Compiling erc20 v0.2.0 (/home/circleci/project/Contracts/mock-erc20)
    Finished release [optimized] target(s) in 41.05s
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
cargo build --release -p liquid-helper -p liquid-helper-proxy --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
   Compiling liquid-helper-proxy v0.2.0 (/home/circleci/project/Contracts/liquid-helper/liquid-helper-proxy)
   Compiling liquid-helper v0.2.0 (/home/circleci/project/Contracts/liquid-helper/liquid-helper)
    Finished release [optimized] target(s) in 2.49s
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
cargo build --release -p liquid-locker -p liquid-locker-proxy -p cep47 -p erc20 --target wasm32-unknown-unknown && wasm-strip target/wasm32-unknown-unknown/release/*.wasm 2>/dev/null | true
   Compiling liquid-locker-proxy v0.2.0 (/home/circleci/project/Contracts/liquid-locker/liquid-locker-proxy)
warning: unnecessary parentheses around method argument
   --> Contracts/liquid-locker/liquid-locker-crate/src/liquid_locker.rs:216:21
    |
216 |                     (prepay_amount
    |                     ^
217 |                         .checked_div(epoch_payback)
218 |                         .unwrap_or_revert_with(Error::LiquidLockerDivision0)),
    |                                                                             ^
    |
    = note: `#[warn(unused_parens)]` on by default
help: remove these parentheses
    |
216 ~                     prepay_amount
217 |                         .checked_div(epoch_payback)
218 ~                         .unwrap_or_revert_with(Error::LiquidLockerDivision0),
    |

warning: `liquid-locker-crate` (lib) generated 1 warning
   Compiling liquid-locker v0.2.0 (/home/circleci/project/Contracts/liquid-locker/liquid-locker)
    Finished release [optimized] target(s) in 3.75s
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
cp target/wasm32-unknown-unknown/release/liquid-factory.wasm JsClients/LiquidNFT-Factory/LiquidNFT-Factory/wasm
cp target/wasm32-unknown-unknown/release/erc20-token.wasm JsClients/uniswapV2Core-erc20/ERC20/wasm
cp target/wasm32-unknown-unknown/release/cep47-token.wasm JsClients/casper-cep47/wasm
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
rm -rf keys
rm -rf JsClients/keys	
rm -rf JsClients/casper-cep47/keys
rm -rf JsClients/LiquidNFT/LiquidNFT/keys
rm -rf JsClients/LiquidNFT-Factory/LiquidNFT-Factory/keys
rm -rf JsClients/uniswapV2Core-erc20/ERC20/keys
rm -rf JsClients/LiquidNFT-Factory-Tests-Scripts/keys
rm -rf JsClients/LiquidNFT-Factory-Tests-Scripts/mainContractFlowScript/keys
rm -rf JsClients/LiquidNFT-Factory-Tests-Scripts/tooLateLiquidateFlowScript/keys
casper-client keygen ./keys
Wrote files to ./keys
cp -R ./keys JsClients/casper-cep47 
cp -R ./keys JsClients/LiquidNFT-Factory/LiquidNFT-Factory
cp -R ./keys JsClients/LiquidNFT-Factory-Tests-Scripts
cp -R ./keys JsClients/LiquidNFT/LiquidNFT
cp -R ./keys JsClients/uniswapV2Core-erc20/ERC20
cp -R ./keys JsClients/LiquidNFT-Factory-Tests-Scripts/mainContractFlowScript
cp -R ./keys JsClients/LiquidNFT-Factory-Tests-Scripts/tooLateLiquidateFlowScript
cp -R ./keys JsClients	
make[1]: Leaving directory '/home/circleci/project'
make[1]: Entering directory '/home/circleci/project'
cd JsClients/LiquidNFT-Factory/LiquidNFT-Factory/ && npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.

> secp256k1@4.0.3 install /home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/ethereum-cryptography/node_modules/secp256k1
> node-gyp-build || exit 0


> keccak@3.0.2 install /home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/keccak
> node-gyp-build || exit 0


> secp256k1@3.7.1 install /home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/secp256k1
> npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."


> secp256k1@3.7.1 rebuild /home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/secp256k1
> node-gyp rebuild

make[2]: Entering directory '/home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/secp256k1/build'
  CXX(target) Release/obj.target/secp256k1/src/addon.o
In file included from ../src/addon.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../src/addon.cc:1:
../src/addon.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
   50 | NODE_MODULE(secp256k1, Init)
      | ^~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/privatekey.o
In file included from ../src/privatekey.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
   73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
      |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/publickey.o
In file included from ../src/publickey.cc:3:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/signature.o
In file included from ../src/signature.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
In file included from ../src/ecdsa.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
      |                                                                                                                                   ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
      |                                                                                                                                  ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
  CXX(target) Release/obj.target/secp256k1/src/ecdh.o
In file included from ../src/ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
  SOLINK_MODULE(target) Release/obj.target/secp256k1.node
  COPY Release/secp256k1.node
make[2]: Leaving directory '/home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/secp256k1/build'

> eccrypto@1.1.6 install /home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/eccrypto
> node-gyp rebuild || exit 0

make[2]: Entering directory '/home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/eccrypto/build'
  CXX(target) Release/obj.target/ecdh/ecdh.o
In file included from ../ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../ecdh.cc:1:
../ecdh.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
  131 | NODE_MODULE(ecdh, InitAll)
      | ^~~~~~~~~~~
  SOLINK_MODULE(target) Release/obj.target/ecdh.node
  COPY Release/ecdh.node
make[2]: Leaving directory '/home/circleci/project/JsClients/LiquidNFT-Factory/node_modules/eccrypto/build'
added 222 packages in 10.141s
cd JsClients/casper-cep47/ && npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.

> secp256k1@4.0.2 install /home/circleci/project/JsClients/casper-cep47/node_modules/ethereum-cryptography/node_modules/secp256k1
> node-gyp-build || exit 0


> keccak@3.0.2 install /home/circleci/project/JsClients/casper-cep47/node_modules/keccak
> node-gyp-build || exit 0


> secp256k1@3.7.1 install /home/circleci/project/JsClients/casper-cep47/node_modules/secp256k1
> npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."


> secp256k1@3.7.1 rebuild /home/circleci/project/JsClients/casper-cep47/node_modules/secp256k1
> node-gyp rebuild

make[2]: Entering directory '/home/circleci/project/JsClients/casper-cep47/node_modules/secp256k1/build'
  CXX(target) Release/obj.target/secp256k1/src/addon.o
In file included from ../src/addon.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../src/addon.cc:1:
../src/addon.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
   50 | NODE_MODULE(secp256k1, Init)
      | ^~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/privatekey.o
In file included from ../src/privatekey.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
   73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
      |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/publickey.o
In file included from ../src/publickey.cc:3:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/signature.o
In file included from ../src/signature.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
In file included from ../src/ecdsa.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
      |                                                                                                                                   ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
      |                                                                                                                                  ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
  CXX(target) Release/obj.target/secp256k1/src/ecdh.o
In file included from ../src/ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
  SOLINK_MODULE(target) Release/obj.target/secp256k1.node
  COPY Release/secp256k1.node
make[2]: Leaving directory '/home/circleci/project/JsClients/casper-cep47/node_modules/secp256k1/build'

> eccrypto@1.1.6 install /home/circleci/project/JsClients/casper-cep47/node_modules/eccrypto
> node-gyp rebuild || exit 0

make[2]: Entering directory '/home/circleci/project/JsClients/casper-cep47/node_modules/eccrypto/build'
  CXX(target) Release/obj.target/ecdh/ecdh.o
In file included from ../ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../ecdh.cc:1:
../ecdh.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
  131 | NODE_MODULE(ecdh, InitAll)
      | ^~~~~~~~~~~
  SOLINK_MODULE(target) Release/obj.target/ecdh.node
  COPY Release/ecdh.node
make[2]: Leaving directory '/home/circleci/project/JsClients/casper-cep47/node_modules/eccrypto/build'
added 217 packages in 9.591s
cd JsClients/LiquidNFT/LiquidNFT/ && npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.

> secp256k1@4.0.3 install /home/circleci/project/JsClients/LiquidNFT/node_modules/ethereum-cryptography/node_modules/secp256k1
> node-gyp-build || exit 0


> keccak@3.0.2 install /home/circleci/project/JsClients/LiquidNFT/node_modules/keccak
> node-gyp-build || exit 0


> secp256k1@3.7.1 install /home/circleci/project/JsClients/LiquidNFT/node_modules/secp256k1
> npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."


> secp256k1@3.7.1 rebuild /home/circleci/project/JsClients/LiquidNFT/node_modules/secp256k1
> node-gyp rebuild

make[2]: Entering directory '/home/circleci/project/JsClients/LiquidNFT/node_modules/secp256k1/build'
  CXX(target) Release/obj.target/secp256k1/src/addon.o
In file included from ../src/addon.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../src/addon.cc:1:
../src/addon.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
   50 | NODE_MODULE(secp256k1, Init)
      | ^~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/privatekey.o
In file included from ../src/privatekey.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
   73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
      |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/publickey.o
In file included from ../src/publickey.cc:3:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/signature.o
In file included from ../src/signature.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
In file included from ../src/ecdsa.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
      |                                                                                                                                   ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
      |                                                                                                                                  ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
  CXX(target) Release/obj.target/secp256k1/src/ecdh.o
In file included from ../src/ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
  SOLINK_MODULE(target) Release/obj.target/secp256k1.node
  COPY Release/secp256k1.node
make[2]: Leaving directory '/home/circleci/project/JsClients/LiquidNFT/node_modules/secp256k1/build'

> eccrypto@1.1.6 install /home/circleci/project/JsClients/LiquidNFT/node_modules/eccrypto
> node-gyp rebuild || exit 0

make[2]: Entering directory '/home/circleci/project/JsClients/LiquidNFT/node_modules/eccrypto/build'
  CXX(target) Release/obj.target/ecdh/ecdh.o
In file included from ../ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../ecdh.cc:1:
../ecdh.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
  131 | NODE_MODULE(ecdh, InitAll)
      | ^~~~~~~~~~~
  SOLINK_MODULE(target) Release/obj.target/ecdh.node
  COPY Release/ecdh.node
make[2]: Leaving directory '/home/circleci/project/JsClients/LiquidNFT/node_modules/eccrypto/build'
added 229 packages in 9.969s
cd JsClients/uniswapV2Core-erc20/ && npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.

> secp256k1@4.0.3 install /home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/ethereum-cryptography/node_modules/secp256k1
> node-gyp-build || exit 0


> keccak@3.0.2 install /home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/keccak
> node-gyp-build || exit 0


> secp256k1@3.7.1 install /home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/secp256k1
> npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."


> secp256k1@3.7.1 rebuild /home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/secp256k1
> node-gyp rebuild

make[2]: Entering directory '/home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/secp256k1/build'
  CXX(target) Release/obj.target/secp256k1/src/addon.o
In file included from ../src/addon.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../src/addon.cc:1:
../src/addon.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
   50 | NODE_MODULE(secp256k1, Init)
      | ^~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/privatekey.o
In file included from ../src/privatekey.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
   73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
      |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/publickey.o
In file included from ../src/publickey.cc:3:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/signature.o
In file included from ../src/signature.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
In file included from ../src/ecdsa.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
      |                                                                                                                                   ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
      |                                                                                                                                  ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
  CXX(target) Release/obj.target/secp256k1/src/ecdh.o
In file included from ../src/ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
  SOLINK_MODULE(target) Release/obj.target/secp256k1.node
  COPY Release/secp256k1.node
make[2]: Leaving directory '/home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/secp256k1/build'

> eccrypto@1.1.6 install /home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/eccrypto
> node-gyp rebuild || exit 0

make[2]: Entering directory '/home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/eccrypto/build'
  CXX(target) Release/obj.target/ecdh/ecdh.o
In file included from ../ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../ecdh.cc:1:
../ecdh.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
  131 | NODE_MODULE(ecdh, InitAll)
      | ^~~~~~~~~~~
  SOLINK_MODULE(target) Release/obj.target/ecdh.node
  COPY Release/ecdh.node
make[2]: Leaving directory '/home/circleci/project/JsClients/uniswapV2Core-erc20/node_modules/eccrypto/build'
added 232 packages in 9.779s
cd JsClients/LiquidNFT-Factory-Tests-Scripts/mainContractFlowScript/&& npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.
added 68 packages in 1.355s
cd JsClients/LiquidNFT-Factory-Tests-Scripts/tooLateLiquidateFlowScript/&& npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.
added 68 packages in 1.436s
cd JsClientsForFrontend/LiquidNFT/&& npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.

> secp256k1@4.0.3 install /home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/ethereum-cryptography/node_modules/secp256k1
> node-gyp-build || exit 0


> keccak@3.0.2 install /home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/keccak
> node-gyp-build || exit 0


> secp256k1@3.7.1 install /home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/secp256k1
> npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."


> secp256k1@3.7.1 rebuild /home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/secp256k1
> node-gyp rebuild

make[2]: Entering directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/secp256k1/build'
  CXX(target) Release/obj.target/secp256k1/src/addon.o
In file included from ../src/addon.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../src/addon.cc:1:
../src/addon.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
   50 | NODE_MODULE(secp256k1, Init)
      | ^~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/privatekey.o
In file included from ../src/privatekey.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
   73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
      |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/publickey.o
In file included from ../src/publickey.cc:3:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/signature.o
In file included from ../src/signature.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
In file included from ../src/ecdsa.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
      |                                                                                                                                   ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
      |                                                                                                                                  ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
  CXX(target) Release/obj.target/secp256k1/src/ecdh.o
In file included from ../src/ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
  SOLINK_MODULE(target) Release/obj.target/secp256k1.node
  COPY Release/secp256k1.node
make[2]: Leaving directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/secp256k1/build'

> eccrypto@1.1.6 install /home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/eccrypto
> node-gyp rebuild || exit 0

make[2]: Entering directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/eccrypto/build'
  CXX(target) Release/obj.target/ecdh/ecdh.o
In file included from ../ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../ecdh.cc:1:
../ecdh.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
  131 | NODE_MODULE(ecdh, InitAll)
      | ^~~~~~~~~~~
  SOLINK_MODULE(target) Release/obj.target/ecdh.node
  COPY Release/ecdh.node
make[2]: Leaving directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT/node_modules/eccrypto/build'
added 236 packages in 9.72s
cd JsClientsForFrontend/LiquidNFT-Factory/&& npm cache clean --force && npm ci
npm WARN using --force I sure hope you know what you are doing.

> secp256k1@4.0.3 install /home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/ethereum-cryptography/node_modules/secp256k1
> node-gyp-build || exit 0


> keccak@3.0.2 install /home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/keccak
> node-gyp-build || exit 0


> secp256k1@3.7.1 install /home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/secp256k1
> npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."


> secp256k1@3.7.1 rebuild /home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/secp256k1
> node-gyp rebuild

make[2]: Entering directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/secp256k1/build'
  CXX(target) Release/obj.target/secp256k1/src/addon.o
In file included from ../src/addon.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../src/addon.cc:1:
../src/addon.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
   50 | NODE_MODULE(secp256k1, Init)
      | ^~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/privatekey.o
In file included from ../src/privatekey.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
   73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
      |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CXX(target) Release/obj.target/secp256k1/src/publickey.o
In file included from ../src/publickey.cc:3:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/signature.o
In file included from ../src/signature.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
In file included from ../src/ecdsa.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
      |                                                                                                                                   ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
   89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
      |                                                                                                                                  ^
In file included from /home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:67,
                 from ../src/ecdsa.cc:1:
/home/circleci/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
 3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
      |                                     ^~~
  CXX(target) Release/obj.target/secp256k1/src/ecdh.o
In file included from ../src/ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
  CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
  SOLINK_MODULE(target) Release/obj.target/secp256k1.node
  COPY Release/secp256k1.node
make[2]: Leaving directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/secp256k1/build'

> eccrypto@1.1.6 install /home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/eccrypto
> node-gyp rebuild || exit 0

make[2]: Entering directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/eccrypto/build'
  CXX(target) Release/obj.target/ecdh/ecdh.o
In file included from ../ecdh.cc:2:
../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
 2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
      |                                                              ^
In file included from ../ecdh.cc:1:
../ecdh.cc: At global scope:
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
  793 |       (node::addon_register_func) (regfunc),                          \
      |                                           ^
/home/circleci/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
  827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
      |   ^~~~~~~~~~~~~
../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
  131 | NODE_MODULE(ecdh, InitAll)
      | ^~~~~~~~~~~
  SOLINK_MODULE(target) Release/obj.target/ecdh.node
  COPY Release/ecdh.node
make[2]: Leaving directory '/home/circleci/project/JsClientsForFrontend/LiquidNFT-Factory/node_modules/eccrypto/build'
added 242 packages in 9.781s
make[1]: Leaving directory '/home/circleci/project'
```
