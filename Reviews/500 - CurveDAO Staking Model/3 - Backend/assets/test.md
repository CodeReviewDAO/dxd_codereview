```
msalel:~/environment/CasperLabs-Curve-DAO-Backend (main) $ npm test

> curve-backend@0.0.0 test
> mocha tests/index.test.js --timeout 100000



(node:30380) [MONGOOSE] DeprecationWarning: Mongoose: the `strictQuery` option will be switched back to `false` by default in Mongoose 7. Use `mongoose.set('strictQuery', false);` if you want to prepare for this change. Or use `mongoose.set('strictQuery', true);` to suppress this warning.
(Use `node --trace-deprecation ...` to show where the warning was created)
  GraphQL Mutations for guage-controller
Calling handleAddType mutation...
{ handleAddType: { result: true } }
    ✔ handleAddType should return true (3606ms)
Calling handleNewGauge mutation...
{ handleNewGauge: { result: true } }
    ✔ handleNewGauge should return true (3547ms)
Calling handleNewGaugeWeight mutation...
{ handleNewGaugeWeight: { result: true } }
    ✔ handleNewGaugeWeight should return true (1639ms)
Calling handleNewTypeWeight mutation...
{ handleNewTypeWeight: { result: true } }
    ✔ handleNewTypeWeight should return true (43ms)
Calling handleVoteForGauge mutation...
{ handleVoteForGauge: { result: true } }
    ✔ handleVoteForGauge should return true (7026ms)
Calling gaugeVotesByTime query...
{ gaugeVotesByTime: [ { time: '604800' } ] }
    ✔ gaugeVotesByTime Should fetch gaugeVotes sorted by time
Calling gaugeVotesByUser query...
{ gaugeVotesByUser: [ { user: 'user' } ] }
    ✔ gaugeVotesByUser Should fetch gaugeVotes filtered on user

  GraphQL Mutations for Gauge
Calling handleUpdateLiquidityLimit mutation...
{ handleUpdateLiquidityLimit: { result: true } }
    ✔ handleUpdateLiquidityLimit should return true
Calling gauges query...
{ gauges: [ { user: 'user' } ] }
    ✔ gauges Should fetch gauges filtered by user
Calling handleDeposit mutation...
{ handleDeposit: { result: true } }
    ✔ handleDeposit should return true
Calling handleWithdraw mutation...
{ handleWithdraw: { result: true } }
    ✔ handleWithdraw should return true (46ms)

  GraphQL Mutations for Gauge
Calling handleDeposit mutation...
{ handleVotingDeposit: { result: true } }
    ✔ handleVotingDeposit should return true (3522ms)
Calling handleWithdraw mutation...
{ handleVotingWithdraw: { result: true } }
    ✔ handleVotingWithdraw should return true (3533ms)
Calling votingEscrows query...
{ votingEscrows: [ { id: 'provider' }, { id: 'provider' } ] }
    ✔ votingEscrows Should fetch votingEscrows
Calling daoPowersByBlock query...
{ daoPowersByBlock: [ { id: '123123-604800' } ] }
    ✔ daoPowersByBlock Should fetch daoPowers sorted Block
Calling daoPowersByTimestamp query...
{ daoPowersByTimestamp: [ { id: '123123-604800' } ] }
    ✔ daoPowersByTimestamp Should fetch daoPowers sorted by Timestamp
Calling votingPower query...
{ votingPower: { id: 'provider' } }
    ✔ votingPower Should fetch votingPowers filtered by id
Calling userBalancesByUnlockTime query...
{ userBalancesByUnlockTime: [ { id: 'provider' } ] }
    ✔ userBalancesByUnlockTime Should fetch userBalances sorted by Unlock time
Calling userBalancesByWeight query...
{ userBalancesByWeight: [ { id: 'provider' } ] }
    ✔ userBalancesByWeight Should fetch userBalances sorted by weight

  All api endpoints should work
    adminroutes should work for admin user
      ✔ admin user should be logged in successfully (333ms)
    afterDeploymentroutes should work for admin user
      ✔ addcontractandpackageHash should add contract and package hash
    coinsmarketcapapi should return response from coinmarketcap
      ✔ getworthinUSD should return worth in USD (182ms)
      ✔ tokensworthconversion should return converted amount (129ms)
      ✔ priceconversion should return converted price (137ms)
    erc20routes should return response from erc20 contract
      ✔ balanceagainstuser should return balance for user (1102ms)
      ✔ allowanceagainstownerandspender should return allowance for owner and spender (1008ms)
    vestingEscrowRoutes should return response from vesting escrow contract
      ✔ balanceOf should return balance (2754ms)
      ✔ vestedOf should return vested amount (2287ms)
      ✔ lockedOf should return locked amount (2742ms)
    gaugeControllerRoutes should return response from gauge controller contract
      ✔ gaugeRelativeWeight should return gauge relative weight (1018ms)
      ✔ getGaugeWeight should return gauge weight (1928ms)
      ✔ getTotalWeight should return total weight (1749ms)
      ✔ voteUserSlopes should return vote user slopes (1930ms)
      ✔ pointsWeight should return points weight (1470ms)
    votingEscrowRoutes should return response from voting escrow contract
      ✔ balanceagainstuser should return balance (3367ms)
      ✔ totalSupply should return total supply (4762ms)
      ✔ balanceOf should return balance (1018ms)
      ✔ balanceOfAt should return balance (16409ms)
      ✔ getlastUserSlope should return last user slope (2835ms)
      ✔ lockedEnd should return locked end amount (1652ms)
      ✔ CRVStats should return crv stats (8054ms)
    readWasm should return wasm data
      ✔ readWasm should return wasm data


  42 passing (1m)


  ```