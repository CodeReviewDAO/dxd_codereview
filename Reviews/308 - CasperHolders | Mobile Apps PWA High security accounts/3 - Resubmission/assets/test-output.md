```sh
yarn run v1.22.19
$ vue-cli-service test:e2e
 INFO  Starting e2e tests...
 INFO  Starting development server...
 WARNING  Compiled with 5 warnings12:24:04 PM

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
  js/balance-view.f7b265d8.js (561 KiB)
  css/chunk-vendors.56303a1f.css (366 KiB)
  js/chunk-vendors.84da9535.js (2.02 MiB)

 warning  

entrypoint size limit: The following entrypoint(s) combined asset size exceeds the recommended limit (244 KiB). This can impact web performance.
Entrypoints:
  app (2.56 MiB)
      css/chunk-vendors.56303a1f.css
      js/chunk-vendors.84da9535.js
      css/app.6b1608e7.css
      js/app.b23d4adc.js



  App running at:
  - Local:   http://localhost:8080/ 
  - Network: http://192.168.2.101:8080/

  App is served in production mode.
  Note this is for preview or E2E testing only.

Done in 59.58s.
```