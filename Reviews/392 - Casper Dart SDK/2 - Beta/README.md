Grant Proposal | [392 - Casper Dart SDK](https://portal.devxdao.com/public-proposals/392)
------------ | -------------
Milestone | 2
Milestone Title | Beta 
OP | cdolaz
Reviewer | Kien Nguyen

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

In addition to Alpha requirements, the project now implements all available RPC methods, all available Casper types

**Acceptance criteria:**

- All RPC methods can be called and return an appropriate response 
- All Casper Types are available in the Dart SDK

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/cdolaz/casper_dart_sdk | de78cb7

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/cdolaz/casper_dart_sdk, reviewer was
able to successfully build the source code for this milestone.

## Overall Impression of usage testing

The project builds without errors, the documentation provides sufficient installation and execution instructions, and the project functionality meets the acceptance criteria and operates without errors.

``` sh
casper_dart_sdk git:(main) ✗ dart run build_runner build
[INFO] Generating build script completed, took 559ms
[INFO] Precompiling build script... completed, took 4.8s
[INFO] Building new asset graph completed, took 511ms
[INFO] Checking for unexpected pre-existing outputs. completed, took 4.0s
[INFO] Running build completed, took 8.5s
[INFO] Caching finalized dependency graph completed, took 41ms
[INFO] Succeeded after 8.6s with 56 outputs (130 actions)
```

1. rpc.discover
``` dart
 _casperClient.getRpcSchema().then((dynamic result) {
      print('getRpcSchema');
      print(result);
    });
```
``` json
{api_version: 1.3.2, name: OpenRPC Schema, schema: {openrpc: 1.0.0-rc1, info: {version: 1.3.2, title: Client API of Casper Node, description: This describes the JSON-RPC 2.0 API of a node on the Casper network., contact: {name: Casper, url: https://casper.network}, license: {name: Apache License Version 2.0, url: https://raw.githubusercontent.com/casper-network/casper-node/master/LICENSE}}, servers: [{name: any Casper Network node, url: http://IP:PORT/rpc/}], methods: [{name: account_put_deploy, summary: receives a Deploy to be executed by the network, params: [{name: deploy, schema: {description: The `Deploy`., $ref: #/components/schemas/Deploy}, required: true}], result: {name: account_put_deploy_result, schema: {description: Result for "account_put_deploy" RPC response., type: object, required: [api_version, deploy_hash], properties: {api_version: {description: The RPC API version., type: string}, deploy_hash: {description: The deploy hash., $ref: #/components/schemas/DeployHash}}, <…>
```
2. info_get_peers

``` dart
_casperClient.getPeers().then((GetPeersResult result) {
      print('getPeers');
      result.peers.forEach((element) => print(element.address.toString()));
      setState(() {
        _casperPeerIds = result.peers;
      });
    });
```

```
flutter: getPeers
flutter: 54.183.43.215:41898
flutter: 185.206.122.33:52668
flutter: 195.201.142.76:40120
flutter: 65.108.78.120:45876
flutter: 31.7.194.205:35000
flutter: 65.21.79.108:40258
flutter: 135.181.216.81:45586
flutter: 65.21.129.12:35000
flutter: 135.181.140.236:39578
flutter: 65.108.127.242:39930
....
```
3. chain_get_state_root_hash

```dart
_casperClient.getStateRootHash().then((GetStateRootHashResult result) {
      print('getStateRootHash');
      print(result.stateRootHash);
    });
```
```
flutter: getStateRootHash
flutter: 2c6af39cb8bcda66763047ddd424ee2b98f3506af02e2fc3cf5cae2357c8574b
```
4. info_get_deploy
``` dart
 _casperClient
        .getDeploy(
            '82eae6985dfb2e7053b95c9bc4a42a251b52cac040d0f809332f4a4d35baea6d')
        .then((GetDeployResult result) {
      print('getDeploy');
      print(result.deploy.hash.toString());
      printObject(result.deploy.header);
    });
```
```
flutter: getDeploy
flutter: 82eae6985dfb2e7053b95c9bc4a42a251b52cac040d0f809332f4a4d35baea6d
flutter: {
flutter:   "account": "02021172744B5e6bdC83a591b75765712e068e5D40a3bE8Ae360274fB26503b4AD38",
flutter:   "timestamp": "2022-03-29T09:17:01.663Z",
flutter:   "ttl": "30m",
flutter:   "gas_price": 1,
flutter:   "body_hash": "cdd38aff716fe376b4996f516c052af930d7ea22a15219ad54ade941e4f9eea0",
flutter:   "dependencies": [],
flutter:   "chain_name": "casper"
flutter: }
```
5. info_get_status

```dart
 _casperClient.getStatus().then((GetStatusResult result) {
      print('getStatus');
      print(result.chainspecName.toString());
    });
```

```
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: NoSuchMethodError: The method 'split' was called on null.
Receiver: null
Tried calling: split(" ")
#0      Object.noSuchMethod (dart:core-patch/object_patch.dart:38:5)
#1      HumanReadableDurationJsonConverter.fromJson (package:casper_dart_sdk/src/helpers/string_utils.dart:61:37)
#2      _$GetStatusResultFromJson (package:casper_dart_sdk/src/jsonrpc/generated/get_status.g.dart:28:12)
#3      new GetStatusResult.fromJson (package:casper_dart_sdk/src/jsonrpc/get_status.dart:34:66)
#4      CasperNodeRpcClient.getStatus (package:casper_dart_sdk/src/http/casper_node_client.dart:36:28)
<asynchronous suspension>
```
6. chain_get_block

```dart
BlockId blockId = BlockId.fromHeight(755366);
_casperClient.getBlock(blockId).then((GetBlockResult result) {
      print('getBlock');
      print(result.block?.hash.toString());
    });
```

```
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: RPC Exception: -32001 block not known
#0      ServerProxyBase._handleDecoded (package:jsonrpc2/src/client_base.dart:90:7)
#1      ServerProxyBase._handleResponse (package:jsonrpc2/src/client_base.dart:85:12)
#2      ServerProxyBase.call (package:jsonrpc2/src/client_base.dart:63:12)
<asynchronous suspension>
#3      CasperNodeRpcClient.getBlock (package:casper_dart_sdk/src/http/casper_node_client.dart:40:36)
<asynchronous suspension>
```
7. chain_get_block_transfers
```dart
BlockId blockId = BlockId.fromHeight(755366);
 _casperClient
        .getBlockTransfers(blockId)
        .then((GetBlockTransfersResult result) {
      print('getBlockTransfers');
      result.transfers.forEach((element) => print(element.deployHash));
    });
```
```
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: RPC Exception: -32001 block not known
#0      ServerProxyBase._handleDecoded (package:jsonrpc2/src/client_base.dart:90:7)
#1      ServerProxyBase._handleResponse (package:jsonrpc2/src/client_base.dart:85:12)
#2      ServerProxyBase.call (package:jsonrpc2/src/client_base.dart:63:12)
<asynchronous suspension>
#3      CasperNodeRpcClient.getBlockTransfers (package:casper_dart_sdk/src/http/casper_node_client.dart:44:45)
<asynchronous suspension>
```
8. state_get_balance
Reviewer tried to get balance for some account however the balance is always 0.

```dart
  Uref uref = Uref(
        "uref-660086859ff0e57116d05d4311cb21e78fc60ebe17e32eb6d01053d403dc7859-007");
    _casperClient.getBalance(uref).then((GetBalanceResult result) {
      print('getBalance');
      print(result.balanceValue);
    });
```
```
flutter: getBalance
flutter: 0
```
9. query_global_state
OP is using `query_global_state` method which should be `state_get_item`
```dart
_casperClient.queryGlobalState(
        "hash-6fe7d28174ae5946d1f805f38a7cb546842897b33f0220840f0638d156673e97",
        "fd68f20ddb31647ca7c2008c483a1c0ff642e342743b25e14dbc6fc541cdeb1b",
        false,
        ['symbol']).then((QueryGlobalStateResult result) {
      print('queryGlobalState');
      print(result.storedValue);
    });
```
```
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: RPC Exception: -32601 Method not found
#0      ServerProxyBase._handleDecoded (package:jsonrpc2/src/client_base.dart:90:7)
#1      ServerProxyBase._handleResponse (package:jsonrpc2/src/client_base.dart:85:12)
#2      ServerProxyBase.call (package:jsonrpc2/src/client_base.dart:63:12)
<asynchronous suspension>
#3      CasperNodeRpcClient.queryGlobalState (package:casper_dart_sdk/src/http/casper_node_client.dart:52:44)
<asynchronous suspension>
```
10. chain_get_era_info_by_switch_block

```dart
BlockId blockId = BlockId.fromHeight(755366);
_casperClient
        .getEraInfoBySwitchBlock(blockId)
        .then((GetEraInfoBySwitchBlockResult result) {
      print('getEraInfoBySwitchBlock');
      print(result.eraSummary?.blockHash.toString());
    });
```
```
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: RPC Exception: -32001 block not known
#0      ServerProxyBase._handleDecoded (package:jsonrpc2/src/client_base.dart:90:7)
#1      ServerProxyBase._handleResponse (package:jsonrpc2/src/client_base.dart:85:12)
#2      ServerProxyBase.call (package:jsonrpc2/src/client_base.dart:63:12)
<asynchronous suspension>
#3      CasperNodeRpcClient.getEraInfoBySwitchBlock (package:casper_dart_sdk/src/http/casper_node_client.dart:56:51)
<asynchronous suspension>
```
11. state_get_auction_info
```dart
BlockId blockId = BlockId.fromHeight(755366);
_casperClient.getAuctionInfo(blockId).then((GetAuctionInfoResult result) {
      print('getAuctionInfo');
      print(result.auctionState?.bids.length);
    });
```
```
<asynchronous suspension>
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: RPC Exception: -32001 get-auction-info failed to get specified block
#0      ServerProxyBase._handleDecoded (package:jsonrpc2/src/client_base.dart:90:7)
#1      ServerProxyBase._handleResponse (package:jsonrpc2/src/client_base.dart:85:12)
#2      ServerProxyBase.call (package:jsonrpc2/src/client_base.dart:63:12)
<asynchronous suspension>
#3      CasperNodeRpcClient.getAuctionInfo (package:casper_dart_sdk/src/http/casper_node_client.dart:60:42)
```
12. account_put_deploy
```dart
Deploy deploy = Deploy.fromJson({
      "hash":
          "5262541e0e6f71d35835cac105de01d9f1bd5b6e6cada31474245c58b603a91a",
      "header": {
        "account":
            "02038eefdaf2cd5c68222c773b661d62587f0110859147ce9fc00dd0664b0e7ea8c4",
        "timestamp": "2022-05-08T13:29:24.940Z",
        "ttl": "30m",
        "gas_price": 1,
        "body_hash":
            "6180e6f180f7aabb9d159d91b25d850000475397310ece35e42dccbc6f89d1df",
        "dependencies": [],
        "chain_name": "casper"
      },
      "payment": {
        "ModuleBytes": {
          "module_bytes": "",
          "args": [
            [
              "amount",
              {"bytes": "0400e1f505", "cl_type": "U512"}
            ]
          ]
        }
      },
      "session": {
        "Transfer": {
          "args": [
            [
              "amount",
              {"bytes": "0400f90295", "cl_type": "U512"}
            ],
            [
              "target",
              {
                "bytes":
                    "01cb0f3d9ca3123ab3eb9bd5f6522415c0c6603ffeb1916647e66764956000f860",
                "cl_type": "PublicKey"
              }
            ],
            [
              "id",
              {
                "bytes": "010000000000000000",
                "cl_type": {"Option": "U64"}
              }
            ]
          ]
        }
      },
      "approvals": [
        {
          "signer":
              "02038eefdaf2cd5c68222c773b661d62587f0110859147ce9fc00dd0664b0e7ea8c4",
          "signature":
              "023c70af9621bf992ec8d5e7345964481cedf08fe2db81e4b8bbf333574d70fa46542a68ce726197c9b3437fc2dc422af68391ac8b98c9ebcad36352872b1d383b"
        }
      ]
    });

    _casperClient.putDeploy(deploy).then((result) {
      print("putDeploy");
      print(result.deployHash);
    });
```
```
[VERBOSE-2:ui_dart_state.cc(209)] Unhandled Exception: Converting object to an encodable object failed: Instance of 'JsonRpcMethod'
#0      _JsonStringifier.writeObject (dart:convert/json.dart:794:7)
#1      _JsonStringStringifier.printOn (dart:convert/json.dart:983:17)
#2      _JsonStringStringifier.stringify (dart:convert/json.dart:968:5)
#3      JsonEncoder.convert (dart:convert/json.dart:345:30)
#4      JsonCodec.encode (dart:convert/json.dart:231:45)
#5      ServerProxyBase.call (package:jsonrpc2/src/client_base.dart:60:10)
#6      CasperNodeRpcClient.putDeploy (package:casper_dart_sdk/src/http/casper_node_client.dart:64:43)
#7      CasperClient.putDeploy (package:casper_dart_sdk/src/casper_client.dart:94:24)
#8      _HomePageState._fetchPeers (package:flutter_casper_client/main.dart:193:19)
#9      _InkResponseState._handleTap (package:flutter/src/material/ink_well.dart:989:21)
#10     GestureRecognizer.invokeCallback (package:flutter/src/gestures/recognizer.dart:198:24)
#11     TapGestureRecog<…>
```


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

Reviewer can find unit test for all main and helper functions. The test coverage is good for both positive and negative paths.

[Test Logs](assets/test.json)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Reviewer found that all key functions of the project have low-level code documentation that can be used to automatically generate documentation.

Requirement | Finding
------------ | -------------
Low level function documentation | PASS

### Project Documentation

The README file provides minimum but sufficient documentation on how to build the project. But reviewer suggest to add more usages samples

Requirement | Finding
------------ | -------------
Sufficient Project Documentation | PASS with Notes


# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. The project also has CONTRIBUTING and SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project as committed to GitHub but the manual tests fail so reviewer consider this is a **FAIL** submission.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS 
------------ | -------------
