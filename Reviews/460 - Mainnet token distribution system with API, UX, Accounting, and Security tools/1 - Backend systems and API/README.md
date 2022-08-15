Grant Proposal | [460 - Mainnet token distribution system with API, UX, Accounting, and Security tools](https://portal.devxdao.com/public-proposals/460)
------------ | -------------
Milestone | 1
Milestone Title | Backend systems and API - Submission 1
OP | LedgerLeap
Reviewer | Gökhan Gurbetoğlu <crdao@ggurbet.com>


# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

The first of 2 milestones will deliver the system backend environment for CSPR distribution. This includes the ability to generate keys for API access and whitelist the IPs able to use these keys. The system will also assess daily and per transaction rate limits. A token transfer system will send CSPR mainnet tokens if the key is valid, the IP of the request is approved, and the transfer does not surpass rate limits. Keyholders will also provide the address to which the CSPR tokens will go. All transfers will be recorded in a database along with the pertinent security information to verify the sender. The API will have clear error codes for invalid requests. The first milestone expects to have 2 developers assigned for 8 to 9 days to build these features in an optimal way that supports the next milestone built on top.

**Acceptance criteria:**

The environment will support installation, and testing will begin by registering an API key and IP address. Once registered, the system will allow a test send of CSPR by submitting a request including the key, recipient address, and amount of CSPR. The system will check the rate limit logic, then send CSPR and log the transaction if approved.

**Additional notes regarding submission from OP:**

The URL of the backend API staging deployment is at: https://api.casperfyre.com/  
Backend API has been updated and finished to include all required endpoints, throttling, security, documentation, and unit tests. Some test orders have been executed using a test account with 500 CSPR initially deposited. Transactions purposefully meant to succeed have been verified on chain.  
This simple use guide can be followed:
 - Any user can register to use the portal and verify their account application.
 - Your admin must accept your application from the admin panel. Staging credentials for an admin account will be provided discretely.
 - After your application is accepted and your account is active, you can create new API keys, wallets, and whitelist your company IP addresses.
 - Upon account activation, a wallet and API key is automatically issued and displayed on your dashboard. The IP address you applied from will also automatically be added to your whitelist.
 - Deposit some CSPR to your wallet. All keys are kept encrypted and recoverable using server software keys.
 - Use/test the public facing API using the automatically generated documentation found in your dashboard settings as a reference.
A full description and usage guide instruction can be found at https://github.com/ledgerleapllc/casperfyre-backend/blob/main/README.md

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/ledgerleapllc/casperfyre-backend | 1dd0d51


# Install & Usage Testing Procedure and Findings

Reviewer used an Ubuntu 20.04 LTS Gitpod cloud machine and Ubuntu 20.04 LTS GitHub Codespaces cloud machine to test the review.

Reviewer followed instructions given on the README to install the software without errors and connected the frontend to backend successfully.

- [Installation logs](assets/backendsetup.md)

Further user testing was done on [casperfyre.com](https://casperfyre.com/) live instance provided by OP.

### Admin user

OP provided an admin account for the reviewer. Reviewer also signed up for three test accounts manually. Reviewer used the login screen to enter the dashboard. A note here is that `Next` button stays this color even after entering some credentials (implying it is disabled) but sometimes it turns to a more vibrant shade of red (implying it is enabled). Regardless of its color, it is clickable. It would be nice to address this issue.

![](assets/1_login.png)

After an admin logs in, they can approve and deny user applications, check existing API keys and user wallets, and manually change many other settings.

Admin dashboard:

![](assets/admin_dashboard.png)

### Regular user

A regular user can sign up using the greeting screen. They will then need to verify their email address with a verification code sent to their email address. After that, an admin needs to manually approve the registered user. After approval user will receive a greeting email with the confimation of their approval. Similarly, if the user's application is denied, they receive an email stating that.

After a regular user approved and they log in, the dashboard looks like this:

![](assets/2_dashboard.png)

Settings page, where user can set their daily and monthly transaction limits:
 
![](assets/3_settings.png)

Keys and wallets page:

![](assets/4_keys.png)

### Testing rate limit logic

#### Successful transaction

Reviewer set their transfer limits like this:

- Daily limit: 5
- Monthly limit: 10

Then, reviewer made a transfer attempt using the command line with an amount of CSPR 3 from user1 to user2:

```sh
# First transfer, daily limit: 5, monthly limit: 10
ggurbet@harezmi:~/casperfyre $ curl -X POST https://api.casperfyre.com/v1/dispense \
-H 'Content-type: application/json' \
-H 'Authorization: token 04f3fef526b972aad200e28ae8e80ba47e55614b2cf50568e543bf109e9bf27f' \
-d '{ "address": "01d640467ae680e3dae6567c192590cefa28a3c5e4332b88017584d585ea8cc483", "amount": 3 }'
{"status":"success","detail":"Dispensing 3 CSPR to 01d640467ae680e3dae6567c192590cefa28a3c5e4332b88017584d585ea8cc483"}
```

The operation completed successfully and response received. After the operation, details could be seen from the logs screen:

![](assets/5_successful_transaction.png)

Sender's logs:

![](assets/6_after_successful_transaction_sender.png)

Clicking Recipient hash on this screen goes to the respective wallet of the recipient user and clicking on the Deploy Hash goes to the respective deploy hash, both on cspr.live.

Recipient's logs:

![](assets/7_after_successful_transaction_recipient.png)

_Note: Since recipient did not make the transaction, no log is created on their side._

#### Unsuccessful transactions

Then, according to the acceptance criteria, user should not be able to make transfers exceeding their daily and monthly limits. So, reviewer made another transaction attempt of CSPR 3, which with the previous transaction (CSPR 3), makes a total of CSPR 6 which now exceeds the daily transaction limit of CSPR 5.

```sh
# After making a transfer of 3, with the daily limit still 5
ggurbet@harezmi:~/casperfyre $ curl -X POST https://api.casperfyre.com/v1/dispense -H 'Content-type: application/json' \
-H 'Authorization: token 04f3fef526b972aad200e28ae8e80ba47e55614b2cf50568e543bf109e9bf27f' \
-d '{ "address": "01d640467ae680e3dae6567c192590cefa28a3c5e4332b88017584d585ea8cc483", "amount": 3 }'
{"status":"error","detail":"You cannot dispense this many CSPR. You have 2 remaining for today"}
```

As expected, operation failed with the reason given in the response.

Reviewer then adjusted the monthly limit to CSPR 4 and tried to make another transaction of CSPR 3, which would eventually fail due to monthly limit excession.

```sh
# After setting the monthly limit to 4 and having already made a transfer of 3
ggurbet@harezmi:~/casperfyre $ curl -X POST https://api.casperfyre.com/v1/dispense \
-H 'Content-type: application/json' \
-H 'Authorization: token 04f3fef526b972aad200e28ae8e80ba47e55614b2cf50568e543bf109e9bf27f' \
-d '{ "address": "01d640467ae680e3dae6567c192590cefa28a3c5e4332b88017584d585ea8cc483", "amount": 3 }'
{"status":"error","detail":"You cannot dispense this many CSPR. You have 1 remaining for this month"}
```

This also failed, as expected, and proper response was provided.

We can see the transaction logs in the frontend:

![](assets/8_exceeding_limits.png)

A reviewer's note, when clicking on the `View` button on failed transactions, the failure response is not stated. It would be nicer to state them as they are already provided with the command line API call.

### Denying an application

Admin can deny a user's application from the Applications screen:

![](assets/9_deny_user.png)

## Overall Impression of usage testing

Project works as expected. It builds without errors and its functionality covers the acceptance criteria for this milestone.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

All automated unit tests PASS for this milestone. Testing is done via PHPUnit and contains automated tests that cover critical functionality. Reviewer successfully run all automated tests on an Ubuntu 20.04 LTS Gitpod cloud machine. Overall quality of tests are sufficient. Test output is below.

- [Unit tests logs](assets/unit-tests.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

Code documentation is very well prepared and is of high quality. All critical functionality of the code is commented. Many other helping comments and documentation are provided within the code and they are well prepared and detailed.

- [Docs build logs](assets/docs.md)

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

Reviewer was able to generate the necessary documentation provided with the instructions. The documentation includes key components, how to install and run the proect and usage examples.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation for the project is sufficient for this milestone.


# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Project contains clear CONTRIBUTING and SECURITY policies. Pull requests and Issues are enabled on the repository and the project is set up for public participation.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Source code is well-written and thought out. It is easily readable. General best coding practices are used throughout the project. Overall sufficient work is done.


# Final Conclusion

Project is in a working state and it covers the acceptance criteria for this milestone. Reviewer suggests this milestone to PASS.


# Recommendation

Recommendation | PASS
------------ | -------------
