```
Run composer run-script test
> echo ; echo '[+] Running Unit Tests' ; echo ; ./vendor/bin/phpunit --testdox tests/Unit

[+] Running Unit Tests


[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created api_keys table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created ips table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created limits table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created orders table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created schedule table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created sessions table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created settings table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created user table
[CasperFYRE 2022-08-15T22:34:19+00:00] - Created admin
[CasperFYRE 2022-08-15T22:34:19+00:00] - Email:    [ADMIN_EMAIL]
[CasperFYRE 2022-08-15T22:34:19+00:00] - Password: Password123#
[CasperFYRE 2022-08-15T22:34:19+00:00] - Created test user
[CasperFYRE 2022-08-15T22:34:19+00:00] - Email:    casperfyre+integration-test@ledgerleap.com
[CasperFYRE 2022-08-15T22:34:19+00:00] - Password: Password123#
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created wallets table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created twofa table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created mfa_allowance table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created throttle table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created password_resets table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created email_changes table
[CasperFYRE 2022-08-15T22:34:19+00:00] - DB: Created totp table
PHPUnit 9.5.21 #StandWithUkraine

Core
 ✔ Filter
 ✔ Require method

Db
 ✔ Do query
 ✔ Do select
 ✔ Db cleanup

Helper
 ✔ Generate guid
 ✔ Generate api key
 ✔ Generate session token
 ✔ Generate hash
 ✔ Compare datetime
 ✔ Generate wallet
 ✔ Get wallet balance
 ✔ Get dir contents
 ✔ Aes encryption and decryption
 ✔ Correct validator id format
 ✔ Fail incorrect validator id format
 ✔ In cidr range
 ✔ Not in cidr range

Router
 ✔ Directory routes
 ✔ Router rules

Syntax
 ✔ Php syntax
Good syntax on public PHP files
Good syntax on classes PHP files
Good syntax on templates PHP files
Good syntax on tests PHP files

Throttler
 ✔ Throttled endpoints

Totp
 ✔ Totp create key
 ✔ Totp test code

Time: 00:05.379, Memory: 10.00 MB

OK (24 tests, 168 assertions)
```
