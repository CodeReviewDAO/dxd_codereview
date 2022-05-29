```sh
review@crdao:~/casperholdersfront (main)$ yarn build-testnet

yarn run v1.22.19
$ vue-cli-service build --mode testnet

 WARNING  Compiled with 20 warnings4:40:57 AM

Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/components/layout/Connect.vue
  569:9  warning  Unexpected console statement  no-console
  611:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/components/operations/OperationResult.vue
  329:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/components/operations/Validators.vue
  241:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/helpers/genericSendDeploy.js
  63:9  warning  Unexpected console statement  no-console
  82:5  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/account/AccountInfo.vue
  239:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/account/Balance.vue
  292:11  warning  Unexpected console statement  no-console
  313:9   warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/account/Security.vue
  617:11  warning  Unexpected console statement  no-console
  691:9   warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/account/Transfer.vue
  275:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/developers/SmartContract.vue
  189:9  warning  Unexpected console statement  no-console
  245:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/multisig/MultiSig.vue
  458:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/staking/Delegate.vue
  233:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/staking/Undelegate.vue
  198:9  warning  Unexpected console statement  no-console
  230:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/validators/AddBid.vue
  261:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/review/casperholdersfront/src/views/validators/WithdrawBid.vue
  253:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


You may use special comments to disable some warnings.
Use // eslint-disable-next-line to ignore the next line.
Use /* eslint-disable */ to ignore all warnings in a file.
 warning  in ./src/store/index.js

Module Warning (from ./node_modules/thread-loader/dist/cjs.js):

/home/review/casperholdersfront/src/store/index.js
  275:7  warning  Unexpected console statement  no-console
  360:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


 @ ./src/main.js 104:0-28 113:9-14
 @ multi ./src/main.js

 warning  

chunk account-view~addbid-view~balance-view~settings-view~smartcontract-view~stake-view~transfer-view~unst~52c4e50f [mini-css-extract-plugin]
Conflicting order. Following module has been added:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VInput/VInput.sass
despite it was not able to fulfill desired ordering with these modules:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VTextField/VTextField.sass
   - couldn't fulfill desired order of chunk group(s) balance-view, transfer-view, account-view, stake-view, unstake-view, addbid-view, withdrawbid-view, smartcontract-view
   - while fulfilling desired order of chunk group(s) settings-view

 warning  

chunk account-view~addbid-view~balance-view~settings-view~smartcontract-view~stake-view~transfer-view~unst~52c4e50f [mini-css-extract-plugin]
Conflicting order. Following module has been added:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VLabel/VLabel.sass
despite it was not able to fulfill desired ordering with these modules:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VTextField/VTextField.sass
   - couldn't fulfill desired order of chunk group(s) balance-view, transfer-view, account-view, stake-view, unstake-view, addbid-view, withdrawbid-view, smartcontract-view
   - while fulfilling desired order of chunk group(s) settings-view

 warning  

chunk account-view~addbid-view~balance-view~settings-view~smartcontract-view~stake-view~transfer-view~unst~52c4e50f [mini-css-extract-plugin]
Conflicting order. Following module has been added:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VMessages/VMessages.sass
despite it was not able to fulfill desired ordering with these modules:
 * css ./node_modules/css-loader/dist/cjs.js??ref--10-oneOf-3-1!./node_modules/postcss-loader/src??ref--10-oneOf-3-2!./node_modules/sass-loader/dist/cjs.js??ref--10-oneOf-3-3!./node_modules/vuetify/src/components/VTextField/VTextField.sass
   - couldn't fulfill desired order of chunk group(s) balance-view, transfer-view, account-view, stake-view, unstake-view, addbid-view, withdrawbid-view, smartcontract-view
   - while fulfilling desired order of chunk group(s) settings-view

 warning  

asset size limit: The following asset(s) exceed the recommended size limit (244 KiB).
This can impact web performance.
Assets: 
  js/balance-view.6d769cac.js (561 KiB)
  css/chunk-vendors.56303a1f.css (366 KiB)
  js/chunk-vendors.51e07848.js (2.02 MiB)

 warning  

entrypoint size limit: The following entrypoint(s) combined asset size exceeds the recommended limit (244 KiB). This can impact web performance.
Entrypoints:
  app (2.56 MiB)
      css/chunk-vendors.56303a1f.css
      js/chunk-vendors.51e07848.js
      css/app.6b1608e7.css
      js/app.f326fcff.js


  File                                      Size             Gzipped

  dist/js/chunk-vendors.51e07848.js         2067.07 KiB      630.34 KiB
  dist/js/balance-view.6d769cac.js          561.13 KiB       145.68 KiB
  dist/js/balance-view~home-view~stake-v    201.03 KiB       66.56 KiB
  iew.310a22a0.js
  dist/js/app.f326fcff.js                   191.92 KiB       39.49 KiB
  dist/js/stake-view.101558f9.js            114.56 KiB       26.79 KiB
  dist/js/account-view~addbid-view~balan    100.74 KiB       21.77 KiB
  ce-view~smartcontract-view~stake-view~
  transfer-view~unstake-view~withd~486a3
  9ec.78abc697.js
  dist/js/home-view.eb4ea2ae.js             75.59 KiB        18.05 KiB
  dist/js/contact-view.fb874a67.js          69.97 KiB        10.72 KiB
  dist/js/unstake-view.6d3755cc.js          56.61 KiB        12.36 KiB
  dist/js/addbid-view.1c99a230.js           32.18 KiB        8.93 KiB
  dist/js/settings-view.1f5f6969.js         28.87 KiB        7.19 KiB
  dist/js/balance-view~unstake-view.cd60    26.68 KiB        7.54 KiB
  6aa6.js
  dist/js/transfer-view.2c802858.js         26.24 KiB        6.77 KiB
  dist/js/account-view~addbid-view~balan    24.79 KiB        6.94 KiB
  ce-view~settings-view~smartcontract-vi
  ew~stake-view~transfer-view~unst~52c4e
  50f.1c4ee662.js
  dist/js/smartcontract-view.d31f6632.js    24.34 KiB        6.89 KiB
  dist/js/account-view.23b0e908.js          21.30 KiB        5.80 KiB
  dist/js/withdrawbid-view.6463f3bc.js      20.61 KiB        5.44 KiB
  dist/js/addbid-view~smartcontract-view    18.72 KiB        4.26 KiB
  ~stake-view~transfer-view~unstake-view
  ~withdrawbid-view.88bc0289.js
  dist/js/faq-view.8c54250b.js              6.57 KiB         2.00 KiB
  dist/precache-manifest.d800119f992b63f    4.56 KiB         1.25 KiB
  7646493b208f66907.js
  dist/service-worker.js                    1.02 KiB         0.48 KiB
  dist/css/chunk-vendors.56303a1f.css       365.79 KiB       44.19 KiB
  dist/css/account-view~addbid-view~bala    22.82 KiB        3.11 KiB
  nce-view~settings-view~smartcontract-v
  iew~stake-view~transfer-view~unst~52c4
  e50f.ed7a7d4f.css
  dist/css/balance-view.ab7462e1.css        11.53 KiB        1.85 KiB
  dist/css/account-view~addbid-view~bala    9.49 KiB         1.95 KiB
  nce-view~smartcontract-view~stake-view
  ~transfer-view~unstake-view~withd~486a
  39ec.1311a611.css
  dist/css/addbid-view.2d728a8a.css         6.27 KiB         1.22 KiB
  dist/css/stake-view.294c150b.css          5.54 KiB         1.26 KiB
  dist/css/balance-view~unstake-view.500    5.29 KiB         1.16 KiB
  529fb.css
  dist/css/settings-view.cf6fe5fe.css       3.83 KiB         0.96 KiB
  dist/css/home-view.dc456265.css           3.21 KiB         0.75 KiB
  dist/css/app.6b1608e7.css                 1.41 KiB         0.66 KiB
  dist/css/smartcontract-view.76a811a3.c    1.36 KiB         0.38 KiB
  ss
  dist/css/unstake-view.f20af4b7.css        0.06 KiB         0.08 KiB

  Images and other types of assets omitted.

 DONE  Build complete. The dist directory is ready to be deployed.
 INFO  Check out deployment instructions at https://cli.vuejs.org/guide/deployment.html
      
Done in 138.77s.
```