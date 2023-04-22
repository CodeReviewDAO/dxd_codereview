# Server Test Logs

```
 PASS  tests/auth.test.js
 PASS  tests/surveys.test.js
  ● Console

    console.log
      Request body JSON: {"title":"Test Survey","questions":[{"text":"What is your favorite color?","answers":[{"text":"Red"},{"text":"Green"},{"text":"Blue"}]}],"startDate":"2023-04-13T15:19:07.414Z","endDate":"2023-04-13T15:19:07.414Z","createdBy":"64381d6bee4c5ac5bf2ed2cd","creationFee":10,"rewardPerResponse":1}

      at log (src/controllers/surveys.js:5:13)

 PASS  tests/users.test.js

Test Suites: 3 passed, 3 total
Tests:       12 passed, 12 total
Snapshots:   0 total
Time:        2.219 s, estimated 3 s
Ran all test suites.
```