# Casper Dash build and test information logging
## Testing
### Command: 

```
yarn test
```

### Result:
 
 ```
$ jest --coverage
 PASS  src/utils/helpers/currency.test.js
 PASS  src/utils/helpers/format.test.js
 PASS  src/utils/services/userServices.test.js
 PASS  src/utils/helpers/identicon.test.js
 PASS  src/utils/services/stakeService.test.js
 PASS  src/utils/helpers/validator.test.js
 PASS  src/utils/services/ledgerServices.test.js
 PASS  src/utils/helpers/key.test.js
 PASS  src/utils/services/tokenServices.test.js
 PASS  src/utils/services/casperServices.test.js
 PASS  src/utils/helpers/balance.test.js
-------------------|---------|----------|---------|---------|-------------------
File               | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s 
-------------------|---------|----------|---------|---------|-------------------
All files          |   91.38 |    83.73 |    92.5 |   91.35 |                   
 config            |     100 |       50 |     100 |     100 |                   
  env.testnet.js   |     100 |      100 |     100 |     100 |                   
  index.js         |     100 |       50 |     100 |     100 | 1                 
 constants         |     100 |      100 |     100 |     100 |                   
  key.js           |     100 |      100 |     100 |     100 |                   
  ledger.js        |     100 |      100 |     100 |     100 |                   
  nft.js           |     100 |      100 |     100 |     100 |                   
  stack.js         |     100 |      100 |     100 |     100 |                   
 helpers           |   89.51 |    88.65 |   95.65 |   89.51 |                   
  balance.js       |     100 |      100 |     100 |     100 |                   
  currency.js      |     100 |      100 |     100 |     100 |                   
  format.js        |   70.58 |    76.47 |    87.5 |   70.58 | 59,112,128-141    
  identicon.js     |     100 |      100 |     100 |     100 |                   
  key.js           |     100 |        0 |     100 |     100 | 12                
  validator.js     |     100 |    96.72 |     100 |     100 | 13,169            
 services          |   91.57 |    66.66 |   88.23 |   91.48 |                   
  ...erServices.js |   84.37 |      100 |      75 |   84.37 | 139-146,154       
  ...erServices.js |   94.44 |    68.42 |     100 |   94.28 | 51-52             
  stakeServices.js |     100 |      100 |     100 |     100 |                   
  tokenServices.js |    87.5 |        0 |     100 |    87.5 | 29                
  userServices.js  |     100 |      100 |     100 |     100 |                   
-------------------|---------|----------|---------|---------|-------------------
 
Test Suites: 11 passed, 11 total
Tests:       75 passed, 75 total
Snapshots:   0 total
Time:        1.889 s
Ran all test suites.
✨  Done in 3.21s.
 ```
