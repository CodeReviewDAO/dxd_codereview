# Output of the "yarn start" command for examples of the project

```sh

furkan@furkan-Victus-by-HP-Laptop-16-e1xxx:~/casperdash-mobile-wallet/android$ yarn start
yarn run v1.22.19
$ react-native start
warn Package d3-shape has been ignored because it contains invalid configuration. Reason: Package subpath './package.json' is not defined by "exports" in /home/furkan/casperdash-mobile-wallet/node_modules/d3-shape/package.json
                                                      
                        #######                       
                   ################                   
                #########     #########               
            #########             ##########          
        #########        ######        #########      
       ##########################################     
      #####      #####################       #####    
      #####          ##############          #####    
      #####    ###       ######       ###    #####    
      #####    #######            #######    #####    
      #####    ###########    ###########    #####    
      #####    ##########################    #####    
      #####    ##########################    #####    
      #####      ######################     ######    
       ######        #############        #######     
         #########        ####       #########        
              #########          #########            
                  ######### #########                 
                       #########                      
                                                      
                                                      
                    Welcome to Metro!
              Fast - Scalable - Integrated



To reload the app press "r"
To open developer menu press "d"

 BUNDLE  ./index.js 

 WARN  Require cycle: node_modules/react-native-crypto/index.js -> node_modules/react-native-randombytes/index.js -> node_modules/sjcl/sjcl.js -> node_modules/react-native-crypto/index.js

Require cycles are allowed, but can result in uninitialized values. Consider refactoring to remove the need for a cycle.
 WARN  Require cycle: node_modules/stream-browserify/index.js -> node_modules/stream-browserify/node_modules/readable-stream/readable.js -> node_modules/stream-browserify/index.js

Require cycles are allowed, but can result in uninitialized values. Consider refactoring to remove the need for a cycle.
 LOG  Running "CasperDash" with {"rootTag":1}
 GROUP     action GET_CONFIGURATIONS @ 15:04:21.410
 LOG     prev state {"home": {"CSPRMarketInfo": null, "tokenInfoWithBalance": null}, "main": {"CMessageData": null, "casperdash": null, "configurations": null, "deploysStakes": null, "deploysTransfer": null, "loader": {"actions": [Array], "refreshing": [Array]}, "overview": null, "tokensAddressList": []}, "market": {"priceHistoryData": null}, "nft": {"isLoading": false, "listNfts": [], "prevSort": "SORT_NAME"}, "staking": {"listValidators": []}, "user": {"casperdash": null, "currentAccount": null, "info": null, "selectedWallet": null}}
 LOG     action     {"type": "GET_CONFIGURATIONS"}
 LOG     next state {"home": {"CSPRMarketInfo": null, "tokenInfoWithBalance": null}, "main": {"CMessageData": null, "casperdash": null, "configurations": null, "deploysStakes": null, "deploysTransfer": null, "loader": {"actions": [Array], "refreshing": [Array]}, "overview": null, "tokensAddressList": []}, "market": {"priceHistoryData": null}, "nft": {"isLoading": false, "listNfts": [], "prevSort": "SORT_NAME"}, "staking": {"listValidators": []}, "user": {"casperdash": null, "currentAccount": null, "info": null, "selectedWallet": null}}
 LOG   [HTTP Interceptor Request] {"DATA": undefined, "HEADER": {"Authorization": "Bearer ", "Content-Type": "application/json", "common": {"Accept": "application/json, text/plain, */*"}, "delete": {}, "get": {}, "head": {}, "patch": {"Content-Type": "application/x-www-form-urlencoded"}, "post": {"Content-Type": "application/x-www-form-urlencoded"}, "put": {"Content-Type": "application/x-www-form-urlencoded"}}, "METHOD": "get", "PARAMS": undefined, "URL": "https://api.casperdash.io/configurations"}
 LOG   [HTTP Interceptor Response] {"DATA": {"API_VERSION": "1.5.1", "CSPR_AUCTION_DELEGATE_FEE": 2.5, "CSPR_AUCTION_UNDELEGATE_FEE": 2.5, "CSPR_TRANSFER_FEE": 0.1, "IPFS_GATEWAY": "ipfs.dweb.link", "MAX_DELEGATOR_PER_VALIDATOR": 951, "MIN_CSPR_DELEGATE_TO_NEW_VALIDATOR": 500, "MOTE_RATE": 1000000000, "OLD_NFT_SMART_CONTRACT_ADDRESSES": ["b779e1b099e52a86d6d4ac69eb09f0a458e7fda27b1b8fe806d12b00a5723174", "e6376c6f97c9464a79bfc100247bea4ee054b264d19bc9294fc85b151ec3fb8c", "b779E1b099e52A86D6D4Ac69eB09F0a458E7Fda27B1B8Fe806D12b00a5723174"], "STAKE_AUCTION_HASH": "ccb576d6ce6dec84a551e48f0d0b7af89ddba44c7390b690036257a04a3ae9ea", "TOKEN_TRANSFER_FEE": 1}, "METHOD": "get", "URL": "/configurations"}
 GROUP     action GET_CONFIGURATIONS_SUCCESS @ 15:04:21.735
 LOG     prev state {"home": {"CSPRMarketInfo": null, "tokenInfoWithBalance": null}, "main": {"CMessageData": null, "casperdash": null, "configurations": null, "deploysStakes": null, "deploysTransfer": null, "loader": {"actions": [Array], "refreshing": [Array]}, "overview": null, "tokensAddressList": []}, "market": {"priceHistoryData": null}, "nft": {"isLoading": false, "listNfts": [], "prevSort": "SORT_NAME"}, "staking": {"listValidators": []}, "user": {"casperdash": null, "currentAccount": null, "info": null, "selectedWallet": null}}
 LOG     action     {"payload": {"API_VERSION": "1.5.1", "CSPR_AUCTION_DELEGATE_FEE": 2.5, "CSPR_AUCTION_UNDELEGATE_FEE": 2.5, "CSPR_TRANSFER_FEE": 0.1, "IPFS_GATEWAY": "ipfs.dweb.link", "MAX_DELEGATOR_PER_VALIDATOR": 951, "MIN_CSPR_DELEGATE_TO_NEW_VALIDATOR": 500, "MOTE_RATE": 1000000000, "OLD_NFT_SMART_CONTRACT_ADDRESSES": ["b779e1b099e52a86d6d4ac69eb09f0a458e7fda27b1b8fe806d12b00a5723174", "e6376c6f97c9464a79bfc100247bea4ee054b264d19bc9294fc85b151ec3fb8c", "b779E1b099e52A86D6D4Ac69eB09F0a458E7Fda27B1B8Fe806D12b00a5723174"], "STAKE_AUCTION_HASH": "ccb576d6ce6dec84a551e48f0d0b7af89ddba44c7390b690036257a04a3ae9ea", "TOKEN_TRANSFER_FEE": 1}, "type": "GET_CONFIGURATIONS_SUCCESS"}
 LOG     next state {"home": {"CSPRMarketInfo": null, "tokenInfoWithBalance": null}, "main": {"CMessageData": null, "casperdash": null, "configurations": {"API_VERSION": "1.5.1", "CSPR_AUCTION_DELEGATE_FEE": 2.5, "CSPR_AUCTION_UNDELEGATE_FEE": 2.5, "CSPR_TRANSFER_FEE": 0.1, "IPFS_GATEWAY": "ipfs.dweb.link", "MAX_DELEGATOR_PER_VALIDATOR": 951, "MIN_CSPR_DELEGATE_TO_NEW_VALIDATOR": 500, "MOTE_RATE": 1000000000, "OLD_NFT_SMART_CONTRACT_ADDRESSES": [Array], "STAKE_AUCTION_HASH": "ccb576d6ce6dec84a551e48f0d0b7af89ddba44c7390b690036257a04a3ae9ea", "TOKEN_TRANSFER_FEE": 1}, "deploysStakes": null, "deploysTransfer": null, "loader": {"actions": [Array], "refreshing": [Array]}, "overview": null, "tokensAddressList": []}, "market": {"priceHistoryData": null}, "nft": {"isLoading": false, "listNfts": [], "prevSort": "SORT_NAME"}, "staking": {"listValidators": []}, "user": {"casperdash": null, "currentAccount": null, "info": null, "selectedWallet": null}}

```
