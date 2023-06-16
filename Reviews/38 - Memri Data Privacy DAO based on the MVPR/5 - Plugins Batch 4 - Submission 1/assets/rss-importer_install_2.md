```
$ git clone https://github.com/postlight/parser-api.git
cd parser-api
yarn install
yarn serve
Cloning into 'parser-api'...
remote: Enumerating objects: 109, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 109 (delta 1), reused 10 (delta 1), pack-reused 97
Receiving objects: 100% (109/109), 504.58 KiB | 1.88 MiB/s, done.
Resolving deltas: 100% (43/43), done.
yarn install v1.22.19
warning package.json: License should be a valid SPDX license expression
warning parser-api@0.0.1: License should be a valid SPDX license expression
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
warning "serverless > @serverless/components > inquirer-autocomplete-prompt@1.4.0" has unmet peer dependency "inquirer@^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0".
warning "serverless-webpack > ts-node@10.7.0" has unmet peer dependency "@types/node@*".
warning "@postlight/parser@2.2.2" is missing a bundled dependency "jquery". This should be reported to the package maintainer.
warning "@postlight/parser@2.2.2" is missing a bundled dependency "moment-timezone". This should be reported to the package maintainer.
warning "@postlight/parser@2.2.2" is missing a bundled dependency "browser-request". This should be reported to the package maintainer.
[4/4] Building fresh packages...
Done in 6.90s.
yarn run v1.22.19
warning package.json: License should be a valid SPDX license expression
$ serverless offline start
Serverless: Bundling with Webpack...

  Error --------------------------------------------------

  Error: error:0308010C:digital envelope routines::unsupported
      at new Hash (node:internal/crypto/hash:71:19)
      at Object.createHash (node:crypto:133:10)
      at module.exports (Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\webpack\lib\util\createHash.js:135:53)
      at NormalModule._initBuildHash (Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\webpack\lib\NormalModule.js:417:16)
      at handleParseError (Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\webpack\lib\NormalModule.js:471:10)
      at Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\webpack\lib\NormalModule.js:503:5
      at Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\webpack\lib\NormalModule.js:358:12
      at Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\loader-runner\lib\LoaderRunner.js:373:3
      at iterateNormalLoaders (Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\loader-runner\lib\LoaderRunner.js:214:10)
      at iterateNormalLoaders (Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\loader-runner\lib\LoaderRunner.js:221:10)
      at Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\loader-runner\lib\LoaderRunner.js:236:3
      at context.callback (Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\loader-runner\lib\LoaderRunner.js:111:13)
      at Z:\CRDAO\4 - Plugins Batch 4 - Submission 1\rss-importer-dev\parser-api\node_modules\babel-loader\lib\index.js:59:71
      at processTicksAndRejections (node:internal/process/task_queues:95:5)

     For debugging logs, run again after setting the "SLS_DEBUG=*" environment variable.

  Get Support --------------------------------------------
     Docs:          docs.serverless.com
     Bugs:          github.com/serverless/serverless/issues
     Issues:        forum.serverless.com

  Your Environment Information ---------------------------
     Operating System:          win32
     Node Version:              18.15.0
     Framework Version:         1.83.3 (local)
     Plugin Version:            3.8.4
     SDK Version:               2.3.2
     Components Version:        2.34.9

error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```