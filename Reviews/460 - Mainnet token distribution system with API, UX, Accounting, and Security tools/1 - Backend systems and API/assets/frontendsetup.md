```sh
gitpod /workspace/casperfyre-frontend (main) $ yarn install
yarn install v1.22.19
info No lockfile found.
[1/4] Resolving packages...
warning react-scripts > @svgr/webpack > @svgr/plugin-svgo > svgo@1.3.2: This SVGO version is no longer supported. Upgrade to v2.x.x.
warning react-scripts > @svgr/webpack > @svgr/plugin-svgo > svgo > stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
warning react-scripts > css-minimizer-webpack-plugin > cssnano > cssnano-preset-default > postcss-svgo > svgo > stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
[2/4] Fetching packages...
[3/4] Linking dependencies...
warning " > @testing-library/user-event@13.5.0" has unmet peer dependency "@testing-library/dom@>=7.21.4".
warning "react-scripts > eslint-config-react-app > eslint-plugin-flowtype@8.0.3" has unmet peer dependency "@babel/plugin-syntax-flow@^7.14.5".
warning "react-scripts > eslint-config-react-app > eslint-plugin-flowtype@8.0.3" has unmet peer dependency "@babel/plugin-transform-react-jsx@^7.14.9".
warning "react-scripts > react-dev-utils > fork-ts-checker-webpack-plugin@6.5.2" has unmet peer dependency "typescript@>= 2.7".
warning "react-scripts > eslint-config-react-app > @typescript-eslint/eslint-plugin > tsutils@3.21.0" has unmet peer dependency "typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta".
[4/4] Building fresh packages...
success Saved lockfile.
Done in 41.04s.
gitpod /workspace/casperfyre-frontend (main) $
```

```sh
gitpod /workspace/casperfyre-frontend (main) $ yarn build
yarn run v1.22.19
$ react-scripts build
Creating an optimized production build...
Compiled successfully.

File sizes after gzip:

  101.09 kB  build/static/js/main.ba27b4a3.js
  20.83 kB   build/static/js/184.af3bb153.chunk.js
  12.31 kB   build/static/js/964.a55ef649.chunk.js
  9.54 kB    build/static/js/74.8c100cfc.chunk.js
  9.24 kB    build/static/js/134.5a088c15.chunk.js
  8.08 kB    build/static/js/809.7147c5ec.chunk.js
  6.23 kB    build/static/js/671.c8382979.chunk.js
  6.21 kB    build/static/css/main.c832c53e.css
  6.09 kB    build/static/js/102.28b0e9b8.chunk.js
  5.86 kB    build/static/js/268.00bc9120.chunk.js
  4.96 kB    build/static/js/926.a8c95e68.chunk.js
  4.42 kB    build/static/js/311.180df9f9.chunk.js
  4.4 kB     build/static/js/924.68f74f89.chunk.js
  4.3 kB     build/static/js/36.af41bb5b.chunk.js
  3.88 kB    build/static/js/898.300b498b.chunk.js
  3.49 kB    build/static/js/460.f9ff7ca8.chunk.js
  3.12 kB    build/static/js/7.965cda5a.chunk.js
  2.82 kB    build/static/js/730.cfa98945.chunk.js
  2.64 kB    build/static/js/843.e2876fa1.chunk.js
  2.11 kB    build/static/js/445.31104edb.chunk.js
  2.06 kB    build/static/js/297.cfce2b52.chunk.js
  1.87 kB    build/static/js/368.e8bac147.chunk.js
  1.86 kB    build/static/css/809.c8993926.chunk.css
  1.84 kB    build/static/css/460.45adb00e.chunk.css
  1.78 kB    build/static/js/787.82adfcd8.chunk.js
  1.69 kB    build/static/js/846.e84571a7.chunk.js
  1.68 kB    build/static/js/304.635aca1b.chunk.js
  1.65 kB    build/static/css/926.ce3b4594.chunk.css
  1.48 kB    build/static/css/843.115ed38b.chunk.css
  1.46 kB    build/static/js/910.3b1010fa.chunk.js
  1.41 kB    build/static/css/898.664be4af.chunk.css
  1.41 kB    build/static/css/445.440af624.chunk.css
  1.41 kB    build/static/css/910.75f9549f.chunk.css
  1.39 kB    build/static/css/36.43ed8213.chunk.css
  1.39 kB    build/static/css/730.029ec073.chunk.css
  1.38 kB    build/static/css/690.3d317fc5.chunk.css
  1.37 kB    build/static/js/690.e7779534.chunk.js
  1.29 kB    build/static/js/421.bb26bba1.chunk.js
  1.28 kB    build/static/css/297.710cc1aa.chunk.css
  1.16 kB    build/static/css/102.9404197a.chunk.css
  1.16 kB    build/static/css/304.9404197a.chunk.css
  1.16 kB    build/static/css/421.9404197a.chunk.css
  1.16 kB    build/static/css/846.9404197a.chunk.css
  1.16 kB    build/static/css/964.9404197a.chunk.css
  1.16 kB    build/static/css/50.9404197a.chunk.css
  1.16 kB    build/static/css/74.9404197a.chunk.css
  929 B      build/static/css/311.d6800cab.chunk.css
  769 B      build/static/css/368.2f154b63.chunk.css
  691 B      build/static/js/50.a1e42871.chunk.js
  574 B      build/static/js/848.92882027.chunk.js
  224 B      build/static/js/153.7a09a5e8.chunk.js

The project was built assuming it is hosted at /.
You can control this with the homepage field in your package.json.

The build folder is ready to be deployed.
You may serve it with a static server:

  yarn global add serve
  serve -s build

Find out more about deployment here:

  https://cra.link/deployment

Done in 29.58s.
gitpod /workspace/casperfyre-frontend (main) $
```

```sh
gitpod /workspace/casperfyre-frontend (main) $ yarn dev
Starting the development server...

Compiled successfully!

You can now view casperfyre in the browser.

  Local:            http://localhost:3000
  On Your Network:  http://10.0.5.2:3000

Note that the development build is not optimized.
To create a production build, use yarn build.

webpack compiled successfully
```