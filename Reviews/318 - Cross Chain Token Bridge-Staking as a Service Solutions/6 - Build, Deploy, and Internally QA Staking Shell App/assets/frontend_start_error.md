```bash
Starting the development server...

Error: error:0308010C:digital envelope routines::unsupported
    at new Hash (node:internal/crypto/hash:71:19)
    at Object.createHash (node:crypto:133:10)
    at module.exports (/workspace/staking-casper-frontend/node_modules/webpack/lib/util/createHash.js:135:53)
    at NormalModule._initBuildHash (/workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:417:16)
    at handleParseError (/workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:471:10)
    at /workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:503:5
    at /workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:358:12
    at /workspace/staking-casper-frontend/node_modules/loader-runner/lib/LoaderRunner.js:373:3
    at iterateNormalLoaders (/workspace/staking-casper-frontend/node_modules/loader-runner/lib/LoaderRunner.js:214:10)
    at iterateNormalLoaders (/workspace/staking-casper-frontend/node_modules/loader-runner/lib/LoaderRunner.js:221:10)
/workspace/staking-casper-frontend/node_modules/react-scripts/scripts/start.js:19
  throw err;
  ^

Error: error:0308010C:digital envelope routines::unsupported
    at new Hash (node:internal/crypto/hash:71:19)
    at Object.createHash (node:crypto:133:10)
    at module.exports (/workspace/staking-casper-frontend/node_modules/webpack/lib/util/createHash.js:135:53)
    at NormalModule._initBuildHash (/workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:417:16)
    at /workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:452:10
    at /workspace/staking-casper-frontend/node_modules/webpack/lib/NormalModule.js:323:13
    at /workspace/staking-casper-frontend/node_modules/loader-runner/lib/LoaderRunner.js:367:11
    at /workspace/staking-casper-frontend/node_modules/loader-runner/lib/LoaderRunner.js:233:18
    at context.callback (/workspace/staking-casper-frontend/node_modules/loader-runner/lib/LoaderRunner.js:111:13)
    at /workspace/staking-casper-frontend/node_modules/react-scripts/node_modules/babel-loader/lib/index.js:59:103 {
  opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
  library: 'digital envelope routines',
  reason: 'unsupported',
  code: 'ERR_OSSL_EVP_UNSUPPORTED'
}

Node.js v18.16.0
```