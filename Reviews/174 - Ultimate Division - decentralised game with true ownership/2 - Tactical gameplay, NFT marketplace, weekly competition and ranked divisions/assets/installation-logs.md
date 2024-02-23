# Installation Logs

```sh
gitpod /workspace/ultimatedivision (develop) $ docker run --name=db -e POSTGRES_PASSWORD='123456' -p 5432:5432 -d --rm post
gres
Unable to find image 'postgres:latest' locally
latest: Pulling from library/postgres
faef57eae888: Pull complete 
a33c10a72186: Pull complete 
d662a43776d2: Pull complete 
a3ba86413420: Pull complete 
a627f37e9916: Pull complete 
424bade69494: Pull complete 
dd8d4fcd466b: Pull complete 
03d0efeea592: Pull complete 
4f27e1518a67: Pull complete 
0c8ac8b8eb90: Pull complete 
c08e79653ad2: Pull complete 
d5724e8c22af: Pull complete 
3db4aa0d2013: Pull complete 
Digest: sha256:362a63cb1e864195ea2bc29b5066bdb222bc9a4461bfaff2418f63a06e56bce0
Status: Downloaded newer image for postgres:latest
7dc712b86bdce6569ae381463ca79f6d55f86160726f9e36e16418ce960f8d17
gitpod /workspace/ultimatedivision (develop) $ docker exec -it db createdb -U postgres ultimatedivisiondb_test
gitpod /workspace/ultimatedivision (develop) $ go run cmd/ultimatedivision/main.go setup
gitpod /workspace/ultimatedivision (develop) $ go run cmd/currencysigner/main.go setup
gitpod /workspace/ultimatedivision (develop) $ go run cmd/nftsigner/main.go setup
```

```sh
gitpod /workspace/ultimatedivision (develop) $ cd web/console/
gitpod /workspace/ultimatedivision/web/console (develop) $ npm i --force && npm run build
npm WARN using --force Recommended protections disabled.
npm WARN deprecated w3c-hr-time@1.0.2: Use your platform's native performance.now() and performance.timeOrigin.
npm WARN deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
npm WARN deprecated workbox-cacheable-response@6.6.0: workbox-background-sync@6.6.0
npm WARN deprecated rollup-plugin-terser@7.0.2: This package has been deprecated and is no longer maintained. Please use @rollup/plugin-terser
npm WARN deprecated sourcemap-codec@1.4.8: Please use @jridgewell/sourcemap-codec instead
npm WARN deprecated mini-create-react-context@0.4.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @types/redux-thunk@2.1.0: This is a stub types definition for Redux Thunk (https://github.com/gaearon/redux-thunk). Redux Thunk provides its own type definitions, so you don't need @types/redux-thunk installed!
npm WARN deprecated @types/redux@3.6.0: This is a stub types definition for Redux (https://github.com/reactjs/redux). Redux provides its own type definitions, so you don't need @types/redux installed!
npm WARN deprecated @types/history@5.0.0: This is a stub types definition. history provides its own type definitions, so you do not need this installed.
npm WARN deprecated @stylelint/postcss-markdown@0.36.2: Use the original unforked package instead: postcss-markdown
npm WARN deprecated @stylelint/postcss-css-in-js@0.37.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated svgo@1.3.2: This SVGO version is no longer supported. Upgrade to v2.x.x.

added 1688 packages, and audited 1689 packages in 22s

361 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
npm notice 
npm notice New minor version of npm available! 9.5.1 -> 9.8.1
npm notice Changelog: https://github.com/npm/cli/releases/tag/v9.8.1
npm notice Run npm install -g npm@9.8.1 to update!
npm notice 

> cryptofotball@0.1.0 build
> webpack --mode production

(node:11990) [DEP_WEBPACK_TEMPLATE_PATH_PLUGIN_REPLACE_PATH_VARIABLES_HASH] DeprecationWarning: [hash] is now [fullhash] (also consider using [chunkhash] or [contenthash], see documentation for details)
(Use `node --trace-deprecation ...` to show where the warning was created)
assets by info 22.8 MiB [immutable] 115 assets
assets by path *.css 522 KiB
  asset 691.css 215 KiB [emitted] 1 related asset
  asset 453.css 58 KiB [emitted] 1 related asset
  + 17 assets
assets by path webGl/ 58.7 MiB
  assets by path webGl/*.js 272 KiB 2 assets
  asset webGl/Football.wasm 37.2 MiB [emitted] [from: src/app/static/webGl/Football.wasm] [copied] [big]
  asset webGl/Football.data 21.2 MiB [emitted] [from: src/app/static/webGl/Football.data] [copied] [big]
asset index.html 1.61 KiB [emitted]
asset favicon.ico 533 bytes [emitted]
Entrypoint main [big] 456 KiB (642 KiB) = 722.05df16d97dd5fe73da10.js 378 KiB main.css 24.3 KiB main.05df16d97dd5fe73da10.js 53.3 KiB 24 auxiliary assets
orphan modules 1.51 MiB [orphan] 318 modules
runtime modules 9.89 KiB 16 modules
modules by path ./ 3.01 MiB (javascript) 497 KiB (css/mini-extract) 20.3 MiB (asset)
  javascript modules 3.01 MiB
    modules by path ./node_modules/ 2.63 MiB 262 modules
    modules by path ./src/ 394 KiB 68 modules
  css modules 497 KiB
    modules by path ./src/app/components/ 409 KiB 46 modules
    modules by path ./src/app/views/ 68.9 KiB 15 modules
    modules by path ./node_modules/ 16 KiB 3 modules
    css ./node_modules/css-loader/dist/cjs.js!./node_modules/sass-loader/dist/cjs.js!./src/index.scss 3.11 KiB [built] [code generated]
  asset modules 2.54 KiB (javascript) 20.3 MiB (asset) 62 modules
optional modules 30 bytes [optional]
  buffer (ignored) 15 bytes [optional] [built] [code generated]
  buffer (ignored) 15 bytes [optional] [built] [code generated]

WARNING in asset size limit: The following asset(s) exceed the recommended size limit (244 KiB).
This can impact web performance.
Assets: 
  images/background9acd5.svg (309 KiB)
  images/represent-logo6583d.gif (11.7 MiB)
  images/diamondCardea9e0.webp (871 KiB)
  images/playing-field5117d.svg (1.93 MiB)
  images/player-left8406f.svg (1.85 MiB)
  images/player-right4c58e.svg (1.85 MiB)
  images/field-animationbeb31.webp (737 KiB)
  54.05df16d97dd5fe73da10.js (984 KiB)
  722.05df16d97dd5fe73da10.js (378 KiB)
  webGl/Football.data (21.2 MiB)
  webGl/Football.framework.js (252 KiB)
  webGl/Football.wasm (37.2 MiB)
  images/player-right4c58e.svg.br (1.36 MiB)
  images/player-left8406f.svg.br (1.36 MiB)
  images/playing-field5117d.svg.br (1.43 MiB)

WARNING in entrypoint size limit: The following entrypoint(s) combined asset size exceeds the recommended limit (244 KiB). This can impact web performance.
Entrypoints:
  main (456 KiB)
      722.05df16d97dd5fe73da10.js
      main.css
      main.05df16d97dd5fe73da10.js


webpack 5.88.2 compiled with 2 warnings in 35937 ms
gitpod /workspace/ultimatedivision (develop) $ go run cmd/ultimatedivision/main.go run
```