
Grant Proposal | [318 - Cross Chain Token Bridge-Staking as a Service Solutions](https://portal.devxdao.com/public-proposals/318)
------------ | -------------
Milestones | 4 & 5
Milestone Title | Mainnet deployment, testing and incorporation of final feedback - Token Bridge & Incorporate audit feedback and launch - Token Bridge
OP | nickodio_ferrum
Reviewer | Gökay Şatır

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Deploy bridge on mainnet - Incorporate audit feedback if audit is completed - Conduct internal testing - Share the bridge with DEVxDAO and incorporate the final feedback
- Incorporate final audit feedback provided by a third party - Launching the bridge on production mainnet

**Acceptance criteria:**

- Ability to conduct swaps across below networks with Casper: 1. Casper <> Ethereum 2. Casper <> BSC 3. Casper <> Polygon - Able to add/remove liquidity on all networks - DEVxDAO signs off on mainnet testing
- Sign-off on audit completion by the third party auditor - Launch on production mainnet - Bridge is live and available to users to bridge token

**Additional notes regarding submission from OP:**

https://mail.google.com/mail/u/0?ui=2&ik=f20012be9d&attid=0.1&permmsgid=msg-a:r7591766417104732950&view=att&disp=safe&realattid=f_lkh0obzj0

https://casper-mainnet-bridge.netlify.app/

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
https://github.com/ferrumnet/bridge-casper-smart-contracts/releases/tag/v0.4.10 | f06ef2c


# Install & Usage Testing Procedure and Findings

Project successfuly builds. Usage examples of the contract are provided.

## Overall Impression of usage testing

Project builds without errors.
Documentation provides sufficient installation/execution instructions.

# Unit / Automated Testing

One of the tests is failing: "should_be_able_to_install_and_add_liquidity_and_withdraw_signed".

# Documentation

### Code Documentation

cargo doc command needs to be provided in readme and in the makefile or the output of the command needs to be added and kept updated.

### Project Documentation

Notes: Though the usage is documented, it couldn't be tested in production.

## Overall Conclusion on Documentation

Documentation seems good in general. To be checked again against the missing pieces.

# Open Source Practices

## Licenses

MIT license is provided.

## Contribution Policies

There is note in the readme file regarding contribution.

# Final Conclusion

* GitHub dependabot and GitHub code scanning are suggested for security checks (via GitHub -> Settings -> Code security and analysis).
	* There are 4 critical 4 moderate alerts on dependabot.
	* GitHub code scanning should also be active.
	* Neither of them are active for the repository at the moment.
* Given mail attachment links are broken. I couldn't see a security audit report.

Since this is the final review, we'll need to complete the missing pieces before accepting these milestones.

# Recommendation

Project doesn't seem to be complete. Production tests couldn't be performed. The UI in https://casper-mainnet-bridge.netlify.app/ is not working properly.
Web page shows errors after connecting with a wallet.
