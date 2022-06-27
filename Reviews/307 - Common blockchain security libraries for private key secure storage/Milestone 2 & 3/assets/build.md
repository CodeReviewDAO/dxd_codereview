## `build` Logs

*Developer's note: Compile TypeScript to JavaScript with declarations.*

```sh
review@crdao:~/devxdao/casper-storage $ yarn build
yarn run v1.22.19
$ tsc -p tsconfig.build.json --downlevelIteration
Done in 2.42s.
```


## `build-all` Logs

*Developer's note: To build the library to final output.*

```sh
review@crdao:~/devxdao/casper-storage $ yarn build-all
yarn run v1.22.19
$ yarn clean && yarn build && yarn esbuild-node && yarn esbuild-browser
$ rimraf dist build package coverage docs
$ tsc -p tsconfig.build.json --downlevelIteration
$ esbuild src/cli.ts --bundle --platform=node --minify --sourcemap=external --outfile=dist/esbuild/cli.js

  dist/esbuild/cli.js      315.1kb
  dist/esbuild/cli.js.map  955.7kb

$ esbuild src/browser.ts --bundle --minify --sourcemap=external --format=esm --outfile=dist/esbuild/browser.js

  dist/esbuild/browser.js      342.2kb
  dist/esbuild/browser.js.map    1.0mb

Done in 3.51s.
```