```sh
gitpod /workspace/CasperLabs-Uniswap-DemoApp (main) $ npm run build

> uniswap-demo-app@0.1.0 build
> react-scripts build

Creating an optimized production build...
Compiled with warnings.

./src/app/components/Modals/AllowanceModal.js
  Line 1:10:  'Button' is defined but never used          no-unused-vars
  Line 1:54:  'InputAdornment' is defined but never used  no-unused-vars

./src/app/containers/Pages/Users/AddLiquidity.js
  Line 2:8:     'OutlinedInput' is defined but never used                  no-unused-vars
  Line 60:29:   'setApproveAIsLoading' is assigned a value but never used  no-unused-vars
  Line 61:29:   'setApproveBIsLoading' is assigned a value but never used  no-unused-vars
  Line 728:33:  'result' is assigned a value but never used                no-unused-vars

./src/app/components/Modals/TokenBModal.js
  Line 33:116:  Unexpected mix of '&&' and '||'  no-mixed-operators
  Line 33:139:  Unexpected mix of '&&' and '||'  no-mixed-operators
  Line 33:139:  Unexpected mix of '||' and '&&'  no-mixed-operators
  Line 33:173:  Unexpected mix of '||' and '&&'  no-mixed-operators

./src/app/components/Modals/TokenAModal.js
  Line 35:120:  Unexpected mix of '&&' and '||'  no-mixed-operators
  Line 35:143:  Unexpected mix of '&&' and '||'  no-mixed-operators
  Line 35:143:  Unexpected mix of '||' and '&&'  no-mixed-operators
  Line 35:177:  Unexpected mix of '||' and '&&'  no-mixed-operators

./src/app/containers/Pages/Users/Swap.js
  Line 3:8:      'OutlinedInput' is defined but never used                     no-unused-vars
  Line 58:27:    'setApproveAIsLoading' is assigned a value but never used     no-unused-vars
  Line 398:18:   'approveMakeDeploy' is defined but never used                 no-unused-vars
  Line 635:17:   'contractHashAsByteArray' is assigned a value but never used  no-unused-vars
  Line 638:17:   'entryPoint' is assigned a value but never used               no-unused-vars
  Line 748:17:   'contractHashAsByteArray' is assigned a value but never used  no-unused-vars
  Line 751:17:   'entryPoint' is assigned a value but never used               no-unused-vars
  Line 965:17:   'contractHashAsByteArray' is assigned a value but never used  no-unused-vars
  Line 968:17:   'entryPoint' is assigned a value but never used               no-unused-vars
  Line 1071:17:  'contractHashAsByteArray' is assigned a value but never used  no-unused-vars
  Line 1074:17:  'entryPoint' is assigned a value but never used               no-unused-vars

./src/app/containers/Pages/Users/RemoveLiquidity.js
  Line 4:10:   'AccessRights' is defined but never used                   no-unused-vars
  Line 77:29:  'setApproveAIsLoading' is assigned a value but never used  no-unused-vars
  Line 80:10:  'mainPurse' is assigned a value but never used             no-unused-vars

./src/app/components/Headers/Header.js
  Line 66:6:    React Hook useEffect has a missing dependency: 'alertUser'. Either include it or remove the dependency array                                                                                                                                                                                                                                                                      react-hooks/exhaustive-deps
  Line 162:6:   React Hook useEffect has missing dependencies: 'checkConnection', 'getActiveKeyFromSigner', 'props', and 'signerConnected'. Either include them or remove the dependency array. However, 'props' will change when *any* prop changes, so the preferred fix is to destructure the 'props' object outside of the useEffect call and refer to those specific props inside useEffect  react-hooks/exhaustive-deps
  Line 372:17:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/anchor-is-valid.md                  jsx-a11y/anchor-is-valid
  Line 383:17:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/anchor-is-valid.md                  jsx-a11y/anchor-is-valid
  Line 400:17:  The href attribute requires a valid value to be accessible. Provide a valid, navigable address as the href value. If you cannot provide a valid href, but still need the element to resemble a link, use a button and change it with appropriate styles. Learn more: https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/anchor-is-valid.md                  jsx-a11y/anchor-is-valid

./src/app/components/Modals/WalletModal.js
  Line 7:8:  'Torus' is defined but never used  no-unused-vars

Search for the keywords to learn more about each warning.
To ignore, add // eslint-disable-next-line to the line before.

File sizes after gzip:

  565.84 KB  build/static/js/2.72d2fa12.chunk.js
  55.61 KB   build/static/css/main.99a8ef89.chunk.css
  27.93 KB   build/static/js/main.7077ecc4.chunk.js
  781 B      build/static/js/runtime-main.0700cbc7.js

The project was built assuming it is hosted at /.
You can control this with the homepage field in your package.json.

The build folder is ready to be deployed.
You may serve it with a static server:

  npm install -g serve
  serve -s build

Find out more about deployment here:

  bit.ly/CRA-deploy
```

```sh
gitpod /workspace/CasperLabs-Uniswap-DemoApp (main) $ npm install -g serve
npm WARN config global `--global`, `--local` are deprecated. Use `--location=global` instead.

added 89 packages, and audited 90 packages in 4s

23 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```

```sh
gitpod /workspace/CasperLabs-Uniswap-DemoApp (main) $ npm install -g serve
npm WARN config global `--global`, `--local` are deprecated. Use `--location=global` instead.

added 89 packages, and audited 90 packages in 4s

23 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
gitpod /workspace/CasperLabs-Uniswap-DemoApp (main) $ serve -s build
ERROR: Cannot copy server address to clipboard: Couldn't find the `xsel` binary and fallback didn't work. On Debian/Ubuntu you can install xsel with: sudo apt install xsel.

   ┌───────────────────────────────────────────────┐
   │                                               │
   │   Serving!                                    │
   │                                               │
   │   - Local:            http://localhost:3000   │
   │   - On Your Network:  http://10.0.5.2:3000    │
   │                                               │
   └───────────────────────────────────────────────┘

^C
INFO: Gracefully shutting down. Please wait...
gitpod /workspace/CasperLabs-Uniswap-DemoApp (main) $
```