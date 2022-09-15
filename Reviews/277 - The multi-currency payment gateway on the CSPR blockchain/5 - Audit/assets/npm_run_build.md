'''
muharremsalel@Muharrems-MacBook-Pro dhf-pay-front % npm run build

> build
> next build

info  - Loaded env from /Users/muharremsalel/Desktop/CRDao/dhf-pay-front/.env
Attention: Next.js now collects completely anonymous telemetry regarding usage.
This information is used to shape Next.js' roadmap and prioritize features.
You can learn more, including how to opt-out if you'd not like to participate in this anonymous program, by visiting the following URL:
https://nextjs.org/telemetry

Browserslist: caniuse-lite is outdated. Please run:
  npx browserslist@latest --update-db
  Why you should do it regularly: https://github.com/browserslist/browserslist#browsers-data-updating
info  - Checking validity of types  

./src/components/Forms/Bill/index.tsx
157:6  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps
169:6  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/InvoicesBuilder/index.tsx
46:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
56:8  Warning: React Hook useEffect has missing dependencies: 'activeStores', 'dispatch', and 'user.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/Login/index.tsx
63:8  Warning: React Hook useEffect has missing dependencies: 'form', 'userData.email', and 'userData.password'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
118:8  Warning: React Hook useEffect has a missing dependency: 'userData'. Either include it or remove the dependency array. You can also do a functional update 'setUserData(u => ...)' if you only need 'userData' in the 'setUserData' call.  react-hooks/exhaustive-deps

./src/components/Forms/PaymentsButton/index.tsx
47:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/Register/index.tsx
91:8  Warning: React Hook useEffect has a missing dependency: 'form'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps
95:26  Warning: Assignments to the 'fieldError' variable from inside React Hook useEffect will be lost after each render. To preserve the value over time, store it in a useRef Hook and keep the mutable value in the '.current' property. Otherwise, you can move this variable directly inside useEffect.  react-hooks/exhaustive-deps
104:8  Warning: React Hook useEffect has a missing dependency: 'userData'. Either include it or remove the dependency array. You can also do a functional update 'setUserData(u => ...)' if you only need 'userData' in the 'setUserData' call.  react-hooks/exhaustive-deps
255:8  Warning: React Hook useEffect has missing dependencies: 'fieldError' and 'form'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/Restore/index.tsx
82:8  Warning: React Hook useEffect has a missing dependency: 'form'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps
105:8  Warning: React Hook useEffect has a missing dependency: 'userData'. Either include it or remove the dependency array. You can also do a functional update 'setUserData(u => ...)' if you only need 'userData' in the 'setUserData' call.  react-hooks/exhaustive-deps
186:8  Warning: React Hook useEffect has missing dependencies: 'fieldError' and 'form'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/Payment/index.tsx
75:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
82:8  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/Store/index.tsx
77:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/Transaction/index.tsx
57:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/User/index.tsx
32:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/ReCaptcha/ReCaptcha.tsx
21:6  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Paymets/index.tsx
53:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
70:8  Warning: React Hook useEffect has missing dependencies: 'activeStores', 'dispatch', and 'user.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
76:8  Warning: React Hook useEffect has a missing dependency: 'currentStore'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Stores/index.tsx
89:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'user.id'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Transactions/index.tsx
59:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
65:8  Warning: React Hook useEffect has missing dependencies: 'activeStores', 'dispatch', and 'user.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Users/index.tsx
42:8  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

info  - Need to disable some ESLint rules? Learn more here: https://nextjs.org/docs/basic-features/eslint#disabling-rules
info  - Disabled SWC as replacement for Babel because of custom Babel configuration ".babelrc" https://nextjs.org/docs/messages/swc-disabled
Browserslist: caniuse-lite is outdated. Please run:
npx browserslist@latest --update-db

Why you should do it regularly:
https://github.com/browserslist/browserslist#browsers-data-updating
info  - Using external babel configuration from /Users/muharremsalel/Desktop/CRDao/dhf-pay-front/.babelrc
(node:21981) [DEP_WEBPACK_MODULE_UPDATE_HASH] DeprecationWarning: Module.updateHash: Use new ChunkGraph API
(Use `node --trace-deprecation ...` to show where the warning was created)
info  - Creating an optimized production build  
info  - Compiled successfully
info  - Collecting page data ...secp256k1 unavailable, reverting to browser version
secp256k1 unavailable, reverting to browser version
secp256k1 unavailable, reverting to browser version
secp256k1 unavailable, reverting to browser version
info  - Collecting page data  
[    ] info  - Generating static pages (0/19)secp256k1 unavailable, reverting to browser version
secp256k1 unavailable, reverting to browser version
secp256k1 unavailable, reverting to browser version
secp256k1 unavailable, reverting to browser version
info  - Generating static pages (19/19)
info  - Finalizing page optimization  

Page                                       Size     First Load JS
┌ ○ /                                      1.67 kB         205 kB
├   /_app                                  0 B             102 kB
├ ○ /404                                   2.85 kB         105 kB
├ λ /api/hello                             0 B             102 kB
├ ○ /bill/[slug] (381 ms)                  54.7 kB         486 kB
├ ○ /buttons                               357 B           281 kB
├ ○ /buttons/[slug]                        401 B           248 kB
├ ○ /buttonsBuilder                        3.96 kB         252 kB
├ ○ /invoices                              352 B           281 kB
├ ○ /invoices/[slug]                       397 B           248 kB
├ ○ /invoicesBuilder                       3.08 kB         251 kB
├ ○ /login                                 6.1 kB          230 kB
├ ○ /register                              6.01 kB         230 kB
├ ○ /restore                               6.06 kB         230 kB
├ ○ /stores (364 ms)                       3.2 kB          523 kB
├ ○ /stores/[slug] (363 ms)                5.27 kB         467 kB
├ ○ /transactions                          2.18 kB         280 kB
├ ○ /transactions/[slug] (304 ms)          3.15 kB         436 kB
├ ○ /users                                 1.84 kB         280 kB
└ ○ /users/[slug]                          3.07 kB         216 kB
+ First Load JS shared by all              102 kB
  ├ chunks/framework-bb5c596eafb42b22.js   42.1 kB
  ├ chunks/main-8a0fe121e379d1aa.js        29.9 kB
  ├ chunks/pages/_app-fcb2e068f3039844.js  28.3 kB
  ├ chunks/webpack-fa1c5fe73b1a0886.js     1.6 kB
  └ css/b3ff8ad54ff5b445.css               272 B

λ  (Server)  server-side renders at runtime (uses getInitialProps or getServerSideProps)
○  (Static)  automatically rendered as static HTML (uses no initial props)

'''