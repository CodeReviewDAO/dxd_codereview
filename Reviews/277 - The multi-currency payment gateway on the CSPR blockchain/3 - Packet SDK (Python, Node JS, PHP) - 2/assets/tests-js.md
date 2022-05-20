```

dhf-pay-js % npm test

> dhf-pay-js@1.0.10 test /Users/th/rep/dhf/dhf-pay-js
> jest --config jestconfig.json  src/e2e.test.ts

 PASS  src/e2e.test.ts
  Create payment
    ✓ Create Payment returns correctly (491 ms)
    ✓ Create Payment throws error on bad request (20 ms)
    ○ skipped Create Payment throws error on small amount
  Get payment
    ✓ Get payment returns correctly (437 ms)
    ✓ Get payment throws exception on bad request (3 ms)
  Get Payments
    ✓ Get Payments returns correctly (297 ms)
    ✓ Get Payments throws error on bad request (3 ms)
    ✓ Get Payments returns empty errors on bad token (216 ms)
  Get Transactions
    ✓ Get Transactions returns correctly (235 ms)
    ✓ Get Transactions  throws exception on bad request (3 ms)
    ✓ Get Transactions  return empty arr on bad token (262 ms)

Test Suites: 1 passed, 1 total
Tests:       1 skipped, 10 passed, 11 total
Snapshots:   0 total
Time:        4.704 s, estimated 6 s
Ran all test suites matching /src\/e2e.test.ts/i.


```
