Grant Proposal | [340 - NodeRED - Casper integration](https://portal.devxdao.com/app/proposal/340) 
------------ |-----------------------------------------------------------------------------------
Milestone | 1 & 2
Milestone Title | Create Node Red Blocs & Add NodeRED put_deploy
OP | Mikael | CasperCommunity.io
Reviewer | Killian Hascoet <killianh@live.fr>                                              

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Create a node for the following RPC requests :
- chain_get_state_root_hash
- info_get_peers  
- info_get_deploy
- info_get_status
- chain_get_block_transfers
- chain_get_block
- chain_get_era_info_by_switch_block    
- state_get_item
- state_get_dictionary_item
- state_get_balance
- state_get_auction_info

Each node consists in :
- A javascript file with the logic
    - Connectors (IN/OUT)
    - Errors
    - Execution of code
- An HTML file :
    - Parameters
    - Labels
    - Icons
    - Help Texts
    - ...
      More info about how to create a node : https://nodered.org/docs/creating-nodes/first-node

Finally we'll propose this package on npm so it can be installed easily in nodered

We'll provide a set of flows to demonstrate the power of NodeRed and the Casper's blockchain.

Create the node put_deploy and the needed dependencies

**Acceptance criteria:**

The package will consist in NodeJS files and html files.

Test in an nodered environment by installing the NPM package.

A flow will be provided with all the nodes :
- chain_get_state_root_hash
- info_get_peers
- info_get_deploy
- info_get_status
- chain_get_block_transfers
- chain_get_block
- chain_get_era_info_by_switch_block
- state_get_item
- state_get_dictionary_item
- state_get_balance
- state_get_auction_info

The package will consist in NodeJS files and html files.
Test in an nodered environment by installing the NPM package.

A flow will be provided with all the nodes :
- put_deploy

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/caspercommunityio/node-red-contrib-casper | a16aeb0

# Install & Usage Testing Procedure and Findings

Reviewer was able to build and run the project by using the instructions given on the README of the project.  
The reviewer was facing an issue because the recommended install procedure use npm and not the package that install the systemd service.  
So the reviewer just rebooted the server.  
Except that, the documentation is well done overall on all the components created for node-red.  
However, the software ecosystem is new for the reviewer and took some time to understand how it works.

```
npm install -g --unsafe-perm node-red
cd ~/.node-red
npm install node-red-contrib-casper
node-red
```

Reviewer was able to test the first exemple provided in the exemple folder after the OP fixed it.


## Overall Impression of usage testing

The reviewer was able to run the tests successfully. 

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The tests run successfully: 

```
npm test

> node-red-contrib-casper@1.0.5 test
> nyc mocha "test/**/**_spec.js" --timeout 7000



  convert-to-runtime-args Node
    ✔ should be loaded
    ✔ should convert to CLString
    ✔ should error to CLString
    ✔ should convert to CLI32
    ✔ should error to CLI32
    ✔ should convert to CLU512
    ✔ should error to CLU512
    ✔ should convert to CLList
    ✔ should convert to CLPublicKey
    ✔ should error to CLPublicKey
    ✔ should convert to CLAccountHash
    ✔ should error to CLAccountHash

  get-account-balance-by-uref Node
    ✔ should be loaded
    ✔ should return something (83ms)
    ✔ should give an error (55ms)

  get-account-uref-by-account-hash Node
    ✔ should be loaded
    ✔ should return something (81ms)
    ✔ should give an error (53ms)

  get-account-uref-by-public-key Node
    ✔ should be loaded
    ✔ should return something (82ms)
    ✔ should give an error

  get-block-info Node
    ✔ should be loaded
    ✔ should return something (87ms)
    ✔ should give an error (79ms)

  get-block-info-by-height Node
    ✔ should be loaded
    ✔ should return something (80ms)
    ✔ should give an error (81ms)

  get-block-state Node
    ✔ should be loaded
    ✔ should return something (56ms)
    ✔ should give an error (53ms)

  get-deploy Node
    ✔ should be loaded
    ✔ should return something (54ms)
    ✔ should give an error (53ms)

  get-dictionary-item-by-uref Node
    ✔ should be loaded
    ✔ should return something (376ms)
    ✔ should give an error (214ms)

  get-era-switch-block-info Node
    ✔ should be loaded
    ✔ should return something (477ms)
    ✔ should give an error (54ms)

  get-latest-block-info Node
    ✔ should be loaded
    ✔ should return something (78ms)
    ✔ Wrong peer (267ms)

  get-peers Node
    ✔ should be loaded
    ✔ should return something (80ms)

  get-state-root-hash Node
    ✔ should be loaded
    ✔ should return something (56ms)

  get-status Node
    ✔ should be loaded
    ✔ should return something (83ms)

  get-transfers Node
    ✔ should be loaded
    ✔ should return something (68ms)

  get-validators-info Node
    ✔ should be loaded
    ✔ should return something (1231ms)

  module-bytes Node
    ✔ should be loaded
    ✔ should return something

  put-deploy Node
    ✔ should be loaded
    ✔ should transfert Ed25519 (46ms)
e { transfer: t { tag: 5, args: e { args: [Map] } } }
    ✔ should transfert Secp256K1
    ✔ should not transfert

  stored-contract-by-hash Node
    ✔ should be loaded
    ✔ should return something
    ✔ should return error

  stored-contract-by-name Node
    ✔ should be loaded
    ✔ should return something
    ✔ should return error

  stored-versioned-contract-by-hash Node
    ✔ should be loaded
    ✔ should return something
    ✔ should return error

  stored-versioned-contract-by-name Node
    ✔ should be loaded
    ✔ should return something
    ✔ should return error


  70 passing (4s)

---------------------------------------|---------|----------|---------|---------|----------------------------------------------------
File                                   | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s
---------------------------------------|---------|----------|---------|---------|----------------------------------------------------
All files                              |    84.9 |    64.13 |   92.23 |    84.9 |
 convert-to-runtime-args               |   62.31 |    60.52 |    87.5 |   62.31 |
  convert-to-runtime-args.js           |   62.31 |    60.52 |    87.5 |   62.31 | 13,17,19,21,23,25,27,31,35,41-43,45-48,50-54,61-69
 get-account-balance-by-uref           |     100 |       50 |     100 |     100 |
  get-account-balance-by-uref.js       |     100 |       50 |     100 |     100 | 14
 get-account-uref-by-account-hash      |     100 |       50 |     100 |     100 |
  get-account-uref-by-account-hash.js  |     100 |       50 |     100 |     100 | 14
 get-account-uref-by-public-key        |   81.81 |       50 |      80 |   81.81 |
  get-account-uref-by-public-key.js    |   81.81 |       50 |      80 |   81.81 | 32-37
 get-block-info                        |     100 |       50 |     100 |     100 |
  get-block-info.js                    |     100 |       50 |     100 |     100 | 14
 get-block-info-by-height              |     100 |       50 |     100 |     100 |
  get-block-info-by-height.js          |     100 |       50 |     100 |     100 | 14
 get-block-state                       |     100 |       50 |     100 |     100 |
  get-block-state.js                   |     100 |       50 |     100 |     100 | 14
 get-deploy                            |     100 |       50 |     100 |     100 |
  get-deploy.js                        |     100 |       50 |     100 |     100 | 14
 get-dictionary-item-by-uref           |     100 |       50 |     100 |     100 |
  get-dictionary-item-by-uref.js       |     100 |       50 |     100 |     100 | 14
 get-era-switch-block-info             |     100 |       50 |     100 |     100 |
  get-era-switch-block-info.js         |     100 |       50 |     100 |     100 | 14
 get-latest-block-info                 |     100 |       50 |     100 |     100 |
  get-latest-block-info.js             |     100 |       50 |     100 |     100 | 14
 get-peers                             |   76.47 |       50 |      80 |   76.47 |
  get-peers.js                         |   76.47 |       50 |      80 |   76.47 | 26-31
 get-state-root-hash                   |   76.47 |       50 |      80 |   76.47 |
  get-state-root-hash.js               |   76.47 |       50 |      80 |   76.47 | 26-31
 get-status                            |   76.47 |       50 |      80 |   76.47 |
  get-status.js                        |   76.47 |       50 |      80 |   76.47 | 26-31
 get-transfers                         |   76.47 |       50 |      80 |   76.47 |
  get-transfers.js                     |   76.47 |       50 |      80 |   76.47 | 27-32
 get-validators-info                   |   76.47 |       50 |      80 |   76.47 |
  get-validators-info.js               |   76.47 |       50 |      80 |   76.47 | 26-31
 module-bytes                          |   82.35 |      100 |     100 |   82.35 |
  module-bytes.js                      |   82.35 |      100 |     100 |   82.35 | 24-28
 put-deploy                            |   89.18 |       50 |      80 |   89.18 |
  put-deploy.js                        |   89.18 |       50 |      80 |   89.18 | 69-72
 stored-contract-by-hash               |   83.33 |      100 |     100 |   83.33 |
  stored-contract-by-hash.js           |   83.33 |      100 |     100 |   83.33 | 29-33
 stored-contract-by-name               |   83.33 |      100 |     100 |   83.33 |
  stored-contract-by-name.js           |   83.33 |      100 |     100 |   83.33 | 31-35
 stored-versioned-contract-by-hash     |   84.21 |    85.71 |     100 |   84.21 |
  stored-versioned-contract-by-hash.js |   84.21 |    85.71 |     100 |   84.21 | 31-35
 stored-versioned-contract-by-name     |   84.21 |    85.71 |     100 |   84.21 |
  stored-versioned-contract-by-name.js |   84.21 |    85.71 |     100 |   84.21 | 30-34
---------------------------------------|---------|----------|---------|---------|----------------------------------------------------

```

The reviewer add the package NYC to the project to get the code coverage of the project out of curiosity.  
The tests and code coverage are impressive.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The OP added documentation as the reviewer asked it.
The documentation is now acceptable.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The reviewer observed that the README of the project has minimal general and usage documentation.
The README could be improved to be more user-friendly for people that don't know the node-red software.
However, the documentation inside each node is well documented. 

Requirement | Finding
------------ | -------------
Usage Documented | PASS with notes

## Overall Conclusion on Documentation

The reviewer concludes that the project has sufficient documentation but the README could be improved. 

# Open Source Practices

## Licenses

The Project is released under the MIT License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. The repository does contain a CONTRIBUTING and a SECURITY policy.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and readable but not documented.

Even if the README is clear enough to understand the basic step to install & test the project, it should be good to improve it with : 
- More detailed exemple for users that doesn't know the node-red software
- A dedicated website for the technical documentation (eg : using Github Pages)

# Final Conclusion
The project meets the functional requirements. The reviewer was able to build and run the unit tests.
The documentation could also be improved for a better user experience.

I would also recommend that the OP add some sort of code coverage with NYC and maybe some code analysis. (Sonarqube / codecov)

Thus, in the reviewer's opinion, this submission should PASS with notes.

# Recommendation

Recommendation | PASS with notes
------------ | -------------

