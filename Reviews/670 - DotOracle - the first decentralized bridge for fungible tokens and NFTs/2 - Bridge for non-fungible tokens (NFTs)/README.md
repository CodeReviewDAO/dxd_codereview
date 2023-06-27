Grant Proposal | [670 - DotOracle - the first decentralized bridge for fungible tokens and NFTs](https://portal.devxdao.com/public-proposals/670)
------------ | -------------
Milestone | 2
Milestone Title | Bridge for non-fungible tokens (NFTs)
OP | AuroraNguyen
Reviewer | Muhammet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The detailed specification of how different NFT standards including ERC721s are bridged to NFTs CEP78 on Casper Launch NFT bridge for ERC721s from EVM chains to Casper blockchain and back. The bridge is governed by the DotOracle validator network Both NFT standards bridge will be supported on https://nftbridge.dotoracle.network Partners with NFT-driven applications on Casper to integrate NFT bridge with those applications to further develop the Casper ecosystem

**Acceptance criteria:**

DotOracle bridge launch that allows users to transfer NFT assets for ERC721s back-and-forth from between Ethereum, Avalanche, BSC, MoonBeam, and OKC Chain, to Casper blockchain. Users use our DotOracle bridge service on https://nftbridge.dotoracle.network and will receive wrapped NFT tokens on the Casper blockchain. NFT DotOracle bridge will help users to transfer NFT-related assets from Casper network to Ethereum, Avalanche, BSC … to use NFT-driven applications of these chains such as Opensea, Binance NFT, Rarible … Deliverable : Smart contracts for bridging fungible tokens from Ethereum and BSC to Casper ERC20 tokens and back— smart contracts for bridging NFTs between Casper (CEP78) and Ethereum/BSC (ERC721 NFTs) Backend code for the bridges Frontend apps support for the bridges Acceptance criteria: User will be able to use our bridge apps to transfer ERC20 tokens from Ethereum/BSC to Casper and back User will be able to use our bridge apps to transfer CEP78 NFTs and ERC721 NFTs tokens back-and-forth between Ethereum/BSC and Casper

**Additional notes regarding submission from OP:**

https://github.com/dotoracle/dto-validator: contains code for validators to validate NFT bridge transactions between Casper and other supported EVM chains.  
https://github.com/dotoracle/bridge-contracts: Smart contracts on EVM chains  
https://github.com/dotoracle/cep-78-enhanced-nft: customized wrapped NFT on Casper  
https://github.com/dotoracle/dotoracle-casper-contracts: Custodian contracts that lock/unlock NFTs on Casper side when bridging  
https://bridge.dotoracle.network/: Official bridge application link

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/dotoracle/dto-validator | 1a97c03
https://github.com/dotoracle/bridge-contracts | 34fadca
https://github.com/dotoracle/cep-78-enhanced-nft | 7a5cd06
https://github.com/dotoracle/dotoracle-casper-contracts | 8b37998
https://bridge.dotoracle.network/ | Retrieved on 2023-06-27

# Final Conclusion

In the reviewer's opinion, this submission should fail directly due to matching one or more of the criteria listed on [possible causes of a direct failure by the CRDAO](https://github.com/CodeReviewDAO/dxd_codereview/blob/main/DIRECT-FAILURE-CAUSES.md) for at least one of the repositories submitted, including but not limited to:

- **No README file**, missing crucial parts such as the instructions for installing and running the code, running the tests, and the user/project documentation.
- No license
- No contribution guidelines or security policy
- No CI action or static code analysis.
- Dependabot alerts are not enabled or not attended to. (There are critical and high severity security alerts when enabled.)
- There are no functional tests or no instructions to properly run tests.
- There are multiple security vulnerability alerts of critical severity on multiple repositories submitted.
- The forked repository of cep-78 is 40 commits behind the original repository.

The recommendation being a DIRECT FAILURE, a full review was not done, and the review was priced accordingly, as per the DxD and the CRDAO's joint policy.


# Recommendation

Recommendation | DIRECT FAILURE
------------ | -------------
