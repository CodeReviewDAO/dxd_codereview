
Grant Proposal | [451 - Analytics & Portfolio Management for DeFi Automatic Market Makers (AMM)](https://portal.devxdao.com/public-proposals/451)
------------ | -------------
Milestone | 1
Milestone Title | Establish Infrastructure & Proof of Concept
OP | FLUIDEFI
Reviewer | Muhammet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Infrastructure design and setup
- Create GitHub repository
- Connect to Blockchain 
- Set up primary and backup nodes on mainnet for production use
- Connect to Testnet
- Define FLUIDEFI DB schema for AMM (Example: CasperSwap)
- Test current DEVxDAO Python & Javascript SDKs to ensure there is functionality in place to build the entire FLUIDEFI proposed project. A large amount of effort will be put into this step. Specifically, FLUIDEFI’s current production platform is built entirely with Web3. For this step we will need to code test scripts to ensure Python & Javascript SDKs have the necessary functionality and are working without errors. If problems with the SDKs are found, our team will work with the SDK developers to resolve those issues. During this time, this project may be put on hold.

**Acceptance criteria:**

CODE: Test scripts and results
DOCUMENT: Infrastructure design diagram
LINK: GitHub repository
NODES: Set up primary and backup nodes on mainnet for production use Connect to Testnet
DOCUMENT: Completed DB schema for AMM (for example: CasperSwap)
DOCUMENT: API Definition for RESTful API calls that provide ranking and summary analytics of liquidity pools with metrics including, but not limited to: 
Open, close, high, low prices of underlying assets
total_period_return	Total rate of return for a liquidity pool in the specified period
yield_on_lp_fees	Return from fees in the specified period
price_change_ret	Return from the change in price of the underlying tokens in the specified period
hodl_return		Return if tokens were held (not staked in a liquidity pool) in the specified period
fees_apy	Return from fees in the specified period, annualized
Cumulative total return metrics on investment in base_currency
impermanent_loss_level	The percentage difference in portfolio value between staking tokens in an AMM and holding tokens in a wallet. Fees are not taken into account in this calculation
impermanent_loss_impact	The percentage difference in ROI between staking tokens in an AMM and holding tokens in a wallet. Fees are not taken into account in this calculation
Volume & transactions during the time_period specified
Reserves & Poolsize

Definition of Done (DOD): Provide the above documents, links, and proof of node setup.

**Additional notes regarding submission from OP:**

LINK: GitHub repository. Above URL. There is an aggregator repo as well (see below).

CODE: Test scripts and results. In the above repo; see test folder.

DOCUMENT: Infrastructure design diagram. https://github.com/fluidefi/fluidefi-caspernet-aggregator-tools/blob/master/casper-infra.drawio.pdf 

NODES: Set up primary and backup nodes on mainnet for production use Connect to Testnet. Servers are located at: 
Mainnet: caspernet02.fluidefi.io
Testnet: caspertest1.fluidefi.io

DOCUMENT: Completed DB schema for AMM (for example: CasperSwap). Two (2) .pdf docs, here: https://github.com/fluidefi/fluidefi-caspernet-aggregator-tools/tree/master/src/schema

DOCUMENT: API Definition for RESTful API calls that provide ranking and summary analytics of liquidity pools with metrics. Docs are online, here: https://analytics.fluidefi.com/api/docs/#overview

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/fluidefi/caspernet-sdk-examples | 602a477

# Final Conclusion

In the reviewer's opinion, this submission should fail directly due to matching one or more of the criteria listed on [possible causes of a direct failure by the CRDAO](https://github.com/CodeReviewDAO/dxd_codereview/blob/main/DIRECT-FAILURE-CAUSES.md), including but not limited to:

- **License missing**
- **README file is practically empty**, missing crucial parts such as the instructions for installing and running the code, running the tests, and the user/project documentation
- No contribution guidelines or security policy
- No CI action or static code analysis
- Dependabot alerts are not enabled or not attended to. (There are critical security alerts when enabled.)

The recommendation being a DIRECT FAILURE, a full review was not done, and the review was priced accordingly, as per the DxD and the CRDAO's joint policy.

# Recommendation

Recommendation | DIRECT FAILURE
------------ | -------------
