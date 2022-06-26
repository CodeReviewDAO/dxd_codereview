```
1..7
ok 1 - Test get state root hash based on block_identifier of type hash, Passed
ok 2 - Test get state root hash based on block_identifier of type height, Passed
ok 3 - Test get state root hash with block identifier set with no param - latest state_root_hash is retrieved, Passed
ok 4 - Test get state root hash with wrong block identifier hash - latest state_root_hash is retrieved, Passed
ok 5 - Test error get state root hash with block height > U64.max, error code checked, Passed
ok 6 - Test error get state root hash with block height > U64.max, error is thrown, error message checked, Passed
ok 7 - Test get state root hash with wrong block identifier height, but value <= U64.max value - latest state_root_hash is retrieved, Passed
```
