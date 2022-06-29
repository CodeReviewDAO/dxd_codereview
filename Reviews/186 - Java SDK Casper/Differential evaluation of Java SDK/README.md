
# Casper Java SDK checklist

## Required methods

https://docs.casperlabs.io/dapp-dev-guide/sdkspec/json-rpc-minimal/


| Method                    |                                                              Source                                                              |  Implemented   |    Notes    |
| ------------------------- |:--------------------------------------------------------------------------------------------------------------------------------:| --- |:-----------:|
| chain_get_block           |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L55)         | ✅  |   Should be merged into a single call          |
| info_get_deploy           |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L130)         | ✅  |             |
| account_put_deploy        |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L192)          | ✅  |             |
| chain_get_state_root_hash |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L98)   | ✅  |             |
| state_get_account_info    |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L149)                                                                | ✅  | |
| state_get_balance         |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L182)        | ✅  |             |
| state_get_dictionary_item |        [source](https://github.com/syntifi/casper-sdk/blob/main/src/main/java/com/syntifi/casper/sdk/service/CasperService.java#L171)  | ✅  |             |
| query_global_state        |        N/A        | ❌  | Est. : 4 hours|


## Reviewer notes

* There are one missing method : query_global_state. The estimated implementation time for this method is 4 hours.
* The implementation for chain_get_block should be merged to single function and take BlockIdentifier param. The estimated update time for this merge is 1 hour.
* Others methods and types are aligned with the SDK standard.
