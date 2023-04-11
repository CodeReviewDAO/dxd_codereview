
Grant Proposal | [318 - Cross Chain Token Bridge-Staking as a Service Solutions](https://portal.devxdao.com/public-proposals/318)
------------ | -------------
Milestone | 2
Milestone Title | Build, Deploy, and Internally QA Bridging Shell App
OP | nickodio_ferrum
Reviewer | Muhammet Kara

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Build and deploy a shell app that will allow swaps among:
1. Casper <> Ethereum
2. Casper <> BSC
3. Casper <> Polygon

- Integrate bridge with one of the Casper’s compatible wallets

- Share Bridging shell app with internal QA and incorporate QA feedback

**Acceptance criteria:**

- UI deployment for bridge interaction
- Smart Contract Deployment of bridge
- Casper compatible wallet integration
- Ability to run swaps among:
1. Casper <> Ethereum
2. Casper <> BSC
3. Casper <> Polygon
- Internal QA feedback incorporation

**Additional notes regarding submission from OP:**

Release notes can be found in the repositories shared above. A demo of the shell app can be seen using the link below.

https://ferrum.network/espast/2023/04/CasperBridgePresentation.mp4

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/ferrumnet/staking-casper-frontend/tree/v0.4.0 | 7642c53
https://github.com/ferrumnet/bridge-casper-smart-contracts/tree/v0.4.0 | d2670b4
https://github.com/ferrumnet/ferrum-gateway | 36cdf39

# Final Conclusion

In the reviewer's opinion, this submission should fail directly due to matching one or more of the criteria listed on [possible causes of a direct failure by the CRDAO](https://github.com/CodeReviewDAO/dxd_codereview/blob/main/DIRECT-FAILURE-CAUSES.md), including but not limited to:

- **README files are empty**, for all repositories submitted, missing crucial parts such as the instructions for installing and running the code, running the tests, and the user/project documentation.
- No contribution guidelines or security policy
- No CI action or static code analysis on the first two repositories. The 3rd repository has a CI action, but with a failure on the latest commit.
- Dependabot alerts are not enabled or not attended to. (There are critical and high severity security alerts when enabled.)
- There are no functional tests on the first repo. When the reviewer tried the common commands to run the tests, the attempt resulted in error. The second repository seems to have some tests, but is missing proper instructions.
- Project level documentation practically does not exist for any of the submitted repositories. Code-level documentation is not adequate either.

The recommendation being a DIRECT FAILURE, a full review was not done, and the review was priced accordingly, as per the DxD and the CRDAO's joint policy.

# Recommendation

Recommendation | DIRECT FAILURE
------------ | -------------


