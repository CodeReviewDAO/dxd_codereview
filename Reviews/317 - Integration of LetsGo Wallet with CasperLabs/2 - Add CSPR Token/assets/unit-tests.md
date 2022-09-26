```sh
root@caspergo:/var/www# npm test

> chat-bot-api@1.0.1 test
> jest

 PASS  ./milestone.2.test.js (11.764 s)
  ✓ Load homepage of public website (38 ms)
  ✓ Manage CSPR keys using a simple key manager to allow for custodial accounts (3130 ms)
  ✓ Generate CSPR keys using a simple key manager to allow for custodial accounts in a deterministic pattern which can be backed up using a BIP39 seed phrase (1671 ms)
  ✓ Monitor blocks (monitor each block looking for specific addresses, when a transaction is pending / confirmed, we can trigger an update on that specific user account to prevent system polling) and Monitor balances (based on the block monitor) (40 ms)
  ✓ Send transactions (compile, sign and deliver) (954 ms)

Test Suites: 1 passed, 1 total
Tests:       5 passed, 5 total
Snapshots:   0 total
Time:        11.888 s
Ran all test suites.
```
