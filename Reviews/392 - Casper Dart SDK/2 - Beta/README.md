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
https://github.com/cdolaz/casper_dart_sdk | 1907a06

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
flutter: getStatus
flutter: {
flutter:   "api_version": "1.4.5",
flutter:   "build_version": "1.4.5-a7f6a648d-casper-mainnet",
flutter:   "chainspec_name": "casper",
flutter:   "last_added_block_info": {
flutter:     "creator": "01b205C2bd03CE19cD2876CCC21a3566C407b631F3E714532cE0c9956bbac85811",
flutter:     "era_id": 4848,
flutter:     "hash": "4522459433cb7fe51617b501e86ac1ac473270a982b8c90f0b8b42688bb8cee7",
flutter:     "height": 769542,
flutter:     "state_root_hash": "adad015fb3680ebcdde75b3d3f792643b556d7f2861b37fba51218fff34cc9ea",
flutter:     "timestamp": "2022-05-10T14:28:55.936Z"
flutter:   },
flutter:   "next_upgrade": null,
flutter:   "our_public_signing_key": "01e61C8B8227AFD8F7d4Daece145546aa6775cf1c4EbfB6F3f56C18df558AEd72D",
...
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
flutter: getBlock
flutter: {
flutter:   "api_version": "1.4.5",
flutter:   "block": {
flutter:     "hash": "5aba403c1f53803aa7cec736ca965a94ee3615c376451d9443c2a3443c584cbe",
flutter:     "header": {
flutter:       "accumulated_seed": "17c84945ff5092eba468e2474be1b29a751086d13c1b6b478f424b60b25cc980",
flutter:       "body_hash": "6da90c09f3fc4559d27b9fff59ab2453be5752260b07aec65e0e3a61734f656a",
flutter:       "era_end": {
flutter:         "era_report": {
flutter:           "equivocators": [],
flutter:           "inactive_validators": [],
flutter:           "rewards": [
flutter:             {
flutter:               "amount": 113719376251,
flutter:               "validator": "01000E6fce753895c0d08d5D6Af62dB4E9B0D070f10e69E2C6bAdF977b29BBeEeE"
flutter:             },
...
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
flutter: getBlockTransfers
flutter: {
flutter:   "amount": "1191512800000",
flutter:   "deploy_hash": "cb99b492ca6b2b06aaa69525bdb762cb5c85707b73b389ab2fb70f01753bd089",
flutter:   "from": "account-hash-45f3AA6Ce2A450dd5A4F2cC4cC9054Aded66De6B6CfC4ad977e7251CF94B649B",
flutter:   "gas": "0",
flutter:   "id": 1,
flutter:   "source": "uref-6Ad5075aDDCDef0308BF9100a88292fD16e49edeB724DEa2Cc9f6F3730352d97-007",
flutter:   "target": "uref-d41D943D61090B2E792BdF630D3564E73071769f235B987530a7933dEa49dC7e-004",
flutter:   "to": "account-hash-87814ec49fe15f2cb21e033227fb83cfb5f9dd5ac19918d874e3f872013dd959"
flutter: }
flutter: {
flutter:   "amount": "108499900000000",
flutter:   "deploy_hash": "3099d24e811f72cd7f3182475c6d5325774426e8292e66f6f19cc79bb2bdc0f8",
flutter:   "from": "account-hash-FF6b05951976F43E51Ef6cf01eC29a70908Caf623778DEbf414620dAC6b75bbD",
flutter:   "gas": "0",
flutter:   "id": 1,
flutter:   "source": "uref-9C72551dDd3F8D56d4CB72146EE5e5ae040F0DbBE7f7F41C6D77773970540ea9-007",
flutter:   "target": "uref-7950bf87377371651E0927198e2Bc73074A43A804037cC4E20F4a2C21115b7EF-004",
flutter:   "to": "account-hash-496d542527e1a29f576ab7c3f4c947bfcdc9b4145f75f6ec40e36089432d7351"
flutter: }
```
8. state_get_balance


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
flutter: 12164980094631
```
9. query_global_state

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
flutter: queryGlobalState
flutter: {
flutter:   "cl_type": "String",
flutter:   "bytes": "0500000047484f5354",
flutter:   "parsed": "GHOST"
flutter: }
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
flutter: getEraInfoBySwitchBlock
flutter: 5aba403c1f53803aa7cec736ca965a94ee3615c376451d9443c2a3443c584cbe
```
11. state_get_auction_info
```dart
BlockId blockId = BlockId.fromHeight(755366);
_casperClient.getAuctionInfo(blockId).then((GetAuctionInfoResult result) {
      print('getAuctionInfo');
      result.auctionState?.eraValidators[0].validatorWeights
          .forEach((element) => print(element.publicKey.toString()));
    });
```
```
<asynchronous suspension>
flutter: getAuctionInfo
flutter: 01000E6fce753895c0d08d5D6Af62dB4E9B0D070f10e69E2C6bAdF977b29BBeEeE
flutter: 01026Ca707C348eD8012Ac6a1F28Db031fADD6Eb67203501a353b867a08c8b9a80
flutter: 01031cdcE87d5fe53246492f9262932F9eB7421ea54b30dA1ecA06874fd2A7dF60
flutter: 0103dD8b2B18Ef0B9FD5b7C8E340B104EE4d966f2A167Eb1a938963f8C8F699a45
flutter: 010427c1d1227C9D2aAfE8C06c6e6B276DA8DCD8FD170Ca848b8e3E8e1038a6DC8
flutter: 01098d1758f1ca75350DfEC8a1C4c1984a88D1EA5EAb5590Fbc9e856D67CdE31Eb
flutter: 010A78eEF78966A56A633c665411388f97f850609960D5D898f3992272b8d4BccA
flutter: 010A8aC8d23e6c57Fa340C552dDF9199d9cBa9166ECc0daEE640053ebfc6254610
flutter: 010bDF698F2906D01bC4E7643ea7f713ca28433928058aCF54B03FAc9CB6716Db8
flutter: 010e29c0ae47626690861047c5118685421b0F9A77Ee9fecfEDD842a929E3A9F06
...
```
12. account_put_deploy
```dart
 const deploy = {
      "deploy": {
        "hash":
            "c0f3d2f150aca411accaf99c1cdb95bc3a6e69e82ee27fa520e9231b727c3644",
        "header": {
          "account":
              "02021172744b5e6bdc83a591b75765712e068e5d40a3be8ae360274fb26503b4ad38",
          "timestamp": "2022-05-10T17:10:25.748Z",
          "ttl": "30m",
          "gas_price": 1,
          "body_hash":
              "b4592477bd325a8e10ed8d899b6e629e963f750164e8fd95e292cb9df5fe5936",
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
                      "02021172744b5e6bdc83a591b75765712e068e5d40a3be8ae360274fb26503b4ad38",
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
                "02021172744b5e6bdc83a591b75765712e068e5d40a3be8ae360274fb26503b4ad38",
            "signature":
                "0276f38378b3cd13985ac4abc0b4af0ef7eded32ee8b1118274547348c91bddede7c995b8cd2d4ff60aa160a2d66a4daa444624bd752be5ea1d55d4a99b2adbd7e"
          }
        ]
      }
    };
    print(deploy);
    _casperClient.putDeployJson(deploy).then((result) {
      print("putDeploy");
      printObject(result);
    });
```
```
flutter: putDeploy
flutter: {
flutter:   "api_version": "1.4.5",
flutter:   "deploy_hash": "c0f3d2f150aca411accaf99c1cdb95bc3a6e69e82ee27fa520e9231b727c3644"
flutter: }
```
https://cspr.live/deploy/c0f3d2f150aca411accaf99c1cdb95bc3a6e69e82ee27fa520e9231b727c3644

13. All Casper Types are available


Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

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

The README file provides minimum but sufficient documentation on how to build the project. But reviewer suggest to add more usages samples.

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

Code is generally well-structured and readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

The last milestone is about unit testing and documentation. The OP should update the last milestone with more details and usage documentation.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS 
------------ | -------------
