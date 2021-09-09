Grant Proposal | [60 - Financial crime prevention and risk intelligence on-chain tool](https://portal.devxdao.com/public-proposals/60)
------------ | -------------
Milestone | 2
Milestone Title | Sample Implementation
OP | Michael Steuer <michael@make.software>
Reviewer | David Tai <dtaipublic@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- As a Project, I shall include an example implementation of resolving validators against the Smart Contract

**Acceptance criteria:**

- An open source example that can be run by anyone that checks it out will be able to resolve a Validator's public key against the Smart Contract and retrieve metadata for the Validator, such as name, icon and other details.

**Additional notes regarding submission from OP:**

The repository provides for detailed examples in the main README, but also a bash based script that provides an end-to-end example in:
/tools/get-account-info.sh

Use this script from a Casper Testnet node, and you can test it simply by calling:

`./get-account-info.sh --public-key=0106ca7c39cd272dbf21a86eeb3b36b7c26e2e9b94af64292419f7862936bca2ca`

If you look at the example script, you will note that it meets the acceptance criteria by
- accepting input of a (Testnet) validator's public key
- checks the on-chain smart contract for the entry associated with the public key
- if one is found, subsequently retrieves the validator's metadata in the format provided by the account information standard (https://github.com/make-software/casper-account-info-standard)

The provided example above retrieves the metadata as set for several of MAKE's validator node's on the Casper Testnet.  The source code as well as the documentation provided function as the example that shows other participants on the Casper Network how to use and query the Casper Account Information

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/make-software/casper-account-info-contract | 48c9ee1

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/make-software/casper-account-info-contract, reviewer was
able to successfully build and run the manual test for this milestone and
automated tests.

Automated testing generates the following outputs:

```
running 12 tests
test tests::test_add_admin_security - should panic ... ok
test tests::test_add_admin_twice - should panic ... ok
test tests::test_add_and_disable_admin ... ok
test tests::test_delete - should panic ... ok
test tests::test_delete_url_for_account - should panic ... ok
test tests::test_disable_admin_security - should panic ... ok
test tests::test_remove_last_admin - should panic ... ok
test tests::test_remove_non_existing_admin - should panic ... ok
test tests::test_delete_url_for_account_security - should panic ... ok
test tests::test_set_url ... ok
test tests::test_set_url_for_account_security - should panic ... ok
test tests::test_set_url_for_account ... ok

test result: ok. 12 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 19.73s
```

These tests rule out regressions against the first milestone that this milestone
could have potentially introduced.

Upon first attempt to run the project with the milestone manual test `./get-account-info.sh --public-key=0106ca7c39cd272dbf21a86eeb3b36b7c26e2e9b94af64292419f7862936bca2ca` as indicated in the additional notes for the milestone, the reviewer ran into an error.

However, this was later resolved by pointing at a public testnet validator.  The
error thrown was a non descript one from the casper client and not an issue with
the end-to-end testing script and outside of scope of this review.

After getting an up to date copy of the blockchain locally, I was able to get
the following output

```
{
	"data": {
		"account_hash": "fa12d2dd5547714f8c2754d418aa8c9d59dc88780350cb4254d622e2d4ef7e69",
		"url": "https://casper-account-info-standard-test.make.services",
		"is_active": true,
		"info": {
			"nodes": [{
				"location": {
					"name": "N. Virginia",
					"country": "US",
					"latitude": 0,
					"longitude": 0
				},
				"public_key": "0106ca7c39cd272dbf21a86eeb3b36b7c26e2e9b94af64292419f7862936bca2ca",
				"description": "Make's first Casper Testnet validator",
				"functionality": ["validator"]
			}, {
				"location": {
					"name": "N. Virginia",
					"country": "US",
					"latitude": 0,
					"longitude": 0
				},
				"public_key": "017d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e",
				"description": "Make's second Casper Testnet validator",
				"functionality": ["validator"]
			}],
			"owner": {
				"name": "Make Software!",
				"type": ["validator"],
				"email": "hello@make.services",
				"social": {
					"github": "make-software",
					"medium": "",
					"reddit": "",
					"wechat": "",
					"keybase": "",
					"twitter": "@theRealMAKEllc",
					"youtube": "",
					"facebook": "makellc",
					"telegram": ""
				},
				"website": "https://make.services",
				"branding": {
					"logo": {
						"svg": "",
						"png_256": "https://pbs.twimg.com/profile_images/926126811418730496/vZpeIgPp_400x400.jpg",
						"png_1024": ""
					}
				},
				"identity": {
					"ownership_disclosure_url": "",
					"casper_association_kyc_url": "",
					"casper_association_kyc_onchain": ""
				},
				"location": {
					"name": "Woodinville, WA",
					"country": "US",
					"latitude": 0,
					"longitude": 0
				},
				"resources": {
					"other": [],
					"privacy_policy_url": "https://testnet.cspr.live/privacy",
					"code_of_conduct_url": "",
					"terms_of_service_url": "https://testnet.cspr.live/tos"
				},
				"description": "",
				"affiliated_accounts": [{
					"public_key": "017d96b9a63abcb61c870a4f55187a0a7ac24096bdb5fc585c12a686a4d892009e"
				}]
			}
		},
		"deploy_hash": "0bc46b9d6ff078b4fbd99611df9b1270033e0eb33d8c25de486bc1ec55963e08",
		"verified_account_hashes": ["21eaea584903e79365bcb1f7607179cc118807033c8919cff7489a91c3a822d1", "fa12d2dd5547714f8c2754d418aa8c9d59dc88780350cb4254d622e2d4ef7e69"]
	}
}
```

## Overall Impression of usage testing

Manual testing was pretty simple and straight forward. The end-to-end manual
testing interfaces with the contract via the casper-client and succeeds or
errors out in reasonable ways.

Requirement | Finding
------------ | -------------
Project builds and runs without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Casper-Client Contract Calls work without error | PASS

# Unit / Automated Testing

Project contains 12 unit tests that can be executed from the console. Tests cover both positive and negative test paths.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

The scripts used in the manual test and the other scripts have command line documentation in them.

Requirement | Finding
------------ | -------------
Bash Scripts Documented | PASS

### Project Documentation

README.md has a large body of documentation and examples.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the Apache License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS (request for improvements)
------------ | -------------

