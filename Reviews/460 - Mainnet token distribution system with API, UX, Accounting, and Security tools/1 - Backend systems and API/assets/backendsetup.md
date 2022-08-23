```sh
gitpod /workspace/casperfyre-backend (main) $ ./setup.sh 
Setting up CasperFYRE API..

Is this for a dev build? (y/n) >y
DEV BUILD
Your email address (Admin email)
Your email: crdaotest@ggurbet.com
Generating entropy...
Keys created
Configuring...
Checking for required software...
Hit:1 http://ppa.launchpad.net/git-core/ppa/ubuntu focal InRelease
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease                   
Get:3 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]  
Get:5 http://ppa.launchpad.net/ondrej/apache2/ubuntu focal InRelease [23.8 kB]
Get:6 http://ppa.launchpad.net/ondrej/nginx-mainline/ubuntu focal InRelease [23.8 kB]
Get:7 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Get:8 https://download.docker.com/linux/ubuntu focal InRelease [57.7 kB] 
Get:9 http://ppa.launchpad.net/ondrej/php/ubuntu focal InRelease [23.9 kB]
Get:11 http://ppa.launchpad.net/ondrej/apache2/ubuntu focal/main amd64 Packages [5,142 B]
Get:10 https://apt.llvm.org/focal llvm-toolchain-focal InRelease [6,824 B]
Get:12 http://security.ubuntu.com/ubuntu focal-security/main amd64 Packages [2,047 kB]
Get:13 http://security.ubuntu.com/ubuntu focal-security/universe amd64 Packages [886 kB]
Get:14 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 Packages [1,416 kB]
Get:15 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 Packages [27.5 kB]
Get:16 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages [1,175 kB]
Get:17 http://archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 Packages [30.2 kB]
Get:18 http://archive.ubuntu.com/ubuntu focal-updates/restricted amd64 Packages [1,525 kB]
Get:19 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages [2,498 kB]
Get:20 http://ppa.launchpad.net/ondrej/nginx-mainline/ubuntu focal/main amd64 Packages [6,415 B]
Get:21 http://archive.ubuntu.com/ubuntu focal-backports/universe amd64 Packages [27.5 kB]
Get:22 http://archive.ubuntu.com/ubuntu focal-backports/main amd64 Packages [55.2 kB]
Get:23 http://ppa.launchpad.net/ondrej/php/ubuntu focal/main amd64 Packages [170 kB]
Get:24 https://download.docker.com/linux/ubuntu focal/stable amd64 Packages [19.8 kB]
Get:25 https://apt.llvm.org/focal llvm-toolchain-focal/main amd64 Packages [12.4 kB]
Fetched 10.4 MB in 1s (10.8 MB/s)                            
Reading package lists... Done
PHP installed
Installing Casper Client
deb https://repo.casperlabs.io/releases bionic main
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--  100  3179  100  3179    0     0  39737      0 --:--:-- --:--:-- --:--:-- 39737
OK
Hit:1 http://archive.ubuntu.com/ubuntu focal InRelease
Hit:2 http://ppa.launchpad.net/git-core/ppa/ubuntu focal InRelease       
Hit:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease           
Hit:5 https://download.docker.com/linux/ubuntu focal InRelease           
Hit:6 http://archive.ubuntu.com/ubuntu focal-backports InRelease         
Hit:7 http://ppa.launchpad.net/ondrej/apache2/ubuntu focal InRelease     
Hit:8 http://ppa.launchpad.net/ondrej/nginx-mainline/ubuntu focal InRelease
Hit:9 http://ppa.launchpad.net/ondrej/php/ubuntu focal InRelease
Hit:10 http://security.ubuntu.com/ubuntu focal-security InRelease
Hit:3 https://apt.llvm.org/focal llvm-toolchain-focal InRelease
Get:11 https://repo.casperlabs.io/releases bionic InRelease [3,170 B]
Get:12 https://repo.casperlabs.io/releases bionic/main amd64 Packages [5,548 B]
Fetched 8,718 B in 1s (5,964 B/s)      
Reading package lists... Done
Building dependency tree       
Reading state information... Done
26 packages can be upgraded. Run 'apt list --upgradable' to see them.
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following NEW packages will be installed:
  casper-client
0 upgraded, 1 newly installed, 0 to remove and 26 not upgraded.
Need to get 3,720 kB of archives.
After this operation, 18.2 MB of additional disk space will be used.
Get:1 https://repo.casperlabs.io/releases bionic/main amd64 casper-client amd64 1.5.0-0+bionic [3,720 kB]
Fetched 3,720 kB in 0s (12.6 MB/s)  
debconf: delaying package configuration, since apt-utils is not installed
Selecting previously unselected package casper-client.
(Reading database ... 36091 files and directories currently installed.)
Preparing to unpack .../casper-client_1.5.0-0+bionic_amd64.deb ...
Unpacking casper-client (1.5.0-0+bionic) ...
Setting up casper-client (1.5.0-0+bionic) ...
Reading package lists... Done
Building dependency tree       
Reading state information... Done
curl is already the newest version (7.68.0-1ubuntu2.12).
0 upgraded, 0 newly installed, 0 to remove and 26 not upgraded.
No composer.lock file present. Updating dependencies to latest instead of installing from lock file. See https://getcomposer.org/install for more information.
Loading composer repositories with package information
Info from https://repo.packagist.org: #StandWithUkraine
Updating dependencies
Lock file operations: 40 installs, 0 updates, 0 removals
  - Locking beberlei/assert (v3.3.2)
  - Locking doctrine/instantiator (1.4.1)
  - Locking myclabs/deep-copy (1.11.0)
  - Locking nikic/php-parser (v4.14.0)
  - Locking paragonie/constant_time_encoding (v2.6.3)
  - Locking paragonie/random_compat (v9.99.100)
  - Locking paragonie/sodium_compat (v1.17.1)
  - Locking phar-io/manifest (2.0.3)
  - Locking phar-io/version (3.2.1)
  - Locking phpdocumentor/reflection-common (2.2.0)
  - Locking phpdocumentor/reflection-docblock (5.3.0)
  - Locking phpdocumentor/type-resolver (1.6.1)
  - Locking phpmailer/phpmailer (v6.6.3)
  - Locking phpspec/prophecy (v1.15.0)
  - Locking phpunit/php-code-coverage (9.2.15)
  - Locking phpunit/php-file-iterator (3.0.6)
  - Locking phpunit/php-invoker (3.1.1)
  - Locking phpunit/php-text-template (2.0.4)
  - Locking phpunit/php-timer (5.0.3)
  - Locking phpunit/phpunit (9.5.21)
  - Locking sebastian/cli-parser (1.0.1)
  - Locking sebastian/code-unit (1.0.8)
  - Locking sebastian/code-unit-reverse-lookup (2.0.3)
  - Locking sebastian/comparator (4.0.6)
  - Locking sebastian/complexity (2.0.2)
  - Locking sebastian/diff (4.0.4)
  - Locking sebastian/environment (5.1.4)
  - Locking sebastian/exporter (4.0.4)
  - Locking sebastian/global-state (5.0.5)
  - Locking sebastian/lines-of-code (1.0.3)
  - Locking sebastian/object-enumerator (4.0.4)
  - Locking sebastian/object-reflector (2.0.4)
  - Locking sebastian/recursion-context (4.0.4)
  - Locking sebastian/resource-operations (3.0.3)
  - Locking sebastian/type (3.0.0)
  - Locking sebastian/version (3.0.2)
  - Locking spomky-labs/otphp (v10.0.3)
  - Locking thecodingmachine/safe (v2.2.3)
  - Locking theseer/tokenizer (1.2.1)
  - Locking webmozart/assert (1.11.0)
Writing lock file
Installing dependencies from lock file (including require-dev)
Package operations: 40 installs, 0 updates, 0 removals
  - Downloading paragonie/random_compat (v9.99.100)
  - Downloading paragonie/sodium_compat (v1.17.1)
  - Downloading webmozart/assert (1.11.0)
  - Downloading phpdocumentor/reflection-common (2.2.0)
  - Downloading phpdocumentor/type-resolver (1.6.1)
  - Downloading phpdocumentor/reflection-docblock (5.3.0)
  - Downloading phpmailer/phpmailer (v6.6.3)
  - Downloading sebastian/version (3.0.2)
  - Downloading sebastian/type (3.0.0)
  - Downloading sebastian/resource-operations (3.0.3)
  - Downloading sebastian/recursion-context (4.0.4)
  - Downloading sebastian/object-reflector (2.0.4)
  - Downloading sebastian/object-enumerator (4.0.4)
  - Downloading sebastian/global-state (5.0.5)
  - Downloading sebastian/exporter (4.0.4)
  - Downloading sebastian/environment (5.1.4)
  - Downloading sebastian/diff (4.0.4)
  - Downloading sebastian/comparator (4.0.6)
  - Downloading sebastian/code-unit (1.0.8)
  - Downloading sebastian/cli-parser (1.0.1)
  - Downloading phpunit/php-timer (5.0.3)
  - Downloading phpunit/php-text-template (2.0.4)
  - Downloading phpunit/php-invoker (3.1.1)
  - Downloading phpunit/php-file-iterator (3.0.6)
  - Downloading theseer/tokenizer (1.2.1)
  - Downloading nikic/php-parser (v4.14.0)
  - Downloading sebastian/lines-of-code (1.0.3)
  - Downloading sebastian/complexity (2.0.2)
  - Downloading sebastian/code-unit-reverse-lookup (2.0.3)
  - Downloading phpunit/php-code-coverage (9.2.15)
  - Downloading doctrine/instantiator (1.4.1)
  - Downloading phpspec/prophecy (v1.15.0)
  - Downloading phar-io/version (3.2.1)
  - Downloading phar-io/manifest (2.0.3)
  - Downloading myclabs/deep-copy (1.11.0)
  - Downloading phpunit/phpunit (9.5.21)
  - Downloading thecodingmachine/safe (v2.2.3)
  - Downloading paragonie/constant_time_encoding (v2.6.3)
  - Downloading beberlei/assert (v3.3.2)
  - Downloading spomky-labs/otphp (v10.0.3)
  - Installing paragonie/random_compat (v9.99.100): Extracting archive
  - Installing paragonie/sodium_compat (v1.17.1): Extracting archive
  - Installing webmozart/assert (1.11.0): Extracting archive
  - Installing phpdocumentor/reflection-common (2.2.0): Extracting archive
  - Installing phpdocumentor/type-resolver (1.6.1): Extracting archive
  - Installing phpdocumentor/reflection-docblock (5.3.0): Extracting archive
  - Installing phpmailer/phpmailer (v6.6.3): Extracting archive
  - Installing sebastian/version (3.0.2): Extracting archive
  - Installing sebastian/type (3.0.0): Extracting archive
  - Installing sebastian/resource-operations (3.0.3): Extracting archive
  - Installing sebastian/recursion-context (4.0.4): Extracting archive
  - Installing sebastian/object-reflector (2.0.4): Extracting archive
  - Installing sebastian/object-enumerator (4.0.4): Extracting archive
  - Installing sebastian/global-state (5.0.5): Extracting archive
  - Installing sebastian/exporter (4.0.4): Extracting archive
  - Installing sebastian/environment (5.1.4): Extracting archive
  - Installing sebastian/diff (4.0.4): Extracting archive
  - Installing sebastian/comparator (4.0.6): Extracting archive
  - Installing sebastian/code-unit (1.0.8): Extracting archive
  - Installing sebastian/cli-parser (1.0.1): Extracting archive
  - Installing phpunit/php-timer (5.0.3): Extracting archive
  - Installing phpunit/php-text-template (2.0.4): Extracting archive
  - Installing phpunit/php-invoker (3.1.1): Extracting archive
  - Installing phpunit/php-file-iterator (3.0.6): Extracting archive
  - Installing theseer/tokenizer (1.2.1): Extracting archive
  - Installing nikic/php-parser (v4.14.0): Extracting archive
  - Installing sebastian/lines-of-code (1.0.3): Extracting archive
  - Installing sebastian/complexity (2.0.2): Extracting archive
  - Installing sebastian/code-unit-reverse-lookup (2.0.3): Extracting archive
  - Installing phpunit/php-code-coverage (9.2.15): Extracting archive
  - Installing doctrine/instantiator (1.4.1): Extracting archive
  - Installing phpspec/prophecy (v1.15.0): Extracting archive
  - Installing phar-io/version (3.2.1): Extracting archive
  - Installing phar-io/manifest (2.0.3): Extracting archive
  - Installing myclabs/deep-copy (1.11.0): Extracting archive
  - Installing phpunit/phpunit (9.5.21): Extracting archive
  - Installing thecodingmachine/safe (v2.2.3): Extracting archive
  - Installing paragonie/constant_time_encoding (v2.6.3): Extracting archive
  - Installing beberlei/assert (v3.3.2): Extracting archive
  - Installing spomky-labs/otphp (v10.0.3): Extracting archive
12 package suggestions were added by new dependencies, use `composer suggest` to see details.
Generating autoload files
26 packages you are using are looking for funding.
Use the `composer fund` command to find out more!
Loading composer repositories with package information
Updating dependencies
Nothing to modify in lock file
Installing dependencies from lock file (including require-dev)
Nothing to install, update or remove
Generating autoload files
26 packages you are using are looking for funding.
Use the `composer fund` command to find out more!
> echo ; echo '[+] Running Unit Tests' ; echo ; ./vendor/bin/phpunit --testdox tests/Unit

[+] Running Unit Tests


[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created api_keys table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created ips table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created limits table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created orders table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created schedule table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created sessions table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created settings table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created user table
[CasperFYRE 2022-08-09T13:00:51+00:00] - Created admin
[CasperFYRE 2022-08-09T13:00:51+00:00] - Email:    crdaotest@ggurbet.com
[CasperFYRE 2022-08-09T13:00:51+00:00] - Password: Password123#
[CasperFYRE 2022-08-09T13:00:51+00:00] - Created test user
[CasperFYRE 2022-08-09T13:00:51+00:00] - Email:    casperfyre+integration-test@ledgerleap.com
[CasperFYRE 2022-08-09T13:00:51+00:00] - Password: Password123#
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created wallets table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created twofa table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created mfa_allowance table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created throttle table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created password_resets table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created email_changes table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created totp table
[CasperFYRE 2022-08-09T13:00:51+00:00] - DB: Created totp_logins tablePHPUnit 9.5.21 #StandWithUkraine

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

Time: 00:03.985, Memory: 10.00 MB

OK (24 tests, 168 assertions)
[+] Done

Please note, you will need to setup emailer credentials information in your .env before the email scheduler will work.

BACKUP YOUR MASTER KEY --> 31ce287f7d94aa07ba4637ca20c7f219
Wallet keys/token balances will be lost if this key is lost.
gitpod /workspace/casperfyre-backend (main) $
```

```sh
gitpod /workspace/casperfyre-backend (main) $ apachectl start
```