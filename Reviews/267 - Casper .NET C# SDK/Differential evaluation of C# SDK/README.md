# Casper C# checklist

## Required methods

| Method                    |                                                              Source                                                              |     |    Notes    |
| ------------------------- |:--------------------------------------------------------------------------------------------------------------------------------:| --- |:-----------:|
| chain_get_block           |        [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L241)         | ✅  |             |
| info_get_deploy           |        [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L220)         | ✅  |             |
| account_put_deploy        |        [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L205)         | ✅  |             |
| chain_get_state_root_hash |    [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L13)     | ✅  |             |
| state_get_account_info    |                                                               [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L101)                                                                | ✅  | |
| state_get_balance         |       [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L188)        | ✅  |             |
| state_get_dictionary_item | [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L352) | ✅  |             |
| query_global_state        |        [source](https://github.com/make-software/casper-net-sdk/blob/master/Casper.Network.SDK/JsonRpc/CasperMethods.cs#L162)        | ✅  | |


## Reviewer notes

The SKD is aligned with the SDK standard.