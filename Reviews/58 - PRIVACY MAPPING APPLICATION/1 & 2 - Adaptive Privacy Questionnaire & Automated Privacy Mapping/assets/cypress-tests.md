```
$ npm run cy:run

> mydpo-automation@1.0.0 cy:run
> ./node_modules/.bin/cypress run

[20212:1002/220301.447811:ERROR:zygote_host_impl_linux.cc(263)] Failed to adjust OOM score of renderer with pid 20382: Permission denied (13)
[20382:1002/220301.480057:ERROR:gpu_memory_buffer_support_x11.cc(44)] dri3 extension not supported.

====================================================================================================

  (Run Starting)

  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ Cypress:        10.4.0                                                                         │
  │ Browser:        Electron 102 (headless)                                                        │
  │ Node Version:   v16.17.1 (/home/gitpod/.nvm/versions/node/v16.17.1/bin/node)                   │
  │ Specs:          1 found (check-page.cy.js)                                                     │
  │ Searched:       cypress/e2e/**/*.cy.{js,jsx,ts,tsx}                                            │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘


────────────────────────────────────────────────────────────────────────────────────────────────────
                                                                                                    
  Running:  check-page.cy.js                                                                (1 of 1)
[20212:1002/220303.766589:ERROR:zygote_host_impl_linux.cc(263)] Failed to adjust OOM score of renderer with pid 20481: Permission denied (13)


  Check myDPO Page
    ✓ Check if the site is available (3009ms)
    ✓ Check if the email is invalid for authorization (7826ms)
    ✓ Check if the email is valid for authorization (7369ms)


  3 passing (18s)


  (Results)

  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ Tests:        3                                                                                │
  │ Passing:      3                                                                                │
  │ Failing:      0                                                                                │
  │ Pending:      0                                                                                │
  │ Skipped:      0                                                                                │
  │ Screenshots:  0                                                                                │
  │ Video:        true                                                                             │
  │ Duration:     18 seconds                                                                       │
  │ Spec Ran:     check-page.cy.js                                                                 │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘


  (Video)

  -  Started processing:  Compressing to 32 CRF                                                     
  -  Finished processing: /workspace/PRIVACYMAP/myDPO-automation/cypress/videos/check     (1 second)
                          -page.cy.js.mp4                                                           


====================================================================================================

  (Run Finished)


       Spec                                              Tests  Passing  Failing  Pending  Skipped  
  ┌────────────────────────────────────────────────────────────────────────────────────────────────┐
  │ ✔  check-page.cy.js                         00:18        3        3        -        -        - │
  └────────────────────────────────────────────────────────────────────────────────────────────────┘
    ✔  All specs passed!                        00:18        3        3        -        -        - 
```
