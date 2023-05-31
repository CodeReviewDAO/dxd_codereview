Grant Proposal | [718 - Casper Shops](https://portal.devxdao.com/public-proposals/718)
------------ | -------------
Milestone | 4
Milestone Title |  Payment Integration with CSPR token (100 hours)
OP | droplinked
Reviewer | Mehmet Sait Gülmez <cenggulmez.65@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Payment system integration via Stripe with CSPR settlement

**Acceptance criteria:**

Live integration with CasperPunks Shop

**Additional notes regarding submission from OP:**

Here you can review checkout with CSPR payment on products using the Casper Wallet: https://casper.droplinked.com Repo for Casper Shop: https://github.com/FLATLAY/droplinked_casper

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/FLATLAY/droplinked_casper | 00d6a0f


# Install & Usage Testing Procedure and Findings

The reviewer used Fedora Linux 35 for review of this project and followed instructions given on README. After reviewing the project, the reviewer observed that documentation needed some improvements, ```About``` section in github repository was empty, Deploy example on README file didn't work and negative test cases were not available. There were 5 integration tests. The reviewer's first attemp to build the project by following the instructions given on the README resulted in [failure](assets/fail-to-build-logs.md). However, it was successfully built after the reviewer has done some research on this issue. It was solved by running ```rustup target add wasm32-unknown-unknown``` then ```make build-contract``` commands in succession. The reviewer contacted to the OP to discuss on the issues mentioned above. OP immediately started to work on these issues. OP improved the project documentation, updated deploy command given on README, added description on github ```About``` section and also added more test cases both positive and negative test cases. 



## Overall Impression of usage testing

- [Build logs](assets/backend-build.md)

Example of sending WASM file to casper node and deploy it on the chain.

```bash
ndpc_contract (main)$ casper-client put-deploy -n http://89.58.52.245:7777 \
--chain-name casper-test --payment-amount 231420060000 \
-k keys/m.pem --session-path deploy/contract.wasm \
--session-arg "ratio_verifier:string='0144f5adf499591351807bc83490314262bd6846beee80a16269a83c9901ecec8a'" \
--session-arg "fee:u64='100'" \
--ttl "5hour"
{
  "id": 6348862178308581047,
  "jsonrpc": "2.0",
  "result": {
    "api_version": "1.4.15",
    "deploy_hash": "397b1cb7941f75e34a898e89caceac3fc6f51b4b1b9d7e353fc9ec948c44416e"
  }
}
```

Deploy the contract: https://testnet.cspr.live/deploy/397b1cb7941f75e34a898e89caceac3fc6f51b4b1b9d7e353fc9ec948c44416e


Documentation provides clear and sufficient instructions for build and installation.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS 

# Unit / Automated Testing

The project has 16 test cases which including both unit and integration tests. The reviewer observed that all of the tests successfully pass.

- [Unit and integration tests logs](assets/backend-tests.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS 
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation

The reviewer has observed that the project documentation is an acceptable level.

Requirement | Finding
------------ | -------------
Code Documented | PASS 

### Project Documentation

The project documentation is sufficient. However, it will be more clear and concise for the users of this project, if the OP provides a better example.

Requirement | Finding
------------ | -------------
Usage Documented | PASS 
Example Documented | PASS with Notes

## Overall Conclusion on Documentation

In the reviewer's opinion, documentation should be improved. The code-level documentation is sufficient.

# Open Source Practices

## Licenses

On the grant, It is stated that License will be Creative commons (for research and documents only) for this project. However, the reviewer observed that OP added MIT license to the repository.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

## Contribution Policies

The project contains a CONTRIBUTING and SECURITY policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS 

# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub and all 16 tests passed.

# Final Conclusion

The project builds successfully and passes all tests. The documentation is sufficient. Source code is well written and reviewer observed that standard comments were applied properly on the critical functions. This enables code-level documentation. However, the project documentation needs to be improved.

In the reviewers opinion, this submission should pass with notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------