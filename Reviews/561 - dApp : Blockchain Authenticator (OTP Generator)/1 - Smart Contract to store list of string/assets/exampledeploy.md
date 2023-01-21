# Output of the "put-deploy" command

```sh

gitpod /workspace/blockchain-authenticator-contract (master) $ casper-client put-deploy --chain-name casper-test -n http://95.216.67.162:7777 -k /workspace/blockchain-authenticator-contract/reviewstemp_secret_key.pem -p 10000000000 -s /workspace/blockchain-authenticator-contract/contract/target/wasm32-unknown-unknown/release/contract.wasm --session-args-complex /workspace/blockchain-authenticator-contract/args.txt
{
  "id": 1962383722417384944,
  "jsonrpc": "2.0",
  "result": {
    "api_version": "1.4.10",
    "deploy_hash": "c15a386c98adadad561f2a557e33346e746d3ab9a8348d914a611ef71117a2a7"
  }
}

```
