Grant Proposal | [359 - Improved Golang SDK for Casper Network](https://portal.devxdao.com/app/proposal/359)
------------ | -------------
Milestone | 1
Milestone Title | Go SDK improvement
OP | Pavlo Kravchenko
Reviewer | Mikael Grouwet <m.grouwet@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Adding documentation
- Test coverage
- Adding methods for contract deployment
- Basic logic improvements
- Pull-requests review

**Acceptance criteria:**

- Library implements Casper encoding/decoding scheme
- Library implements communication with node RPC
- Library implements wrappers for key pairs under the curves ED25519 and SECP256K1

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/casper-ecosystem/casper-golang-sdk | 718690b

# Install & Usage Testing Procedure and Findings

Reviewer was able to build and run the project by using the instructions given on the README of the project.
The reviewer was facing an issue because the package installer (ubuntu) installed an old version of Go and I had a lot of errors.
So the reviewer installed the version directly from the official website.
Except that, the documentation is clear enough to build and write some examples.

```
go get -u github.com/casper-ecosystem/casper-golang-sdk
go: downloading github.com/pkg/errors v0.9.1
go: downloading golang.org/x/crypto v0.0.0-20210920023735-84f357641f63
go: downloading github.com/robpike/filter v0.0.0-20150108201509-2984852a2183
go: downloading golang.org/x/crypto v0.0.0-20220131195533-30dcbda58838
go: downloading golang.org/x/sys v0.0.0-20210903071746-97244b99971b
go: downloading golang.org/x/sys v0.0.0-20220128215802-99c3d69c2c27
go: downloading github.com/robpike/filter v0.0.0-20210831053821-dcb4225e6ac8
go get: github.com/robpike/filter@v0.0.0-20210831053821-dcb4225e6ac8: parsing go.mod:
	module declares its path as: robpike.io/filter
	        but was required as: github.com/robpike/filter


```

Reviewer was able to make a deploy and runs RPC requests based on the documentation provided :

```
go run example.go 
Result%!(EXTRA sdk.JsonPutDeployRes={e7f466774baad119214787f41ccb84c99750c4234997ea7844237f2dc9ecd531})
```


## Overall Impression of usage testing

The reviewer was able to run the tests successfully. 
Reviewer notes that the tests regarding "SECP256K1" are missing.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The tests run successfully: 

```
?   	github.com/casper-ecosystem/casper-golang-sdk/keypair	[no test files]
=== RUN   TestEd25519KeyPair_AccountHash
--- PASS: TestEd25519KeyPair_AccountHash (0.00s)
=== RUN   TestEd25519KeyPair_AccountHex
--- PASS: TestEd25519KeyPair_AccountHex (0.00s)
=== RUN   TestEd25519KeyPair_ExportPublicKeyInPem
--- PASS: TestEd25519KeyPair_ExportPublicKeyInPem (0.00s)
=== RUN   TestEd25519KeyPair_ParseKeyFiles
--- PASS: TestEd25519KeyPair_ParseKeyFiles (0.00s)
=== RUN   TestEd25519KeyPair_ParseKeyPair
--- PASS: TestEd25519KeyPair_ParseKeyPair (0.00s)
=== RUN   TestEd25519KeyPair_ParseKey32
--- PASS: TestEd25519KeyPair_ParseKey32 (0.00s)
=== RUN   TestEd25519KeyPair_ParseKey64
--- PASS: TestEd25519KeyPair_ParseKey64 (0.00s)
=== RUN   TestEd25519KeyPair_ParseError
--- PASS: TestEd25519KeyPair_ParseError (0.00s)
=== RUN   TestEd25519KeyPair_Random
--- PASS: TestEd25519KeyPair_Random (0.00s)
=== RUN   TestEd25519KeyPair_ExportPrivateKeyInPem
--- PASS: TestEd25519KeyPair_ExportPrivateKeyInPem (0.00s)
=== RUN   TestEd25519KeyPair_Sign
--- PASS: TestEd25519KeyPair_Sign (0.00s)
=== RUN   TestEd25519KeyPair_Verify
--- PASS: TestEd25519KeyPair_Verify (0.00s)
=== RUN   TestEd25519KeyPair_VerifyFalse
--- PASS: TestEd25519KeyPair_VerifyFalse (0.00s)
PASS
ok  	github.com/casper-ecosystem/casper-golang-sdk/keypair/ed25519	0.008s
?   	github.com/casper-ecosystem/casper-golang-sdk/keypair/secp256k1	[no test files]
=== RUN   TestTimeMarshaling
--- PASS: TestTimeMarshaling (0.00s)
=== RUN   TestDeployUtil_HashDeployHeaderCorrectly
--- PASS: TestDeployUtil_HashDeployHeaderCorrectly (0.00s)
=== RUN   TestDeployUtil_HashBodyAndMarshalJSONCorrectly
--- PASS: TestDeployUtil_HashBodyAndMarshalJSONCorrectly (0.00s)
=== RUN   TestDeployUtil_UnmarshalJSONCorrectly
--- PASS: TestDeployUtil_UnmarshalJSONCorrectly (0.00s)
=== RUN   TestDeployUtil_IsDeploy
--- PASS: TestDeployUtil_IsDeploy (0.00s)
=== RUN   TestDeployUtil_MarshalTransfer
--- PASS: TestDeployUtil_MarshalTransfer (0.00s)
=== RUN   TestDeployUtil_NewTransferWithoutId
--- PASS: TestDeployUtil_NewTransferWithoutId (0.00s)
=== RUN   TestDeployUtil_UnmarshalTransfer
--- PASS: TestDeployUtil_UnmarshalTransfer (0.00s)
=== RUN   TestDeployUtil_UnmarshalIncorrectTransfer
--- PASS: TestDeployUtil_UnmarshalIncorrectTransfer (0.00s)
=== RUN   TestDeployUtil_StoredContractByHash
--- PASS: TestDeployUtil_StoredContractByHash (0.00s)
=== RUN   TestDeployUtil_MarshalStoredContractByHash
--- PASS: TestDeployUtil_MarshalStoredContractByHash (0.00s)
=== RUN   TestDeployUtil_MarshalStoredContractByHashMapValue
--- PASS: TestDeployUtil_MarshalStoredContractByHashMapValue (0.00s)
=== RUN   TestDeployUtil_UnmarshalStoredContractByHash
--- PASS: TestDeployUtil_UnmarshalStoredContractByHash (0.00s)
=== RUN   TestDeployUtil_StoredContractByName
--- PASS: TestDeployUtil_StoredContractByName (0.00s)
=== RUN   TestDeployUtil_MarshalStoredContractByName
--- PASS: TestDeployUtil_MarshalStoredContractByName (0.00s)
=== RUN   TestDeployUtil_UnmarshalStoredContractByName
--- PASS: TestDeployUtil_UnmarshalStoredContractByName (0.00s)
=== RUN   TestDeployUtil_StoredVersionedContractByHash
--- PASS: TestDeployUtil_StoredVersionedContractByHash (0.00s)
=== RUN   TestDeployUtil_MarshalStoredVersionedContractByHash
--- PASS: TestDeployUtil_MarshalStoredVersionedContractByHash (0.00s)
=== RUN   TestDeployUtil_UnmarshalStoredVersionedContractByHash
--- PASS: TestDeployUtil_UnmarshalStoredVersionedContractByHash (0.00s)
=== RUN   TestDeployUtil_StoredVersionedContractByName
--- PASS: TestDeployUtil_StoredVersionedContractByName (0.00s)
=== RUN   TestDeployUtil_MarshalStoredVersionedContractByName
--- PASS: TestDeployUtil_MarshalStoredVersionedContractByName (0.00s)
=== RUN   TestDeployUtil_UnmarshalStoredVersionedContractByName
--- PASS: TestDeployUtil_UnmarshalStoredVersionedContractByName (0.00s)
=== RUN   TestDeployUtil_MarshalStoredContractByHashPublicKey
--- PASS: TestDeployUtil_MarshalStoredContractByHashPublicKey (0.00s)
=== RUN   TestDeployUtil_UnmarshalStoredContractByHashPublicKey
--- PASS: TestDeployUtil_UnmarshalStoredContractByHashPublicKey (0.00s)
=== RUN   TestDeployUtil_SetArg
--- PASS: TestDeployUtil_SetArg (0.00s)
=== RUN   TestDeployUtil_SetArgToDeploy
--- PASS: TestDeployUtil_SetArgToDeploy (0.00s)
=== RUN   TestDeployUtil_ShouldNotSetArgToSignedDeploy
--- PASS: TestDeployUtil_ShouldNotSetArgToSignedDeploy (0.00s)
=== RUN   TestDeployUtil_ValidateDeploy
--- PASS: TestDeployUtil_ValidateDeploy (0.00s)
=== RUN   TestDeployUtil_SignDeploy
--- PASS: TestDeployUtil_SignDeploy (0.00s)
=== RUN   TestRpcClient_GetLatestBlock
--- PASS: TestRpcClient_GetLatestBlock (0.22s)
=== RUN   TestRpcClient_GetDeploy
--- PASS: TestRpcClient_GetDeploy (0.11s)
=== RUN   TestRpcClient_GetBlockState
--- PASS: TestRpcClient_GetBlockState (0.13s)
=== RUN   TestRpcClient_GetAccountBalance
--- PASS: TestRpcClient_GetAccountBalance (0.61s)
=== RUN   TestRpcClient_GetAccountBalanceByKeypair
--- PASS: TestRpcClient_GetAccountBalanceByKeypair (0.72s)
=== RUN   TestRpcClient_GetBlockByHeight
--- PASS: TestRpcClient_GetBlockByHeight (0.10s)
=== RUN   TestRpcClient_GetBlockTransfersByHeight
--- PASS: TestRpcClient_GetBlockTransfersByHeight (0.11s)
=== RUN   TestRpcClient_GetBlockByHash
--- PASS: TestRpcClient_GetBlockByHash (0.11s)
=== RUN   TestRpcClient_GetBlockTransfersByHash
--- PASS: TestRpcClient_GetBlockTransfersByHash (0.11s)
=== RUN   TestRpcClient_GetLatestBlockTransfers
--- PASS: TestRpcClient_GetLatestBlockTransfers (0.18s)
=== RUN   TestRpcClient_GetValidator
--- PASS: TestRpcClient_GetValidator (2.70s)
=== RUN   TestRpcClient_GetStatus
--- PASS: TestRpcClient_GetStatus (0.11s)
=== RUN   TestRpcClient_GetPeers
--- PASS: TestRpcClient_GetPeers (0.11s)
=== RUN   TestRpcClient_PutDeploy
--- PASS: TestRpcClient_PutDeploy (0.11s)
PASS
ok  	github.com/casper-ecosystem/casper-golang-sdk/sdk	5.431s
=== RUN   TestEncoding
--- PASS: TestEncoding (0.00s)
=== RUN   TestDecoding
--- PASS: TestDecoding (0.00s)
PASS
ok  	github.com/casper-ecosystem/casper-golang-sdk/serialization	0.005s
=== RUN   TestEncoding
--- PASS: TestEncoding (0.00s)
=== RUN   TestDecoding
--- PASS: TestDecoding (0.00s)
=== RUN   TestParsingURefString
--- PASS: TestParsingURefString (0.00s)
=== RUN   TestToURefString
--- PASS: TestToURefString (0.00s)
PASS
ok  	github.com/casper-ecosystem/casper-golang-sdk/types	0.003s

```

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS with notes
Unit Tests - At least one negative path test | PASS with notes
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The code could be more commented but the name of the functions are clear enough to understand theirs goals.

Requirement | Finding
------------ | -------------
Code Documented | PASS with notes

### Project Documentation

The reviewer observed that the README of the project has detailed general and usage documentation. The README could be improved to be more readable.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with notes

## Overall Conclusion on Documentation

The reviewer concludes that the project has sufficient comprehensive general documentation. 

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. The repository doesnt contains a CONTRIBUTING and a SECURITY policy. The repository lacks also relevant tags, hindering its discoverability.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes

# Coding Standards

## General Observations

Code is generally well-structured and readable but could be more documented. Also the unit tests regarding SECP256K1 can be added to have more code coverage.

Even if the README is clear enough to understand the SDK, it should be good to improve it with : 
- Which version og Go the user should install
- A dedicated website for the technical documentation (eg : using Github Pages) instead of having most of the structs in the README

# Final Conclusion
The project meets the functional requirements. The reviewer was able to build and run the unit tests. The reviewer recommend to add unit tests for the keypairs under the curve SECP256K1.
The documentation could also be improved for a better user experience. Especially the installation procedure which was not clear about the version of Go to install.
The reviewer suggest to add the missing policies and complete the the repository's informations to improve its discoverability.

Thus, in the reviewer's opinion, this submission should PASS with notes.

# Recommendation

Recommendation | PASS with notes
------------ | -------------

