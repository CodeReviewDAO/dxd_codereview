## Tests

```sh
review@crdao:~/devxdao/casper-storage $ yarn test
yarn run v1.22.19
$ jest --env=./test/test-env.js
PASS test/utils/type-utils.test.ts (6.463 s)
PASS test/utils/validator-utils.test.ts (6.915 s)
PASS test/cryptography/key/secp256k1.test.ts
PASS test/storage/providers/default-storage.test.ts
PASS test/cryptography/utils/encoder-utils.test.ts
PASS test/cryptography/key/parser/auto-key-parser.test.ts
PASS test/storage/storage-manager.test.ts
PASS test/wallet/hdwallet/hdwallet.ed25519.test.ts (8.604 s)
PASS test/wallet/hdwallet/hdwallet.secp256k1.test.ts (8.887 s)
PASS test/wallet/common/casper/casper-legacy-wallet.secp256k1.test.ts
PASS test/key/mnemonic/mnemonic-key.test.ts (9.376 s)
PASS test/wallet/core/coin-path.test.ts
PASS test/wallet/common/casper/casper-legacy-wallet.ed25519.test.ts
PASS test/wallet/common/casper/casper-hd-wallet.sec256k1.test.ts
PASS test/wallet/common/casper/casper-hd-wallet.ed25519.test.ts
PASS test/cryptography/key/parser/secp256k1-key-parser.test.ts
PASS test/bips/bip32/hd-key-manager-secp256k1.test.ts
PASS test/cryptography/key/ed25519.test.ts
PASS test/cryptography/key/parser/ed25519-key-parser.test.ts
PASS test/bips/bip32/hd-key-manager-ed25519.test.ts
PASS test/cryptography/key/parser/core.test.ts
PASS test/wallet/legacywallet/legacy-wallet.ed25519.test.ts
PASS test/wallet/legacywallet/legacy-wallet.secp256k1.test.ts
PASS test/bips/bip32/hd-key-manager-factory.test.ts
PASS test/utils/validation-result.test.ts
PASS test/cryptography/key/parser/key-parser.test.ts
PASS test/wallet/common/casper/casper-wallet-utils.test.ts
PASS test/key/key-factory.test.ts
PASS test/cryptography/utils/crypto-utils.test.ts
PASS test/user/user.test.ts (13.869 s)
PASS test/cryptography/utils/aes-util.test.ts (14.151 s)

Test Suites: 31 passed, 31 total
Tests:       227 passed, 227 total
Snapshots:   0 total
Time:        15.789 s
Ran all test suites.
Done in 16.68s.
```


## Tests with coverage

