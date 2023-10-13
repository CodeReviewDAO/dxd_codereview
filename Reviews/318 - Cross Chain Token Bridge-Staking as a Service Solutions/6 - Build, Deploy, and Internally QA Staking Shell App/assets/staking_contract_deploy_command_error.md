```bash
$ casper-client put-deploy \
    --chain-name casper-test \
    --node-address http://44.208.234.65:7777 \
    --secret-key ./contract/keys/secret_key.pem \
    --session-path ./contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm \
    --payment-amount 220000000000
Cryptographic error: secret_key: secret key load failed: could not read './contract/keys/secret_key.pem': No such file or directory (os error 2)

$ casper-client put-deploy \
    --chain-name casper-test \
    --node-address http://44.208.234.65:7777 \
    --secret-key ./staking_contract/keys/secret_key.pem \
    --session-path ./contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm \
    --payment-amount 220000000000
IO error: unable to read session file at './contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm': No such file or directory (os error 2)

$ casper-client put-deploy \
    --chain-name casper-test \
    --node-address http://44.208.234.65:7777 \
    --secret-key ./staking_contract/keys/secret_key.pem \
    --session-path ./staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm \
    --payment-amount 220000000000
Deploy size too large: deploy size of 2000576 bytes exceeds limit of 1048576
```