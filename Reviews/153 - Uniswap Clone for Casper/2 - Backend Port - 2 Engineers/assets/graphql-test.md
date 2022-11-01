Example Query 1:
```
query tokensbyId {
  tokensbyId(first: 50, id: ["03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa", "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f", "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813"]) {
    id
    name
    symbol
    derivedETH
    tradeVolume
    tradeVolumeUSD
    untrackedVolumeUSD
    totalLiquidity
    txCount
    __typename
  }
}
```
Example Response 1:
```
{
  "data": {
    "tokensbyId": [
      {
        "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
        "name": "Wrapper Ether",
        "symbol": "WETH",
        "derivedETH": "389.270432643339984464",
        "tradeVolume": "546525380195",
        "tradeVolumeUSD": "475862832851.365344718031647041",
        "untrackedVolumeUSD": "852929190428.482398574988295947480320537437771226",
        "totalLiquidity": "561155557864737771",
        "txCount": "202",
        "__typename": "Token"
      },
      {
        "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
        "name": "Coinstox",
        "symbol": "CSX",
        "derivedETH": "0.011053420523050266",
        "tradeVolume": "24946546161843",
        "tradeVolumeUSD": "405296715460.630678882632292469",
        "untrackedVolumeUSD": "708870384458.196498913369414695457451846390426104",
        "totalLiquidity": "6011041750372255331",
        "txCount": "133",
        "__typename": "Token"
      },
      {
        "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
        "name": "Wrapped Casper",
        "symbol": "WCSPR",
        "derivedETH": "1",
        "tradeVolume": "4782316146637",
        "tradeVolumeUSD": "78132822137.238065087981376608",
        "untrackedVolumeUSD": "158233816658.779927158858963034996260842151536770",
        "totalLiquidity": "64245475395698",
        "txCount": "199",
        "__typename": "Token"
      }
    ]
  }
}
```

---

Example Query 2:
```
fragment PairFields on Pair {
  id
  txCount
  token0 {
    id
    symbol
    name
    totalLiquidity
    derivedETH
    __typename
  }
  token1 {
    id
    symbol
    name
    totalLiquidity
    derivedETH
    __typename
  }
  reserve0
  reserve1
  reserveUSD
  totalSupply
  trackedReserveETH
  reserveETH
  volumeUSD
  untrackedVolumeUSD
  token0Price
  token1Price
  createdAtTimestamp
  __typename
}

query pairbyId {
  pairbyId(id: "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060") {
    ...PairFields
    __typename
  }
}
```
Example Response 2:
```
{
  "data": {
    "pairbyId": [
      {
        "id": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
        "txCount": "134",
        "token0": {
          "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
          "symbol": "WETH",
          "name": "Wrapper Ether",
          "totalLiquidity": "10017924743324",
          "derivedETH": "0",
          "__typename": "Token"
        },
        "token1": {
          "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
          "symbol": "WCSPR",
          "name": "Wrapped Casper",
          "totalLiquidity": "1000000000",
          "derivedETH": "0",
          "__typename": "Token"
        },
        "reserve0": "138841254374",
        "reserve1": "54046795158911",
        "reserveUSD": "4336499652773.4840321199485986126070699222501222",
        "totalSupply": "2668742671223",
        "trackedReserveETH": "109721227999068.076148514212863248",
        "reserveETH": "108053657674730.332455031121145962",
        "volumeUSD": "74349469763.986365461690365590",
        "untrackedVolumeUSD": "151146311314.532913410238922143509564766599440946",
        "token0Price": "0.002568908183469015",
        "token1Price": "389.270432643339984464",
        "createdAtTimestamp": 1650287562,
        "__typename": "Pair"
      }
    ]
  }
}
```

---

Example Query 3:
```
query pairsbyId {
  pairsbyId(first: 200, id: ["c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485", "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060", "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d"]) {
    id
    reserveUSD
    trackedReserveETH
    volumeUSD
    untrackedVolumeUSD
    __typename
  }
}
```
Example Response 3:
```
{
  "data": {
    "pairsbyId": [
      {
        "id": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
        "reserveUSD": "8702477364817801611.73227217194845623708014447831272528",
        "trackedReserveETH": "220314762347728517832.224857015112634421",
        "volumeUSD": "401513363087.378979256341281451",
        "untrackedVolumeUSD": "701782879113.949485164749373803970755770838330280",
        "__typename": "Pair"
      },
      {
        "id": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
        "reserveUSD": "4336499652773.4840321199485986126070699222501222",
        "trackedReserveETH": "109721227999068.076148514212863248",
        "volumeUSD": "74349469763.986365461690365590",
        "untrackedVolumeUSD": "151146311314.532913410238922143509564766599440946",
        "__typename": "Pair"
      },
      {
        "id": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
        "reserveUSD": "824781326117.626595114747397581922451972227582624",
        "trackedReserveETH": "20547637230117.516756876058248555",
        "volumeUSD": "3783352373.251699626291011018",
        "untrackedVolumeUSD": "7087505344.247013748620040891486696075552095824",
        "__typename": "Pair"
      }
    ]
  }
}
```

---

Example Query 4:
```
query tokensbyId {
  tokensbyId(first: 50, id: ["03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa", "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f", "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813"]) {
    id
    name
    symbol
    derivedETH
    tradeVolume
    tradeVolumeUSD
    untrackedVolumeUSD
    totalLiquidity
    txCount
    __typename
  }
}
```
Example Response 4:
```
{
  "data": {
    "tokensbyId": [
      {
        "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
        "name": "Wrapper Ether",
        "symbol": "WETH",
        "derivedETH": "389.270432643339984464",
        "tradeVolume": "546525380195",
        "tradeVolumeUSD": "475862832851.365344718031647041",
        "untrackedVolumeUSD": "852929190428.482398574988295947480320537437771226",
        "totalLiquidity": "561155557864737771",
        "txCount": "202",
        "__typename": "Token"
      },
      {
        "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
        "name": "Coinstox",
        "symbol": "CSX",
        "derivedETH": "0.011053420523050266",
        "tradeVolume": "24946546161843",
        "tradeVolumeUSD": "405296715460.630678882632292469",
        "untrackedVolumeUSD": "708870384458.196498913369414695457451846390426104",
        "totalLiquidity": "6011041750372255331",
        "txCount": "133",
        "__typename": "Token"
      },
      {
        "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
        "name": "Wrapped Casper",
        "symbol": "WCSPR",
        "derivedETH": "1",
        "tradeVolume": "4782316146637",
        "tradeVolumeUSD": "78132822137.238065087981376608",
        "untrackedVolumeUSD": "158233816658.779927158858963034996260842151536770",
        "totalLiquidity": "64245475395698",
        "txCount": "199",
        "__typename": "Token"
      }
    ]
  }
}
```

---

Example Query 5:
```
fragment TokenFields on Token {
  id
  name
  symbol
  derivedETH
  tradeVolume
  tradeVolumeUSD
  untrackedVolumeUSD
  totalLiquidity
  txCount
  __typename
}

{
  tokenbyId(id: "") {
    ...TokenFields
    __typename
  }
  pairs0: pairsbytoken0(first: 50, token0: "") {
    id
    __typename
  }
  pairs1: pairsbytoken1(first: 50, token1: "") {
    id
    __typename
  }
}
```
Example Response 5:
```
{
  "data": {
    "tokenbyId": null,
    "pairs0": [],
    "pairs1": []
  }
}
```

---

Example Query 6:
```
query tokendaydatasbydate($date: String) {
  tokendaydatasbydate(first: 50, date: $date) {
    id
    date
    __typename
  }
}
```
Example Response 6:
```
{
  "data": {
    "tokendaydatasbydate": []
  }
}
```

---

Example Query 7:
```
query uniswapfactory {
  uniswapfactory(id: "f329330b99110d9f8589b8a94f0e5b3c4cd5e1710fb443d04472682ae9b212d0") {
    id
    totalVolumeUSD
    totalVolumeETH
    untrackedVolumeUSD
    totalLiquidityUSD
    totalLiquidityETH
    txCount
    pairCount
    __typename
  }
}
```
Example Response 7:
```
{
  "data": {
    "uniswapfactory": {
      "id": "f329330b99110d9f8589b8a94f0e5b3c4cd5e1710fb443d04472682ae9b212d0",
      "totalVolumeUSD": "479646185224.617044344322658059",
      "totalVolumeETH": "11908709257872.205000830174420507",
      "untrackedVolumeUSD": "860016695772.729412323608336838967016612989867050",
      "totalLiquidityUSD": "8774454372463156672.00615748561103122993069222088820864",
      "totalLiquidityETH": "220314892616593747017.817762405383746224",
      "txCount": "265",
      "pairCount": "3",
      "__typename": "UniswapFactory"
    }
  }
}
```

---

Example Query 8:
```
query pairs {
  pairs(first: 200, skip: 0) {
    id
    __typename
  }
}
```
Example Response 8:
```
{
  "data": {
    "pairs": [
      {
        "id": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
        "__typename": "Pair"
      },
      {
        "id": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
        "__typename": "Pair"
      },
      {
        "id": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
        "__typename": "Pair"
      }
    ]
  }
}
```

---

Example Query 9:
```
query bundle {
  bundle(id: "1") {
    id
    ethPrice
    __typename
  }
}
```
Example Response 9:
```
{
  "data": {
    "bundle": {
      "id": "1",
      "ethPrice": "0.03982687810275736",
      "__typename": "Bundle"
    }
  }
}
```

---

