```sh
gitpod /workspace/casperfyre-backend (main) $ composer run-script test
> echo ; echo '[+] Running Unit Tests' ; echo ; ./vendor/bin/phpunit --testdox tests/Unit

[+] Running Unit Tests

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

Time: 00:03.767, Memory: 10.00 MB

OK (24 tests, 168 assertions)
```