```sh
review@crdao:~/devxdao/casper-storage $ yarn testci
yarn run v1.22.19
$ jest --env=./test/test-env.js --coverage
PASS test/utils/type-utils.test.ts (5.388 s)
PASS test/utils/validator-utils.test.ts (5.452 s)
PASS test/key/mnemonic/mnemonic-key.test.ts (6.622 s)
PASS test/wallet/common/casper/casper-legacy-wallet.secp256k1.test.ts
PASS test/wallet/common/casper/casper-hd-wallet.sec256k1.test.ts
PASS test/wallet/hdwallet/hdwallet.ed25519.test.ts (7.434 s)
PASS test/wallet/hdwallet/hdwallet.secp256k1.test.ts (7.663 s)
PASS test/wallet/common/casper/casper-hd-wallet.ed25519.test.ts
PASS test/cryptography/key/ed25519.test.ts
PASS test/bips/bip32/hd-key-manager-ed25519.test.ts
PASS test/cryptography/utils/crypto-utils.test.ts
PASS test/cryptography/key/secp256k1.test.ts
PASS test/wallet/common/casper/casper-wallet-utils.test.ts
PASS test/wallet/common/casper/casper-legacy-wallet.ed25519.test.ts
PASS test/cryptography/key/parser/secp256k1-key-parser.test.ts
PASS test/cryptography/key/parser/auto-key-parser.test.ts
PASS test/key/key-factory.test.ts
PASS test/cryptography/utils/encoder-utils.test.ts
PASS test/cryptography/key/parser/core.test.ts
PASS test/bips/bip32/hd-key-manager-secp256k1.test.ts
PASS test/wallet/legacywallet/legacy-wallet.secp256k1.test.ts
PASS test/wallet/legacywallet/legacy-wallet.ed25519.test.ts
PASS test/wallet/core/coin-path.test.ts
PASS test/cryptography/key/parser/ed25519-key-parser.test.ts
PASS test/storage/providers/default-storage.test.ts
PASS test/utils/validation-result.test.ts
PASS test/bips/bip32/hd-key-manager-factory.test.ts
PASS test/storage/storage-manager.test.ts
PASS test/cryptography/key/parser/key-parser.test.ts
PASS test/cryptography/utils/aes-util.test.ts (10.604 s)
PASS test/user/user.test.ts (11.248 s)
------------------------------|---------|----------|---------|---------|--------------------------------
File                          | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s              
------------------------------|---------|----------|---------|---------|--------------------------------
All files                     |   90.78 |    73.29 |   93.46 |   91.44 |                                
 bips/bip32                   |     100 |      100 |     100 |     100 |                                
  core.ts                     |     100 |      100 |     100 |     100 |                                
  hd-key-manager-base.ts      |     100 |      100 |     100 |     100 |                                
  hd-key-manager-ed25519.ts   |     100 |      100 |     100 |     100 |                                
  hd-key-manager-factory.ts   |     100 |      100 |     100 |     100 |                                
  hd-key-manager-secp256k1.ts |     100 |      100 |     100 |     100 |                                
 bips/bip32/hdkey             |    92.3 |    64.28 |     100 |   92.12 |                                
  hd-key-ed25519.ts           |   94.11 |       50 |     100 |   94.11 | 26                             
  hd-key-secp256k1.ts         |   83.78 |       50 |     100 |   83.78 | 19,26,40,56,61-64              
  hd-key.ts                   |   96.05 |       75 |     100 |   95.89 | 91,150,157                     
 cryptography/core            |     100 |      100 |     100 |     100 |                                
  encryption-type.ts          |     100 |      100 |     100 |     100 |                                
 cryptography/key             |     100 |      100 |     100 |     100 |                                
  ed25519.ts                  |     100 |      100 |     100 |     100 |                                
  secp256k1.ts                |     100 |      100 |     100 |     100 |                                
 cryptography/key/parser      |   91.42 |    73.91 |     100 |   91.42 |                                
  auto-key-parser.ts          |     100 |      100 |     100 |     100 |                                
  base-key-parser.ts          |   88.88 |        0 |     100 |   88.88 | 17                             
  core.ts                     |     100 |      100 |     100 |     100 |                                
  ed25519-key-parser.ts       |   77.77 |    63.63 |     100 |   77.77 | 15,25,28,35                    
  key-parser.ts               |   92.85 |       75 |     100 |   92.85 | 33                             
  secp256k1-key-parser.ts     |     100 |      100 |     100 |     100 |                                
 cryptography/utils           |   89.47 |    73.33 |   85.71 |   89.47 |                                
  aes-utils.ts                |     100 |      100 |     100 |     100 |                                
  crypto-utils.ts             |   77.14 |    33.33 |      75 |   77.14 | 24,27,49-56,66,97              
  encoder-utils.ts            |     100 |      100 |     100 |     100 |                                
 key                          |     100 |      100 |     100 |     100 |                                
  key-factory.ts              |     100 |      100 |     100 |     100 |                                
 key/mnemonic                 |     100 |      100 |     100 |     100 |                                
  mnemonic-key.ts             |     100 |      100 |     100 |     100 |                                
 storage                      |      80 |    66.66 |     100 |      80 |                                
  storage-manager.ts          |      80 |    66.66 |     100 |      80 | 19-20,29                       
 storage/providers            |      65 |        0 |   58.33 |      65 |                                
  async-storage.ts            |      40 |        0 |   16.66 |      40 | 22-39                          
  local-storage.ts            |      90 |      100 |     100 |      90 | 33                             
 user                         |   85.97 |    65.21 |      90 |   89.26 |                                
  password.ts                 |   91.66 |    66.66 |     100 |      90 | 27-28                          
  user.ts                     |   89.47 |    79.16 |   91.66 |   91.54 | 97-98,138,193-194,218          
  wallet-info.ts              |   79.68 |    43.75 |   85.71 |    86.2 | 37,129,133,216-217,225,236-237 
 utils                        |   97.61 |    94.44 |     100 |   97.22 |                                
  type-utils.ts               |   96.66 |    91.66 |     100 |   95.83 | 112                            
  validator-utils.ts          |     100 |      100 |     100 |     100 |                                
 wallet/common/casper         |   96.42 |       60 |     100 |   96.15 |                                
  casper-hd-wallet.ts         |     100 |       50 |     100 |     100 | 33                             
  casper-legacy-wallet.ts     |     100 |      100 |     100 |     100 |                                
  casper-wallet-utils.ts      |    90.9 |    66.66 |     100 |   88.88 | 19                             
 wallet/core                  |   95.55 |      100 |   92.85 |   95.55 |                                
  base-wallet.ts              |   88.23 |      100 |    87.5 |   88.23 | 64-65                          
  coin-path.ts                |     100 |      100 |     100 |     100 |                                
  coin-type.ts                |     100 |      100 |     100 |     100 |                                
  network.ts                  |     100 |      100 |     100 |     100 |                                
  purpose.ts                  |     100 |      100 |     100 |     100 |                                
  signature.ts                |     100 |      100 |     100 |     100 |                                
 wallet/hdwallet              |   81.25 |       50 |     100 |   81.25 |                                
  hd-wallet.ts                |   77.77 |       50 |     100 |   77.77 | 21,24,27,30,57-58              
  wallet.ts                   |     100 |      100 |     100 |     100 |                                
 wallet/legacywallet          |     100 |      100 |     100 |     100 |                                
  legacy-wallet.ts            |     100 |      100 |     100 |     100 |                                
------------------------------|---------|----------|---------|---------|--------------------------------

Test Suites: 31 passed, 31 total
Tests:       227 passed, 227 total
Snapshots:   0 total
Time:        13.096 s, estimated 15 s
Ran all test suites.
Done in 13.98s.
```
