# Output of "yarn test" command

```sh

 PASS  src/markup/Layout/__test__/HeaderMenu.test.js (11.008 s)
 PASS  src/markup/Element/__test__/ListForSaleNFT.test.js (11.098 s)
 PASS  src/api/__test__/getSpecificData.test.js (12.654 s)
 PASS  src/api/__test__/campaignInfo.test.js (12.809 s)
 PASS  src/api/__test__/beneficiaryInfo.test.js (12.847 s)
 PASS  src/api/__test__/updateCachedProfile.test.js (13.325 s)
 PASS  src/markup/Layout/__test__/Footer1.test.js
 PASS  src/markup/Element/__test__/NFTCard.test.js (13.564 s)
 PASS  src/markup/Element/__test__/BuyNFT.test.js
 PASS  src/api/__test__/collectionInfo.test.js
  ● Console

    console.log
      Error: Tried to unwrap None
          at NoneImpl.unwrap (/workspace/Verified-Impact-NFTs/node_modules/src/option.ts:68:15)
          at CEP47Client.getCollection (/workspace/Verified-Impact-NFTs/src/lib/cep47.ts:318:39)
          at processTicksAndRejections (node:internal/process/task_queues:96:5)
          at getCollectionDetails (/workspace/Verified-Impact-NFTs/src/api/collectionInfo.ts:7:29)
          at getCollectionsList (/workspace/Verified-Impact-NFTs/src/api/collectionInfo.ts:58:5)
          at Object.<anonymous> (/workspace/Verified-Impact-NFTs/src/api/__test__/collectionInfo.test.js:11:16)
          at _callCircusTest (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/run.js:212:5)
          at _runTest (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/run.js:149:3)
          at _runTestsForDescribeBlock (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/run.js:63:9)
          at _runTestsForDescribeBlock (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/run.js:57:9)
          at run (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/run.js:25:3)
          at runAndTransformResultsToJestFormat (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/legacy-code-todo-rewrite/jestAdapterInit.js:176:21)
          at jestAdapter (/workspace/Verified-Impact-NFTs/node_modules/jest-circus/build/legacy-code-todo-rewrite/jestAdapter.js:109:19)
          at runTestInternal (/workspace/Verified-Impact-NFTs/node_modules/jest-runner/build/runTest.js:380:16)
          at runTest (/workspace/Verified-Impact-NFTs/node_modules/jest-runner/build/runTest.js:472:34)
          at Object.worker (/workspace/Verified-Impact-NFTs/node_modules/jest-runner/build/testWorker.js:133:12)

      at src/api/collectionInfo.ts:71:17

 PASS  src/markup/Element/__test__/VideoPopup.test.js
 PASS  src/api/__test__/getProfileCachedData.test.js
 PASS  src/api/__test__/getProfileList.test.js (44.157 s)
 PASS  src/api/__test__/updateProfile.test.js (65.942 s)
  ● Console

    console.log
      entityInfo.publicKey 014b2f7c0b006bf3b09901fe123381cdf252f0772abbbd3d3bc5582c884234e4dd

      at Object.<anonymous> (src/api/__test__/updateProfile.test.js:9:9)

    console.log
      6b18d6665e05d6fd8b1617c8eafa6282ab641994248a21d7510ba94c8efdaf88      =================saveDeployHash

      at UpdateProfile (src/api/updateProfile.ts:35:17)

    console.log
      ...... Profile Saved successfully e {
        approvals: [
          e {
            signer: '014b2f7c0b006bf3b09901fe123381cdf252f0772abbbd3d3bc5582c884234e4dd',
            signature: '01a04c4edf8670c47f5a53d66628066db2a485b2c1e43f0545aef2b5ac65416c29bce8bcab49f95a63d88074d96819da6867b5b65dfce4a12469fa51f4b5825a05'
          }
        ],
        session: e {
          storedContractByHash: t {
            tag: 1,
            entryPoint: 'create_profile',
            args: [e],
            hash: [Uint8Array]
          }
        },
        payment: e {
          moduleBytes: t { tag: 0, moduleBytes: Uint8Array(0) [], args: [e] }
        },
        header: e {
          account: t { isCLValue: true, data: [Uint8Array], tag: 1 },
          timestamp: 1674637378539,
          ttl: 1800000,
          gasPrice: 1,
          bodyHash: Uint8Array(32) [
              4, 240, 247,  62, 135, 102, 183,
            170, 150, 119, 225, 190, 214, 214,
            122, 116,  93, 145, 209,  64,  96,
             11, 192,  94, 167, 113,  19, 140,
             78, 166, 137, 196
          ],
          dependencies: [],
          chainName: 'casper-test'
        },
        hash: Uint8Array(32) [
          107,  24, 214, 102,  94,   5, 214, 253,
          139,  22,  23, 200, 234, 250,  98, 130,
          171, 100,  25, 148,  36, 138,  33, 215,
           81,  11, 169,  76, 142, 253, 175, 136
        ]
      }

      at UpdateProfile (src/api/updateProfile.ts:37:17)

    console.log
      chnaged Data {
        '6436a9a3adb3880c94eb7de6a3a10ea3851a176451e0bbf65c7bc3050ffc1d4f': {
          normal: {
            address: '6436a9a3adb3880c94eb7de6a3a10ea3851a176451e0bbf65c7bc3050ffc1d4f',
            username: 'test from  test api',
            address_pk: '014b2f7c0b006bf3b09901fe123381cdf252f0772abbbd3d3bc5582c884234e4dd',
            ein: '',
            externalLink: '',
            facebook: '',
            firstName: '',
            has_receipt: false,
            imgUrl: '',
            instagram: '',
            isApproved: 'false',
            lastName: '',
            mail: '',
            medium: '',
            nftUrl: 'https://images.pexels.com/photos/14524982/pexels-photo-14524982.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2',
            phone: '',
            tagline: '',
            telegram: '',
            twitter: '',
            bio: ''
          },
          beneficiary: {},
          creator: {}
        }
      }

      at UpdateProfile (src/api/updateProfile.ts:73:17)

    console.log
      {
        '6436a9a3adb3880c94eb7de6a3a10ea3851a176451e0bbf65c7bc3050ffc1d4f': {
          normal: {
            address: '6436a9a3adb3880c94eb7de6a3a10ea3851a176451e0bbf65c7bc3050ffc1d4f',
            username: 'test from  test api',
            address_pk: '014b2f7c0b006bf3b09901fe123381cdf252f0772abbbd3d3bc5582c884234e4dd',
            ein: '',
            externalLink: '',
            facebook: '',
            firstName: '',
            has_receipt: false,
            imgUrl: '',
            instagram: '',
            isApproved: 'false',
            lastName: '',
            mail: '',
            medium: '',
            nftUrl: 'https://images.pexels.com/photos/14524982/pexels-photo-14524982.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2',
            phone: '',
            tagline: '',
            telegram: '',
            twitter: '',
            bio: ''
          },
          beneficiary: {},
          creator: {}
        }
      }

      at Object.<anonymous> (src/api/__test__/updateProfile.test.js:18:9)


Test Suites: 14 passed, 14 total
Tests:       14 passed, 14 total
Snapshots:   0 total
Time:        69.737 s
Ran all test suites.

```
