```
yusuf@ubuntu:~$ git clone https://github.com/casperholders/casperholdersfront
Cloning into 'casperholdersfront'...
remote: Enumerating objects: 2522, done.
remote: Counting objects: 100% (422/422), done.
remote: Compressing objects: 100% (192/192), done.
remote: Total 2522 (delta 268), reused 233 (delta 230), pack-reused 2100
Receiving objects: 100% (2522/2522), 2.73 MiB | 522.00 KiB/s, done.
Resolving deltas: 100% (1630/1630), done.
yusuf@ubuntu:~$ cd casperholdersfront/
yusuf@ubuntu:~/casperholdersfront$ ls
babel.config.js     kubernetes    README.md                 vue.config.js
CODE_OF_CONDUCT.md  LICENSE       SECURITY.md               yarn.lock
CONTRIBUTING.md     nginx.conf    sonar-project.properties
cypress.json        package.json  src
Dockerfile          public        tests
yusuf@ubuntu:~/casperholdersfront$ yarn --version
1.22.18
yusuf@ubuntu:~/casperholdersfront$ yarn install
yarn install v1.22.18
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
warning "@casperholders/core > casper-js-sdk > eslint-plugin-prettier@3.4.1" has unmet peer dependency "prettier@>=1.13.0".
warning " > @toruslabs/casper-embed@1.2.0" has unmet peer dependency "@babel/runtime@7.x".
warning "@toruslabs/casper-embed > @toruslabs/base-controllers@1.6.11" has unmet peer dependency "@babel/runtime@7.x".
warning "@toruslabs/casper-embed > @toruslabs/http-helpers@2.2.0" has unmet peer dependency "@babel/runtime@7.x".
warning "@toruslabs/casper-embed > @toruslabs/openlogin-jrpc@1.7.0" has unmet peer dependency "@babel/runtime@7.x".
warning "@toruslabs/casper-embed > @toruslabs/openlogin-jrpc > @toruslabs/openlogin-utils@1.7.0" has unmet peer dependency "@babel/runtime@7.x".
warning " > @vue/eslint-config-airbnb@5.3.0" has unmet peer dependency "eslint-plugin-import@^2.18.2".
warning "@vue/eslint-config-airbnb > eslint-import-resolver-webpack@0.13.2" has unmet peer dependency "webpack@>=1.11.0".
warning " > sass-loader@10.2.1" has unmet peer dependency "webpack@^4.36.0 || ^5.0.0".
warning "vue-cli-plugin-vuetify > null-loader@4.0.1" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
warning " > vuetify-loader@1.7.3" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
warning "vuetify-loader > file-loader@6.2.0" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
[4/4] Building fresh packages...
Done in 103.34s.

yusuf@ubuntu:~/casperholdersfront$ yarn serve
yarn run v1.22.18
$ vue-cli-service serve
 INFO  Starting development server...
98% after emitting CopyPlugin

 DONE  Compiled successfully in 35945ms                                                                                                                             8:18:51 PM


  App running at:
  - Local:   http://localhost:8080/ 
  - Network: http://192.168.0.105:8080/

  Note that the development build is not optimized.
  To create a production build, run yarn build.

^C
yusuf@ubuntu:~/casperholdersfront$ yarn test:e2e
yarn test:e2e
yarn run v1.22.18
$ vue-cli-service test:e2e
 INFO  Starting e2e tests...
 INFO  Starting development server...


 WARNING  Compiled with 20 warnings                                                                                                                                 8:19:49 PM

Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/components/layout/Connect.vue
  569:9  warning  Unexpected console statement  no-console
  611:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/components/operations/OperationResult.vue
  329:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/components/operations/Validators.vue
  241:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/account/AccountInfo.vue
  239:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/account/Balance.vue
  292:11  warning  Unexpected console statement  no-console
  313:9   warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/account/Security.vue
  617:11  warning  Unexpected console statement  no-console
  691:9   warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/account/Transfer.vue
  275:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/developers/SmartContract.vue
  189:9  warning  Unexpected console statement  no-console
  245:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/multisig/MultiSig.vue
  458:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/staking/Delegate.vue
  233:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/staking/Undelegate.vue
  198:9  warning  Unexpected console statement  no-console
  230:9  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/validators/AddBid.vue
  261:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


Module Warning (from ./node_modules/eslint-loader/index.js):

/home/yusuf/casperholdersfront/src/views/validators/WithdrawBid.vue
  253:9  warning  Unexpected console statement  no-console

✖ 1 problem (0 errors, 1 warning)


You may use special comments to disable some warnings.
Use // eslint-disable-next-line to ignore the next line.
Use /* eslint-disable */ to ignore all warnings in a file.
 warning  in ./src/helpers/genericSendDeploy.js

Module Warning (from ./node_modules/thread-loader/dist/cjs.js):

/home/yusuf/casperholdersfront/src/helpers/genericSendDeploy.js
  63:9  warning  Unexpected console statement  no-console
  82:5  warning  Unexpected console statement  no-console

✖ 2 problems (0 errors, 2 warnings)


 @ ./node_modules/cache-loader/dist/cjs.js??ref--13-0!./node_modules/thread-loader/dist/cjs.js!./node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--1-0!./node_modules/vue-loader/lib??vue-loader-options!./src/views/developers/SmartContract.vue?vue&type=script&lang=js& 1052:0-60 1281:23-40
 @ ./src/views/developers/SmartContract.vue?vue&type=script&lang=js&
 @ ./src/views/developers/SmartContract.vue
 @ ./src/router/index.js
 @ ./src/main.js
 @ multi ./src/main.js

 warning  in ./src/store/index.js

Module Warning (from ./node_modules/thread-loader/dist/cjs.js):

/home/yusuf/casperholdersfront/src/store/index.js
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
  js/balance-view.55b19395.js (561 KiB)
  css/chunk-vendors.56303a1f.css (366 KiB)
  js/chunk-vendors.ff301da6.js (2.02 MiB)

 warning  

entrypoint size limit: The following entrypoint(s) combined asset size exceeds the recommended limit (244 KiB). This can impact web performance.
Entrypoints:
  app (2.56 MiB)
      css/chunk-vendors.56303a1f.css
      js/chunk-vendors.ff301da6.js
      css/app.6b1608e7.css
      js/app.91e561da.js
```
