```
muharremsalel@Muharrems-MacBook-Pro CasperLabs-Curve-DAO-Backend % npm test

> curve-backend@0.0.0 test
> mocha tests/index.test.js --timeout 100000



(node:61648) [MONGOOSE] DeprecationWarning: Mongoose: the `strictQuery` option will be switched back to `false` by default in Mongoose 7. Use `mongoose.set('strictQuery', false);` if you want to prepare for this change. Or use `mongoose.set('strictQuery', true);` to suppress this warning.
(Use `node --trace-deprecation ...` to show where the warning was created)
  GraphQL Mutations for guage-controller
Calling handleAddType mutation...
    ✔ handleAddType should return true
Calling handleNewGauge mutation...
    ✔ handleNewGauge should return true
Calling handleNewGaugeWeight mutation...
    ✔ handleNewGaugeWeight should return true
Calling handleNewTypeWeight mutation...
    ✔ handleNewTypeWeight should return true
Calling handleVoteForGauge mutation...
    ✔ handleVoteForGauge should return true
Calling gaugeVotesByTime query...
{ gaugeVotesByTime: [] }
    ✔ gaugeVotesByTime Should fetch gaugeVotes sorted by time
Calling gaugeVotesByUser query...
{ gaugeVotesByUser: [] }
    ✔ gaugeVotesByUser Should fetch gaugeVotes filtered on user

  GraphQL Mutations for Gauge
Calling handleUpdateLiquidityLimit mutation...
    ✔ handleUpdateLiquidityLimit should return true
Calling gauges query...
{ gauges: [] }
    ✔ gauges Should fetch gauges filtered by user
Calling handleDeposit mutation...
    ✔ handleDeposit should return true
Calling handleWithdraw mutation...
    ✔ handleWithdraw should return true

  GraphQL Mutations for Gauge
Calling handleDeposit mutation...
    ✔ handleVotingDeposit should return true
Calling handleWithdraw mutation...
    ✔ handleVotingWithdraw should return true
Calling votingEscrows query...
{ votingEscrows: [] }
    ✔ votingEscrows Should fetch votingEscrows
Calling daoPowersByBlock query...
{ daoPowersByBlock: [] }
    ✔ daoPowersByBlock Should fetch daoPowers sorted Block
Calling daoPowersByTimestamp query...
{ daoPowersByTimestamp: [] }
    ✔ daoPowersByTimestamp Should fetch daoPowers sorted by Timestamp
Calling votingPower query...
{ votingPower: null }
    ✔ votingPower Should fetch votingPowers filtered by id
Calling userBalancesByUnlockTime query...
{ userBalancesByUnlockTime: [] }
    ✔ userBalancesByUnlockTime Should fetch userBalances sorted by Unlock time
Calling userBalancesByWeight query...
{ userBalancesByWeight: [] }
    ✔ userBalancesByWeight Should fetch userBalances sorted by weight

  All api endpoints should work
    adminroutes should work for admin user
      ✔ admin user should be logged in successfully (245ms)
    afterDeploymentroutes should work for admin user
      ✔ addcontractandpackageHash should add contract and package hash (687ms)
    coinsmarketcapapi should return response from coinmarketcap
      ✔ getworthinUSD should return worth in USD (525ms)
      ✔ tokensworthconversion should return converted amount (335ms)
      ✔ priceconversion should return converted price (340ms)
    erc20routes should return response from erc20 contract
      ✔ balanceagainstuser should return balance for user
      ✔ allowanceagainstownerandspender should return allowance for owner and spender
    vestingEscrowRoutes should return response from vesting escrow contract
      ✔ balanceOf should return balance
      ✔ vestedOf should return vested amount
      ✔ lockedOf should return locked amount
    gaugeControllerRoutes should return response from gauge controller contract
      ✔ gaugeRelativeWeight should return gauge relative weight
      ✔ getGaugeWeight should return gauge weight
      ✔ getTotalWeight should return total weight
      ✔ voteUserSlopes should return vote user slopes
      ✔ pointsWeight should return points weight
    votingEscrowRoutes should return response from voting escrow contract
      ✔ balanceagainstuser should return balance
      ✔ totalSupply should return total supply
      ✔ balanceOf should return balance
      ✔ balanceOfAt should return balance
      ✔ getlastUserSlope should return last user slope
      ✔ lockedEnd should return locked end amount
      ✔ CRVStats should return crv stats
    readWasm should return wasm data
      ✔ readWasm should return wasm data


  42 passing (18s)

  ```