Grant Proposal | [151 - CASPER Earning Calculator and Node Monitor](https://portal.devxdao.com/public-proposals/151)
------------ | -------------
Milestone | 1
Milestone Title | New Features and Improvement of current site
OP | BlockShark
Reviewer | Muhammet Kara

# Milestone Details
This is the only and final milestone of the grant, thus there will be no option of passing with notes.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Improve the speed of Reward Calculation by using pre-calculated data from our dedicated server.
- Estimate Node Uptime and rank how stable each node is.
- Trusted List of Validator
- Black list of bad validator with (cheating/poor node performance)
- Validator Statistics with graphical chart interface to show: Node payment, node uptime, node delegation, node total stake

**Acceptance criteria:**

- Create API server to store pre-calculated and cached Casper blockchain data
- Server API secured via https
- Server API response in less than 5 seconds
- Server API returns: node information, general blockchain information, delegator information and earning information.
- Front-end shows APY, Uptime data, Node Name/Website and graphical chart of earnings (line chart)
- Uptime shows from 0% to 100%

**Additional notes regarding submission from OP:**



## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/nad128668/casper-calculator | 26ef4dd028d430acaba025da05864a6d243ebde5
https://github.com/nad128668/casper-calculator-api | 3c40be8c6c832d514f970be669071c5c6b0211b6

# Install & Usage Testing Procedure and Findings

The reviewer attempted to build and run the project following the instructions in the `CasperTool.docx` file under the `docs` directory of both repositories. Because no specific versions were mentioned by the OP, the latest/current versions of MongoDB (v5.0.4) and Node.js (v16.13.0) were installed as requirement. Ubuntu 20.04 LTS was used as the build and test environment.

At first attempt of building the `casper-calculator` repository, the `npm install` command failed with error
```bash
npm ERR! gyp verb `which` failed  python2 Error: not found: python2
```

The aforementioned error disappeared after installing the python2 package which was not mentioned anywhere in the given documentation. At second attempt of building the `casper-calculator` repository, the `npm install` command failed due to incompatible/outdated dependency on the `node-sass` package. This error was also eliminated by the reviewer by manually editing the source to upgrade the version of `node-sass` package to `6.0.1`.

At 3rd attempt to build the project after making the manual changes mentioned above, the build succeeded for both repositories.

Reviewer tried to run the project by following the instructions given in the repository. At first attempt, the `node casper-api.js` command given as part of the run instructions failed with error `ENOENT: no such file or directory, open './server.key'` which revealed that there was a need for certificates to run the `calculator-api` with SSL support although the front-end part was configured to run without SSL, and there was no mention of the needed certificates on the document given. Moreover, it was seen that no proper handling of the error was in place, and there was no documentation or explanation about it either.

Reviewer eliminated the error by creating the needed certificates by following outside sources found on a best-effort basis. However, at the next attempt of running the `calculator-api`, another error was encountered:
```
node casper-api.js failed with
		MongoNetworkError: failed to connect to server [127.0.0.1:27017] on first connect [Error: connect ECONNREFUSED 127.0.0.1:27017
		    at TCPConnectWrap.afterConnect [as oncomplete] (node:net:1161:16) {
		  name: 'MongoNetworkError'
		}]
```

Reviewer concluded that the above error might be due to an undocumented version incompatibility or misconfiguration, however he was not able to mitigate it with reasonable amount of effort within the scope of this review.

Reviewer then examined the sample installation provided by the OP to test the observable functionality. Based on the observations on the provided installation, the app seems generally functional, and providing the functional requirements promised. However, the validator count value seen on the app (109) doesn't match the real number of validators (100) on the network, effectively giving erroneous information to the users.

## Overall Impression of usage testing

The reviewer was not able to build or run the project by following the instructions provided on the repository. Observational usage tests were done on the provided sample installation. It was also observed that the sample installation is giving erroneous information to the users.

The documentation is missing the requirements and detailed configuration needed. Moreover, the repositories are missing README.md files which is the best-practice to provide general information and documentation for the open-source projects.


Requirement | Finding
------------ | -------------
Project builds without errors | FAIL
Documentation provides sufficient installation/execution instructions | FAIL
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL

# Unit / Automated Testing

No tests were found on either of the repositories.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL
Unit Tests - Additional path tests | FAIL

# Documentation

### Code Documentation

The document on the repository provides general information about the project and its architecture. However, the code-level documentation is very sparse. Most functions don't have documentation.

Requirement | Finding
------------ | -------------
Code Documented | FAIL

### Project Documentation

The project doesn't have README.md files on either of the repositories, but provides general documentation on the given document. The reviewer highly recommends adding README.md files, and properly documenting the project following the best-practices. However, as the general documentation is provided in another form, and the README.md file requirement was not clearly communicated before this submission, the usage documentation shall not be failed.

Requirement | Finding
------------ | -------------
Usage Documented | PASS

## Overall Conclusion on Documentation

The over-all documentation is not following the open-source best-practices, not easily discoverable, missing important parts as exact requirements. The code-level documentation is also mostly missing. Thus, in the opinion of this Reviewer, this submission should fail for not meeting the documentation requirements.

# Open Source Practices

## Licenses

The Project is released under the MIT License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled. However, the project does not contain a CONTRIBUTING policy. It is highly suggested that the OP should add a proper contribution policy to provide guidelines for the potential contributors as it is crucial for the sustainability of an open-source project. However, this is not a reason to fail the submission, in the reviewer's opinion.

Requirement | Finding
------------ | -------------
OSS contribution best practices | FAIL

# Coding Standards

## General Observations

The project has 7 high and 1 critical level security vulnerabilities in its dependencies, along with incompatible/outdated dependencies such as `node-sass`.

# Final Conclusion

The project is poorly documented, has security vulnerabilities, and gives erroneous information to the users. Thus, in the reviewer's opinion, this submission should fail.

# Recommendation

Recommendation | FAIL
------------ | -------------

