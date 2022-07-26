```
yusuf@Yusuf-MacBook-Pro dhf-pay-js % npm test

> dhf-pay-js@1.0.11 test
> jest --config jestconfig.json  src/e2e.test.ts

 PASS  src/e2e.test.ts
  Create payment
    ✓ Create Payment returns correctly (258 ms)
    ✓ Create Payment throws error on bad request (24 ms)
    ○ skipped Create Payment throws error on small amount
  Get payment
    ✓ Get payment returns correctly (119 ms)
    ✓ Get payment throws exception on bad request (3 ms)
  Get Payments
    ✓ Get Payments returns correctly (152 ms)
    ✓ Get Payments throws error on bad request (8 ms)
    ✓ Get Payments returns empty errors on bad token (127 ms)
  Get Transactions
    ✓ Get Transactions returns correctly (127 ms)
    ✓ Get Transactions  throws exception on bad request (3 ms)
    ✓ Get Transactions  return empty arr on bad token (122 ms)

Test Suites: 1 passed, 1 total
Tests:       1 skipped, 10 passed, 11 total
Snapshots:   0 total
Time:        3.759 s
Ran all test suites matching /src\/e2e.test.ts/i.
```
