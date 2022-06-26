# Casper PHP checklist

## Required methods

| Method                    |                                                              Source                                                              |     |    Notes    |
| ------------------------- |:--------------------------------------------------------------------------------------------------------------------------------:| --- |:-----------:|
| chain_get_block           |        [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L111)         | ✅  | Missing BlockIdentifier type Ets: 1hour            |
| info_get_deploy           |        [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L96)         | ✅  |             |
| account_put_deploy        |        [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L76)         | ✅  |             |
| chain_get_state_root_hash |    [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L194)     | ✅  |             |
| state_get_account_info    |                                                               [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L204)                                                                | ✅  | |
| state_get_balance         |       [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L222)        | ✅  |             |
| state_get_dictionary_item | [source](https://github.com/make-software/casper-php-sdk/blob/master/src/Rpc/RpcClient.php#L329) | ✅  |             |
| query_global_state        |      N/A        | ❌  | Est: 4hours |


## Reviewer notes

There a missing method `query_global_state`. The estimated implementation time for the method is 4 hours. 
The implementation for `chain_get_block` should be merged to single function and take `BlockIdentifier` param. The estimated update time for the method is 1 hour
Others methods and types are aligned with the SDK standard.