Example Query 10:
```
query transactions {
  transactions(first: 1000) {
    mints {
      transactionid
      transactiontimestamp
      pair {
        token0 {
          id
          symbol
          __typename
        }
        token1 {
          id
          symbol
          __typename
        }
        __typename
      }
      to
      liquidity
      amount0
      amount1
      amountUSD
      __typename
    }
    burns {
      transactionid
      transactiontimestamp
      pair {
        token0 {
          id
          symbol
          __typename
        }
        token1 {
          id
          symbol
          __typename
        }
        __typename
      }
      sender
      liquidity
      amount0
      amount1
      amountUSD
      __typename
    }
    swaps {
      transactionid
      transactiontimestamp
      pair {
        token0 {
          id
          symbol
          __typename
        }
        token1 {
          id
          symbol
          __typename
        }
        __typename
      }
      amount0In
      amount0Out
      amount1In
      amount1Out
      amountUSD
      to
      __typename
    }
    __typename
  }
}
```
Example Response 10:
```
{
  "data": {
    "transactions": [
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8fa16b1e60d5a939afce61a770efbda953fe532bd252290ba756eb6ff6b98c97",
            "transactiontimestamp": 1667321096,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "440000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "8fa16b1e60d5a939afce61a770efbda953fe532bd252290ba756eb6ff6b98c97",
            "transactiontimestamp": 1667321096,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "40958861032",
            "amount1In": "440000000000",
            "amount1Out": "0",
            "amountUSD": "317598186069.329324480993647494",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "35f8242eec776086be35663d8b0df953038ff71acad4839fa3466370c04a0dce",
            "transactiontimestamp": 1667315363,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "110000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "35f8242eec776086be35663d8b0df953038ff71acad4839fa3466370c04a0dce",
            "transactiontimestamp": 1667315363,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10239716192",
            "amount1In": "110000000000",
            "amount1Out": "0",
            "amountUSD": "80056209340.358417479284234689",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1c53cdf0e5c4fc5796223232466d6c3f07ade3cd1995c317594204b0bb6739a5",
            "transactiontimestamp": 1667314763,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "1c53cdf0e5c4fc5796223232466d6c3f07ade3cd1995c317594204b0bb6739a5",
            "transactiontimestamp": 1667314763,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "20000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1807477949012",
            "amountUSD": "800748770.181982658039098963",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "108bf7f03ecc7477dc3c1781d97cc41edbaf9ee31922da36047f26c1dc70b787",
            "transactiontimestamp": 1667314622,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "108bf7f03ecc7477dc3c1781d97cc41edbaf9ee31922da36047f26c1dc70b787",
            "transactiontimestamp": 1667314622,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "51242991",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "801305095.208457720526331841",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "f2765670286d535cf2636011c4f554788cba8087650ca8ea471869c568a64e8f",
            "transactiontimestamp": 1667074848,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "7582421863",
            "amount0": "386916119",
            "amount1": "150503722991",
            "amountUSD": "12266714818.62343417127600685283398420000485184",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "f2765670286d535cf2636011c4f554788cba8087650ca8ea471869c568a64e8f",
            "transactiontimestamp": 1667074848,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "386916119",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "f2765670286d535cf2636011c4f554788cba8087650ca8ea471869c568a64e8f",
            "transactiontimestamp": 1667074848,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "150503722991",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "86345edf195693240af1705813da2827589bdc5419277962aaa7ab4d50f9f63e",
            "transactiontimestamp": 1667073963,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "488600884",
            "amount0": "24932344",
            "amount1": "9698253838",
            "amountUSD": "791817633.15969077894979345324145093579781448",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "32fb88a2d2fdedfd94d57a80401fbfcc8ad28d286316909073d152f797892280",
            "transactiontimestamp": 1667073836,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "488600884",
            "amount0": "24932345",
            "amount1": "9698253841",
            "amountUSD": "791940934.1610281873765049197147924951000745",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "32fb88a2d2fdedfd94d57a80401fbfcc8ad28d286316909073d152f797892280",
            "transactiontimestamp": 1667073836,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "24932345",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "32fb88a2d2fdedfd94d57a80401fbfcc8ad28d286316909073d152f797892280",
            "transactiontimestamp": 1667073836,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9698253841",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "cd278ff86c20ad2725ce48523442187f41680002fddfcda145c90ac5f1278aae",
            "transactiontimestamp": 1667073758,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "cd278ff86c20ad2725ce48523442187f41680002fddfcda145c90ac5f1278aae",
            "transactiontimestamp": 1667073758,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25635710",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "407735172.097450707474648162",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c72fd8a3b2f56f95247327a68928ec2dfc5ad621b23c34ebc9e2207a8f5b570a",
            "transactiontimestamp": 1667073493,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "7794937601",
            "amount0": "397834000",
            "amount1": "154693236019",
            "amountUSD": "12625085507.383073598655040176206383206909056000",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "0114150e3c0f3b66e97df9b539a78cf00f50e17f0a46cb99198038d2a992631d",
            "transactiontimestamp": 1667073169,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "7794937601",
            "amount0": "397834001",
            "amount1": "154693236215",
            "amountUSD": "12596134318.21787433406165834995563960827230144",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "0114150e3c0f3b66e97df9b539a78cf00f50e17f0a46cb99198038d2a992631d",
            "transactiontimestamp": 1667073169,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "397834001",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "0114150e3c0f3b66e97df9b539a78cf00f50e17f0a46cb99198038d2a992631d",
            "transactiontimestamp": 1667073169,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "154693236215",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "03c99888e4f12e739b62c05c2ea7936bef455249a5f804d1124a67572cdf828e",
            "transactiontimestamp": 1667072908,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "4879016201",
            "amount0": "249012709",
            "amount1": "96825766074",
            "amountUSD": "7872628539.86402737356779184769689044500690544",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2d2949cc084a0fa6a2634c207fdb350fe392460761c8f26a58a8a71d5f56c275",
            "transactiontimestamp": 1667072781,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "1956612746",
            "amount0": "99860591",
            "amount1": "38829657504",
            "amountUSD": "3157492188.1246306283251937464281750273761455",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "d32ab825278b1d49d62f26e3d6a3423013cb5fbc47f09e9db8bb6652fdbab1e5",
            "transactiontimestamp": 1667072633,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "4879016201",
            "amount0": "249012710",
            "amount1": "96825766084",
            "amountUSD": "7879180617.510121304272097681014104894040931610",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "d32ab825278b1d49d62f26e3d6a3423013cb5fbc47f09e9db8bb6652fdbab1e5",
            "transactiontimestamp": 1667072633,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "249012710",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "d32ab825278b1d49d62f26e3d6a3423013cb5fbc47f09e9db8bb6652fdbab1e5",
            "transactiontimestamp": 1667072633,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "96825766084",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "cc9fab16c291a527d99290d6b9f7feb376d8b5b445bd2b63856c502d91246e26",
            "transactiontimestamp": 1667072338,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "cc9fab16c291a527d99290d6b9f7feb376d8b5b445bd2b63856c502d91246e26",
            "transactiontimestamp": 1667072338,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25645212",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "406251844.262833799452426583",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "03681ad111e866bd238bd78fa90c1c5323be6f1c2be717847888371279b71d43",
            "transactiontimestamp": 1667072195,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "03681ad111e866bd238bd78fa90c1c5323be6f1c2be717847888371279b71d43",
            "transactiontimestamp": 1667072195,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25654716",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "406376114.279973307252659463",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "67947b0151c4ed561f9797d8ab750d588ee65a6465ad5b992c94d96904148a85",
            "transactiontimestamp": 1667072066,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "67947b0151c4ed561f9797d8ab750d588ee65a6465ad5b992c94d96904148a85",
            "transactiontimestamp": 1667072066,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25664226",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "406518791.096240150609470603",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "28f0339d5f2805ff3cd49b10eedbd4e735afd213cd203988d1c55857ea7fb1b5",
            "transactiontimestamp": 1667071059,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "28f0339d5f2805ff3cd49b10eedbd4e735afd213cd203988d1c55857ea7fb1b5",
            "transactiontimestamp": 1667071059,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25673741",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "406318951.696423109602666609",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b33a51ae52f45c891e9b2f5bd34e81d82e9bfd362d734fbd247af6f65062e6f1",
            "transactiontimestamp": 1666821160,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "b33a51ae52f45c891e9b2f5bd34e81d82e9bfd362d734fbd247af6f65062e6f1",
            "transactiontimestamp": 1666821160,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "102790304",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1914043115.061178824090729747",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "e111c5528c3b684f8864642c7fbe6153fe0d6f567544ede7ddf6787b1b9414e4",
            "transactiontimestamp": 1666818962,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "1956612746",
            "amount0": "100008568",
            "amount1": "38772030844",
            "amountUSD": "3726085274.439050789340169714147855111871533552",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "e111c5528c3b684f8864642c7fbe6153fe0d6f567544ede7ddf6787b1b9414e4",
            "transactiontimestamp": 1666818962,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "liquidity": "100008568",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "e111c5528c3b684f8864642c7fbe6153fe0d6f567544ede7ddf6787b1b9414e4",
            "transactiontimestamp": 1666818962,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "38772030844",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5bb9315620c2d733cbfec950a78b66c8c0674983c5654e5f749ebd4716146e79",
            "transactiontimestamp": 1666818793,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5bb9315620c2d733cbfec950a78b66c8c0674983c5654e5f749ebd4716146e79",
            "transactiontimestamp": 1666818793,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "102943020",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1921496433.620524231401364824",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d4739d0dcda7f1948aedeffa45af22b5a3be44fb8ed1ebada373d30f3484e8f8",
            "transactiontimestamp": 1666818722,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d4739d0dcda7f1948aedeffa45af22b5a3be44fb8ed1ebada373d30f3484e8f8",
            "transactiontimestamp": 1666818722,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "103096132",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1922147640.618907719148134604",
            "to": "0ac4d8a6025fd36908bb05d2bbd52c4e287d5f891c8fa07e18819be6ab4b62d9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "8ef0628ea04bfd1042af9c26fd50fdedf815c4e226a414277240d7816a48c341",
            "transactiontimestamp": 1666813865,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "5053971215",
            "amount0": "258707841",
            "amount1": "100000000000",
            "amountUSD": "9518832907.75279039098052972290115643472062708",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "8ef0628ea04bfd1042af9c26fd50fdedf815c4e226a414277240d7816a48c341",
            "transactiontimestamp": 1666813865,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "258707841",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "8ef0628ea04bfd1042af9c26fd50fdedf815c4e226a414277240d7816a48c341",
            "transactiontimestamp": 1666813865,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "491b3b5fc98b512f3202739c3b9091f2604f44ddee68c06b380568f0d79d61c8",
            "transactiontimestamp": 1666813177,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "10890935739",
            "amount0": "1142898030",
            "amount1": "103800000000",
            "amountUSD": "108835117.36474819622707160123688067200000000",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "491b3b5fc98b512f3202739c3b9091f2604f44ddee68c06b380568f0d79d61c8",
            "transactiontimestamp": 1666813177,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "103800000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "491b3b5fc98b512f3202739c3b9091f2604f44ddee68c06b380568f0d79d61c8",
            "transactiontimestamp": 1666813177,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1142898030",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "6a874788c0c1fc5e4e884d0c2b6af7c856af89253a5f2d0a8493fa283c86473a",
            "transactiontimestamp": 1666812511,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "10107942431",
            "amount0": "517415682",
            "amount1": "200000000000",
            "amountUSD": "19015591091.37026474795402764584377463578159620",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "6a874788c0c1fc5e4e884d0c2b6af7c856af89253a5f2d0a8493fa283c86473a",
            "transactiontimestamp": 1666812511,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "517415682",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "6a874788c0c1fc5e4e884d0c2b6af7c856af89253a5f2d0a8493fa283c86473a",
            "transactiontimestamp": 1666812511,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "200000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "eb217caed8862d91be3def5f5a275b6787daf198cefdf83ec670d65bc28bd426",
            "transactiontimestamp": 1666812304,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "eb217caed8862d91be3def5f5a275b6787daf198cefdf83ec670d65bc28bd426",
            "transactiontimestamp": 1666812304,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "20000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1814518119789",
            "amountUSD": "947839550.349103030186208392",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "41e01f67ca34a6777c0214335c36e30af9dbe3a8fda86aaf1946501362b8829b",
            "transactiontimestamp": 1666811309,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "19d072ea8c4941c4216da656933457b8d6fa4f4fc57867c7971f4567e16970fa",
            "liquidity": "1959517239",
            "amount0": "100305769",
            "amount1": "38771832144",
            "amountUSD": "3720325345.48315253003987053365020565760447587",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "5033364d777b4622577d0da69b5e8af1f0eb1466b57ad9620c391cb2d8224e8f",
            "transactiontimestamp": 1666811151,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "19d072ea8c4941c4216da656933457b8d6fa4f4fc57867c7971f4567e16970fa",
            "liquidity": "1959517239",
            "amount0": "100305770",
            "amount1": "38771832147",
            "amountUSD": "3722417311.712067660371736309531057870858543000",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "5033364d777b4622577d0da69b5e8af1f0eb1466b57ad9620c391cb2d8224e8f",
            "transactiontimestamp": 1666811151,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "19d072ea8c4941c4216da656933457b8d6fa4f4fc57867c7971f4567e16970fa",
            "liquidity": "100305770",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "5033364d777b4622577d0da69b5e8af1f0eb1466b57ad9620c391cb2d8224e8f",
            "transactiontimestamp": 1666811151,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "38771832147",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "bcc0f620fced885ad7d467bbcee7beb471b14eb1d26f5e8611c57309d673b5b4",
            "transactiontimestamp": 1666810992,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "bcc0f620fced885ad7d467bbcee7beb471b14eb1d26f5e8611c57309d673b5b4",
            "transactiontimestamp": 1666810992,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "103250018",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1920053218.496438814040464248",
            "to": "19d072ea8c4941c4216da656933457b8d6fa4f4fc57867c7971f4567e16970fa",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a7bf3e9718fa31d345972a474862adca6c72dd07dbb2da290191338f2470b2a7",
            "transactiontimestamp": 1666809236,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "liquidity": "3919122469",
            "amount0": "200765961",
            "amount1": "77487325775",
            "amountUSD": "7538675295.616359744685301341766981787932331548",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "0ef884917248da27871ab38d4ffd012fb056e0a08ab38ed64a76cca1b3e1a4df",
            "transactiontimestamp": 1666806341,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "liquidity": "3919122469",
            "amount0": "200765962",
            "amount1": "77487325776",
            "amountUSD": "7457066660.22493028404397533349985427776779656",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "0ef884917248da27871ab38d4ffd012fb056e0a08ab38ed64a76cca1b3e1a4df",
            "transactiontimestamp": 1666806341,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "liquidity": "200765962",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "0ef884917248da27871ab38d4ffd012fb056e0a08ab38ed64a76cca1b3e1a4df",
            "transactiontimestamp": 1666806341,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "77487325776",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2ee7ffa7987e998407ea21256e54382c83ad12966fada064b8dd472df86cdfad",
            "transactiontimestamp": 1666806228,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2ee7ffa7987e998407ea21256e54382c83ad12966fada064b8dd472df86cdfad",
            "transactiontimestamp": 1666806228,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "103404681",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1920898953.654908453971139116",
            "to": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "f04d7358196d208df855957ca60f00b90b2ad8dffc3092b3c8ae927f0d30edab",
            "transactiontimestamp": 1666750539,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "liquidity": "1963882609",
            "amount0": "100679589",
            "amount1": "38799999569",
            "amountUSD": "3757523174.452850380127312915452667819405014680",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "177acc9bcf958784f0e512677126c775d4fc9b4b7f4d8e680902eb0288fb22af",
            "transactiontimestamp": 1666750330,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "liquidity": "1963882609",
            "amount0": "100679590",
            "amount1": "38799999572",
            "amountUSD": "3749211686.2869271360311975133111634261284440",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "177acc9bcf958784f0e512677126c775d4fc9b4b7f4d8e680902eb0288fb22af",
            "transactiontimestamp": 1666750330,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "liquidity": "100679590",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "177acc9bcf958784f0e512677126c775d4fc9b4b7f4d8e680902eb0288fb22af",
            "transactiontimestamp": 1666750330,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "38799999572",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "85b06291aa06944ebebb13952c2f5d2afe3daa603e263f3ec4a6f75b73eeca1c",
            "transactiontimestamp": 1666750180,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "85b06291aa06944ebebb13952c2f5d2afe3daa603e263f3ec4a6f75b73eeca1c",
            "transactiontimestamp": 1666750180,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "103559692",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1928654636.226879548964273439",
            "to": "6ee8d0cda497b15766a56d634229ebf848275994fc5155216edd2abf78cff7b7",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "82c1cb794983828ffbfb77ca07c970fa1bc1030d8c86fc50acabf32530987661",
            "transactiontimestamp": 1666749754,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "liquidity": "1965356773",
            "amount0": "100830569",
            "amount1": "38799998647",
            "amountUSD": "3755846185.173188667942516779041575478182917745",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d734c76615cc873df945e7011cf4377b12cd67386b7e527def63a2698d6a2180",
            "transactiontimestamp": 1666748650,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "2555101733",
            "amount0": "131086817",
            "amount1": "50442721213",
            "amountUSD": "4862936026.93207245397789843402760646121602846",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "53c71cea244ecd70147632d4d5b38154b9f00cd934f4ab78a9d4c2cec09e1a14",
            "transactiontimestamp": 1666745290,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "liquidity": "1965356773",
            "amount0": "100830570",
            "amount1": "38799998658",
            "amountUSD": "3688336146.58727699893289337836190080681660100",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "53c71cea244ecd70147632d4d5b38154b9f00cd934f4ab78a9d4c2cec09e1a14",
            "transactiontimestamp": 1666745290,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "liquidity": "100830570",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "53c71cea244ecd70147632d4d5b38154b9f00cd934f4ab78a9d4c2cec09e1a14",
            "transactiontimestamp": 1666745290,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "38799998658",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "58439aff6096d0e236a0c752fda08e95d2d6e1cfe03abe82381566096c042feb",
            "transactiontimestamp": 1666744969,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "58439aff6096d0e236a0c752fda08e95d2d6e1cfe03abe82381566096c042feb",
            "transactiontimestamp": 1666744969,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "51838036",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "948782634.398115316194822844",
            "to": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c6c4abb7759cbce4f6ee2fbe97784b4730c2f53f8ed0565b301dbc06f48f4457",
            "transactiontimestamp": 1666741269,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "liquidity": "491892475",
            "amount0": "25245466",
            "amount1": "9707281169",
            "amountUSD": "920767374.11988049775963972913688307414937944",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "76b5485a24c871f6b01476a367fe12d6824ca9987aa4829b471426f8dd54516f",
            "transactiontimestamp": 1666740041,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "76b5485a24c871f6b01476a367fe12d6824ca9987aa4829b471426f8dd54516f",
            "transactiontimestamp": 1666740041,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "103792702",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1901436434.168757622446661636",
            "to": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "bf5012533d6311e4e19ebf9e549788ba5d44ddfe53d02c62cbfd3b841542ad22",
            "transactiontimestamp": 1666739596,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "liquidity": "491892475",
            "amount0": "25264360",
            "amount1": "9699999787",
            "amountUSD": "920348025.29433787830630652357959224502904960",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "bf5012533d6311e4e19ebf9e549788ba5d44ddfe53d02c62cbfd3b841542ad22",
            "transactiontimestamp": 1666739596,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "liquidity": "25264360",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "bf5012533d6311e4e19ebf9e549788ba5d44ddfe53d02c62cbfd3b841542ad22",
            "transactiontimestamp": 1666739596,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9699999787",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "52cd04f11d9ab7fd60121736f149f590e719850a22225a8f952d7026801c2e95",
            "transactiontimestamp": 1666739474,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "52cd04f11d9ab7fd60121736f149f590e719850a22225a8f952d7026801c2e95",
            "transactiontimestamp": 1666739474,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25972470",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "473459393.193495625293010618",
            "to": "da6d7ef263e8b11ad6f5862c6e9e001b5ec92932cd48d2f57ba26320f4f13814",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "11c51ee50f128ca5cbd003d272b11257b0882d0cdbba9073c890d02f6b9aef8a",
            "transactiontimestamp": 1666735348,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "liquidity": "2951909006",
            "amount0": "151642999",
            "amount1": "58200000343",
            "amountUSD": "5564374494.18871575991193797651653635830211040",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "58113d95d5567aa5c8185f0e414dc6d16f88ebc44d8ac17639087bd2416e4c31",
            "transactiontimestamp": 1666735186,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "liquidity": "2951909006",
            "amount0": "151643000",
            "amount1": "58200000348",
            "amountUSD": "5565685005.797231958588693078373008220620000",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "58113d95d5567aa5c8185f0e414dc6d16f88ebc44d8ac17639087bd2416e4c31",
            "transactiontimestamp": 1666735186,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "liquidity": "151643000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "58113d95d5567aa5c8185f0e414dc6d16f88ebc44d8ac17639087bd2416e4c31",
            "transactiontimestamp": 1666735186,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "58200000348",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "69ab0be44ffb6cb71d720dfc1c1b5e6e7e1945edf3a54c4a5bb25d5bf7a99917",
            "transactiontimestamp": 1666734942,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "69ab0be44ffb6cb71d720dfc1c1b5e6e7e1945edf3a54c4a5bb25d5bf7a99917",
            "transactiontimestamp": 1666734942,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25982209",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "480242248.819374781444694850",
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "098f6cf44b974008666d5ed454601d8a9a91e86dac22c8b6da5198aba12354cf",
            "transactiontimestamp": 1666734867,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "098f6cf44b974008666d5ed454601d8a9a91e86dac22c8b6da5198aba12354cf",
            "transactiontimestamp": 1666734867,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25991953",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "480242235.560223679009715214",
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "311df592ad9f187cde956715c355c8704cd439a4c2153cbd4d0520ef322e3a58",
            "transactiontimestamp": 1666734470,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "311df592ad9f187cde956715c355c8704cd439a4c2153cbd4d0520ef322e3a58",
            "transactiontimestamp": 1666734470,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26001703",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "480018596.393429875886592009",
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1d00ad41b1ac65dfb857322851a023a5ce6d65b250998abbc3f6cced2eab9f06",
            "transactiontimestamp": 1666734233,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "1d00ad41b1ac65dfb857322851a023a5ce6d65b250998abbc3f6cced2eab9f06",
            "transactiontimestamp": 1666734233,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26021220",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "480437058.001284618685365636",
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "293ac1db99a3098fed7e5e03aeb95546454050e86bd2ed2580ddbe7fff96576d",
            "transactiontimestamp": 1666734217,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "293ac1db99a3098fed7e5e03aeb95546454050e86bd2ed2580ddbe7fff96576d",
            "transactiontimestamp": 1666734217,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26011459",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "480167159.310207674236051839",
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9798cd534d08912d4bbdb72f76e6426ed5a120a10764be70890843164c01d240",
            "transactiontimestamp": 1666733857,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9798cd534d08912d4bbdb72f76e6426ed5a120a10764be70890843164c01d240",
            "transactiontimestamp": 1666733857,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26030986",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "480394869.932142775870725943",
            "to": "0c7e7f23bcd5f56d82a58e5312029ddb65dedc4c353870ba1c5dac10bc8b1297",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "803f9c4a57199b14f7ff1ace04a1822985399cb2813e118d3e4be8755a9db168",
            "transactiontimestamp": 1666663050,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "803f9c4a57199b14f7ff1ace04a1822985399cb2813e118d3e4be8755a9db168",
            "transactiontimestamp": 1666663050,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "90911206490",
            "amountUSD": "46551061.545118145717161909",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1a4ef82bba0d33c53f71c72e8b0e35996de5a7db61ecc25ba4a3610471e8b299",
            "transactiontimestamp": 1666651840,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "2555101740",
            "amount0": "131406121",
            "amount1": "50319782077",
            "amountUSD": "4743441057.622279847246499722590072550355404848",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "c088e1abb9a28fde90507c3bb5ecc31089a5544c46e6ace44e1a9fbb33b6e4ea",
            "transactiontimestamp": 1666624104,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "492539610",
            "amount0": "25330780",
            "amount1": "9699999600",
            "amountUSD": "910358140.31212214196972233727816837381788160",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "c088e1abb9a28fde90507c3bb5ecc31089a5544c46e6ace44e1a9fbb33b6e4ea",
            "transactiontimestamp": 1666624104,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "25330780",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "c088e1abb9a28fde90507c3bb5ecc31089a5544c46e6ace44e1a9fbb33b6e4ea",
            "transactiontimestamp": 1666624104,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9699999600",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "87b63629fa1360f254abc05fbf89cdcbc4ceb22c337f57f43ccbe6a51c16656c",
            "transactiontimestamp": 1666623656,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "123000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "87b63629fa1360f254abc05fbf89cdcbc4ceb22c337f57f43ccbe6a51c16656c",
            "transactiontimestamp": 1666623656,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "320982595",
            "amount1In": "123000000000",
            "amount1Out": "0",
            "amountUSD": "5746816985.644509951491502882",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "23a746fac9648a6a3703cf4aa0825c3e18ae839e043301def583f574ab8e7546",
            "transactiontimestamp": 1666573766,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "497894406",
            "amount0": "25665280",
            "amount1": "9782805819",
            "amountUSD": "906126185.76194427329574922332681781216450560",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "23a746fac9648a6a3703cf4aa0825c3e18ae839e043301def583f574ab8e7546",
            "transactiontimestamp": 1666573766,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "25665280",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "23a746fac9648a6a3703cf4aa0825c3e18ae839e043301def583f574ab8e7546",
            "transactiontimestamp": 1666573766,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9782805819",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "3d39f54212ddc7286190468defd4c36c414ccae3d6f99d3e28c92cf6ecc81b40",
            "transactiontimestamp": 1666573594,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "497894406",
            "amount0": "25665280",
            "amount1": "9782805819",
            "amountUSD": "906237208.19048501425960962489151715867426560",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "3d39f54212ddc7286190468defd4c36c414ccae3d6f99d3e28c92cf6ecc81b40",
            "transactiontimestamp": 1666573594,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "25665280",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "3d39f54212ddc7286190468defd4c36c414ccae3d6f99d3e28c92cf6ecc81b40",
            "transactiontimestamp": 1666573594,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9782805819",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a46daf3f3ebde180403928909f79f9b5622c9879c59629cde0f401e735eb5a38",
            "transactiontimestamp": 1666572438,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a46daf3f3ebde180403928909f79f9b5622c9879c59629cde0f401e735eb5a38",
            "transactiontimestamp": 1666572438,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26161311",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "462372402.805975240325929640",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "49e358a8e2eb717ca52585d9071cf10de71a6505eae05d1bd760e509a6f95e2d",
            "transactiontimestamp": 1666562459,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "49e358a8e2eb717ca52585d9071cf10de71a6505eae05d1bd760e509a6f95e2d",
            "transactiontimestamp": 1666562459,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "262155995",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "4619822478.044396729340993246",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "e0999f491a3f5b7d95400b3719c1d14e44b1be62ad54214060689e0173eb53ac",
            "transactiontimestamp": 1666493378,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "138948155069",
            "amount0": "14551455289",
            "amount1": "1327000000000",
            "amountUSD": "1346371184.8749251913079904504120550000000000",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "e0999f491a3f5b7d95400b3719c1d14e44b1be62ad54214060689e0173eb53ac",
            "transactiontimestamp": 1666493378,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "1327000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "e0999f491a3f5b7d95400b3719c1d14e44b1be62ad54214060689e0173eb53ac",
            "transactiontimestamp": 1666493378,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "14551455289",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "eba20e4e30f0ca101857b43fa188587fb29284b1df14203f4cc5a3f6d95b73af",
            "transactiontimestamp": 1666472467,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "2550024395",
            "amount0": "131719755",
            "amount1": "50000000000",
            "amountUSD": "4618095644.938493525554711966635431644801734775",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "eba20e4e30f0ca101857b43fa188587fb29284b1df14203f4cc5a3f6d95b73af",
            "transactiontimestamp": 1666472467,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "131719755",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "eba20e4e30f0ca101857b43fa188587fb29284b1df14203f4cc5a3f6d95b73af",
            "transactiontimestamp": 1666472467,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "50000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "457d17b46e85117630b4f1f744fb21474fa1f1ca10955097e75ac5d26fe2014a",
            "transactiontimestamp": 1666392494,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "457d17b46e85117630b4f1f744fb21474fa1f1ca10955097e75ac5d26fe2014a",
            "transactiontimestamp": 1666392494,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "263146212",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "4595372559.249818612839820717",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "198fb7ece4b042049020c1808a35078ec43d94f20feff663b8a6a95722bec032",
            "transactiontimestamp": 1666229439,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "198fb7ece4b042049020c1808a35078ec43d94f20feff663b8a6a95722bec032",
            "transactiontimestamp": 1666229439,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "264142523",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "4066274898.252843879455621846",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a9063db1cc0b6f851d447021cb7ba8ff7887883e21152299d3238c22f125d72b",
            "transactiontimestamp": 1666199752,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a9063db1cc0b6f851d447021cb7ba8ff7887883e21152299d3238c22f125d72b",
            "transactiontimestamp": 1666199752,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26469199",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "423315131.602952716395925808",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "c55f8f9cf6ba0c1dfbd1d121b4821bfc14854ec7bf3b821bf0dc2c6a2df23a89",
            "transactiontimestamp": 1666104613,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "2560179078",
            "amount0": "132769328",
            "amount1": "50000000000",
            "amountUSD": "4672344983.04337476047843121329240427289814144",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "c55f8f9cf6ba0c1dfbd1d121b4821bfc14854ec7bf3b821bf0dc2c6a2df23a89",
            "transactiontimestamp": 1666104613,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "132769328",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "c55f8f9cf6ba0c1dfbd1d121b4821bfc14854ec7bf3b821bf0dc2c6a2df23a89",
            "transactiontimestamp": 1666104613,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "50000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a8074d792df6a7be925e41ab560ca157696932d921ed942ea22423e03492e8c1",
            "transactiontimestamp": 1665966443,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "500000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a8074d792df6a7be925e41ab560ca157696932d921ed942ea22423e03492e8c1",
            "transactiontimestamp": 1665966443,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "1336393098",
            "amount1In": "500000000000",
            "amount1Out": "0",
            "amountUSD": "23743260106.942702227245576547",
            "to": "516bae78a83f7b0f6a34a256507434e0f1a432cb0bb2212ca54a01d9ca5a15c9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "df046c2d8215fcea0506ae7d2d052dd53200528ce3868d9717c7b7a66683edc2",
            "transactiontimestamp": 1665705201,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "12938943",
            "amount0": "677415",
            "amount1": "250297868",
            "amountUSD": "18061047.29555678641457084841168187917264190",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "873c27518085dcba26c28432525d35f13816abb5cdd72e6c5a4d2c192522f08e",
            "transactiontimestamp": 1665615110,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "873c27518085dcba26c28432525d35f13816abb5cdd72e6c5a4d2c192522f08e",
            "transactiontimestamp": 1665615110,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "90928928603",
            "amountUSD": "34991741.798828493933923714",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ed4f93c8340fb1654dbaa8d777d4bf1d16ebef75c28256ab8a80d5b3d570ec76",
            "transactiontimestamp": 1665321019,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ed4f93c8340fb1654dbaa8d777d4bf1d16ebef75c28256ab8a80d5b3d570ec76",
            "transactiontimestamp": 1665321019,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26988353",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "360231148.472250056526145969",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "989d36991e941a612c7064ada01bc93e18e1b9588ccdcc2ac1d6bf2a6d5a971c",
            "transactiontimestamp": 1665294493,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "51695",
            "amount0": "2707",
            "amount1": "999825",
            "amountUSD": "69969.72175930523344766553527163817808232",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "989d36991e941a612c7064ada01bc93e18e1b9588ccdcc2ac1d6bf2a6d5a971c",
            "transactiontimestamp": 1665294493,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "2707",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "989d36991e941a612c7064ada01bc93e18e1b9588ccdcc2ac1d6bf2a6d5a971c",
            "transactiontimestamp": 1665294493,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999825",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "a9b4d80dd6306ba19418ee5449df8b470ddcb69be55f83270f19fc74e688a6f2",
            "transactiontimestamp": 1665294399,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "3272483",
            "amount0": "1000000",
            "amount1": "10710257",
            "amountUSD": "12917377.269256721118074049478133578168650288",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "a9b4d80dd6306ba19418ee5449df8b470ddcb69be55f83270f19fc74e688a6f2",
            "transactiontimestamp": 1665294399,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "1000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "a9b4d80dd6306ba19418ee5449df8b470ddcb69be55f83270f19fc74e688a6f2",
            "transactiontimestamp": 1665294399,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "10710257",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "175ba6616c1ba2735edc78f22e2b25143726d165c002c652a175350998018a0c",
            "transactiontimestamp": 1665294014,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "175ba6616c1ba2735edc78f22e2b25143726d165c002c652a175350998018a0c",
            "transactiontimestamp": 1665294014,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "910267037788",
            "amountUSD": "347790240.502552836591201886",
            "to": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "fb051fed23748713b8594343136d8884aa96727c92b366174a4806d001df93bf",
            "transactiontimestamp": 1665293373,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "51704077",
            "amount0": "2707473",
            "amount1": "999999814",
            "amountUSD": "69665820.122244529313173491744538134998586785",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "fb051fed23748713b8594343136d8884aa96727c92b366174a4806d001df93bf",
            "transactiontimestamp": 1665293373,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "liquidity": "2707473",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "fb051fed23748713b8594343136d8884aa96727c92b366174a4806d001df93bf",
            "transactiontimestamp": 1665293373,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999814",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "aff5b74616d778305d3bb718e6b30bd7852cff0ee77906bf45e2a4242b0e7ea4",
            "transactiontimestamp": 1665292905,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "aff5b74616d778305d3bb718e6b30bd7852cff0ee77906bf45e2a4242b0e7ea4",
            "transactiontimestamp": 1665292905,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26998685",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "347783320.895112731091889655",
            "to": "f50178ca772b2821d67336fcd333b50cdcfcdd626203b2fd00424cc6cb9e4be5",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b029a6a837a9e9eb24665a96795eb109f234912cc13ee54a3432958791af370c",
            "transactiontimestamp": 1665270971,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "50000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "b029a6a837a9e9eb24665a96795eb109f234912cc13ee54a3432958791af370c",
            "transactiontimestamp": 1665270971,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "135148770",
            "amount1In": "50000000000",
            "amount1Out": "0",
            "amountUSD": "1742553025.648953972999850068",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ceea0381297f2dcdb80f067f5bc1ca03f2c59b1f0af899cda780cb8872caff31",
            "transactiontimestamp": 1665082734,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ceea0381297f2dcdb80f067f5bc1ca03f2c59b1f0af899cda780cb8872caff31",
            "transactiontimestamp": 1665082734,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27060802",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "350364748.797800770129000301",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9db86acd980b9b1fbb1b33a969540ed1775e422da4ca473737a23f528443470d",
            "transactiontimestamp": 1665082676,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9db86acd980b9b1fbb1b33a969540ed1775e422da4ca473737a23f528443470d",
            "transactiontimestamp": 1665082676,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27071175",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "350289885.539200753673541991",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "089f735f0a67780db998c46e8fb53312b050fa79fdc7c605f39654fcfc6ed016",
            "transactiontimestamp": 1665067261,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "089f735f0a67780db998c46e8fb53312b050fa79fdc7c605f39654fcfc6ed016",
            "transactiontimestamp": 1665067261,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27081555",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "329524731.334741634231366968",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "bf8845fc8b68a2dbf7583e76d9d401cb7f53a17f71560a35724d9fafe71ef19f",
            "transactiontimestamp": 1665066959,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "bf8845fc8b68a2dbf7583e76d9d401cb7f53a17f71560a35724d9fafe71ef19f",
            "transactiontimestamp": 1665066959,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "912046234838",
            "amountUSD": "328474689.621023481583025052",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "329d0ddf12d2112828cec5d03fbc85a95348030640ec0e3a9fdff546ca722af0",
            "transactiontimestamp": 1665066853,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "50000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "329d0ddf12d2112828cec5d03fbc85a95348030640ec0e3a9fdff546ca722af0",
            "transactiontimestamp": 1665066853,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "135563836",
            "amount1In": "50000000000",
            "amount1Out": "0",
            "amountUSD": "1641565397.007650721122245708",
            "to": "d4c146f36525c2a04f421c845c7a88af065376e28961618a1d292abd95a3174f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5f3e35a0071237b0755f547f0469d4721095f415e6bdd76466a1471dfe18d19d",
            "transactiontimestamp": 1664952183,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5f3e35a0071237b0755f547f0469d4721095f415e6bdd76466a1471dfe18d19d",
            "transactiontimestamp": 1664952183,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "91302559663",
            "amountUSD": "30052231.834106059741496633",
            "to": "fda48750d6f7218d5f31613887315cb432485d2dd08412bc20e6fd9e1db4f0d7",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "179759a9bd84fed41d6a42b125432a9933302106e28dab4113fd8ca8bb26c00f",
            "transactiontimestamp": 1664301538,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9569309411",
            "amount0": "999999999",
            "amount1": "91586228762",
            "amountUSD": "56500775.92876624907988070297248718182664920",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "179759a9bd84fed41d6a42b125432a9933302106e28dab4113fd8ca8bb26c00f",
            "transactiontimestamp": 1664301538,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "91586228762",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "179759a9bd84fed41d6a42b125432a9933302106e28dab4113fd8ca8bb26c00f",
            "transactiontimestamp": 1664301538,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0d23e337778dfa7e40aeb5ffbfac2ac276e56423327da7e729cf565cea63e435",
            "transactiontimestamp": 1664301404,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "0d23e337778dfa7e40aeb5ffbfac2ac276e56423327da7e729cf565cea63e435",
            "transactiontimestamp": 1664301404,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "91320409921",
            "amountUSD": "28137282.234739898118133798",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ef395386d14363c45ece2abe90a4c74b563137a5cff43f6c5e2e3cf05ca99bbb",
            "transactiontimestamp": 1663652948,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "21489467979",
            "amount0": "2245445654",
            "amount1": "205692109663",
            "amountUSD": "124296707.324270961086707489454560068874247758",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "f560312ef77cc28c6395937068f3c5e9cb7dd2453f1c9b7a645ca5f6d3ed56e4",
            "transactiontimestamp": 1663652719,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "518431993",
            "amount0": "27220403",
            "amount1": "9999999942",
            "amountUSD": "553074091.200340512724628087963082937785467616",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "f560312ef77cc28c6395937068f3c5e9cb7dd2453f1c9b7a645ca5f6d3ed56e4",
            "transactiontimestamp": 1663652719,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "27220403",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "f560312ef77cc28c6395937068f3c5e9cb7dd2453f1c9b7a645ca5f6d3ed56e4",
            "transactiontimestamp": 1663652719,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9999999942",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "981bd1cb871b9d685a0d5b2f23f1de2c276ae4ff6c29fd270728a6fcac47d549",
            "transactiontimestamp": 1663652586,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "981bd1cb871b9d685a0d5b2f23f1de2c276ae4ff6c29fd270728a6fcac47d549",
            "transactiontimestamp": 1663652586,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "271910081",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "2757365709.578292440149661615",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "66c872d93399abba75d63cc262fc7c5279b17c78b277ef91029803c0e1fbb28c",
            "transactiontimestamp": 1663652431,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "32724834",
            "amount0": "10000000",
            "amount1": "107102576",
            "amountUSD": "101155847.806346759173795608288069283635011968",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "66c872d93399abba75d63cc262fc7c5279b17c78b277ef91029803c0e1fbb28c",
            "transactiontimestamp": 1663652431,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "107102576",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "66c872d93399abba75d63cc262fc7c5279b17c78b277ef91029803c0e1fbb28c",
            "transactiontimestamp": 1663652431,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "b2e13bbda79bb10c177fd7c7a799a1f36baac005d68bf09add1a26e468bd0e86",
            "transactiontimestamp": 1663652163,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "9570246303",
            "amount0": "1000000000",
            "amount1": "91604136230",
            "amountUSD": "55282903.834572272153647376369875650571183560",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "b2e13bbda79bb10c177fd7c7a799a1f36baac005d68bf09add1a26e468bd0e86",
            "transactiontimestamp": 1663652163,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "91604136230",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "b2e13bbda79bb10c177fd7c7a799a1f36baac005d68bf09add1a26e468bd0e86",
            "transactiontimestamp": 1663652163,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a9ee22ebd1d0a9d5cbd45bc0f7703ee50fbcd32176c15982ab92a00741c7b9d2",
            "transactiontimestamp": 1663619891,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a9ee22ebd1d0a9d5cbd45bc0f7703ee50fbcd32176c15982ab92a00741c7b9d2",
            "transactiontimestamp": 1663619891,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27248465",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "274195549.342426500880985125",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1c8853ccc9c1b849b3406f2c1eca01cae54d158dc3df5b31039f309ad51cb99a",
            "transactiontimestamp": 1663619780,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "1c8853ccc9c1b849b3406f2c1eca01cae54d158dc3df5b31039f309ad51cb99a",
            "transactiontimestamp": 1663619780,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27258949",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "274185727.650871536279696724",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5af02b2df25f4c30d1fa2a7be6e4dd98ca844acbca9517a440e840fb9410b69c",
            "transactiontimestamp": 1663619113,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5af02b2df25f4c30d1fa2a7be6e4dd98ca844acbca9517a440e840fb9410b69c",
            "transactiontimestamp": 1663619113,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27269439",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "274232267.931927551187444562",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d8f56b738723ccb5475da5003293fcfc90dcef8d1a41c0b9eab5eebe337d1403",
            "transactiontimestamp": 1663256161,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d8f56b738723ccb5475da5003293fcfc90dcef8d1a41c0b9eab5eebe337d1403",
            "transactiontimestamp": 1663256161,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10895431449",
            "amount1In": "1000000000000",
            "amount1Out": "0",
            "amountUSD": "321284684.736516362366331566",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0c7b3da2e437abdc96a9c4ef0b4303b0ed2e95a0a5b10312c099ede93a4c1df9",
            "transactiontimestamp": 1663202638,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "0c7b3da2e437abdc96a9c4ef0b4303b0ed2e95a0a5b10312c099ede93a4c1df9",
            "transactiontimestamp": 1663202638,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "912237281214",
            "amountUSD": "291211751.968923097752645614",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "28b5db3a6e5d45c4bec8c488acccce8e894df34d1b9da19ba16fadc18e5c4e08",
            "transactiontimestamp": 1663170165,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "76387625614",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7bdf255706de70afa03e78e5716aae9a811c056f74bd876df0352a7a0c0da8bd",
            "transactiontimestamp": 1663169704,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "50925083742",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "c00cdc865d2454aadd1df36f45ae40c059c21163c7b85ac2888c8d4fa97fe22b",
            "transactiontimestamp": 1663169492,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "95694074822",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "c00cdc865d2454aadd1df36f45ae40c059c21163c7b85ac2888c8d4fa97fe22b",
            "transactiontimestamp": 1663169492,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "915875166310",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "c00cdc865d2454aadd1df36f45ae40c059c21163c7b85ac2888c8d4fa97fe22b",
            "transactiontimestamp": 1663169492,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "509cf769925196e303b82aa90d2019f10397647642fe6a0c4e9ef73eb1a8cabc",
            "transactiontimestamp": 1663169190,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "509cf769925196e303b82aa90d2019f10397647642fe6a0c4e9ef73eb1a8cabc",
            "transactiontimestamp": 1663169190,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10897405873",
            "amount1In": "1000000000000",
            "amount1Out": "0",
            "amountUSD": "316392931.110476971058867331",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a196be3a37eacf13ad9a47a1e7d3013db797908d30080fc7a41fb4f24ca59e91",
            "transactiontimestamp": 1663169001,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a196be3a37eacf13ad9a47a1e7d3013db797908d30080fc7a41fb4f24ca59e91",
            "transactiontimestamp": 1663169001,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "912071856028",
            "amountUSD": "289877437.368328591202916160",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ba6116b20f19e265de9a299440fdf3770cc6a676be2b5952aaae555f7c5fe23b",
            "transactiontimestamp": 1663144315,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "108006260148",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "dd0672690380bc4516d8131108636572a42f8668970c74eb77f5afdb9d8f6980",
            "transactiontimestamp": 1663144078,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "72004173432",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "6ae31331c49377db38b1f6fcc02abfb973513976ed7ee38a335114e2995643d1",
            "transactiontimestamp": 1663142528,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "287057016964",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "6ae31331c49377db38b1f6fcc02abfb973513976ed7ee38a335114e2995643d1",
            "transactiontimestamp": 1663142528,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "2747126143239",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "6ae31331c49377db38b1f6fcc02abfb973513976ed7ee38a335114e2995643d1",
            "transactiontimestamp": 1663142528,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "30000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4e7f7f3f3ffb49d06202669ae7e7444cf4e3d06c606fd9634a5d8c7ef223e205",
            "transactiontimestamp": 1663142312,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4e7f7f3f3ffb49d06202669ae7e7444cf4e3d06c606fd9634a5d8c7ef223e205",
            "transactiontimestamp": 1663142312,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "913856723956",
            "amountUSD": "285916825.758118915053595802252425876153266484",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6996a526562c1797329325b8d889fe53827b95af2b6cd3f2df1c35bcd143f2a0",
            "transactiontimestamp": 1663142211,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6996a526562c1797329325b8d889fe53827b95af2b6cd3f2df1c35bcd143f2a0",
            "transactiontimestamp": 1663142211,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "915647818729",
            "amountUSD": "285991458.211229001095095808867961245627549652",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9e118ad1cf34a02c5ad12354c6ca6c534942748db71da3ec39dfc1afdbd7aa0b",
            "transactiontimestamp": 1663142117,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9e118ad1cf34a02c5ad12354c6ca6c534942748db71da3ec39dfc1afdbd7aa0b",
            "transactiontimestamp": 1663142117,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "917444186944",
            "amountUSD": "286026375.53073936664572925623704731475278912",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "4610956e56fc8bfda9c73caa7df1dd929279374618f1fa643224a437106ebbbf",
            "transactiontimestamp": 1663141998,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "959676764",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "4610956e56fc8bfda9c73caa7df1dd929279374618f1fa643224a437106ebbbf",
            "transactiontimestamp": 1663141998,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "9211060995",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "4610956e56fc8bfda9c73caa7df1dd929279374618f1fa643224a437106ebbbf",
            "transactiontimestamp": 1663141998,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "99999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "69ebf3743d1b86ceda47268ed25af3e7a8b5d79949e5c5d088fa21e020cf18f4",
            "transactiontimestamp": 1663141511,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "69ebf3743d1b86ceda47268ed25af3e7a8b5d79949e5c5d088fa21e020cf18f4",
            "transactiontimestamp": 1663141511,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "27279935",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "287578828.599716149777973082581406307040615190",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6dc7223a15a44f03e4b5fb91951a65b7e20b76fad84952baa81f7565b83a5a66",
            "transactiontimestamp": 1663141302,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6dc7223a15a44f03e4b5fb91951a65b7e20b76fad84952baa81f7565b83a5a66",
            "transactiontimestamp": 1663141302,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "91843300905",
            "amountUSD": "28826678.877973840106688344219262249584080300",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7e270cc6e8a1f06511fae7c1e31da2f5706c6ad3bd1fe8d559a6431d0138fea7",
            "transactiontimestamp": 1663113131,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "193866223",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "7e270cc6e8a1f06511fae7c1e31da2f5706c6ad3bd1fe8d559a6431d0138fea7",
            "transactiontimestamp": 1663113131,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "193866223",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "70722734375",
            "amountUSD": "2017839182.946454098718676215825708332245750436",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9e0cb5d956c63f734b70b0cb388155ddde1fd61a34f4ee41988b98ce2aa2abd3",
            "transactiontimestamp": 1663105673,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "193868894",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9e0cb5d956c63f734b70b0cb388155ddde1fd61a34f4ee41988b98ce2aa2abd3",
            "transactiontimestamp": 1663105673,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "193868894",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "70917070312",
            "amountUSD": "2038647833.113580765397281660624466920837960415",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "86dd9c933deb3690e24e84ce3c7fa9a177f089fbc7ae906d2bdcbf54ee2e3880",
            "transactiontimestamp": 1663087283,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "485682425",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "86dd9c933deb3690e24e84ce3c7fa9a177f089fbc7ae906d2bdcbf54ee2e3880",
            "transactiontimestamp": 1663087283,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "485682425",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "178516992187",
            "amountUSD": "5137057127.256951290958874165337090833621864860",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1f3ea068e909ec946fd66c0720bd85e754913978e45f90a836342ff1645a3978",
            "transactiontimestamp": 1663081649,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "2711296",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "1f3ea068e909ec946fd66c0720bd85e754913978e45f90a836342ff1645a3978",
            "transactiontimestamp": 1663081649,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "2711296",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1000000000",
            "amountUSD": "28696256.909622733254890029249400970478488576",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a9470fb3021b5850cf576c30971ba7f2a9374ab7588d239a61dbaffc1f8aa847",
            "transactiontimestamp": 1663081488,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a9470fb3021b5850cf576c30971ba7f2a9374ab7588d239a61dbaffc1f8aa847",
            "transactiontimestamp": 1663081488,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "3688605972",
            "amountUSD": "105868169.525848704882904827396181293920000000",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "833e996e3c561ea5f8a26659fb64ff397e5b5eb1f615c4d306b21a174bbae575",
            "transactiontimestamp": 1663080774,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1074248504",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "833e996e3c561ea5f8a26659fb64ff397e5b5eb1f615c4d306b21a174bbae575",
            "transactiontimestamp": 1663080774,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "100000000",
            "amount1In": "1074248504",
            "amount1Out": "0",
            "amountUSD": "530256891.3396258403885731740948684276619840",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "19d7ac6d64446a4c8f40ce282ac8c0be4be75774f0523ee083e203f85496b523",
            "transactiontimestamp": 1663080463,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "19d7ac6d64446a4c8f40ce282ac8c0be4be75774f0523ee083e203f85496b523",
            "transactiontimestamp": 1663080463,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "93088330",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "496097695.424959503253041387035132173817711280",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1024915af03a462ff77f64223020b8481eadaeec0f7a19b9277aed9781dd0a93",
            "transactiontimestamp": 1663080281,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "1024915af03a462ff77f64223020b8481eadaeec0f7a19b9277aed9781dd0a93",
            "transactiontimestamp": 1663080281,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "10678126821",
            "amountUSD": "5340478433.32553880096172274470068620627867900",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "06f78f80aacd2a61a8ff394dcbd7bd00386df7ea912a4e08ae5ca31e760d578e",
            "transactiontimestamp": 1663079945,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10887033",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "06f78f80aacd2a61a8ff394dcbd7bd00386df7ea912a4e08ae5ca31e760d578e",
            "transactiontimestamp": 1663079945,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10887033",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1000000000",
            "amountUSD": "313910.48301381258504561005591979000000000",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "42ea171634a1395dc8fccb761afded28fca1c568a694af9aaba653f9f0a7baa6",
            "transactiontimestamp": 1663079741,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "42ea171634a1395dc8fccb761afded28fca1c568a694af9aaba653f9f0a7baa6",
            "transactiontimestamp": 1663079741,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "91861519182",
            "amountUSD": "28811880.77823759205463990732476139295615337",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "178d27b5771e526c51a55d840e233276db7afd167b72ddb7a0585bf6004431c8",
            "transactiontimestamp": 1663078891,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "178d27b5771e526c51a55d840e233276db7afd167b72ddb7a0585bf6004431c8",
            "transactiontimestamp": 1663078891,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26951352",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "284740107.932080140026942574136548200845562512",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "b1447a9d831809ba71a1f80ffcb0833c3a58f64841bdd9a64767df5bdd3368a6",
            "transactiontimestamp": 1663077674,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "30554666552",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "b1447a9d831809ba71a1f80ffcb0833c3a58f64841bdd9a64767df5bdd3368a6",
            "transactiontimestamp": 1663077674,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "b1447a9d831809ba71a1f80ffcb0833c3a58f64841bdd9a64767df5bdd3368a6",
            "transactiontimestamp": 1663077674,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9336843576",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "783282bb391dc0bf798b14c7bc9bd58a923da9788b4e54e4054f4f194431ee65",
            "transactiontimestamp": 1663077301,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "95986639759",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "783282bb391dc0bf798b14c7bc9bd58a923da9788b4e54e4054f4f194431ee65",
            "transactiontimestamp": 1663077301,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "921469593392",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "783282bb391dc0bf798b14c7bc9bd58a923da9788b4e54e4054f4f194431ee65",
            "transactiontimestamp": 1663077301,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "63d383957434207e2501c1df3ffb1563621e6e67f0fd2232f6d21fd306e1f125",
            "transactiontimestamp": 1663077123,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "95986639759",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "63d383957434207e2501c1df3ffb1563621e6e67f0fd2232f6d21fd306e1f125",
            "transactiontimestamp": 1663077123,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "921469593392",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "63d383957434207e2501c1df3ffb1563621e6e67f0fd2232f6d21fd306e1f125",
            "transactiontimestamp": 1663077123,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ed5658fc56874bfbad8c149d544b5bddffb0f53b3179f203c8047654e872377e",
            "transactiontimestamp": 1663071840,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ed5658fc56874bfbad8c149d544b5bddffb0f53b3179f203c8047654e872377e",
            "transactiontimestamp": 1663071840,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "93088330",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "515709488.84582262052254848514125109638035190",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "7e223d247d330887db03330bf6fc58a5dc7a5d8072810efcc3aa1a3d2bd6ba80",
            "transactiontimestamp": 1663067679,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1833279993523613896",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "7e223d247d330887db03330bf6fc58a5dc7a5d8072810efcc3aa1a3d2bd6ba80",
            "transactiontimestamp": 1663067679,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "6000000000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "7e223d247d330887db03330bf6fc58a5dc7a5d8072810efcc3aa1a3d2bd6ba80",
            "transactiontimestamp": 1663067679,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "560210614772514383",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "36e1fd433e9314c6676a57b0c833ecca4b3fb68c420a2e67e7de37d4b9ab9f41",
            "transactiontimestamp": 1663067417,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "36e1fd433e9314c6676a57b0c833ecca4b3fb68c420a2e67e7de37d4b9ab9f41",
            "transactiontimestamp": 1663067417,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "93088339",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "510297001.90175162123012239237643320684227411",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c47b554ab5d92dd9e2ac6fa1fd858d6fc229d9c90c6e28d12d4b546801a4500c",
            "transactiontimestamp": 1662988573,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "974762159",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c47b554ab5d92dd9e2ac6fa1fd858d6fc229d9c90c6e28d12d4b546801a4500c",
            "transactiontimestamp": 1662988573,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "974762159",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "361939023437",
            "amountUSD": "10801375022.838727822697883916689619679023390088",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "583e46203da2898283f6ea10c8e13fb33feb993e0e3f01189b93584f663d9705",
            "transactiontimestamp": 1662912249,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "583e46203da2898283f6ea10c8e13fb33feb993e0e3f01189b93584f663d9705",
            "transactiontimestamp": 1662912249,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "26591036",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "305160987.104266810497312245705154581958204800",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2d689c0dfff4be580fae33020f447b41ad4bd40de47b833e84cee64dba089337",
            "transactiontimestamp": 1662766216,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "485692115",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2d689c0dfff4be580fae33020f447b41ad4bd40de47b833e84cee64dba089337",
            "transactiontimestamp": 1662766216,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "485692115",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "182154960937",
            "amountUSD": "5127773889.034009162314887513550858814459586775",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "4c4e959ff3938c25c720a4fe01e158b0066f578e7f194ebe925ae0948b075bae",
            "transactiontimestamp": 1662732194,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "95986639759",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "4c4e959ff3938c25c720a4fe01e158b0066f578e7f194ebe925ae0948b075bae",
            "transactiontimestamp": 1662732194,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "921469593392",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "4c4e959ff3938c25c720a4fe01e158b0066f578e7f194ebe925ae0948b075bae",
            "transactiontimestamp": 1662732194,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "9999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2727b6e278c2bf350af7df7232ec82749e22ab66ef48d935fe61f2a0b73d3060",
            "transactiontimestamp": 1662732038,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2727b6e278c2bf350af7df7232ec82749e22ab66ef48d935fe61f2a0b73d3060",
            "transactiontimestamp": 1662732038,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "264625654",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "2787890988.503178726279033331373110408606999536",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "98b7828e567fbd910b7eddf1a6d3b34341e703ba400568afaab3058c83cf026e",
            "transactiontimestamp": 1662729053,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "98b7828e567fbd910b7eddf1a6d3b34341e703ba400568afaab3058c83cf026e",
            "transactiontimestamp": 1662729053,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10831257356",
            "amount1In": "1000000000000",
            "amount1Out": "0",
            "amountUSD": "302705600.443675907756446336040604000000000000",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4492066abc9c19e63c53216a3fa31278a96b78cc740f9b9fc1d90706508ce676",
            "transactiontimestamp": 1662728693,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4492066abc9c19e63c53216a3fa31278a96b78cc740f9b9fc1d90706508ce676",
            "transactiontimestamp": 1662728693,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "20000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1837105249948",
            "amountUSD": "558590832.204276992538947608377731169265419020",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c186e82c5d05629a3a6e9091cf84c8ef74fd67a2b77237c80dad3b576759181f",
            "transactiontimestamp": 1662728102,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c186e82c5d05629a3a6e9091cf84c8ef74fd67a2b77237c80dad3b576759181f",
            "transactiontimestamp": 1662728102,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10811780393",
            "amount1In": "1000000000000",
            "amount1Out": "0",
            "amountUSD": "304414146.76184305010770822236623500000000000",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "296472ffe491f88d11393f07dc677c28dfff07171164b6d9a6d38f8ca69fab36",
            "transactiontimestamp": 1662727981,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "296472ffe491f88d11393f07dc677c28dfff07171164b6d9a6d38f8ca69fab36",
            "transactiontimestamp": 1662727981,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "20000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1840419761308",
            "amountUSD": "560697658.688181272486516483718031726861286928",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4f888f285d115f9b6459c3caee7a35712bd7e0fd08de556b48f7ff6e4abac09a",
            "transactiontimestamp": 1662727536,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4f888f285d115f9b6459c3caee7a35712bd7e0fd08de556b48f7ff6e4abac09a",
            "transactiontimestamp": 1662727536,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "107808727",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "3038193.399628325505326872312701740000000000",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a7f74878b719d3a7a40604a1f07c5169c011b376084a8e7e791c7b2a4dda87e7",
            "transactiontimestamp": 1662678562,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "50000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a7f74878b719d3a7a40604a1f07c5169c011b376084a8e7e791c7b2a4dda87e7",
            "transactiontimestamp": 1662678562,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "4654440440",
            "amount1In": "50000000000",
            "amount1Out": "0",
            "amountUSD": "23330662315.243461225697092501728741213787210400",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a3b1812bbf63469f550e25564e3564dd1c0029de8f2d106abe9061dd93a2b255",
            "transactiontimestamp": 1662678304,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "5000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a3b1812bbf63469f550e25564e3564dd1c0029de8f2d106abe9061dd93a2b255",
            "transactiontimestamp": 1662678304,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "5000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "53390379376",
            "amountUSD": "25074809240.699654033242933003160978526317811344",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b268cd4fb0d6a2d211f727ff9a10824c51f91f7cd41b9cc256247d76b1f735e7",
            "transactiontimestamp": 1662677164,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "974820309",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "b268cd4fb0d6a2d211f727ff9a10824c51f91f7cd41b9cc256247d76b1f735e7",
            "transactiontimestamp": 1662677164,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "974820309",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "368041171875",
            "amountUSD": "9854968034.33403903020887344204347382738054096",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d90b301b00aef78ed6e120d955722a640c8a98711a0be18f1b1948c6ec0e8fe5",
            "transactiontimestamp": 1662676577,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "500000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d90b301b00aef78ed6e120d955722a640c8a98711a0be18f1b1948c6ec0e8fe5",
            "transactiontimestamp": 1662676577,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "46546441639",
            "amount1In": "500000000000",
            "amount1Out": "0",
            "amountUSD": "236600929889.77428229585137180376296858300963837",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4972a665423c7077674e3cbf1bd88f5d4464eb3f4448657975e5ce1181185884",
            "transactiontimestamp": 1662673684,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "liquidity": "974864215",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4972a665423c7077674e3cbf1bd88f5d4464eb3f4448657975e5ce1181185884",
            "transactiontimestamp": 1662673684,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "974864215",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "373249375000",
            "amountUSD": "9938749964.15691399078294888855456042761464650",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "318624edde7e1c705db9836bd37de9ca45cfe8119f7b11f34c078b7940b1d037",
            "transactiontimestamp": 1662669645,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "318624edde7e1c705db9836bd37de9ca45cfe8119f7b11f34c078b7940b1d037",
            "transactiontimestamp": 1662669645,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "51579889",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "527357088.91469388877311195201591337464153999",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8275ee6a701861d676bfdeadde5c3d95accca96857ba9636923f9c88d8de10f9",
            "transactiontimestamp": 1662662733,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "8275ee6a701861d676bfdeadde5c3d95accca96857ba9636923f9c88d8de10f9",
            "transactiontimestamp": 1662662733,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "51618515",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "524880136.595586397585044219102659848234178115",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e5e3a89f21c99a4e82c5a17375b35a511005e60a8241759c62b89bcca9e0140c",
            "transactiontimestamp": 1662585909,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "e5e3a89f21c99a4e82c5a17375b35a511005e60a8241759c62b89bcca9e0140c",
            "transactiontimestamp": 1662585909,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25823748",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "265995636.77045823146630263190612903666287008",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "08e34447eaefc1823b8955438c298491e9cbe5bb409b296064f31702d63f3bc1",
            "transactiontimestamp": 1662558723,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "08e34447eaefc1823b8955438c298491e9cbe5bb409b296064f31702d63f3bc1",
            "transactiontimestamp": 1662558723,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "51676536",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "515439729.615759502529862600235218716506840880",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "3728d0e1b5015d930a3eebb133e2dd2a7842ceb7a7529639726e2d1e05db42eb",
            "transactiontimestamp": 1662551250,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "3728d0e1b5015d930a3eebb133e2dd2a7842ceb7a7529639726e2d1e05db42eb",
            "transactiontimestamp": 1662551250,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "258965159",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "2559714455.63416328064081871583393536790105671",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "68efa91c9795a7657cece2fb8cf4036bd4c7a0e5feb0d2110cc66d343c3cfe26",
            "transactiontimestamp": 1662513187,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "930975613",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "4587270842.11094371302389416556776895396941728",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1f33eee59957329e8942a8e3b61ed2498dda117707981402df441632dcfc542a",
            "transactiontimestamp": 1662512331,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "1f33eee59957329e8942a8e3b61ed2498dda117707981402df441632dcfc542a",
            "transactiontimestamp": 1662512331,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "51909600",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "511247224.829030611064411180210885685604856000",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0b17fe89192c73947665819eac9fa1a24ac6359bb41d43f08dc340721dbdfa35",
            "transactiontimestamp": 1662510956,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "0b17fe89192c73947665819eac9fa1a24ac6359bb41d43f08dc340721dbdfa35",
            "transactiontimestamp": 1662510956,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2596501",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "25515369.363882394527058898522575951924432812",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7d13e8014e610a435b8d06eab754a356b002423ea8d7e530debf4e816eaf68cc",
            "transactiontimestamp": 1662510440,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "7d13e8014e610a435b8d06eab754a356b002423ea8d7e530debf4e816eaf68cc",
            "transactiontimestamp": 1662510440,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2596599",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "25521741.234218043006799762440326410695118944",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d076eb420ba8712eeabca6b6c9d9c7e83467f335fe39070cdbb0bda9f35e8468",
            "transactiontimestamp": 1662509886,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d076eb420ba8712eeabca6b6c9d9c7e83467f335fe39070cdbb0bda9f35e8468",
            "transactiontimestamp": 1662509886,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2596696",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "25867839.961287031262986161684095802025404024",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9f8c5d75184e1a05c2df92c0f09a93970d2dccb81e207a5249a37fcac45f35ce",
            "transactiontimestamp": 1662509355,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9f8c5d75184e1a05c2df92c0f09a93970d2dccb81e207a5249a37fcac45f35ce",
            "transactiontimestamp": 1662509355,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2596794",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "25851831.97895061128714701652025811286795968",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "add6fd1b004507f15701cd61533a41ef522302f2f8ce890421810be22f346e2e",
            "transactiontimestamp": 1662508712,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "add6fd1b004507f15701cd61533a41ef522302f2f8ce890421810be22f346e2e",
            "transactiontimestamp": 1662508712,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2596891",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "25720737.085732658824388188420493217063006605",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6aa527519f1db4fc6fe6cfdefc5350acbc399e4673d950a3e37fd813b13cf2b2",
            "transactiontimestamp": 1662500037,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6aa527519f1db4fc6fe6cfdefc5350acbc399e4673d950a3e37fd813b13cf2b2",
            "transactiontimestamp": 1662500037,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "25974290",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "260170568.913404149736748403206879447043025805",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "bc9c7a84e7fdc41310238158880bb44f6dcce8be246d7d77067d7db35edc51e8",
            "transactiontimestamp": 1662493711,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "4807979005",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "bc9c7a84e7fdc41310238158880bb44f6dcce8be246d7d77067d7db35edc51e8",
            "transactiontimestamp": 1662493711,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "46238807005",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "bc9c7a84e7fdc41310238158880bb44f6dcce8be246d7d77067d7db35edc51e8",
            "transactiontimestamp": 1662493711,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "500000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8ae684a2cfa90690c8e6157b6bfee7ff7a21b3b4ffb72907afc4ee86afc830ee",
            "transactiontimestamp": 1662490051,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "8ae684a2cfa90690c8e6157b6bfee7ff7a21b3b4ffb72907afc4ee86afc830ee",
            "transactiontimestamp": 1662490051,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "92209285306",
            "amountUSD": "25855161.696753407302182449401325832531377808",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ef48b3a458f855309e0fe4aa79caf9099842ee98eac9347d227485f251202a35",
            "transactiontimestamp": 1662489294,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ef48b3a458f855309e0fe4aa79caf9099842ee98eac9347d227485f251202a35",
            "transactiontimestamp": 1662489294,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "260281147",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "2581627241.33272927727313396605211848891590445",
            "to": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c1ff94132c26497973e345491f25a4aaee4c36dc5b225b268b4b9b6fac9d3a48",
            "transactiontimestamp": 1662482968,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "30000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c1ff94132c26497973e345491f25a4aaee4c36dc5b225b268b4b9b6fac9d3a48",
            "transactiontimestamp": 1662482968,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "30000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "320311736",
            "amountUSD": "155025932.978844606592513144887583934669690720",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "547923a8b4abee7ca029dc9d8363074a4fc099d9b41f4d27b11bc92112b6cf2a",
            "transactiontimestamp": 1662481776,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "547923a8b4abee7ca029dc9d8363074a4fc099d9b41f4d27b11bc92112b6cf2a",
            "transactiontimestamp": 1662481776,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "92227469862",
            "amountUSD": "26939685.468326861254070633831186549074916732",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2f7a2553bf8e6536772c8c4442bc88ce087970f757274649dbbecb6991e32f13",
            "transactiontimestamp": 1662481681,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "111000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2f7a2553bf8e6536772c8c4442bc88ce087970f757274649dbbecb6991e32f13",
            "transactiontimestamp": 1662481681,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "290061539",
            "amount1In": "111000000000",
            "amount1Out": "0",
            "amountUSD": "2987583150.594946327950923310755691305005232400",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "3a5788b2ad96b93f3038be2e72e901dfd1ae295aa81d26435ec2be8ef4edfd15",
            "transactiontimestamp": 1662471454,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "40000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "3a5788b2ad96b93f3038be2e72e901dfd1ae295aa81d26435ec2be8ef4edfd15",
            "transactiontimestamp": 1662471454,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "104824285",
            "amount1In": "40000000000",
            "amount1Out": "0",
            "amountUSD": "1093092851.88929207633725836806763345100155660",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "0d8b6c81ccf785abfaa28c8ed48dade9b93e21f98656bab28c91ede4ced3d6d8",
            "transactiontimestamp": 1662470805,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "20000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "213541169",
            "amountUSD": "104527901.430632051742860140986822530811700164",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ce2d9c0f58d70f7b68dc5d557865904c9d01aedf97f112d486f865e045fa0f70",
            "transactiontimestamp": 1662470368,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ce2d9c0f58d70f7b68dc5d557865904c9d01aedf97f112d486f865e045fa0f70",
            "transactiontimestamp": 1662470368,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "20000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1848381667542",
            "amountUSD": "548521965.4618660466545709715706982727514780",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5900fd3751c76ee1e65ec0002ff07f89616e8122f04dc0be4a903b345de1cd80",
            "transactiontimestamp": 1662469330,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5900fd3751c76ee1e65ec0002ff07f89616e8122f04dc0be4a903b345de1cd80",
            "transactiontimestamp": 1662469330,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "52471472",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "548873545.87412246535978511639192287252983904",
            "to": "675e10b7e268c61db84dbc4ddd0dc6c92230b6898e8d2109a3fdc49de8fedab4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "65c04c98c0ba382fcfe3d7bbf0d8a2d9925de22325d4a46684883a087cd8a939",
            "transactiontimestamp": 1662425077,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "50000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "65c04c98c0ba382fcfe3d7bbf0d8a2d9925de22325d4a46684883a087cd8a939",
            "transactiontimestamp": 1662425077,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "50000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "533852962",
            "amountUSD": "261172755.472156423128908482724936227871255580",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6be6a09ad666013a7213bd093f45bfaa94c5686d7acf2f12f566e2452c9cc259",
            "transactiontimestamp": 1662420655,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "60000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6be6a09ad666013a7213bd093f45bfaa94c5686d7acf2f12f566e2452c9cc259",
            "transactiontimestamp": 1662420655,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "60000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "640623629",
            "amountUSD": "306606758.33681160834652622605094413933017936",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9f2135cfd96dac0eb7de0bbe7714cc6ffa7a7385e4cd4370e435d3f1daaf7e31",
            "transactiontimestamp": 1662400836,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9f2135cfd96dac0eb7de0bbe7714cc6ffa7a7385e4cd4370e435d3f1daaf7e31",
            "transactiontimestamp": 1662400836,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "92610592692",
            "amountUSD": "27024229.410849018473194436322826297654988096",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "053b3120c49dc225877be60910e6b0c0d54254c936017a7c5617a283118f9d23",
            "transactiontimestamp": 1662400760,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "300000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "053b3120c49dc225877be60910e6b0c0d54254c936017a7c5617a283118f9d23",
            "transactiontimestamp": 1662400760,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "791859608",
            "amount1In": "300000000000",
            "amount1Out": "0",
            "amountUSD": "8080185738.711197953505423110998771080304172356",
            "to": "0dc58556828f1bee0593177abcf5b276ea0605ae1b0b6ae44c6aa98716a1f459",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8a2c4b5c08a7babbf44f142894a175d2a54b8e70dba5eea5d1eea4f0139c72b0",
            "transactiontimestamp": 1662397298,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "1100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "8a2c4b5c08a7babbf44f142894a175d2a54b8e70dba5eea5d1eea4f0139c72b0",
            "transactiontimestamp": 1662397298,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "102407394",
            "amount1In": "1100000000",
            "amount1Out": "0",
            "amountUSD": "521546939.846149068070554837843611542746869187",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7439fc5d60436d78ce43797c5e0c11e5516437da8068ecd357c6b1ac4ab36e52",
            "transactiontimestamp": 1662395992,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "7439fc5d60436d78ce43797c5e0c11e5516437da8068ecd357c6b1ac4ab36e52",
            "transactiontimestamp": 1662395992,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "53111029",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "541993307.01187018439052103380349308122473950",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4e6f77321b426f6ef018e3979121f585e235d06145423076f5dfcef7d1388aff",
            "transactiontimestamp": 1662395037,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4e6f77321b426f6ef018e3979121f585e235d06145423076f5dfcef7d1388aff",
            "transactiontimestamp": 1662395037,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "92628896155",
            "amountUSD": "27136155.593480443885929592608829908930290835",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8e7bb3595773e163132814d389fec262a4093c4dc9e4efb30faf24e822cd8945",
            "transactiontimestamp": 1662394939,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "8e7bb3595773e163132814d389fec262a4093c4dc9e4efb30faf24e822cd8945",
            "transactiontimestamp": 1662394939,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "266162075",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "2711180146.294130528181436384750439691336786031",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "03335a04b2c1ebcd361c5c5c1769244f37edf2ce8ead208fbfe96ba7243055fa",
            "transactiontimestamp": 1662394696,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3055619745999603",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "03335a04b2c1ebcd361c5c5c1769244f37edf2ce8ead208fbfe96ba7243055fa",
            "transactiontimestamp": 1662394696,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10000000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "03335a04b2c1ebcd361c5c5c1769244f37edf2ce8ead208fbfe96ba7243055fa",
            "transactiontimestamp": 1662394696,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "933777751443295",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "57fb73d38860b9b15bbe4d9db3227a694423e2bfbeb4e5f16abf5e1971248f36",
            "transactiontimestamp": 1662394426,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "21791254071",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "57fb73d38860b9b15bbe4d9db3227a694423e2bfbeb4e5f16abf5e1971248f36",
            "transactiontimestamp": 1662394426,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "424000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "57fb73d38860b9b15bbe4d9db3227a694423e2bfbeb4e5f16abf5e1971248f36",
            "transactiontimestamp": 1662394426,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1134073432",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "6273a170cfe8dc4b7f01e40036ca7031556fcefbacbd6a85842dc6cbb5b403c4",
            "transactiontimestamp": 1662394204,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "113067827763",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "6273a170cfe8dc4b7f01e40036ca7031556fcefbacbd6a85842dc6cbb5b403c4",
            "transactiontimestamp": 1662394204,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "5884343281",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "6273a170cfe8dc4b7f01e40036ca7031556fcefbacbd6a85842dc6cbb5b403c4",
            "transactiontimestamp": 1662394204,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "2200000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "78f6dffc33a54815afcab28b4f7549dfa2b8c26d9dea3d2c28b558e2d507ac89",
            "transactiontimestamp": 1662393905,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "96387981286899",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "78f6dffc33a54815afcab28b4f7549dfa2b8c26d9dea3d2c28b558e2d507ac89",
            "transactiontimestamp": 1662393905,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "929167863041755",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "78f6dffc33a54815afcab28b4f7549dfa2b8c26d9dea3d2c28b558e2d507ac89",
            "transactiontimestamp": 1662393905,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "dfc59a1ebcf4f8ed85666219afeaf8bd082bba25381dc1bd3cf73e0915c1558e",
            "transactiontimestamp": 1662393745,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "2497953791502",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "dfc59a1ebcf4f8ed85666219afeaf8bd082bba25381dc1bd3cf73e0915c1558e",
            "transactiontimestamp": 1662393745,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "130000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "dfc59a1ebcf4f8ed85666219afeaf8bd082bba25381dc1bd3cf73e0915c1558e",
            "transactiontimestamp": 1662393745,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "48603554601825",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ecc8b918e1bab7ac8ae3c3f1b442c34432122de9c40f83a174c76089885e2afe",
            "transactiontimestamp": 1662145179,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ecc8b918e1bab7ac8ae3c3f1b442c34432122de9c40f83a174c76089885e2afe",
            "transactiontimestamp": 1662145179,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1067715489",
            "amountUSD": "520965632.813757801181908847485544733016302675",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "3fb121b9192560cf88faef79fa1783abacfdd769a620e85a95e228e274ee3f17",
            "transactiontimestamp": 1662144970,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "3fb121b9192560cf88faef79fa1783abacfdd769a620e85a95e228e274ee3f17",
            "transactiontimestamp": 1662144970,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10731138",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "299592.13949155766213786275504555500000000",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "b39e911a75b4725a9507f22ce68c09f05e5040bc881db34d0918dbf7762c0b76",
            "transactiontimestamp": 1662072693,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1067734671",
            "amountUSD": "521900260.235641978893235549890676856332200840",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e2a2f0e2af954aeb53591f8ceacaecbac972697504669061c700067828100b12",
            "transactiontimestamp": 1662035414,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "45000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "e2a2f0e2af954aeb53591f8ceacaecbac972697504669061c700067828100b12",
            "transactiontimestamp": 1662035414,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "124478937",
            "amount1In": "45000000000",
            "amount1Out": "0",
            "amountUSD": "1237160641.039987689068157503824074096943165394",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7abfddd34d4d5a98706835179cc76150edb9499d56dd47c892508c6c3df4fc05",
            "transactiontimestamp": 1662015487,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "107857613",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "7abfddd34d4d5a98706835179cc76150edb9499d56dd47c892508c6c3df4fc05",
            "transactiontimestamp": 1662015487,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "107857613",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "10000000000",
            "amountUSD": "3014740.781395003008038120882528000000000000",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "59c471410c65c973ae5dd4b412453cacf073b9369b3b1cae2e5bb65cff2e7806",
            "transactiontimestamp": 1661987875,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "20000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "59c471410c65c973ae5dd4b412453cacf073b9369b3b1cae2e5bb65cff2e7806",
            "transactiontimestamp": 1661987875,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "58350331",
            "amount1In": "20000000000",
            "amount1Out": "0",
            "amountUSD": "549779499.784821342273581114511794244838089072",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "78fce3395d1438827124dd7cdb3730110c3840277f763ecdc107483e7e963166",
            "transactiontimestamp": 1661972145,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "78fce3395d1438827124dd7cdb3730110c3840277f763ecdc107483e7e963166",
            "transactiontimestamp": 1661972145,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "296682",
            "amount1In": "100000000",
            "amount1Out": "0",
            "amountUSD": "2760520.47430409718990342509488040253544712",
            "to": "b435c66fd1423dba514af2015b43eeceae8bf71f4b201ac379934400b74bc02d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d9d53028254ad272a982d3e69afe1d3bff5cb518a7fd81e40e13028537edd31b",
            "transactiontimestamp": 1661970836,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d9d53028254ad272a982d3e69afe1d3bff5cb518a7fd81e40e13028537edd31b",
            "transactiontimestamp": 1661970836,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "29923142",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "274841513.30362196649815244350448470991795528",
            "to": "b435c66fd1423dba514af2015b43eeceae8bf71f4b201ac379934400b74bc02d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "53f99f5316c56ee9b3ca3b5f2bd9f6394c5f270e5d57f3ec98e5bbd5b2d258f8",
            "transactiontimestamp": 1661969702,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "53f99f5316c56ee9b3ca3b5f2bd9f6394c5f270e5d57f3ec98e5bbd5b2d258f8",
            "transactiontimestamp": 1661969702,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "30435775",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "274982369.236667585808464432983200495411090625",
            "to": "c4d3720f66c1423d81f1f287f71c3229c7f1ff5d82d50ab2c3679ffd13630de4",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d8b590da3b03e6f84067ee0c029a39f4f48cfa70fa38f72a210ac478d8d13114",
            "transactiontimestamp": 1661965400,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "b435c66fd1423dba514af2015b43eeceae8bf71f4b201ac379934400b74bc02d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d8b590da3b03e6f84067ee0c029a39f4f48cfa70fa38f72a210ac478d8d13114",
            "transactiontimestamp": 1661965400,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1067753854",
            "amountUSD": "445560287.982962450158747669507464945134418000",
            "to": "b435c66fd1423dba514af2015b43eeceae8bf71f4b201ac379934400b74bc02d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "bbe39a1c78001ca7f3a640aac3af1b63edfd32bf5d43d310de89d1de2723f5e7",
            "transactiontimestamp": 1661965202,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "b435c66fd1423dba514af2015b43eeceae8bf71f4b201ac379934400b74bc02d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "bbe39a1c78001ca7f3a640aac3af1b63edfd32bf5d43d310de89d1de2723f5e7",
            "transactiontimestamp": 1661965202,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1067773037",
            "amountUSD": "445697758.807510266121537795442980523073781000",
            "to": "b435c66fd1423dba514af2015b43eeceae8bf71f4b201ac379934400b74bc02d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "066d97d249feaec5a835db7e74a78f68c65dc013eddc46ddcc00b54d8fad046c",
            "transactiontimestamp": 1661953322,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "573efd90132e73b2c9660403ae286b49d05c3f02e65f8ac52225b99051e87f2a",
            "liquidity": "10000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e32bbe2778704140afaab538796302a6e0d0a286d0a4e59fd586dab706f8ddb6",
            "transactiontimestamp": 1661953116,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "17fe78de725b1c5a8b53b7c91ef62c6824ae73e8b2cb83ec39ddaa1a125ebe66",
            "transactiontimestamp": 1661947331,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "17fe78de725b1c5a8b53b7c91ef62c6824ae73e8b2cb83ec39ddaa1a125ebe66",
            "transactiontimestamp": 1661947331,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "92811414",
            "amountUSD": "27879.30623370815316555444796017282916800",
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "65ea5695efdf09c06f39ba28a15f8631836aad987fdc8a8a78d030a4a8e204f4",
            "transactiontimestamp": 1661945045,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "3053",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "65ea5695efdf09c06f39ba28a15f8631836aad987fdc8a8a78d030a4a8e204f4",
            "transactiontimestamp": 1661945045,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "10000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "65ea5695efdf09c06f39ba28a15f8631836aad987fdc8a8a78d030a4a8e204f4",
            "transactiontimestamp": 1661945045,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "4a2d7b35723a70c69e0f4c01df65df9bf8dced1d1542f11426aed570bcf2cbab",
            "liquidity": "933",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "3d9799e8dbfb0b406ba963057d1f57c907e813a74ee6feb0267221fa638518ba",
            "transactiontimestamp": 1661855017,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "078e9b80cfff8401acdf366f61ec00805bfc470fb07fd5ab75be9f54a24a5984",
            "transactiontimestamp": 1661854770,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "26000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "fbbf61b06b52e18c6aab52aaf60bfd8ee2c4d388b45c4e7e3b349a1d26f0d97b",
            "transactiontimestamp": 1661756151,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "2000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9db400cf3d375aa3c24805ee6e4af15d893a26df9c351e26276466152139f8bd",
            "transactiontimestamp": 1661754630,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "2000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a82eecc8d807a50aa691ad965ffab96065eb9635c47e00835cdde1937bdf298e",
            "transactiontimestamp": 1661754521,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "107633026",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c7cabded6fac101263b895ce7314399005f8057bca22702535e2c8a1ce3fabd6",
            "transactiontimestamp": 1661754407,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5bc1e6079712d0aebd0f4dee1084a95946118becba5c63b6dd73dd40f34db829",
            "transactiontimestamp": 1661754245,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "53733325",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "384076ce6df9a9a3241d4865e2c97ad1d68849c813259c26bf5e6ac623bdccef",
            "transactiontimestamp": 1661588467,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9662842940",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "384076ce6df9a9a3241d4865e2c97ad1d68849c813259c26bf5e6ac623bdccef",
            "transactiontimestamp": 1661588467,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "93380187186",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "384076ce6df9a9a3241d4865e2c97ad1d68849c813259c26bf5e6ac623bdccef",
            "transactiontimestamp": 1661588467,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "dc38b55a5fa3c29aff937dd7373426bc278e188e0f9b64203c83826b1b02f1fd",
            "transactiontimestamp": 1661587518,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "966284295",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "dc38b55a5fa3c29aff937dd7373426bc278e188e0f9b64203c83826b1b02f1fd",
            "transactiontimestamp": 1661587518,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9338018719",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "dc38b55a5fa3c29aff937dd7373426bc278e188e0f9b64203c83826b1b02f1fd",
            "transactiontimestamp": 1661587518,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "5515a684a3096a3ebdccca338da6056544e33d78fe4332e3823d6a0c5af70ea0",
            "transactiontimestamp": 1661586605,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "57155",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "5515a684a3096a3ebdccca338da6056544e33d78fe4332e3823d6a0c5af70ea0",
            "transactiontimestamp": 1661586605,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3307",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "5515a684a3096a3ebdccca338da6056544e33d78fe4332e3823d6a0c5af70ea0",
            "transactiontimestamp": 1661586605,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999963",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "6bcc2698c14c73ab231eaba3678aca0bc97f636094abcae412cded66e894b745",
            "transactiontimestamp": 1661586405,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9662842940",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "6bcc2698c14c73ab231eaba3678aca0bc97f636094abcae412cded66e894b745",
            "transactiontimestamp": 1661586405,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "93380187185",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "6bcc2698c14c73ab231eaba3678aca0bc97f636094abcae412cded66e894b745",
            "transactiontimestamp": 1661586405,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "da5be376e837b82dd763a773da76cbf2dbd7daa779d73e4deff789d91da96387",
            "transactiontimestamp": 1661586140,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "96628429",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "da5be376e837b82dd763a773da76cbf2dbd7daa779d73e4deff789d91da96387",
            "transactiontimestamp": 1661586140,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "933801872",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "da5be376e837b82dd763a773da76cbf2dbd7daa779d73e4deff789d91da96387",
            "transactiontimestamp": 1661586140,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "497e2ea4a0ab78990754ef52c725ac4c9bafcfc57508b1a398b7f76090556a87",
            "transactiontimestamp": 1661585974,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "51555b3f6d6ef85287d8a7adcb7f2e4f91391d11495e40cad120dec42ab1698c",
            "transactiontimestamp": 1661585781,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "078fd990d178fac602da83f4ae02147f90c64d276db9b7f4fa9e864d3a91aefe",
            "transactiontimestamp": 1661584850,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "305551011864",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "078fd990d178fac602da83f4ae02147f90c64d276db9b7f4fa9e864d3a91aefe",
            "transactiontimestamp": 1661584850,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "078fd990d178fac602da83f4ae02147f90c64d276db9b7f4fa9e864d3a91aefe",
            "transactiontimestamp": 1661584850,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "93371064902",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c099bb9b06e884510989a5865e377d07398168c1ebdde2d8e83e9764c7a9f981",
            "transactiontimestamp": 1659523968,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c099bb9b06e884510989a5865e377d07398168c1ebdde2d8e83e9764c7a9f981",
            "transactiontimestamp": 1659523968,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9319539674",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "3858967677.691237296063399268",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "72331d36d740df23a13bb310b44aaf7f851311504e5dfad78ed7845d7f654b2c",
            "transactiontimestamp": 1659523835,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3058653378",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "72331d36d740df23a13bb310b44aaf7f851311504e5dfad78ed7845d7f654b2c",
            "transactiontimestamp": 1659523835,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "72331d36d740df23a13bb310b44aaf7f851311504e5dfad78ed7845d7f654b2c",
            "transactiontimestamp": 1659523835,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "935629804",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "4e9b5e03556a5ce0ed78088ea7be8a889e5ef9dfcbd8f5a1c9f70857d94a0841",
            "transactiontimestamp": 1659523553,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "30586533811",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "4e9b5e03556a5ce0ed78088ea7be8a889e5ef9dfcbd8f5a1c9f70857d94a0841",
            "transactiontimestamp": 1659523553,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "4e9b5e03556a5ce0ed78088ea7be8a889e5ef9dfcbd8f5a1c9f70857d94a0841",
            "transactiontimestamp": 1659523553,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9356298049",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "ca132732acd713484ec39d03be5e1f3cd684e96fc5a893115571044a2e4219a8",
            "transactiontimestamp": 1658325232,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "306152214",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "ca132732acd713484ec39d03be5e1f3cd684e96fc5a893115571044a2e4219a8",
            "transactiontimestamp": 1658325232,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "ca132732acd713484ec39d03be5e1f3cd684e96fc5a893115571044a2e4219a8",
            "transactiontimestamp": 1658325232,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "93738308",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0beb4001b2266015cc1bcf2bbd4a2bed9a3532b332c90ddcd28efd9d9f0704f6",
            "transactiontimestamp": 1656340132,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "50000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "0beb4001b2266015cc1bcf2bbd4a2bed9a3532b332c90ddcd28efd9d9f0704f6",
            "transactiontimestamp": 1656340132,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2385246327",
            "amount1In": "50000000000",
            "amount1Out": "0",
            "amountUSD": "1903152271.84630022820865471862847389912880684",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "38e547eba7e509942e0de0db77a1e69e71e10f004b63e27a0abafb97d8eb43c2",
            "transactiontimestamp": 1656336506,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "liquidity": "2453300718",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "38e547eba7e509942e0de0db77a1e69e71e10f004b63e27a0abafb97d8eb43c2",
            "transactiontimestamp": 1656336506,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "liquidity": "605904241",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "38e547eba7e509942e0de0db77a1e69e71e10f004b63e27a0abafb97d8eb43c2",
            "transactiontimestamp": 1656336506,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "03618fad91c99c0cedc772271c8b035487e2da82077f83ba2dbf4cc610a3250f",
            "transactiontimestamp": 1656335816,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "liquidity": "2453300718",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "03618fad91c99c0cedc772271c8b035487e2da82077f83ba2dbf4cc610a3250f",
            "transactiontimestamp": 1656335816,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "liquidity": "605904241",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "03618fad91c99c0cedc772271c8b035487e2da82077f83ba2dbf4cc610a3250f",
            "transactiontimestamp": 1656335816,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "c933617365ea0453e5588ad7a285a936b763ee4268ce84d2c23ffba68a0bcaac",
            "transactiontimestamp": 1656201441,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "liquidity": "2453300718",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "c933617365ea0453e5588ad7a285a936b763ee4268ce84d2c23ffba68a0bcaac",
            "transactiontimestamp": 1656201441,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "liquidity": "605904241",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "c933617365ea0453e5588ad7a285a936b763ee4268ce84d2c23ffba68a0bcaac",
            "transactiontimestamp": 1656201441,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "294f1f619fec0c09100621a112131ccab08b64952dae670deff2185674b0a01f",
            "transactiontimestamp": 1655832322,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "294f1f619fec0c09100621a112131ccab08b64952dae670deff2185674b0a01f",
            "transactiontimestamp": 1655832322,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "645126046",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "272053636.863761454186363550",
            "to": "8922065798095a518c1ef68682419e05353cf40dda33f70ba92369c75e3e369c",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c58602b2a6db7a9b6a2e066c1fc67cdeaceaceefc192734f308c077e3f7a3cb7",
            "transactiontimestamp": 1655826585,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c58602b2a6db7a9b6a2e066c1fc67cdeaceaceefc192734f308c077e3f7a3cb7",
            "transactiontimestamp": 1655826585,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "739029213",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "270047539.458947200460983437",
            "to": "8922065798095a518c1ef68682419e05353cf40dda33f70ba92369c75e3e369c",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ed5e5349d0e4b126dafdcc98164fff5e7e8478a263feaab2474ed10c23548161",
            "transactiontimestamp": 1655826123,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ed5e5349d0e4b126dafdcc98164fff5e7e8478a263feaab2474ed10c23548161",
            "transactiontimestamp": 1655826123,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "855057849",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "272802133.875545028618550188",
            "to": "8922065798095a518c1ef68682419e05353cf40dda33f70ba92369c75e3e369c",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "292b956ff2a784fea26b18d2015499bbcd269477bd6c27a250dfd21c534c9ab5",
            "transactiontimestamp": 1655825807,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "292b956ff2a784fea26b18d2015499bbcd269477bd6c27a250dfd21c534c9ab5",
            "transactiontimestamp": 1655825807,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "1000757884",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "274394430.597921098595922151",
            "to": "8922065798095a518c1ef68682419e05353cf40dda33f70ba92369c75e3e369c",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "60bf0b40216a9f691dafde9d30bfcc891ca5438c2974143f7a9c22f18b6347f8",
            "transactiontimestamp": 1655825723,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "12000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "60bf0b40216a9f691dafde9d30bfcc891ca5438c2974143f7a9c22f18b6347f8",
            "transactiontimestamp": 1655825723,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "1451716575",
            "amount1In": "12000000000",
            "amount1Out": "0",
            "amountUSD": "333665352.350514298859397064",
            "to": "8922065798095a518c1ef68682419e05353cf40dda33f70ba92369c75e3e369c",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b35743cc0c0185491f7b66a01cb9b00d595e8fa312f38f15cb78401f2a7786e9",
            "transactiontimestamp": 1654595958,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "b35743cc0c0185491f7b66a01cb9b00d595e8fa312f38f15cb78401f2a7786e9",
            "transactiontimestamp": 1654595958,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "2385238566",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "8922065798095a518c1ef68682419e05353cf40dda33f70ba92369c75e3e369c",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "874f40eabfc8d620880912dc8d60604e4f48f21f86c3089d51bab482ad29b044",
            "transactiontimestamp": 1654594297,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "11000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "874f40eabfc8d620880912dc8d60604e4f48f21f86c3089d51bab482ad29b044",
            "transactiontimestamp": 1654594297,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "3494387704",
            "amount1In": "11000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "33bc07a0e9aeea61cc62bdbeb32245dc1194bb2d69755f1af7fb945f29ee3606",
            "transactiontimestamp": 1654594120,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "11000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "33bc07a0e9aeea61cc62bdbeb32245dc1194bb2d69755f1af7fb945f29ee3606",
            "transactiontimestamp": 1654594120,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "4965013249",
            "amount1In": "11000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "acb627f7e218c72a6449a71a7e2d26ffe9b2834948987f8d459c632b97eec679",
            "transactiontimestamp": 1654593751,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "acb627f7e218c72a6449a71a7e2d26ffe9b2834948987f8d459c632b97eec679",
            "transactiontimestamp": 1654593751,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "6756443682",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "bd1cd09b025e484c450a06d3c6c4f2b093223db0dfd00bcc36eaf07c79b5b376",
            "transactiontimestamp": 1654593638,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "bd1cd09b025e484c450a06d3c6c4f2b093223db0dfd00bcc36eaf07c79b5b376",
            "transactiontimestamp": 1654593638,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "10947179042",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6748fb6fba8043e3f4e037d178b7e8e91d0cc80e98fb60f3cc4866fe7db2d3f1",
            "transactiontimestamp": 1654593543,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6748fb6fba8043e3f4e037d178b7e8e91d0cc80e98fb60f3cc4866fe7db2d3f1",
            "transactiontimestamp": 1654593543,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "20796349762",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2cdb098aa73db16f692d430c165ca7f0297c5e72df703727548dfaf7e36e865a",
            "transactiontimestamp": 1654593450,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2cdb098aa73db16f692d430c165ca7f0297c5e72df703727548dfaf7e36e865a",
            "transactiontimestamp": 1654593450,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "54847910025",
            "amount1In": "10000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "08f891d59e53093ce4d3dc8a1d4c8d9093c4b85f6eae7858636935a77acf0199",
            "transactiontimestamp": 1654593248,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "99",
            "amount1In": "10",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "08f891d59e53093ce4d3dc8a1d4c8d9093c4b85f6eae7858636935a77acf0199",
            "transactiontimestamp": 1654593248,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4f0aa42c0b0a7bf0f9bc79066f6715fcaecacc582c8536831072169e3d6f5c2d",
            "transactiontimestamp": 1654249895,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4f0aa42c0b0a7bf0f9bc79066f6715fcaecacc582c8536831072169e3d6f5c2d",
            "transactiontimestamp": 1654249895,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "99",
            "amount1In": "10",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d5679a49e31b238e7524a0589f92b05d3b07caf7327378b5f76fc5348800a743",
            "transactiontimestamp": 1654249445,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d5679a49e31b238e7524a0589f92b05d3b07caf7327378b5f76fc5348800a743",
            "transactiontimestamp": 1654249445,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "99",
            "amount1In": "10",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "88143b1c48db33654a49b8155744d3da9bd78f1c70a93c2eed938e45c32c5e99",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a90b18286c1bdebb3e85de98da2ac7f320cd208917036b2cbe0efe7e3758a4ae",
            "transactiontimestamp": 1652974092,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "3010530018",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a90b18286c1bdebb3e85de98da2ac7f320cd208917036b2cbe0efe7e3758a4ae",
            "transactiontimestamp": 1652974092,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "3010530018",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "65114b0b1f8ce2cf847fc8392094a167fbfe2b7bc3b01a105b39d6a7551ca680",
            "transactiontimestamp": 1652973966,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "3010530018",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "65114b0b1f8ce2cf847fc8392094a167fbfe2b7bc3b01a105b39d6a7551ca680",
            "transactiontimestamp": 1652973966,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "30000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "65114b0b1f8ce2cf847fc8392094a167fbfe2b7bc3b01a105b39d6a7551ca680",
            "transactiontimestamp": 1652973966,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "302112978",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "15abdb201894f6483974c10331d8f95f260077de179898d192d1386120344a9a",
            "transactiontimestamp": 1652973857,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10099703",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "15abdb201894f6483974c10331d8f95f260077de179898d192d1386120344a9a",
            "transactiontimestamp": 1652973857,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "10099703",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1000000000",
            "amountUSD": "0",
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b008fe9f13c5341cccb4ce37b2cbd944063ddafcc456dd6807e0b59b69b2d690",
            "transactiontimestamp": 1652897220,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "1904654041",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b008fe9f13c5341cccb4ce37b2cbd944063ddafcc456dd6807e0b59b69b2d690",
            "transactiontimestamp": 1652897220,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "1904654041",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "1e7d8df9e096b7ef84d79dacf45fe69134fbe7d3aa644ee14712d61972af818a",
            "transactiontimestamp": 1652897015,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "1003407755",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1e7d8df9e096b7ef84d79dacf45fe69134fbe7d3aa644ee14712d61972af818a",
            "transactiontimestamp": 1652897015,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1e7d8df9e096b7ef84d79dacf45fe69134fbe7d3aa644ee14712d61972af818a",
            "transactiontimestamp": 1652897015,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100683774",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "388e42b5c6ddce8d39ae5276cc4caf7c2cdba7dd2a330c70f3de0d3e3aa9fe08",
            "transactiontimestamp": 1652896819,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "388e42b5c6ddce8d39ae5276cc4caf7c2cdba7dd2a330c70f3de0d3e3aa9fe08",
            "transactiontimestamp": 1652896819,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "9912312928",
            "amountUSD": "0",
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5bb5ad51ed1f21b1990c3bf8dbbd6ee3d7322871b54fd4feef36b74eeccd77c5",
            "transactiontimestamp": 1652895349,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5bb5ad51ed1f21b1990c3bf8dbbd6ee3d7322871b54fd4feef36b74eeccd77c5",
            "transactiontimestamp": 1652895349,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "9932367856",
            "amountUSD": "0",
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "25513f0fa3bc08113a35f719350f33ba3902d15fb1cbc8377764ef454f6d991f",
            "transactiontimestamp": 1652894848,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "9000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "25513f0fa3bc08113a35f719350f33ba3902d15fb1cbc8377764ef454f6d991f",
            "transactiontimestamp": 1652894848,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "90249834",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "25513f0fa3bc08113a35f719350f33ba3902d15fb1cbc8377764ef454f6d991f",
            "transactiontimestamp": 1652894848,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "liquidity": "901246286",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "98946e3d2580aa6aadf2d1516587022344bad832644553e5932dcd629a79de9d",
            "transactiontimestamp": 1652894531,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "98946e3d2580aa6aadf2d1516587022344bad832644553e5932dcd629a79de9d",
            "transactiontimestamp": 1652894531,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "9952492977",
            "amountUSD": "0",
            "to": "eee535092500bbb5beb8ef2a421d957dfb35894742eceac615f0aa88c83ec53b",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "51a75226dd75339250e49f0fdd507035c30b215fb517cfbfade1c4456fc7c8e5",
            "transactiontimestamp": 1652891649,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "51a75226dd75339250e49f0fdd507035c30b215fb517cfbfade1c4456fc7c8e5",
            "transactiontimestamp": 1652891649,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "99925430073",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "51a75226dd75339250e49f0fdd507035c30b215fb517cfbfade1c4456fc7c8e5",
            "transactiontimestamp": 1652891649,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9996263650",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5254b5d95304dd65019afc3e240ad7926b05f0afdb8640c7d8fbc601909fc81f",
            "transactiontimestamp": 1652885793,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "liquidity": "153075",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5254b5d95304dd65019afc3e240ad7926b05f0afdb8640c7d8fbc601909fc81f",
            "transactiontimestamp": 1652885793,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
            "liquidity": "153075",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "f2006f78a386a75413979c07821eb787e78514a1a25d4b42da5303b6dae7f5cc",
            "transactiontimestamp": 1652885503,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
            "liquidity": "617632355",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "f2006f78a386a75413979c07821eb787e78514a1a25d4b42da5303b6dae7f5cc",
            "transactiontimestamp": 1652885503,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "617632355",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0b433113ddf67e2cc24863c4fa11990126a7d671bb235c91ed87acadd7e53e16",
            "transactiontimestamp": 1652885226,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "5115713318",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "57c1392769294496906ee545f7fe71e545499329cd736ab3e8fd18005e1a7c04",
            "transactiontimestamp": 1652885079,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "liquidity": "15810",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "57c1392769294496906ee545f7fe71e545499329cd736ab3e8fd18005e1a7c04",
            "transactiontimestamp": 1652885079,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
            "liquidity": "15810",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "048860dd62836f50d05802e462627810b55bdfbae6fce26fc00a3a8fb8616d5c",
            "transactiontimestamp": 1652884332,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "liquidity": "99984",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "048860dd62836f50d05802e462627810b55bdfbae6fce26fc00a3a8fb8616d5c",
            "transactiontimestamp": 1652884332,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "048860dd62836f50d05802e462627810b55bdfbae6fce26fc00a3a8fb8616d5c",
            "transactiontimestamp": 1652884332,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "liquidity": "31620",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "d4d52358815db1ef3836d797d1373d8d06c218681c166a0677885ddba03213b7",
            "transactiontimestamp": 1652884072,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "liquidity": "306151",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "d4d52358815db1ef3836d797d1373d8d06c218681c166a0677885ddba03213b7",
            "transactiontimestamp": 1652884072,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "liquidity": "1000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b3f6f00f3862f2b4f936b904bef7d3c2374e7f50d0637c8ddb4ef57890a77c66",
            "transactiontimestamp": 1652883840,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "b3f6f00f3862f2b4f936b904bef7d3c2374e7f50d0637c8ddb4ef57890a77c66",
            "transactiontimestamp": 1652883840,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9969197",
            "amount1In": "1000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "75b2dd2792c3e56d7c5e3e85ca86c2e0e3d1f3071eac567ce738375692aa7b4b",
            "transactiontimestamp": 1652883733,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "75b2dd2792c3e56d7c5e3e85ca86c2e0e3d1f3071eac567ce738375692aa7b4b",
            "transactiontimestamp": 1652883733,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "9962575",
            "amountUSD": "0",
            "to": "2a46defb1d46d6a16b19ab12eb7c8d5adec9893b31c03a01fb56c68fab01093f",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b55a6dfb84cef4b5b835283577c09902f60f2eae9c1d6040216d956f056a1e77",
            "transactiontimestamp": 1652882762,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9373830819",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "b55a6dfb84cef4b5b835283577c09902f60f2eae9c1d6040216d956f056a1e77",
            "transactiontimestamp": 1652882762,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "30615221487",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b55a6dfb84cef4b5b835283577c09902f60f2eae9c1d6040216d956f056a1e77",
            "transactiontimestamp": 1652882762,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5593032c0f2540e2897e0834dec511ca4877b7a6f732e7aba18d23533ce9600c",
            "transactiontimestamp": 1652882505,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10231426636",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5593032c0f2540e2897e0834dec511ca4877b7a6f732e7aba18d23533ce9600c",
            "transactiontimestamp": 1652882505,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "10231426636",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "eb01c963de8fdcf517959f153b16ab0976ae96a22a0ba300a8a1ea15c39f72e7",
            "transactiontimestamp": 1652882325,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "99925633644",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "eb01c963de8fdcf517959f153b16ab0976ae96a22a0ba300a8a1ea15c39f72e7",
            "transactiontimestamp": 1652882325,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "eb01c963de8fdcf517959f153b16ab0976ae96a22a0ba300a8a1ea15c39f72e7",
            "transactiontimestamp": 1652882325,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "CSX",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9996273838",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "31d21f4844b594309f153f579fc8b2fbf1ee0ca2766f75362e813bc0312e2df9",
            "transactiontimestamp": 1650998657,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "31d21f4844b594309f153f579fc8b2fbf1ee0ca2766f75362e813bc0312e2df9",
            "transactiontimestamp": 1650998657,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9371561025",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "deb12beda206fea3857185dcae8e16ae09a677f5972034d636ae695b89a5a304",
            "transactiontimestamp": 1650998521,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "97000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "deb12beda206fea3857185dcae8e16ae09a677f5972034d636ae695b89a5a304",
            "transactiontimestamp": 1650998521,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9107264624",
            "amount1In": "97000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "447ff60830a0501095f0759d4155ece219829f31b772d63745f1f413236692f0",
            "transactiontimestamp": 1650998337,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "96000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "447ff60830a0501095f0759d4155ece219829f31b772d63745f1f413236692f0",
            "transactiontimestamp": 1650998337,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9029758752",
            "amount1In": "96000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d9bd9a67e4b1edb32ae37dccc6d0ec9207df32514594fb48bfba814e6d93d353",
            "transactiontimestamp": 1650998156,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "d9bd9a67e4b1edb32ae37dccc6d0ec9207df32514594fb48bfba814e6d93d353",
            "transactiontimestamp": 1650998156,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9423378639",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "625f7aa719a9433b615229ffe25e7805f52d5d8ae2ec07d708a88bddd0a1e0f4",
            "transactiontimestamp": 1650985586,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "87000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "625f7aa719a9433b615229ffe25e7805f52d5d8ae2ec07d708a88bddd0a1e0f4",
            "transactiontimestamp": 1650985586,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "8212802234",
            "amount1In": "87000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "568e89719c1f4517fa04d0cf5d1ba966e9927ac781cd29f4bc7e102a1878fb95",
            "transactiontimestamp": 1650919613,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "95000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "568e89719c1f4517fa04d0cf5d1ba966e9927ac781cd29f4bc7e102a1878fb95",
            "transactiontimestamp": 1650919613,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "8983416484",
            "amount1In": "95000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2aadce1732341028ee4d72055ac508b04682848f74bafe2bcb9a9dcd2c1f37a3",
            "transactiontimestamp": 1650919534,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "94457120297",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2aadce1732341028ee4d72055ac508b04682848f74bafe2bcb9a9dcd2c1f37a3",
            "transactiontimestamp": 1650919534,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "995000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "2aadce1732341028ee4d72055ac508b04682848f74bafe2bcb9a9dcd2c1f37a3",
            "transactiontimestamp": 1650919534,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "306557444005",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2bab385742f9b8cf8d78304597db5a630be54bf433650084de71b83d06e478fa",
            "transactiontimestamp": 1650919374,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2bab385742f9b8cf8d78304597db5a630be54bf433650084de71b83d06e478fa",
            "transactiontimestamp": 1650919374,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9473743216",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e7edce2791b384dfdedb2134cdb4a944f2c0db95d04bfc676849a43c82203247",
            "transactiontimestamp": 1650919215,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "97000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "e7edce2791b384dfdedb2134cdb4a944f2c0db95d04bfc676849a43c82203247",
            "transactiontimestamp": 1650919215,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9206820887",
            "amount1In": "97000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0f569b0c7cbe854cfe5c647b38b08d7a5050d4db52a6b0259d52f395f8aee2bc",
            "transactiontimestamp": 1650573878,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "0f569b0c7cbe854cfe5c647b38b08d7a5050d4db52a6b0259d52f395f8aee2bc",
            "transactiontimestamp": 1650573878,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9509444086",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "504e9340915cceb30359d4008d97368af30419a03eb722aff0153c73ff770aa5",
            "transactiontimestamp": 1650553710,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "504e9340915cceb30359d4008d97368af30419a03eb722aff0153c73ff770aa5",
            "transactiontimestamp": 1650553710,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9527643662",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "640f2ff26c66e53eb09f778a446beb17ab79d9af744c99b2a067028ae46eacf8",
            "transactiontimestamp": 1650544604,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "99927464720",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "640f2ff26c66e53eb09f778a446beb17ab79d9af744c99b2a067028ae46eacf8",
            "transactiontimestamp": 1650544604,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "640f2ff26c66e53eb09f778a446beb17ab79d9af744c99b2a067028ae46eacf8",
            "transactiontimestamp": 1650544604,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9996365596",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9863bf082f694e2cf74366e0f5cb8d56887120d4d1a6e4b8e2597c95c837ba17",
            "transactiontimestamp": 1650544437,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "95654435003",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "9863bf082f694e2cf74366e0f5cb8d56887120d4d1a6e4b8e2597c95c837ba17",
            "transactiontimestamp": 1650544437,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "9863bf082f694e2cf74366e0f5cb8d56887120d4d1a6e4b8e2597c95c837ba17",
            "transactiontimestamp": 1650544437,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "309270148944",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "186a5715287ea05303bcb40c5934cb9d9d85d3cca2b85ced11a3962637c75bf4",
            "transactiontimestamp": 1650544212,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "50000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "186a5715287ea05303bcb40c5934cb9d9d85d3cca2b85ced11a3962637c75bf4",
            "transactiontimestamp": 1650544212,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "50000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "4981621",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e761126ce3a40dc5d1d73868b0a6d85654a2f1b8d61070b2b69385f6a633124b",
            "transactiontimestamp": 1650538595,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
            "liquidity": "1235264710",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e761126ce3a40dc5d1d73868b0a6d85654a2f1b8d61070b2b69385f6a633124b",
            "transactiontimestamp": 1650538595,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1235264710",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "bee7e240747b11e831bdc1aaf87b4d6d12a46d9ae3f807dd0aefa2c115f726bf",
            "transactiontimestamp": 1650538490,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "470213839",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "bee7e240747b11e831bdc1aaf87b4d6d12a46d9ae3f807dd0aefa2c115f726bf",
            "transactiontimestamp": 1650538490,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "470213839",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6b31b3d2fae7a67231131b92b6db3564de1cffbdb2a45940781df77841f52548",
            "transactiontimestamp": 1650538324,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "940427678",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6b31b3d2fae7a67231131b92b6db3564de1cffbdb2a45940781df77841f52548",
            "transactiontimestamp": 1650538324,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "940427678",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a26782917d36af8be5618779d64d1dbea3f57e37181ad78cc1532269ad749c1c",
            "transactiontimestamp": 1650538200,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1880855355",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a26782917d36af8be5618779d64d1dbea3f57e37181ad78cc1532269ad749c1c",
            "transactiontimestamp": 1650538200,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "1880855355",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7295bdce779b0fdf8a49ae8d87e6999f7430d805e032269df50681ab51ca7af5",
            "transactiontimestamp": 1650535658,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3761710711",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "7295bdce779b0fdf8a49ae8d87e6999f7430d805e032269df50681ab51ca7af5",
            "transactiontimestamp": 1650535658,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "3761710711",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b533e23348c5308cf1dd01acaefd0df1d7df379deaf47f8686d6a104764d841a",
            "transactiontimestamp": 1650535232,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "7523421422",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b533e23348c5308cf1dd01acaefd0df1d7df379deaf47f8686d6a104764d841a",
            "transactiontimestamp": 1650535232,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "7523421422",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8cafb6c15faa3138361643845907fdde3b8dfa94e6703ad7ae869bfef5eb6a6b",
            "transactiontimestamp": 1650533311,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "2470529419",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8cafb6c15faa3138361643845907fdde3b8dfa94e6703ad7ae869bfef5eb6a6b",
            "transactiontimestamp": 1650533311,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
            "liquidity": "2470529419",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4567a2574e01204b5cf5d3acdb80ea2c4cdd3889b10c5955e4402749582f81bf",
            "transactiontimestamp": 1650529503,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9999999994",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4567a2574e01204b5cf5d3acdb80ea2c4cdd3889b10c5955e4402749582f81bf",
            "transactiontimestamp": 1650529503,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "999999999",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "4567a2574e01204b5cf5d3acdb80ea2c4cdd3889b10c5955e4402749582f81bf",
            "transactiontimestamp": 1650529503,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3162277654",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c7f933d16a2753e8ad1d2c7e173429440feae0a4df9dc1e9bcd063619d37505c",
            "transactiontimestamp": 1650529301,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "99936991761",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "c7f933d16a2753e8ad1d2c7e173429440feae0a4df9dc1e9bcd063619d37505c",
            "transactiontimestamp": 1650529301,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9996842844",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c7f933d16a2753e8ad1d2c7e173429440feae0a4df9dc1e9bcd063619d37505c",
            "transactiontimestamp": 1650529301,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4b8cba6555e01abeee9a4612e6079d72e193f4756cf6b215a45952a694dd05db",
            "transactiontimestamp": 1650529059,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4b8cba6555e01abeee9a4612e6079d72e193f4756cf6b215a45952a694dd05db",
            "transactiontimestamp": 1650529059,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "9964379",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e347222d41ee828833e680e717407afb841497cf15cca5b873619d071d512c5a",
            "transactiontimestamp": 1650528972,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "e347222d41ee828833e680e717407afb841497cf15cca5b873619d071d512c5a",
            "transactiontimestamp": 1650528972,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "95368394",
            "amount1In": "1000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5c160a12b131b579eee3ab239f5259ecc0f16924098a1352ab1d46263c326293",
            "transactiontimestamp": 1650494843,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "98000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5c160a12b131b579eee3ab239f5259ecc0f16924098a1352ab1d46263c326293",
            "transactiontimestamp": 1650494843,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9355064128",
            "amount1In": "98000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4c33957624c2299d31ae802fee49d650404557755a5be0af7b31393aa2ae9a08",
            "transactiontimestamp": 1650494632,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "97000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "4c33957624c2299d31ae802fee49d650404557755a5be0af7b31393aa2ae9a08",
            "transactiontimestamp": 1650494632,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9277082883",
            "amount1In": "97000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c8162a8667a3ced90d8c0b36bad60ea94e2ffb96d1cff4b13a73299fd7c55943",
            "transactiontimestamp": 1650493478,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c8162a8667a3ced90d8c0b36bad60ea94e2ffb96d1cff4b13a73299fd7c55943",
            "transactiontimestamp": 1650493478,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9582259571",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "99381e7ca05c559b765553eaaad7e4d10c78566ac16fc48f9cef90a2d7e94660",
            "transactiontimestamp": 1650492729,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "93000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "99381e7ca05c559b765553eaaad7e4d10c78566ac16fc48f9cef90a2d7e94660",
            "transactiontimestamp": 1650492729,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "8928180810",
            "amount1In": "93000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6963ae16977350f0e7d6b19badb1b6c59872ad89d62df3ddfe7a700754f4a176",
            "transactiontimestamp": 1650492584,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "97000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6963ae16977350f0e7d6b19badb1b6c59872ad89d62df3ddfe7a700754f4a176",
            "transactiontimestamp": 1650492584,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9329364688",
            "amount1In": "97000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "98e04bb56885e5591c71049fd5086978310dad1c1b4aa009c992229aa2f68317",
            "transactiontimestamp": 1650491982,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "98e04bb56885e5591c71049fd5086978310dad1c1b4aa009c992229aa2f68317",
            "transactiontimestamp": 1650491982,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9636313038",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "448642e8361e711c76d022af09a5f99367c2a4223645e0f773c391a7b37d4f43",
            "transactiontimestamp": 1650491752,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "448642e8361e711c76d022af09a5f99367c2a4223645e0f773c391a7b37d4f43",
            "transactiontimestamp": 1650491752,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9655058306",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b0ec07d611a490249bd2a924b38e2c4bd229721591a489003517f60777b83030",
            "transactiontimestamp": 1650491579,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "96000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "b0ec07d611a490249bd2a924b38e2c4bd229721591a489003517f60777b83030",
            "transactiontimestamp": 1650491579,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9286541825",
            "amount1In": "96000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "2b277d146b4f639f04d385108224d9b65e2376c544702f8bdbbbf14ee430e11b",
            "transactiontimestamp": 1650491304,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "2b277d146b4f639f04d385108224d9b65e2376c544702f8bdbbbf14ee430e11b",
            "transactiontimestamp": 1650491304,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9691958129",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e606250f87aa1d805b3107df61ac1ac078591280ff0df79cfc03e6b6d76ceca9",
            "transactiontimestamp": 1650491086,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "e606250f87aa1d805b3107df61ac1ac078591280ff0df79cfc03e6b6d76ceca9",
            "transactiontimestamp": 1650491086,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9710866160",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "abe5c45c5b74c14ede6a3c02faf7b24895c5005a46f081d3999e366fd5298667",
            "transactiontimestamp": 1650490395,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "abe5c45c5b74c14ede6a3c02faf7b24895c5005a46f081d3999e366fd5298667",
            "transactiontimestamp": 1650490395,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9729829604",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "84001ee85113d15ef9d8d9efbbb2fb08a9110f2348cffb3be6ec82d6b2f49c0a",
            "transactiontimestamp": 1650466255,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "84001ee85113d15ef9d8d9efbbb2fb08a9110f2348cffb3be6ec82d6b2f49c0a",
            "transactiontimestamp": 1650466255,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9748848679",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "14fc7b9175446ab17e5ccbb92c8e0fe35eab042dedf25357ea05c33b79ddfa90",
            "transactiontimestamp": 1650466119,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "14fc7b9175446ab17e5ccbb92c8e0fe35eab042dedf25357ea05c33b79ddfa90",
            "transactiontimestamp": 1650466119,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9767923602",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "cfa15303da2addc04ca05556f7b919559ee4fde09b4ae4d1a64285c02a286e8a",
            "transactiontimestamp": 1650458459,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "5050000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "cfa15303da2addc04ca05556f7b919559ee4fde09b4ae4d1a64285c02a286e8a",
            "transactiontimestamp": 1650458459,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "a84382872d1402a5ec8d8453f516586166100d8252f997b0bcdeed8c4737588d",
            "liquidity": "5050000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e240d4304086978063c4dcbfb804ddadc075c2e3152e029671d6efec62ebbb8d",
            "transactiontimestamp": 1650458031,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "592927061",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "e240d4304086978063c4dcbfb804ddadc075c2e3152e029671d6efec62ebbb8d",
            "transactiontimestamp": 1650458031,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
            "liquidity": "592927061",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "69cd751780513d8936567d9184d4a4bd397cfbe2f42d97a81656fed334248251",
            "transactiontimestamp": 1650456478,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "cb0f9f291ae73928b739c90c03eca70cd610d945304ea606fe4adced3fa07060",
            "liquidity": "790569414",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "69cd751780513d8936567d9184d4a4bd397cfbe2f42d97a81656fed334248251",
            "transactiontimestamp": 1650456478,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "790569414",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a6449e733f4a386de7d6530bc5249a852b12c5636ca9e1907c5f7a7d14cf6b7f",
            "transactiontimestamp": 1650455182,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "100000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a6449e733f4a386de7d6530bc5249a852b12c5636ca9e1907c5f7a7d14cf6b7f",
            "transactiontimestamp": 1650455182,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "9965535",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1788f781040b78bf831e9644a06a667e500e5adafd331eeb6979e44d03e82322",
            "transactiontimestamp": 1650454818,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1788f781040b78bf831e9644a06a667e500e5adafd331eeb6979e44d03e82322",
            "transactiontimestamp": 1650454818,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "1788f781040b78bf831e9644a06a667e500e5adafd331eeb6979e44d03e82322",
            "transactiontimestamp": 1650454818,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3162277660",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "340be8f316763477c0a5c2ca0fab2953f1b38e50f2ac6ba84d4d9823cd31b525",
            "transactiontimestamp": 1650451479,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10025596",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "340be8f316763477c0a5c2ca0fab2953f1b38e50f2ac6ba84d4d9823cd31b525",
            "transactiontimestamp": 1650451479,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "100000",
            "amount1In": "10025596",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a3eb064b507dc5efbfa8e0ee4b9c0b82b7a4254de98abf25a11504003abf7d7f",
            "transactiontimestamp": 1650451347,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "a3eb064b507dc5efbfa8e0ee4b9c0b82b7a4254de98abf25a11504003abf7d7f",
            "transactiontimestamp": 1650451347,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "997",
            "amount1In": "100000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "fe667fbd806294f4a4822dde10a760d4ed4e98bef8913a12742f91450d0f7d94",
            "transactiontimestamp": 1650451131,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1115",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "fe667fbd806294f4a4822dde10a760d4ed4e98bef8913a12742f91450d0f7d94",
            "transactiontimestamp": 1650451131,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1115",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "111100",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c920cedc1d0f5523304092e586857904c55787e0389468254fceb89de9e34357",
            "transactiontimestamp": 1650449800,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1115",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "c920cedc1d0f5523304092e586857904c55787e0389468254fceb89de9e34357",
            "transactiontimestamp": 1650449800,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "1115",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "111100",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "09b5238b5e4871611d599e7595c75fdbc833a0d17a73c6d5f305a88902f6f712",
            "transactiontimestamp": 1650449693,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "500000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "09b5238b5e4871611d599e7595c75fdbc833a0d17a73c6d5f305a88902f6f712",
            "transactiontimestamp": 1650449693,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "500000",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "49837639",
            "amountUSD": "0",
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "1aa735da06e80b12df4adb6d8332ea385c9ec347146ec1356b42333bd5c00979",
            "transactiontimestamp": 1650448804,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1aa735da06e80b12df4adb6d8332ea385c9ec347146ec1356b42333bd5c00979",
            "transactiontimestamp": 1650448804,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1aa735da06e80b12df4adb6d8332ea385c9ec347146ec1356b42333bd5c00979",
            "transactiontimestamp": 1650448804,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "b9be46f9919a4896c1356a3fdc80be6d998a9f372364d598d15becabc21d9fa9",
            "transactiontimestamp": 1650448254,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b9be46f9919a4896c1356a3fdc80be6d998a9f372364d598d15becabc21d9fa9",
            "transactiontimestamp": 1650448254,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b9be46f9919a4896c1356a3fdc80be6d998a9f372364d598d15becabc21d9fa9",
            "transactiontimestamp": 1650448254,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "ea048572fa8c13b56b58d512d9f3757823e42b74ad3273812ead895df6474d9d",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "27387ee3897daf4d326b304f0a5b59e3b6f3f8f060da032859c3a9e6ada23cc2",
            "transactiontimestamp": 1650378927,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "27387ee3897daf4d326b304f0a5b59e3b6f3f8f060da032859c3a9e6ada23cc2",
            "transactiontimestamp": 1650378927,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9787054591",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6d7521857112b232f8eb560b120241b6d5ec004368312e1423c7d655271aa8cf",
            "transactiontimestamp": 1650349059,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3291350726",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6d7521857112b232f8eb560b120241b6d5ec004368312e1423c7d655271aa8cf",
            "transactiontimestamp": 1650349059,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
            "liquidity": "3291350726",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d037ec6f0a65c9374de82062ad2360a548e9f7282220dfc84e9b44f72279f19d",
            "transactiontimestamp": 1650348889,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "982610273",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "d037ec6f0a65c9374de82062ad2360a548e9f7282220dfc84e9b44f72279f19d",
            "transactiontimestamp": 1650348889,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3134619740",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d037ec6f0a65c9374de82062ad2360a548e9f7282220dfc84e9b44f72279f19d",
            "transactiontimestamp": 1650348889,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "9999999998",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "17ee92bb87ef4405c0694aeaf99aba86b2abb14b44bceb3906ce0c3d6086b15b",
            "transactiontimestamp": 1650348781,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "17ee92bb87ef4405c0694aeaf99aba86b2abb14b44bceb3906ce0c3d6086b15b",
            "transactiontimestamp": 1650348781,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "982610273",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "17ee92bb87ef4405c0694aeaf99aba86b2abb14b44bceb3906ce0c3d6086b15b",
            "transactiontimestamp": 1650348781,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "3134619740",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "ef1eb07448413b7fad3639049e5d96146aaf4c6154ffec9727a1bbb509aa1679",
            "transactiontimestamp": 1650348618,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "313461973",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ef1eb07448413b7fad3639049e5d96146aaf4c6154ffec9727a1bbb509aa1679",
            "transactiontimestamp": 1650348618,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ef1eb07448413b7fad3639049e5d96146aaf4c6154ffec9727a1bbb509aa1679",
            "transactiontimestamp": 1650348618,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "24a56544c522eca7fba93fb7a6cef83e086706fd87b2f344f5c3dad3603d11f1",
            "liquidity": "98261027",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0ebb2bc5e4402c8cc98cb337a9e5489949c27aa3c493f34b328f59f676454e54",
            "transactiontimestamp": 1650323359,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "0ebb2bc5e4402c8cc98cb337a9e5489949c27aa3c493f34b328f59f676454e54",
            "transactiontimestamp": 1650323359,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9806242859",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "015813dd9c27f76c83110b55058c5d145b5d555baa578fbf808877544bb5faff",
            "transactiontimestamp": 1650290912,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "3162277660",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "015813dd9c27f76c83110b55058c5d145b5d555baa578fbf808877544bb5faff",
            "transactiontimestamp": 1650290912,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "015813dd9c27f76c83110b55058c5d145b5d555baa578fbf808877544bb5faff",
            "transactiontimestamp": 1650290912,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "1133ce092724f98bbbd1bf3a493c57bbb630dd08fffafb2902a489cfa4c7e73c",
            "transactiontimestamp": 1650290189,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "31376973459",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1133ce092724f98bbbd1bf3a493c57bbb630dd08fffafb2902a489cfa4c7e73c",
            "transactiontimestamp": 1650290189,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "9845377989",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1133ce092724f98bbbd1bf3a493c57bbb630dd08fffafb2902a489cfa4c7e73c",
            "transactiontimestamp": 1650290189,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "0f581bd78fcb422099d2ff789ca82291fa8f32d506b9523b341c7e2df2e36095",
            "transactiontimestamp": 1650287562,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "0f581bd78fcb422099d2ff789ca82291fa8f32d506b9523b341c7e2df2e36095",
            "transactiontimestamp": 1650287562,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "6251fd6b3f42e8d6ff782e3bf4571c48b1a56405aa5194d539206de78ac7fbd4",
            "transactiontimestamp": 1650286879,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "9999999000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "6251fd6b3f42e8d6ff782e3bf4571c48b1a56405aa5194d539206de78ac7fbd4",
            "transactiontimestamp": 1650286879,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "6251fd6b3f42e8d6ff782e3bf4571c48b1a56405aa5194d539206de78ac7fbd4",
            "transactiontimestamp": 1650286879,
            "pair": {
              "token0": {
                "id": "afcaa550ebb63266fb2752b58ecd7e8fcd78e0a75777ecd57045213a013d9813",
                "symbol": "WCSPR",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "282fabb87a057d991937770223de98ae86f6e652a050825aa196dfd4f480029e",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "8f39fa9f9c99c04ff7553e5d33fe12914f7af5e18fafa04367889346eedb94e8",
            "transactiontimestamp": 1650281019,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "70629f295bebdff4f09073a35946e56720f7aeb0214a9b7f59222b19a9297295",
            "liquidity": "313769731",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8f39fa9f9c99c04ff7553e5d33fe12914f7af5e18fafa04367889346eedb94e8",
            "transactiontimestamp": 1650281019,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "70629f295bebdff4f09073a35946e56720f7aeb0214a9b7f59222b19a9297295",
            "liquidity": "98453779",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8f39fa9f9c99c04ff7553e5d33fe12914f7af5e18fafa04367889346eedb94e8",
            "transactiontimestamp": 1650281019,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "70629f295bebdff4f09073a35946e56720f7aeb0214a9b7f59222b19a9297295",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "9e2c9c5c451066829912f190c79ab6879a7d288c972876835cedad71355dff25",
            "transactiontimestamp": 1650084438,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "9e2c9c5c451066829912f190c79ab6879a7d288c972876835cedad71355dff25",
            "transactiontimestamp": 1650084438,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9825498216",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "b7aad813e06bf385c83c93f11907a4f2fc2a95a9f300116cc368e470f620a53c",
            "transactiontimestamp": 1650083710,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "b7aad813e06bf385c83c93f11907a4f2fc2a95a9f300116cc368e470f620a53c",
            "transactiontimestamp": 1650083710,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9844819946",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "97514fa224ab37bb1821dca2de1320129ffaff930ac7a363b47a989e91bf79b7",
            "transactiontimestamp": 1650083534,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9864198756",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "97514fa224ab37bb1821dca2de1320129ffaff930ac7a363b47a989e91bf79b7",
            "transactiontimestamp": 1650083534,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5596b4c47340038a4259ccb926d67c905c40b038524460f32e08fd476f708a74",
            "transactiontimestamp": 1650083117,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5596b4c47340038a4259ccb926d67c905c40b038524460f32e08fd476f708a74",
            "transactiontimestamp": 1650083117,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9883634869",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "dd5c6c5c7ba7d04a331e7635eedf75b29a07d881762c73e4b45c25ebb0972eac",
            "transactiontimestamp": 1650083037,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "dd5c6c5c7ba7d04a331e7635eedf75b29a07d881762c73e4b45c25ebb0972eac",
            "transactiontimestamp": 1650083037,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9903128512",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "5327e92f3c58ba40b8542e7540938a74ca23e1529e0d6bb2afbe3cfbe2074d3b",
            "transactiontimestamp": 1650082221,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "5327e92f3c58ba40b8542e7540938a74ca23e1529e0d6bb2afbe3cfbe2074d3b",
            "transactiontimestamp": 1650082221,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9922679912",
            "amount1In": "100000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6ab83137805e7e40498e148ca8bf0c779c1519e80121379c4dab78ebfbbf951e",
            "transactiontimestamp": 1649972293,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "95000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "6ab83137805e7e40498e148ca8bf0c779c1519e80121379c4dab78ebfbbf951e",
            "transactiontimestamp": 1649972293,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "9444707512",
            "amount1In": "95000000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "3aa581879a7ef7fbbc5eabcceeb54815c21839207c776e6e57a2896ede2ddeaf",
            "transactiontimestamp": 1649971950,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "31592763462992",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "3aa581879a7ef7fbbc5eabcceeb54815c21839207c776e6e57a2896ede2ddeaf",
            "transactiontimestamp": 1649971950,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "100000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "3aa581879a7ef7fbbc5eabcceeb54815c21839207c776e6e57a2896ede2ddeaf",
            "transactiontimestamp": 1649971950,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "0d72ccd15e717fde4afc91fab70cb20e9986da52c670976386efc91b375f52a8",
            "liquidity": "9981058480428",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "26a91f843e9907509b6076139a47262e069773be070c17e7c649aeefb86e5e17",
            "transactiontimestamp": 1649962303,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
            "liquidity": "15796381730",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "26a91f843e9907509b6076139a47262e069773be070c17e7c649aeefb86e5e17",
            "transactiontimestamp": 1649962303,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "386859a25c3f8355d663fe7bb8a2cad36efa65292ef073b2fbadef8da8f976f2",
            "liquidity": "15796381730",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "26e3db654da6218b1672083be9a19b1f7847533fe5bb4704b51a2ffcdfd75905",
            "transactiontimestamp": 1649961990,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "386859a25c3f8355d663fe7bb8a2cad36efa65292ef073b2fbadef8da8f976f2",
            "liquidity": "9981058480",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "26e3db654da6218b1672083be9a19b1f7847533fe5bb4704b51a2ffcdfd75905",
            "transactiontimestamp": 1649961990,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "386859a25c3f8355d663fe7bb8a2cad36efa65292ef073b2fbadef8da8f976f2",
            "liquidity": "31592763461",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "26e3db654da6218b1672083be9a19b1f7847533fe5bb4704b51a2ffcdfd75905",
            "transactiontimestamp": 1649961990,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "386859a25c3f8355d663fe7bb8a2cad36efa65292ef073b2fbadef8da8f976f2",
            "liquidity": "100000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c9adf9886066e01d2d4db9dc595a7e9697626c201907f31bed27b81654caca65",
            "transactiontimestamp": 1649957250,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "99810584804",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "c9adf9886066e01d2d4db9dc595a7e9697626c201907f31bed27b81654caca65",
            "transactiontimestamp": 1649957250,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "1000000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "c9adf9886066e01d2d4db9dc595a7e9697626c201907f31bed27b81654caca65",
            "transactiontimestamp": 1649957250,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "315927634632",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d5f40e6405d91fbe68e291971b0ee92abf021b31eaf9281c6481f58d84244bfd",
            "transactiontimestamp": 1649956983,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "2074400407",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "d5f40e6405d91fbe68e291971b0ee92abf021b31eaf9281c6481f58d84244bfd",
            "transactiontimestamp": 1649956983,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
            "liquidity": "2074400407",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "dd691abc8d13dab15e4f7c3e31a4bfdf913617716b794a4c9ab369b5eeb7e66e",
            "transactiontimestamp": 1649956405,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "4148800815",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "dd691abc8d13dab15e4f7c3e31a4bfdf913617716b794a4c9ab369b5eeb7e66e",
            "transactiontimestamp": 1649956405,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
            "liquidity": "4148800815",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a92e6a3be84bd1ec8d59cb598307ea405c4baadeb213736b96cd87281a624a3a",
            "transactiontimestamp": 1649953215,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "2765867209",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "a92e6a3be84bd1ec8d59cb598307ea405c4baadeb213736b96cd87281a624a3a",
            "transactiontimestamp": 1649953215,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "c956ddec09b725a217ac5480fc9cef2411c73b6aaac2e6215ca7255d20f77485",
            "liquidity": "2765867209",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6788cc3c14d108850968f13fca587b6bafe99dc0689447d35e6e30451da3415e",
            "transactiontimestamp": 1649951211,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "6788cc3c14d108850968f13fca587b6bafe99dc0689447d35e6e30451da3415e",
            "transactiontimestamp": 1649951211,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "3159276346",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "6788cc3c14d108850968f13fca587b6bafe99dc0689447d35e6e30451da3415e",
            "transactiontimestamp": 1649951211,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "998105846",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4ee080ea766c6edcc6556bbcf9174e1469d2e072eef433acfbb253d5005d80f6",
            "transactiontimestamp": 1649948280,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "5000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "4ee080ea766c6edcc6556bbcf9174e1469d2e072eef433acfbb253d5005d80f6",
            "transactiontimestamp": 1649948280,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "1579638173",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "4ee080ea766c6edcc6556bbcf9174e1469d2e072eef433acfbb253d5005d80f6",
            "transactiontimestamp": 1649948280,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "499052923",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "1e263f7a4d4a6f2a9bc270312e804805ed0f9727e424f0c8bc6a884a14e44a9b",
            "transactiontimestamp": 1649947586,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "100106",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [],
        "swaps": [
          {
            "transactionid": "1e263f7a4d4a6f2a9bc270312e804805ed0f9727e424f0c8bc6a884a14e44a9b",
            "transactiontimestamp": 1649947586,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "100106",
            "amount0Out": "0",
            "amount1In": "0",
            "amount1Out": "1000000",
            "amountUSD": "0",
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "ba037ff2dcd41ab12d637190dac7a015af14dad60dc9b391b97adfd03ea49da8",
            "transactiontimestamp": 1649947356,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "ba037ff2dcd41ab12d637190dac7a015af14dad60dc9b391b97adfd03ea49da8",
            "transactiontimestamp": 1649947356,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "995509",
            "amount1In": "10000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "8bfc90af8fb53fbd9bfdbd6351b136d02397ac4fc898e239efade33f92a1ef34",
            "transactiontimestamp": 1649947223,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "10000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [
          {
            "transactionid": "8bfc90af8fb53fbd9bfdbd6351b136d02397ac4fc898e239efade33f92a1ef34",
            "transactiontimestamp": 1649947223,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "amount0In": "0",
            "amount0Out": "996503",
            "amount1In": "10000000",
            "amount1Out": "0",
            "amountUSD": "0",
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "__typename": "Swap"
          }
        ],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "88548dcde03e47e294fbbb88e3d8861dc44fb7f1cb291ec947fe578230a1824d",
            "transactiontimestamp": 1649933034,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "3162277660",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "88548dcde03e47e294fbbb88e3d8861dc44fb7f1cb291ec947fe578230a1824d",
            "transactiontimestamp": 1649933034,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [],
        "burns": [
          {
            "transactionid": "88548dcde03e47e294fbbb88e3d8861dc44fb7f1cb291ec947fe578230a1824d",
            "transactiontimestamp": 1649933034,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      },
      {
        "mints": [
          {
            "transactionid": "3b54936cb3c6a52e54381a5d8f4e9725de7596cc709a5cbfd308ab19e4505e2c",
            "transactiontimestamp": 1649931075,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "to": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "3162276660",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Mint"
          }
        ],
        "burns": [
          {
            "transactionid": "3b54936cb3c6a52e54381a5d8f4e9725de7596cc709a5cbfd308ab19e4505e2c",
            "transactiontimestamp": 1649931075,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "10000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          },
          {
            "transactionid": "3b54936cb3c6a52e54381a5d8f4e9725de7596cc709a5cbfd308ab19e4505e2c",
            "transactiontimestamp": 1649931075,
            "pair": {
              "token0": {
                "id": "03e3e09b28dc4d41a4507b38073e7a1641becc0b40e79beb72733d2fb022defa",
                "symbol": "WETH",
                "__typename": "Token"
              },
              "token1": {
                "id": "bdcd8c9844cd2f98c81b3f98ce806f20c5a625f954d7b29bf70626fef060ff1f",
                "symbol": "WISER",
                "__typename": "Token"
              },
              "__typename": "Pair"
            },
            "sender": "df245f53215c2e747c2db7a99d6dd4e20f6b30194565ab3ccc4d83bb73ac89f9",
            "liquidity": "1000000000",
            "amount0": "0",
            "amount1": "0",
            "amountUSD": "0",
            "__typename": "Burn"
          }
        ],
        "swaps": [],
        "__typename": "Transaction"
      }
    ]
  }
}
```
