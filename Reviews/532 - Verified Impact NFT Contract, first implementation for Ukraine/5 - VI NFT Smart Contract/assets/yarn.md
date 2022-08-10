```sh
gitpod /workspace/Verified-Impact-NFTs (main) $ yarn install
yarn install v1.22.19
[1/4] Resolving packages...
success Already up-to-date.
Done in 0.50s.
```

```sh
Compiled with warnings.

./src/css/templete.css (./node_modules/css-loader/dist/cjs.js??ref--5-oneOf-4-1!./node_modules/postcss-loader/src??postcss!./src/css/templete.css)
Warning

(3876:5) start value has mixed support, consider using flex-start instead

src/App.js
  Line 17:10:  'body_' is assigned a value but never used  no-unused-vars

src/api/userInfo.ts
  Line 6:10:  'parseNFT' is defined but never used  @typescript-eslint/no-unused-vars

src/markup/Element/BuyNFT.js
  Line 8:10:  'approve' is defined but never used  no-unused-vars

src/markup/Element/ListForSaleNFT.js
  Line 32:35:   Expected '===' and instead saw '=='  eqeqeq
  Line 64:27:   Expected '===' and instead saw '=='  eqeqeq
  Line 76:27:   Expected '===' and instead saw '=='  eqeqeq
  Line 104:27:  Expected '===' and instead saw '=='  eqeqeq

src/markup/Element/NFTCard.js
  Line 61:30:  Expected '===' and instead saw '=='  eqeqeq
  Line 71:31:  Expected '===' and instead saw '=='  eqeqeq

src/markup/Layout/Footer1.js
  Line 15:21:  Using target="_blank" without rel="noreferrer" (which implies rel="noopener") is a security risk in older browsers: see https://mathiasbynens.github.io/rel-noopener/#recommendations  react/jsx-no-target-blank
  Line 23:21:  Using target="_blank" without rel="noreferrer" (which implies rel="noopener") is a security risk in older browsers: see https://mathiasbynens.github.io/rel-noopener/#recommendations  react/jsx-no-target-blank

src/markup/Markup.js
  Line 1:17:  'Component' is defined but never used  no-unused-vars

src/markup/Pages/Admin/AddCampaign.js
  Line 203:49:  Expected '===' and instead saw '=='  eqeqeq
  Line 206:61:  Expected '===' and instead saw '=='  eqeqeq

src/markup/Pages/Admin/MintNFT.js
  Line 35:10:   'uploadingToCloud' is assigned a value but never used  no-unused-vars
  Line 260:61:  Expected '===' and instead saw '=='                    eqeqeq

src/markup/Pages/Index4.js
  Line 82:40:   Expected '===' and instead saw '=='             eqeqeq
  Line 412:21:  'camNumber' is assigned a value but never used  no-unused-vars
  Line 463:53:  Expected '===' and instead saw '=='             eqeqeq

src/markup/Pages/NFTDetail.js
  Line 46:58:  Expected '===' and instead saw '=='  eqeqeq

src/markup/Pages/NFTs/BenefeiciaryNFTs.js
  Line 36:14:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 37:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 40:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 41:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 44:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 109:6:   React Hook useEffect has missing dependencies: 'beneficiary' and 'campaign'. Either include them or remove the dependency array                                                                                                                                                               react-hooks/exhaustive-deps
  Line 132:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 142:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 180:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 190:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 230:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 240:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 306:40:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                           eqeqeq
  Line 485:6:   React Hook useEffect has missing dependencies: 'allCreators?.length', 'beneficiaries?.length', and 'searchFlag'. Either include them or remove the dependency array. You can also do a functional update 'setSearchFlag(s => ...)' if you only need 'searchFlag' in the 'setSearchFlag' call  react-hooks/exhaustive-deps
  Line 494:6:   React Hook useEffect has missing dependencies: 'handleSearch', 'tagCampaign', 'tagCollection', and 'tagCreator'. Either include them or remove the dependency array                                                                                                                           react-hooks/exhaustive-deps

src/markup/Pages/NFTs/CreatorNFTs.js
  Line 1:17:    'Component' is defined but never used                                                                                                                                                                                                                                                                                                                                                                          no-unused-vars
  Line 3:22:    'useLightbox' is defined but never used                                                                                                                                                                                                                                                                                                                                                                        no-unused-vars
  Line 35:14:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 36:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 39:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 40:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 43:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 114:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 124:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 162:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 172:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 210:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 220:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 285:40:  Expected '===' and instead saw '=='                                                                                                                                                                                                                                                                                                                                                                            eqeqeq
  Line 315:13:  Effect callbacks are synchronous to prevent race conditions. Put the async function inside:

useEffect(() => {
  async function fetchData() {
    // You can await here
    const response = await MyAPI.getData(someId);
    // ...
  }
  fetchData();
}, [someId]); // Or [] if effect doesn't need props or state

Learn more about data fetching with Hooks: https://reactjs.org/link/hooks-data-fetching  react-hooks/exhaustive-deps
  Line 454:6:   React Hook useEffect has missing dependencies: 'allCreators?.length', 'beneficiaries?.length', and 'searchFlag'. Either include them or remove the dependency array. You can also do a functional update 'setSearchFlag(s => ...)' if you only need 'searchFlag' in the 'setSearchFlag' call                                                                                                                   react-hooks/exhaustive-deps
  Line 463:6:   React Hook useEffect has missing dependencies: 'handleSearch', 'tagCampaign', 'tagCollection', and 'tagCreator'. Either include them or remove the dependency array                                                                                                                                                                                                                                            react-hooks/exhaustive-deps

src/markup/Pages/NFTs/MyCreations.js
  Line 1:17:    'Component' is defined but never used                                                                                                                                                                                                   no-unused-vars
  Line 3:22:    'useLightbox' is defined but never used                                                                                                                                                                                                 no-unused-vars
  Line 40:14:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 41:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 44:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 45:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 48:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 76:9:    'beneficiary' is assigned a value but never used                                                                                                                                                                                        no-unused-vars
  Line 115:27:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 126:28:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 147:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 157:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 195:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 205:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 243:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 253:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 480:6:   React Hook useEffect has a missing dependency: 'searchFlag'. Either include it or remove the dependency array. You can also do a functional update 'setSearchFlag(s => ...)' if you only need 'searchFlag' in the 'setSearchFlag' call  react-hooks/exhaustive-deps
  Line 489:6:   React Hook useEffect has missing dependencies: 'handleSearch', 'tagCampaign', 'tagCollection', and 'tagCreator'. Either include them or remove the dependency array                                                                     react-hooks/exhaustive-deps
  Line 506:23:  img elements must have an alt prop, either with meaningful text, or an empty string for decorative images                                                                                                                               jsx-a11y/alt-text

src/markup/Pages/NFTs/MyNFTs.js
  Line 1:17:    'Component' is defined but never used                                                                                                                                                                                                   no-unused-vars
  Line 3:22:    'useLightbox' is defined but never used                                                                                                                                                                                                 no-unused-vars
  Line 37:14:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 38:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 41:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 42:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 45:18:   Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 73:9:    'beneficiary' is assigned a value but never used                                                                                                                                                                                        no-unused-vars
  Line 116:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 126:41:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 164:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 174:39:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 212:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 222:38:  Expected '===' and instead saw '=='                                                                                                                                                                                                     eqeqeq
  Line 449:6:   React Hook useEffect has a missing dependency: 'searchFlag'. Either include it or remove the dependency array. You can also do a functional update 'setSearchFlag(s => ...)' if you only need 'searchFlag' in the 'setSearchFlag' call  react-hooks/exhaustive-deps
  Line 458:6:   React Hook useEffect has missing dependencies: 'handleSearch', 'tagCampaign', 'tagCollection', and 'tagCreator'. Either include them or remove the dependency array                                                                     react-hooks/exhaustive-deps

src/utils/contract-utils.ts
  Line 245:11:  'deployerTransfer' is assigned a value but never used     @typescript-eslint/no-unused-vars
  Line 247:11:  'beneficiaryTransfer' is assigned a value but never used  @typescript-eslint/no-unused-vars

Search for the keywords to learn more about each warning.
To ignore, add // eslint-disable-next-line to the line before.
```