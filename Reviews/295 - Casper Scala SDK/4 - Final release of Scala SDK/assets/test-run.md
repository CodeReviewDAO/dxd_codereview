```
  sbt test
  shell: /usr/bin/bash -e {0}
  env:
    JAVA_HOME: /opt/hostedtoolcache/Java_Adopt_jdk/11.0.11-9/x64
copying runtime jar...
[info] [launcher] getting org.scala-sbt sbt 1.6.2  (this may take some time)...
[info] [launcher] getting Scala 2.12.15 (for sbt)...
[info] Updated file /home/runner/work/casper-scala-sdk/casper-scala-sdk/project/build.properties: set sbt.version to 1.6.2
[info] welcome to sbt 1.6.2 (AdoptOpenJDK Java 11.0.11)
[info] loading project definition from /home/runner/work/casper-scala-sdk/casper-scala-sdk/project
[info] loading settings for project casper-scala-sdk from build.sbt ...
[info] set current project to casper-scala-sdk (in build file:/home/runner/work/casper-scala-sdk/casper-scala-sdk/)
[info] compiling 117 Scala sources to /home/runner/work/casper-scala-sdk/casper-scala-sdk/target/scala-3.0.2/classes ...
[info] done compiling
[info] compiling 38 Scala sources to /home/runner/work/casper-scala-sdk/casper-scala-sdk/target/scala-3.0.2/test-classes ...
[info] done compiling
[info] ByteUtilTest:
[info] - ByteUtils join Test 
[info] CLPublicKeySerializerTest:
[info] - Test serialize CLPublicKey 
[info] CLPublicKeyDeserializerTest:
[info] - Deserialize CLPublicKey
[info]   + PublicKey is not null 
[info]   + pubKey.bytes  is the same as new CLPublicKey("017d96b9A63ABCB61C870a4f55187A0a7AC24096Bdb5Fc585c12a686a4D892009e").bytes 
[info] DeployExecutableSerializerTest:
[info] - DeployExecutableSerializerTest with StoredVersionedContractByName
[info] - DeployExecutableSerializerTest with StoredVersionedContractByHash
[info] - DeployExecutableSerializerTest with StoredContractByHash
[info] - DeployExecutableSerializerTest with StoredContractByName
[info] - DeployExecutableSerializerTest with DeployTransfer
[info] CLValueDeSerializerTest:
[info] - Deserialize U512 value
[info]   + value is not null 
[info]   + parsed value = 1000000000  
[info]   + cl_type = U512  
[info]   + bytes same as  HexUtils.fromHex("0400ca9A3B")  
[info] - Deserialize PublicKey value
[info]   + value is not null 
[info]   + parsed value = 017d96B9A63abCB61c870A4F55187a0a7AC24096bdB5fc585C12A686a4D892009e  
[info]   + cl_type = PublicKey  
[info]   + bytes same as  HexUtils.fromHex("017d96B9A63abCB61c870A4F55187a0a7AC24096bdB5fc585C12A686a4D892009e")  
[info] - Deserialize byteArray32 value
[info]   + value is not null 
[info]   + parsed value = 2fe0d35b6a92e17ee8f3ee3693452d6141df5c8db8e17a1c0985572842e13385  
[info]   + cl_type = ByteArray  
[info]   + bytes same as  HexUtils.fromHex("2fe0d35b6a92e17ee8f3ee3693452d6141df5c8db8e17a1c0985572842e13385")  
[info] - Deserialize Option value
[info]   + value is not null 
[info]   + parsed value = null 
[info] GetEraInfoBySwitchBlock : 2974-->2975 with blockHash: 1e46B4c173dB70fDE0E867FF679ACa24e1c5Bea3C4333af94e53B4E3BC548B6B
[info] - should succeed
[info]   + assert  era = 2974 
[info]   + assert  state root hash  = c1A62d5DeB74d3fEAfeCd1EEa526941edd0264895EB8E516474108D4EA4D7D21 
[info] GetEraInfoBySwitchBlock with a non switch bloc : a2C85FD13bba200E47c2d7c74E87F0f0c96aDcEE227877168a639Fa67d046933
[info] - should fail
[info] GetEraInfoBySwitchBlock with an empty switch bloc
[info] - should fail
[info] GetStateItem with stateRoothash=30cE5146268305AeeFdCC05a5f7bE7aa6dAF187937Eed9BB55Af90e1D49B7956h,key= hash-4dd10a0b2a7672e8ec964144634ddabb91504fe50b8461bac23584423318887d
[info] - should succeed and retieves a Contract
[info]   + assert contract is not null  
[info]   + assert contract_package_hash = contract-wasm-8D1c5ab95baaa77c302232a00FE1C6cF6975ffD6430a9ECd87EC5266280BB18D 
[info]   + assert first enry point is an allowance  
[info]   + assert first arg of the first entry point is of type CLType = Key   
[info] GetStateItem with stateRoothash=30cE5146268305AeeFdCC05a5f7bE7aa6dAF187937Eed9BB55Af90e1D49B7956h,key=account-hash-46dE97966cfc2F00C326e654baD000AB7a5E26bEBc316EF4D74715335cF32A88
[info] - should succeed and retieves an Account
[info]   + assert contract is  null  
[info]   + assert account is not null  
[info]   + assert main_purse : uref-9cC68775d07c211e44068D5dCc2cC28A67Cb582C3e239E83Bb0c3d067C4D0363-007 
[info] getStateItem   retrieving CLValue
[info] - should succeed
[info] GetStateItem with wrong parameters
[info] - should fail
[info] GetBalance with an existing account
[info] - should succeed
[info]   + Assert balance = 869077209920 motes  
[info] GetBalance with  non hex key account
[info] - should fail
[info] GetBalance with non uref key account
[info] - should fail
[info] GetDictionaryItem with itemKey=a8261377ef9cf8e741dd6858801c71e38c9322e66355586549b75ab24bdd73f2
[info] - should succeed
[info]   + CLValue is not nul   
[info]   + cl_Type is String    
[info]   + CLValue parsed =  "https://caspercommunity.io"  
[info] PutDeploy with aStandard Transfer
[info] - should succeed
[info] Run completed in 18 seconds, 906 milliseconds.
[info] Total number of tests run: 212
[info] Suites: completed 34, aborted 0
[info] Tests: succeeded 212, failed 0, canceled 0, ignored 0, pending 0
[info] All tests passed.
[success] Total time: 41 s, completed Mar 8, 2022, 10:43:51 AM
```
