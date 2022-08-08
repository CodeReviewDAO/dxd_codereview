# Casper Swift SDK checklist

## Required methods

| Method                    |                                                              Source                                                              |     |    Notes    |
| ------------------------- |:--------------------------------------------------------------------------------------------------------------------------------:| --- |:-----------:|
| chain_get_block           |        [source](https://github.com/hienbui9999/CasperSDKInSwift/blob/main/Sources/CasperSDKInSwift/Chain/GetBlock.swift)         | ✅  |             |
| info_get_deploy           |        [source](https://github.com/hienbui9999/CasperSDKInSwift/blob/main/Sources/CasperSDKInSwift/Info/GetDeploy.swift)         | ✅  |             |
| account_put_deploy        |        [source](https://github.com/hienbui9999/CasperSDKInSwift/blob/main/Sources/CasperSDKInSwift/CasperSDK.swift#L253)         | ✅  |             |
| chain_get_state_root_hash |    [source](https://github.com/hienbui9999/CasperSDKInSwift/blob/main/Sources/CasperSDKInSwift/Chain/GetStateRootHash.swift)     | ✅  |             |
| state_get_account_info    |                                                               N/A                                                                | ❌  | Est: 4hours |
| state_get_balance         |       [source](https://github.com/hienbui9999/CasperSDKInSwift/blob/main/Sources/CasperSDKInSwift/State/GetBalance.swift)        | ✅  |             |
| state_get_dictionary_item | [source](https://github.com/hienbui9999/CasperSDKInSwift/blob/main/Sources/CasperSDKInSwift/State/GetDictionaryItemResult.swift) | ✅  |             |
| query_global_state        |        N/A        | ❌  | Est: 4hours |


## Reviewer notes

There are 2 missing method `state_get_account_info` and `query_global_state`. The estimated implementation time for each method is 4 hours. 
Others methods and types are aligned with the SDK standard.
