# Casper Scala SDK checklist

## Required methods

| Method                    |                                                              Source                                                              |     |    Notes    |
| ------------------------- |:--------------------------------------------------------------------------------------------------------------------------------:| --- |:-----------:|
| chain_get_block           |        [source](https://github.com/caspercommunityio/casper-scala-sdk/blob/master/src/main/scala/com/casper/sdk/CasperSdk.scala#L43)         | ✅  |Should merge into single function             |
| info_get_deploy           |        [source](https://github.com/caspercommunityio/casper-scala-sdk/blob/master/src/main/scala/com/casper/sdk/CasperSdk.scala#L84)         | ✅  |             |
| account_put_deploy        |        [source](https://github.com/caspercommunityio/casper-scala-sdk/blob/master/src/main/scala/com/casper/sdk/CasperSdk.scala#L140)         | ✅  |             |
| chain_get_state_root_hash |    [source](https://github.com/caspercommunityio/casper-scala-sdk/blob/master/src/main/scala/com/casper/sdk/CasperSdk.scala#L35)     | ✅  |             |
| state_get_account_info    |                                                               N/A                                                                | ❌  | Est: 4hours |
| state_get_balance         |       [source](https://github.com/caspercommunityio/casper-scala-sdk/blob/master/src/main/scala/com/casper/sdk/CasperSdk.scala#L108)        | ✅  |             |
| state_get_dictionary_item | [source](https://github.com/caspercommunityio/casper-scala-sdk/blob/master/src/main/scala/com/casper/sdk/CasperSdk.scala#L124) | ✅  |             |
| query_global_state        |        N/A        | ❌  | Est: 4hours |


## Reviewer notes

- There are 2 missing method `state_get_account_info` and `query_global_state`. The estimated implementation time for each method is 4 hours. 
- The implementation for chain_get_block should be merged to single function and take BlockIdentifier param. The estimated update time for the method is 1 hour.
- Others methods and types are aligned with the SDK standard.
