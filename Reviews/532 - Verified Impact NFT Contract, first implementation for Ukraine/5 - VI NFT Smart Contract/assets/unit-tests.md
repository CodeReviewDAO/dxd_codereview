```js
 PASS  src/markup/Layout/__test__/Footer1.test.js
 PASS  src/markup/Element/__test__/VideoPopup.test.js
 PASS  src/markup/Layout/__test__/HeaderMenu.test.js
 PASS  src/markup/Element/__test__/ListForSaleNFT.test.js
 PASS  src/markup/Element/__test__/BuyNFT.test.js
 PASS  src/markup/Element/__test__/NFTCard.test.js
 PASS  src/api/__test__/beneficiaryInfo.test.js (5.741 s)
  ● Console

    console.log
      [
        {
          address: '01501b4037bdeffd70849a86698922f6f3ed2ff52dad5235b2472b09ae66e48e8c',
          description: 'The Ministry of Digital Transformation (Ukrainian: Міністерство цифрової трансформації України) is a government ministry in Ukraine that was established on 29 August 2019 when Mykhailo Fedorov was appointed as Minister of Digital Transformation in the Honcharuk Government. Its current and first minister is Mykhailo Fedorov.',
          id: '1',
          name: 'Ukraine Gov'
        },
        {
          address: '01aa837e4f212d197b00be3d93c5d5ca08df00d6016ce39f293f295bbcb850707d',
          description: 'From our kids to all the kids of Ukraine',
          id: '2',
          name: 'Kids 4 Ukraine'
        }
      ]

      at getBeneficiariesList (src/api/beneficiaryInfo.ts:38:11)

 PASS  src/api/__test__/campaignInfo.test.js (6.539 s)
  ● Console

    console.log
      [
        {
          collection_ids: '0',
          description: 'Stand with Ukraine people in their time of need!',
          id: '1',
          name: 'Stand With Ukraine',
          requested_royalty: '80',
          url: 'https://thedigital.gov.ua/',
          wallet_address: '01501b4037bdeffd70849a86698922f6f3ed2ff52dad5235b2472b09ae66e48e8c'
        },
        {
          collection_ids: '0',
          description: 'Supporting more than 6 million Ukrainian refugees through a rough time!',
          id: '2',
          name: 'Refugees',
          requested_royalty: '80',
          url: 'https://thedigital.gov.ua/',
          wallet_address: '01501b4037bdeffd70849a86698922f6f3ed2ff52dad5235b2472b09ae66e48e8c'
        },
        {
          collection_ids: '0',
          description: "Let's build Ukraine better than ever!",
          id: '3',
          name: 'Reconstruction',
          requested_royalty: '80',
          url: 'https://thedigital.gov.ua/',
          wallet_address: '01501b4037bdeffd70849a86698922f6f3ed2ff52dad5235b2472b09ae66e48e8c'
        }
      ]

      at getCampaignsList (src/api/campaignInfo.ts:37:11)

 PASS  src/api/__test__/collectionInfo.test.js (15.1 s)
  ● Console

    console.log
      1

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 1 details:  Map(6) {
        'creator: ' => '0127271ea03f8cb24e0e3100d18e4d29fc860b35a2c9eb86ae4cca280a8fc40e1f',
        'description: ' => '',
        'id: ' => '1',
        'name: ' => "A Hero's Stand",
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      2

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 2 details:  Map(6) {
        'creator: ' => '0127271ea03f8cb24e0e3100d18e4d29fc860b35a2c9eb86ae4cca280a8fc40e1f',
        'description: ' => '',
        'id: ' => '2',
        'name: ' => 'Never Forget',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      3

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 3 details:  Map(6) {
        'creator: ' => '0127271ea03f8cb24e0e3100d18e4d29fc860b35a2c9eb86ae4cca280a8fc40e1f',
        'description: ' => '',
        'id: ' => '3',
        'name: ' => 'Forever Keys',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      4

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 4 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '4',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      5

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 5 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '5',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      6

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 6 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '6',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      7

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 7 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '7',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      8

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 8 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '8',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      9

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 9 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '9',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      10

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 10 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '10',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      11

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 11 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '11',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      12

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 12 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '12',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      13

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 13 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '13',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      14

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 14 details:  Map(6) {
        'creator: ' => '01c82663493f5042af3b4247b07d3785978fb0491f75508a8da19b2b8792cee866',
        'description: ' => '',
        'id: ' => '14',
        'name: ' => 'Impact Cars',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)

    console.log
      15

      at getCollectionDetails (src/api/collectionInfo.ts:4:11)

    console.log
      Collection 15 details:  Map(6) {
        'creator: ' => '013171ea0c93f82b0d2b680e9f1ecdfbccb2cd79c17a06094d7e43be1274568c52',
        'description: ' => '',
        'id: ' => '15',
        'name: ' => 'Freedom for Ukraine',
        'token_ids: ' => '0',
        'url: ' => ''
      }

      at getCollectionDetails (src/api/collectionInfo.ts:7:11)


Test Suites: 9 passed, 9 total
Tests:       9 passed, 9 total
Snapshots:   0 total
Time:        16.154 s
Ran all test suites.

Watch Usage: Press w to show more.
```