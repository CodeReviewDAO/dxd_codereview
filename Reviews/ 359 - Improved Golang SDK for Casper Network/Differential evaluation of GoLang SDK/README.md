# Casper GO SDK checklist

## Required methods

https://docs.casperlabs.io/dapp-dev-guide/sdkspec/json-rpc-minimal/


| Method                    |                                                              Source                                                              |     |    Notes    |
| ------------------------- |:--------------------------------------------------------------------------------------------------------------------------------:| --- |:-----------:|
| chain_get_block           |        [source](https://github.com/casper-ecosystem/casper-golang-sdk/blob/main/sdk/rpc_client.go#L124)         | ✅  | Should be merged into a single call             |
| info_get_deploy           |        [source](https://github.com/casper-ecosystem/casper-golang-sdk/blob/main/sdk/rpc_client.go#L27)          | ✅  |             |
| account_put_deploy        |        [source](https://github.com/casper-ecosystem/casper-golang-sdk/blob/main/sdk/rpc_client.go#L273)           | ✅  |             |
| chain_get_state_root_hash |        [source](https://github.com/casper-ecosystem/casper-golang-sdk/blob/main/sdk/rpc_client.go#L256)    | ✅  |             |
| state_get_account_info    |        N/A        | ❌  | Est.: 4 hours |
| state_get_balance         |        [source](https://github.com/casper-ecosystem/casper-golang-sdk/blob/main/sdk/rpc_client.go#L67)         | ✅  |             |
| state_get_dictionary_item |        N/A        | ❌  | Est.: 4 hours|
| query_global_state        |        N/A        | ❌  | Est.: 4 hours|


## Reviewer notes

* There are three missing methods :  state_get_account_info, state_get_dictionary_item  and query_global_state. The estimated implementation time for each method is 4 hours.
* The implementation for chain_get_block should be merged into a single function and take BlockIdentifier param. The estimated update time for this merge is 1 hour.
* Other methods and types are aligned with the SDK standard.