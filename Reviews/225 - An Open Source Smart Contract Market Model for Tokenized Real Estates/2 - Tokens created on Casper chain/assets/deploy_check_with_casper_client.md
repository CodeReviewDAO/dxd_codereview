'''
muharremsalel@Muharrems-MacBook-Pro devxdao-m2 % casper-client get-deploy --node-address http://136.243.187.84:7777 f1c198608af2488a694d80d56e4345339c1d7cae1d0bcd6d1b32e49f5331f4ff
{
  "id": -518779149508865306,
  "jsonrpc": "2.0",
  "result": {
    "api_version": "1.4.8",
    "deploy": {
      "approvals": [
        {
          "signature": "017510492930433e44b81718dd48a9ecf973082256797574d6a87a59b2b20d905a63e2efa61e541d986a5fb60d7d4ce19ba150597350b1d90596bcab6d0767840c",
          "signer": "017caa4a44ac15c80046c511cfe901452b4949b9431dfe8c6db30f732805c7b4a1"
        }
      ],
      "hash": "f1c198608af2488a694d80d56e4345339c1d7cae1d0bcd6d1b32e49f5331f4ff",
      "header": {
        "account": "017caa4a44ac15c80046c511cfe901452b4949b9431dfe8c6db30f732805c7b4a1",
        "body_hash": "3e5b78fb622ef54bcdcf58f4ef727130402133f847ac9672ecc6ab21a23abc46",
        "chain_name": "casper-test",
        "dependencies": [],
        "gas_price": 1,
        "timestamp": "2022-10-23T01:06:11.673Z",
        "ttl": "30m"
      },
      "payment": {
        "ModuleBytes": {
          "args": [
            [
              "amount",
              {
                "bytes": "050032c46a26",
                "cl_type": "U512",
                "parsed": "165000000000"
              }
            ]
          ],
          "module_bytes": ""
        }
      },
      "session": {
        "ModuleBytes": {
          "args": [
            [
              "collection_name",
              {
                "bytes": "070000006465767864616f",
                "cl_type": "String",
                "parsed": "devxdao"
              }
            ],
            [
              "collection_symbol",
              {
                "bytes": "03000000445844",
                "cl_type": "String",
                "parsed": "DXD"
              }
            ],
            [
              "total_token_supply",
              {
                "bytes": "e803000000000000",
                "cl_type": "U64",
                "parsed": 1000
              }
            ],
            [
              "ownership_mode",
              {
                "bytes": "02",
                "cl_type": "U8",
                "parsed": 2
              }
            ],
            [
              "whitelist_mode",
              {
                "bytes": "01",
                "cl_type": "U8",
                "parsed": 1
              }
            ],
            [
              "nft_kind",
              {
                "bytes": "02",
                "cl_type": "U8",
                "parsed": 2
              }
            ],
            [
              "nft_metadata_kind",
              {
                "bytes": "03",
                "cl_type": "U8",
                "parsed": 3
              }
            ],
            [
              "json_schema",
              {
                "bytes": "[244 hex chars]",
                "cl_type": "String",
                "parsed": "{\"properties\":{\"type\":{\"name\":\"type\",\"description\":\"How token is created: INITIAL, SPLIT or MERGED\",\"required\":true}}}"
              }
            ],
            [
              "identifier_mode",
              {
                "bytes": "00",
                "cl_type": "U8",
                "parsed": 0
              }
            ],
            [
              "metadata_mutability",
              {
                "bytes": "00",
                "cl_type": "U8",
                "parsed": 0
              }
            ]
          ],
          "module_bytes": "[714936 hex chars]"
        }
      }
    },
    "execution_results": [
      {
        "block_hash": "9e1c673361591590d6739dd5a8d10caf3ebcc2fee438a1aa9984df40db397a0e",
        "result": {
          "Success": {
            "cost": "161762492760",
            "effect": {
              "operations": [],
              "transforms": [
                {
                  "key": "hash-8cf5e4acf51f54eb59291599187838dc3bc234089c46fc6ca8ad17e762ae4401",
                  "transform": "Identity"
                },
                {
                  "key": "hash-624dbe2395b9d9503fbee82162f1714ebff6b639f96d2084d26d944c354ec4c5",
                  "transform": "Identity"
                },
                {
                  "key": "hash-010c3fe81b7b862e50c77ef9a958a05bfa98444f26f96f23d37a13c96244cfb7",
                  "transform": "Identity"
                },
                {
                  "key": "hash-9824d60dc3a5c44a20b9fd260a412437933835b52fc683d8ae36e4ec2114843e",
                  "transform": "Identity"
                },
                {
                  "key": "balance-b73e843efc5f3cd67f99cf24b09f899442e9aeee89e9f3304cfe1073436dd972",
                  "transform": "Identity"
                },
                {
                  "key": "balance-98d945f5324f865243b7c02c0417ab6eac361c5c56602fd42ced834a1ba201b6",
                  "transform": "Identity"
                },
                {
                  "key": "balance-b73e843efc5f3cd67f99cf24b09f899442e9aeee89e9f3304cfe1073436dd972",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "0500dee069c2",
                      "cl_type": "U512",
                      "parsed": "835000000000"
                    }
                  }
                },
                {
                  "key": "balance-98d945f5324f865243b7c02c0417ab6eac361c5c56602fd42ced834a1ba201b6",
                  "transform": {
                    "AddUInt512": "165000000000"
                  }
                },
                {
                  "key": "uref-a8c3ab9d16deb4cf29ef3df8439e2bce2f96a022224151f92bf98206afd656a1-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-8778ca7f46cb5bcf687d709f6402622ed7f180489def290339a0f871081faf9f",
                  "transform": "WriteContractPackage"
                },
                {
                  "key": "account-hash-c0ee0a881c2efdc661b2dacf8dacd7102913cfeee9174f1fc216ab323ef52be4",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "hash-8778ca7f46cb5bcf687d709f6402622ed7f180489def290339a0f871081faf9f",
                        "name": "nft_contract_package"
                      }
                    ]
                  }
                },
                {
                  "key": "account-hash-c0ee0a881c2efdc661b2dacf8dacd7102913cfeee9174f1fc216ab323ef52be4",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-a8c3ab9d16deb4cf29ef3df8439e2bce2f96a022224151f92bf98206afd656a1-007",
                        "name": "nft_contract_package_access"
                      }
                    ]
                  }
                },
                {
                  "key": "hash-8778ca7f46cb5bcf687d709f6402622ed7f180489def290339a0f871081faf9f",
                  "transform": "Identity"
                },
                {
                  "key": "hash-c592d985ffb05f79632095147fbc74b5f7c814d6923dc970b33c3f4d5d5252a9",
                  "transform": "WriteContractWasm"
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": "WriteContract"
                },
                {
                  "key": "hash-8778ca7f46cb5bcf687d709f6402622ed7f180489def290339a0f871081faf9f",
                  "transform": "WriteContractPackage"
                },
                {
                  "key": "account-hash-c0ee0a881c2efdc661b2dacf8dacd7102913cfeee9174f1fc216ab323ef52be4",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                        "name": "nft_contract"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-a6affd5e8bf791b782e53e1bbab582e14bc168edd2e66e80a576338535f30e7c-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "01000000",
                      "cl_type": "U32",
                      "parsed": 1
                    }
                  }
                },
                {
                  "key": "account-hash-c0ee0a881c2efdc661b2dacf8dacd7102913cfeee9174f1fc216ab323ef52be4",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-a6affd5e8bf791b782e53e1bbab582e14bc168edd2e66e80a576338535f30e7c-007",
                        "name": "contract_version"
                      }
                    ]
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": "Identity"
                },
                {
                  "key": "hash-8778ca7f46cb5bcf687d709f6402622ed7f180489def290339a0f871081faf9f",
                  "transform": "Identity"
                },
                {
                  "key": "hash-c592d985ffb05f79632095147fbc74b5f7c814d6923dc970b33c3f4d5d5252a9",
                  "transform": "Identity"
                },
                {
                  "key": "uref-4ac5f91fd03e7bc56a09d0e06b23f5b13ccbae019c10a94e6d4be3b6fdf728d1-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "070000006465767864616f",
                      "cl_type": "String",
                      "parsed": "devxdao"
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-4ac5f91fd03e7bc56a09d0e06b23f5b13ccbae019c10a94e6d4be3b6fdf728d1-007",
                        "name": "collection_name"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-2f0eb18d54b7d55d27ffa9b44fae5fd3a40b00453d37dc4e74845028275f9b20-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "03000000445844",
                      "cl_type": "String",
                      "parsed": "DXD"
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-2f0eb18d54b7d55d27ffa9b44fae5fd3a40b00453d37dc4e74845028275f9b20-007",
                        "name": "collection_symbol"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-94e423a3d08219849ce156df423d68f246a29bb5c7a104bdd989ae2567a30733-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "e803000000000000",
                      "cl_type": "U64",
                      "parsed": 1000
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-94e423a3d08219849ce156df423d68f246a29bb5c7a104bdd989ae2567a30733-007",
                        "name": "total_token_supply"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-1780b06cf5466a7702054c517c2965c5084b230165d5096f5ef993cff32906ad-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "02",
                      "cl_type": "U8",
                      "parsed": 2
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-1780b06cf5466a7702054c517c2965c5084b230165d5096f5ef993cff32906ad-007",
                        "name": "ownership_mode"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-6414dbfeac77dc84ba1468ae069050c15235f3ea293aa3126ac8f7e86884e6d1-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "02",
                      "cl_type": "U8",
                      "parsed": 2
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-6414dbfeac77dc84ba1468ae069050c15235f3ea293aa3126ac8f7e86884e6d1-007",
                        "name": "nft_kind"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-168454069335828652e28a5ec719a156f4719deb1fc5807a405d8a04d5851283-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "[244 hex chars]",
                      "cl_type": "String",
                      "parsed": "{\"properties\":{\"type\":{\"name\":\"type\",\"description\":\"How token is created: INITIAL, SPLIT or MERGED\",\"required\":true}}}"
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-168454069335828652e28a5ec719a156f4719deb1fc5807a405d8a04d5851283-007",
                        "name": "json_schema"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-ab2244109eb51831fb2e627fcf8db3c8bc17417ea839fc7d3fb9e531df0a3e40-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00",
                      "cl_type": "U8",
                      "parsed": 0
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-ab2244109eb51831fb2e627fcf8db3c8bc17417ea839fc7d3fb9e531df0a3e40-007",
                        "name": "minting_mode"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-738a392b5a58fb4c9becd388d3442157951e00bd4757ee38b2b709889ff4e43c-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00",
                      "cl_type": "U8",
                      "parsed": 0
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-738a392b5a58fb4c9becd388d3442157951e00bd4757ee38b2b709889ff4e43c-007",
                        "name": "holder_mode"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-1969d47c046224385477b224a752b6367700c23e0281ebaf7d803f95b0b52b73-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00",
                      "cl_type": "U8",
                      "parsed": 0
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-1969d47c046224385477b224a752b6367700c23e0281ebaf7d803f95b0b52b73-007",
                        "name": "whitelist_mode"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-23390c4088b0f5528787873892ab6b05df02ecc116a5f84747d114670ddc25a0-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00000000",
                      "cl_type": {
                        "List": {
                          "ByteArray": 32
                        }
                      },
                      "parsed": []
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-23390c4088b0f5528787873892ab6b05df02ecc116a5f84747d114670ddc25a0-007",
                        "name": "contract_whitelist"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-efaa87be7bda295be1219021dff2007a6403a77b37e5b8fe590a840b0ff79b62-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00000000",
                      "cl_type": {
                        "List": {
                          "ByteArray": 32
                        }
                      },
                      "parsed": []
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-efaa87be7bda295be1219021dff2007a6403a77b37e5b8fe590a840b0ff79b62-007",
                        "name": "account_whitelist"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-b8cd563e711589fd180da19525d424ac6d4c4af5d7ea2914b84389acdbe7ed8a-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "[202 hex chars]",
                      "cl_type": "String",
                      "parsed": "nft-devxdao-contract-package-wasm8778ca7f46cb5bcf687d709f6402622ed7f180489def290339a0f871081faf9f"
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-b8cd563e711589fd180da19525d424ac6d4c4af5d7ea2914b84389acdbe7ed8a-007",
                        "name": "receipt_name"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-85e513fe97ad9391cc8cc8ce97ffa07b16be2ac95866e0c89ff02c7c70407b03-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "03",
                      "cl_type": "U8",
                      "parsed": 3
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-85e513fe97ad9391cc8cc8ce97ffa07b16be2ac95866e0c89ff02c7c70407b03-007",
                        "name": "nft_metadata_kind"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-2f27f74e6d0e54d0597453d355594ad44128fde748d8b7dcfc8d7609617665de-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00",
                      "cl_type": "U8",
                      "parsed": 0
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-2f27f74e6d0e54d0597453d355594ad44128fde748d8b7dcfc8d7609617665de-007",
                        "name": "identifier_mode"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-d0079b7c73a5bd5d2088ed12605d4562cc9e5dffa35b5a7642cff9f6bbcd9120-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00",
                      "cl_type": "U8",
                      "parsed": 0
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-d0079b7c73a5bd5d2088ed12605d4562cc9e5dffa35b5a7642cff9f6bbcd9120-007",
                        "name": "metadata_mutability"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-e9e5725531091c3a0c7337099652a2f0838eba894faf514f983d44642a108ead-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "01",
                      "cl_type": "Bool",
                      "parsed": true
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-e9e5725531091c3a0c7337099652a2f0838eba894faf514f983d44642a108ead-007",
                        "name": "allow_minting"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-35ff4e77da56c8dbff517f42c848898ebb98c03af1d67bf38dbc83ff2c14f670-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "0000000000000000",
                      "cl_type": "U64",
                      "parsed": 0
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-35ff4e77da56c8dbff517f42c848898ebb98c03af1d67bf38dbc83ff2c14f670-007",
                        "name": "number_of_minted_tokens"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-dcf99979fe29b64665d500301a0aff293bff1b7e43cf92f0321fc274157d830a-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-dcf99979fe29b64665d500301a0aff293bff1b7e43cf92f0321fc274157d830a-007",
                        "name": "token_owners"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-720073e3c7944746c696c3fd84e49abfcefccdaca80d2c42964421840ab12934-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-720073e3c7944746c696c3fd84e49abfcefccdaca80d2c42964421840ab12934-007",
                        "name": "token_issuers"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-59b72c6a147e0659622e913e609f21a820402a857f615ab019a32b4c265967c8-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-59b72c6a147e0659622e913e609f21a820402a857f615ab019a32b4c265967c8-007",
                        "name": "owned_tokens"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-c276a6851b6cfcd15d921f1e1d0d239fe8a4ebb2e522fd28178f547e7e80990f-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-c276a6851b6cfcd15d921f1e1d0d239fe8a4ebb2e522fd28178f547e7e80990f-007",
                        "name": "operator"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-871fc9b69be54585f74b5169f3eb31ced3d43f3c0efabd160cfb4ccbc6dcc70d-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-871fc9b69be54585f74b5169f3eb31ced3d43f3c0efabd160cfb4ccbc6dcc70d-007",
                        "name": "burnt_tokens"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-02d1780280b638d0a9ea972c5b32ed9c63b9387f511bc1ac905a8fcd965a5a68-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-02d1780280b638d0a9ea972c5b32ed9c63b9387f511bc1ac905a8fcd965a5a68-007",
                        "name": "balances"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-20aebbf1fb15a12505123b097c1fe90f08f7f53b1401e10b30b85d25830e7d00-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-20aebbf1fb15a12505123b097c1fe90f08f7f53b1401e10b30b85d25830e7d00-007",
                        "name": "metadata_custom_validated"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-23eaa1ed6cb63e7f5a3faeacbd84cdd64aa9140bc7a7dcdd0141056edd852400-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-23eaa1ed6cb63e7f5a3faeacbd84cdd64aa9140bc7a7dcdd0141056edd852400-007",
                        "name": "metadata_cep78"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-f50a0c45c61348694674376ca6b19eee7022895398933a78cc36d7958baa0715-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-f50a0c45c61348694674376ca6b19eee7022895398933a78cc36d7958baa0715-007",
                        "name": "metadata_nft721"
                      }
                    ]
                  }
                },
                {
                  "key": "uref-1c69d47680de8ec00058d09cb5ebddb9ab41cfb079773de2a3a6c0aef1b12768-000",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "",
                      "cl_type": "Unit",
                      "parsed": null
                    }
                  }
                },
                {
                  "key": "hash-9966c1916af49c6abb42f72df66c9216646aa1236dedd71e652f8559ee327073",
                  "transform": {
                    "AddKeys": [
                      {
                        "key": "uref-1c69d47680de8ec00058d09cb5ebddb9ab41cfb079773de2a3a6c0aef1b12768-007",
                        "name": "metadata_raw"
                      }
                    ]
                  }
                },
                {
                  "key": "deploy-f1c198608af2488a694d80d56e4345339c1d7cae1d0bcd6d1b32e49f5331f4ff",
                  "transform": {
                    "WriteDeployInfo": {
                      "deploy_hash": "f1c198608af2488a694d80d56e4345339c1d7cae1d0bcd6d1b32e49f5331f4ff",
                      "from": "account-hash-c0ee0a881c2efdc661b2dacf8dacd7102913cfeee9174f1fc216ab323ef52be4",
                      "gas": "161762492760",
                      "source": "uref-b73e843efc5f3cd67f99cf24b09f899442e9aeee89e9f3304cfe1073436dd972-007",
                      "transfers": []
                    }
                  }
                },
                {
                  "key": "hash-8cf5e4acf51f54eb59291599187838dc3bc234089c46fc6ca8ad17e762ae4401",
                  "transform": "Identity"
                },
                {
                  "key": "hash-624dbe2395b9d9503fbee82162f1714ebff6b639f96d2084d26d944c354ec4c5",
                  "transform": "Identity"
                },
                {
                  "key": "balance-98d945f5324f865243b7c02c0417ab6eac361c5c56602fd42ced834a1ba201b6",
                  "transform": "Identity"
                },
                {
                  "key": "hash-8cf5e4acf51f54eb59291599187838dc3bc234089c46fc6ca8ad17e762ae4401",
                  "transform": "Identity"
                },
                {
                  "key": "hash-010c3fe81b7b862e50c77ef9a958a05bfa98444f26f96f23d37a13c96244cfb7",
                  "transform": "Identity"
                },
                {
                  "key": "hash-9824d60dc3a5c44a20b9fd260a412437933835b52fc683d8ae36e4ec2114843e",
                  "transform": "Identity"
                },
                {
                  "key": "balance-98d945f5324f865243b7c02c0417ab6eac361c5c56602fd42ced834a1ba201b6",
                  "transform": "Identity"
                },
                {
                  "key": "balance-634bf64a3a6844b330d2f654291d89032a3ef41d8bbf5d75604686fc3cd141a6",
                  "transform": "Identity"
                },
                {
                  "key": "balance-98d945f5324f865243b7c02c0417ab6eac361c5c56602fd42ced834a1ba201b6",
                  "transform": {
                    "WriteCLValue": {
                      "bytes": "00",
                      "cl_type": "U512",
                      "parsed": "0"
                    }
                  }
                },
                {
                  "key": "balance-634bf64a3a6844b330d2f654291d89032a3ef41d8bbf5d75604686fc3cd141a6",
                  "transform": {
                    "AddUInt512": "165000000000"
                  }
                }
              ]
            },
            "transfers": []
          }
        }
      }
    ]
  }
}

'''