# Output of the "yarn test" command for examples of the project

```sh

furkan@furkan-Victus-by-HP-Laptop-16-e1xxx:~/casperdash-mobile-wallet/android$ yarn test
yarn run v1.22.19
$ jest --coverage
● Multiple configurations found:
    * /home/furkan/casperdash-mobile-wallet/jest.config.js
    * `jest` key in /home/furkan/casperdash-mobile-wallet/package.json

  Implicit config resolution does not allow multiple configuration files.
  Either remove unused config files or select one explicitly with `--config`.

  Configuration Documentation:
  https://jestjs.io/docs/configuration.html

 PASS  src/utils/helpers/identicon.test.js
 PASS  src/utils/helpers/key.test.js
 PASS  src/utils/helpers/balance.test.js
 PASS  src/utils/helpers/currency.test.js
 PASS  src/utils/helpers/format.test.js
 PASS  src/utils/services/userServices.test.js
 PASS  src/utils/services/tokenServices.test.js
 PASS  src/utils/services/stakeService.test.js
 PASS  src/utils/services/casperServices.test.js
 PASS  src/utils/services/ledgerServices.test.js
 PASS  src/utils/helpers/validator.test.js
--------------------|---------|----------|---------|---------|-------------------
File                | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s 
--------------------|---------|----------|---------|---------|-------------------
All files           |   91.41 |    84.29 |    92.3 |   91.38 |                   
 config             |     100 |      100 |     100 |     100 |                   
  env.mainnet.js    |     100 |      100 |     100 |     100 |                   
  index.js          |     100 |      100 |     100 |     100 |                   
 constants          |     100 |      100 |     100 |     100 |                   
  key.ts            |     100 |      100 |     100 |     100 |                   
  ledger.ts         |     100 |      100 |     100 |     100 |                   
  nft.ts            |     100 |      100 |     100 |     100 |                   
  stack.ts          |     100 |      100 |     100 |     100 |                   
 helpers            |   89.51 |    88.65 |   95.65 |   89.51 |                   
  balance.ts        |     100 |      100 |     100 |     100 |                   
  currency.ts       |     100 |      100 |     100 |     100 |                   
  format.ts         |   70.58 |    76.47 |    87.5 |   70.58 | 59,118,138-151    
  identicon.ts      |     100 |      100 |     100 |     100 |                   
  key.ts            |     100 |        0 |     100 |     100 | 12                
  validator.ts      |     100 |    96.72 |     100 |     100 | 13,197            
 services           |   91.11 |    66.66 |    87.5 |   91.01 |                   
  casperServices.ts |   82.14 |      100 |   71.42 |   82.14 | 123-131,140       
  ledgerServices.ts |   94.28 |    68.42 |     100 |   94.11 | 51-52             
  stakeServices.ts  |     100 |      100 |     100 |     100 |                   
  tokenServices.ts  |    87.5 |        0 |     100 |    87.5 | 29                
  userServices.ts   |     100 |      100 |     100 |     100 |                   
--------------------|---------|----------|---------|---------|-------------------

Test Suites: 11 passed, 11 total
Tests:       74 passed, 74 total
Snapshots:   0 total
Time:        2.238 s
Ran all test suites.
Done in 3.38s.
furkan@furkan-Victus-by-HP-Laptop-16-e1xxx:~/casperdash-mobile-wallet/android$ 

```

