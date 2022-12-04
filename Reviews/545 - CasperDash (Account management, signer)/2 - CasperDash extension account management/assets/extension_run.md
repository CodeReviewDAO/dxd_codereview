'''
yarn run v1.22.19
warning ../../../../package.json: No license field
$ webpack --mode development --env=type=extension --env=network=testnet --watch
{
  output: {
    filename: 'static/js/[name].js',
    assetModuleFilename: 'assets/images/[name][ext][query]',
    chunkFilename: 'static/js/[name].js',
    path: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/build_extension'
  },
  module: {
    rules: [
      {
        test: /\.(js|jsx)$/,
        use: {
          loader: 'babel-loader',
          options: { plugins: [ '@babel/plugin-syntax-top-level-await' ] }
        }
      },
      {
        test: /\.(css|scss)$/,
        use: [
          '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/node_modules/mini-css-extract-plugin/dist/loader.js',
          'css-loader',
          'sass-loader'
        ]
      },
      { test: /\.html$/, use: [ 'html-loader' ] },
      { test: /\.(?:ico|gif|png|jpg|jpeg)$/i, type: 'asset/resource' },
      { test: /\.svg$/, use: [ '@svgr/webpack' ] }
    ]
  },
  plugins: [
    ProvidePlugin { definitions: { Buffer: [ 'buffer', 'Buffer' ] } },
    ProvidePlugin { definitions: { process: 'process/browser' } },
    MiniCssExtractPlugin {
      _sortedModulesCache: WeakMap { <items unknown> },
      options: {
        filename: 'assets/css/[name].css',
        ignoreOrder: false,
        experimentalUseImportModule: undefined,
        runtime: true,
        chunkFilename: 'assets/css/[name].css'
      },
      runtimeOptions: {
        insert: undefined,
        linkType: 'text/css',
        attributes: undefined
      }
    },
    ProgressPlugin {
      profile: false,
      handler: undefined,
      modulesCount: 5000,
      dependenciesCount: 10000,
      showEntries: true,
      showModules: true,
      showDependencies: true,
      showActiveModules: false,
      percentBy: undefined
    },
    DefinePlugin {
      definitions: {
        'process.env': '{"LC_FIG_SET_PARENT":"809b2b70-37a2-4c8b-b80b-310c77f37ce1","FIG_PID":"589","npm_package_jest_moduleNameMapper___cd_store_____":"<rootDir>/src/store$1","npm_package_scripts_dev_extension_testnet":"webpack --mode development --env=type=extension --env=network=testnet --watch","npm_package_dependencies_ts_results":"^3.3.0","npm_package_dependencies_redux":"^4.0.5","npm_package_devDependencies_jest_extended":"^3.0.1","npm_package_scripts_build_testnet":"webpack --mode production  --env=network=testnet","npm_package_scripts_start_testnet":"webpack-dev-server --mode development --env=network=testnet","TERM_PROGRAM":"Apple_Terminal","NODE":"/usr/local/Cellar/node/18.9.1/bin/node","npm_package_jest_moduleNameMapper___cd_web_extension_____":"<rootDir>/src/components/web-extension$1","npm_package_scripts_dev_extension_mainnet":"webpack --mode development --env=type=extension --env=network=mainnet --watch","INIT_CWD":"/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components/web","npm_package_jest_moduleNameMapper___cd_helpers_____":"<rootDir>/src/helpers$1","npm_package_dependencies_react_idle_timer":"^5.4.2","npm_package_dependencies_big_js":"^6.1.1","npm_package_dependencies_axios":"^0.24.0","npm_config_version_git_tag":"true","TERM":"xterm-256color","SHELL":"/bin/zsh","npm_package_devDependencies__types_webextension_polyfill":"^0.9.0","FIGTERM_SESSION_ID":"809b2b70-37a2-4c8b-b80b-310c77f37ce1","npm_package_devDependencies_style_loader":"^3.3.1","TMPDIR":"/var/folders/0v/wr8zwvfj5tlgk_chw0v7dxh80000gn/T/","npm_package_devDependencies_webpack_merge":"^5.8.0","npm_package_dependencies_identicon_js":"^2.3.3","npm_package_dependencies_casper_js_sdk":"^2.9.1","PERL5LIB":"/Users/muharremsalel/perl5/lib/perl5","npm_package_scripts_lint":"eslint src/ --ext .js,.jsx,.ts,.tsx","npm_package_dependencies_react_bootstrap":"^2.0.3","npm_config_init_license":"MIT","TERM_PROGRAM_VERSION":"447","npm_package_devDependencies_mockzilla":"^0.14.0","npm_package_devDependencies_babel_plugin_module_resolver":"^4.1.0","npm_package_devDependencies_babel_core":"^6.26.3","npm_package_dependencies_browserslist":"^4.13.0","npm_package_dependencies__babel_plugin_transform_runtime":"^7.16.7","npm_package_scripts_dev":"webpack-dev-server --mode development","npm_package_dependencies_cookie":"^0.4.1","npm_package_dependencies__zondax_ledger_casper":"^0.0.1","npm_package_devDependencies_sass_loader":"^12.4.0","PERL_MB_OPT":"--install_base \\"/Users/muharremsalel/perl5\\"","TERM_SESSION_ID":"717B4B30-6CE8-481D-B46D-8DEBEFEA880C","npm_package_devDependencies_webpack_bundle_analyzer":"^4.5.0","npm_package_scripts_test_ci":"CODECOV_TOKEN=f53cf772-9742-494e-af36-d84321b726dc SKIP_PREFLIGHT_CHECK=true CI=true react-scripts test --coverage","npm_package_dependencies_react_apexcharts":"^1.3.9","npm_package_dependencies__metamask_obs_store":"^7.0.0","npm_package_private":"false","npm_config_registry":"https://registry.yarnpkg.com","npm_package_devDependencies_extract_text_webpack_plugin":"^3.0.2","npm_package_dependencies_react_dom":"^17.0.2","npm_package_readmeFilename":"README.md","npm_package_dependencies_dayjs":"^1.8.29","USER":"muharremsalel","npm_package_devDependencies_webpack":"^5.65.0","npm_package_devDependencies_react_select_event":"^5.3.0","npm_package_description":"CasperDash Client","npm_package_devDependencies_webpack_cli":"^4.9.1","npm_package_license":"MIT","npm_package_devDependencies_jest_chrome":"^0.7.2","npm_package_dependencies__testing_library_user_event":"^7.2.1","npm_package_browserslist_development_1":"last 1 firefox version","npm_package_dependencies_redux_persist":"^6.0.0","npm_package_devDependencies_webpack_dev_server":"^4.6.0","npm_package_devDependencies_redux_mock_store":"^1.5.4","npm_package_devDependencies_babel_jest":"^28.1.3","npm_package_browserslist_development_0":"last 1 chrome version","SSH_AUTH_SOCK":"/private/tmp/com.apple.launchd.nLc890Z8wv/Listeners","npm_package_devDependencies_esbuild_loader":"^2.17.0","npm_package_devDependencies_babel_loader":"^8.2.3","npm_package_dependencies_memoize_one":"^6.0.0","npm_package_dependencies_bootstrap_icons":"^1.5.0","__CF_USER_TEXT_ENCODING":"0x1F5:0x0:0x0","npm_package_devDependencies__types_jest":"^28.1.8","npm_package_browserslist_development_2":"last 1 safari version","npm_execpath":"/usr/local/Cellar/yarn/1.22.19/libexec/bin/yarn.js","npm_package_scripts_test_w":"react-scripts test --watchAll ","npm_package_scripts_dev_extension":"webpack --mode development --env=type=extension --watch","npm_package_dependencies_react_redux":"^7.2.0","npm_package_devDependencies_babel_preset_react":"^6.24.1","npm_package_dependencies_webextension_polyfill":"^0.10.0","npm_package_dependencies_reselect":"^4.0.0","npm_package_author_name":"CasperDash","npm_package_devDependencies_mini_css_extract_plugin":"^2.4.5","npm_package_devDependencies_copy_webpack_plugin":"^10.2.0","npm_package_devDependencies__svgr_webpack":"^6.1.2","npm_package_jest_moduleNameMapper___cd_actions_____":"<rootDir>/src/actions$1","npm_package_dependencies_fuse_js":"^6.5.3","PATH":"/var/folders/0v/wr8zwvfj5tlgk_chw0v7dxh80000gn/T/yarn--1670098482858-0.7748314285342845:/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/node_modules/.bin:/Users/muharremsalel/.config/yarn/link/node_modules/.bin:/usr/local/Cellar/node/18.9.1/libexec/lib/node_modules/npm/bin/node-gyp-bin:/usr/local/Cellar/node/18.9.1/lib/node_modules/npm/bin/node-gyp-bin:/usr/local/Cellar/node/18.9.1/bin/node_modules/npm/bin/node-gyp-bin:/Users/muharremsalel/perl5/bin:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/go/bin:/Library/Apple/usr/bin:/Library/Frameworks/Mono.framework/Versions/Current/Commands:/Users/muharremsalel/.cargo/bin:/Users/muharremsalel/.fig/bin:/Users/muharremsalel/.local/bin","npm_config_argv":"{\\"remain\\":[],\\"cooked\\":[\\"run\\",\\"dev-extension-testnet\\"],\\"original\\":[\\"dev-extension-testnet\\"]}","npm_package_devDependencies__babel_plugin_syntax_top_level_await":"^7.14.5","npm_package_jest_moduleNameMapper___cd_web______":"<rootDir>/src/components/web$1","npm_package_jest_moduleNameMapper___cd_constants_____":"<rootDir>/src/constants$1","_":"/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/node_modules/.bin/webpack","__CFBundleIdentifier":"com.apple.Terminal","npm_package_devDependencies_ts_jest":"^28.0.8","npm_package_devDependencies__testing_library_react_hooks":"^8.0.1","npm_package_browserslist_production_1":"not dead","npm_package_scripts_build_extension_testnet":"rimraf -r build_extension && webpack --env=type=extension --mode development --env=network=testnet","npm_package_dependencies_redux_thunk":"^2.3.0","npm_package_dependencies_react_toastify":"^8.1.0","npm_package_dependencies_create_react_class":"^15.7.0","npm_package_dependencies__redux_requests_axios":"^1.1.1","TTY":"/dev/ttys003","PWD":"/Users/muharremsalel/Desktop/CRDao/casperdash-client/client","npm_package_browserslist_production_0":">0.2%","npm_package_dependencies_bootstrap":"^5.1.3","npm_package_jest_moduleNameMapper___cd_services_____":"<rootDir>/src/services$1","npm_package_jest_moduleNameMapper___cd_selectors_____":"<rootDir>/src/selectors$1","npm_package_scripts_snapshot":"react-snapshot","npm_lifecycle_event":"dev-extension-testnet","npm_package_jest_transform_______jt_sx__":"babel-jest","npm_package_browserslist_production_2":"not op_mini all","npm_package_scripts_build_mainnet":"webpack --mode production --env=network=mainnet && react-snapshot","npm_package_scripts_start_mainnet":"webpack-dev-server --mode development --env=network=mainnet","npm_package_dependencies_cross_env":"^7.0.3","npm_package_devDependencies_mockzilla_webextension":"^0.15.0","npm_package_name":"casperdash_client","npm_package_dependencies_react_top_loading_bar":"^2.0.1","npm_package_dependencies_react_snapshot":"^1.3.0","npm_package_jest_collectCoverageFrom_1":"!<rootDir>/node_modules/","npm_package_scripts_build_all":"yarn build-mainnet & yarn build-testnet & yarn build-extension-testnet & yarn build-extension-mainnet","npm_config_version_commit_hooks":"true","XPC_FLAGS":"0x0","npm_package_jest_collectCoverageFrom_0":"src/**/*.{js,jsx,ts,tsx}","npm_package_dependencies_react_router_dom":"^6.1.1","npm_package_dependencies_casper_storage":"1.0.0","npm_package_jest_transformIgnorePatterns_0":"<rootDir>/node_modules/(?!lodash-es)","npm_package_jest_resetMocks":"false","npm_package_reactSnapshot_exclude_0":"/dashboard/**","npm_config_bin_links":"true","npm_package_scripts_build_extension_mainnet":"rimraf -r build_extension && webpack --env=type=extension --mode development --env=network=mainnet","XPC_SERVICE_NAME":"0","npm_package_jest_moduleNameMapper___cd_app_____":"<rootDir>/src/app$1","npm_package_jest_moduleNameMapper___cd_shared_____":"<rootDir>/src/shared$1","npm_package_dependencies__ledgerhq_hw_transport_webusb":"^6.20.0","npm_package_version":"1.1.3.1","npm_package_devDependencies_css_minimizer_webpack_plugin":"^3.2.0","FIG_PARENT":"809b2b70-37a2-4c8b-b80b-310c77f37ce1","SHLVL":"2","HOME":"/Users/muharremsalel","npm_package_scripts_test":"react-scripts test --coverage --watchAll ","npm_package_dependencies_formik":"^2.2.9","npm_package_dependencies_dotenv":"^10.0.0","npm_config_save_prefix":"^","npm_config_strict_ssl":"true","npm_package_dependencies__testing_library_jest_dom":"^4.2.4","npm_config_version_git_message":"v%s","npm_package_jest_moduleNameMapper___cd_hocs_____":"<rootDir>/src/components/hocs$1","FIG_SET_PARENT":"809b2b70-37a2-4c8b-b80b-310c77f37ce1","PERL_LOCAL_LIB_ROOT":"/Users/muharremsalel/perl5","npm_package_devDependencies_babel_preset_env":"^1.7.0","LOGNAME":"muharremsalel","YARN_WRAP_OUTPUT":"false","npm_package_devDependencies_html_webpack_plugin":"^5.5.0","npm_package_jest_moduleNameMapper___cd_common_____":"<rootDir>/src/components/Common$1","npm_package_jest_moduleNameMapper_______css_scss__":"<rootDir>/src/__mocks__/styleMock.js","npm_package_dependencies_react_scripts":"^4.0.3","np'... 1718 more characters
      }
    },
    HtmlWebpackPlugin {
      userOptions: {
        template: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/template/extension/popup.html',
        filename: 'popup.html'
      },
      version: 5
    },
    HtmlWebpackPlugin {
      userOptions: {
        template: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/template/extension/popup.html',
        filename: 'home.html'
      },
      version: 5
    },
    CopyPlugin {
      patterns: [
        {
          from: 'template/extension/manifest.json',
          to: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/build_extension',
          force: true
        }
      ],
      options: {}
    },
    CopyPlugin {
      patterns: [
        {
          from: 'template/extension/512.png',
          to: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/build_extension',
          force: true
        }
      ],
      options: {}
    },
    CopyPlugin {
      patterns: [
        {
          from: 'src/assets/image/',
          to: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/build_extension/assets/images/',
          force: true
        }
      ],
      options: {}
    }
  ],
  experiments: { topLevelAwait: true },
  resolve: {
    extensions: [ '.js', '.jsx' ],
    alias: {
      '@cd/assets': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/assets',
      '@cd/actions': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/actions',
      '@cd/helpers': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/helpers',
      '@cd/selectors': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/selectors',
      '@cd/services': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/services',
      '@cd/shared': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/shared',
      '@cd/store': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/store',
      '@cd/config': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/config',
      '@cd/constants': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/constants',
      '@cd/common': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components/Common',
      '@cd/hooks': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components/hooks',
      '@cd/hocs': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components/hocs',
      '@cd/web': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components/web',
      '@cd/web-extension': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components/web-extension',
      '@cd/components': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/components'
    },
    fallback: {
      stream: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/node_modules/stream-browserify/index.js'
    }
  },
  entry: {
    main: '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/app/web-extension/index.js',
    'sw/service-worker': '/Users/muharremsalel/Desktop/CRDao/casperdash-client/client/src/services/ServiceWorker/serviceWorker.js'
  },
  devtool: 'inline-source-map'
}
Browserslist: caniuse-lite is outdated. Please run:
  npx browserslist@latest --update-db
  Why you should do it regularly: https://github.com/browserslist/browserslist#browsers-data-updating
10% building 0/2 entries 70/200 dependencies 2/59 modules[BABEL] Note: The code generator has deoptimised the styling of /Users/muharremsalel/Desktop/CRDao/casperdash-client/client/node_modules/casper-js-sdk/dist/lib.js as it exceeds the max of 500KB.
11% building 0/2 entries 931/1000 dependencies 96/485 modules[BABEL] Note: The code generator has deoptimised the styling of /Users/muharremsalel/Desktop/CRDao/casperdash-client/client/node_modules/react-dom/cjs/react-dom.development.js as it exceeds the max of 500KB.
assets by path assets/images/ 570 KiB
  assets by path assets/images/*.svg 62.7 KiB 43 assets
  assets by path assets/images/*.png 501 KiB
    assets by chunk 195 KiB (auxiliary name: main) 5 assets
  assets by path assets/images/token-icons/*.png 5.76 KiB 2 assets
assets by path static/js/ 28.9 MiB
  asset static/js/main.js 20.5 MiB [emitted] (name: main)
  asset static/js/sw/service-worker.js 8.29 MiB [emitted] (name: sw/service-worker)
  asset static/js/vendors-node_modules_webextension-polyfill_dist_browser-polyfill_js.js 112 KiB [emitted] (id hint: vendors)
assets by path *.html 3.72 KiB
  asset home.html 1.86 KiB [emitted]
  asset popup.html 1.86 KiB [emitted]
asset assets/css/main.css 698 KiB [emitted] (name: main)
asset 512.png 20.7 KiB [emitted] [from: template/extension/512.png] [copied]
asset manifest.json 431 bytes [emitted] [from: template/extension/manifest.json] [copied]
Entrypoint main 21.2 MiB (195 KiB) = assets/css/main.css 698 KiB static/js/main.js 20.5 MiB 5 auxiliary assets
Entrypoint sw/service-worker 8.29 MiB = static/js/sw/service-worker.js
runtime modules 62.6 KiB 237 modules
orphan modules 823 KiB [orphan] 199 modules
javascript modules 5 MiB
  modules by path ./node_modules/ 4.69 MiB 750 modules
  modules by path ./src/ 321 KiB 241 modules
  optional modules 30 bytes [optional] 2 modules
css modules 261 KiB
  modules by path ./src/components/web-extension/ 35.2 KiB 27 modules
  modules by path ./src/components/Common/ 1.47 KiB 2 modules
  modules by path ./node_modules/ 215 KiB 2 modules
  css ./node_modules/css-loader/dist/cjs.js!./node_modules/sass-loader/dist/cjs.js!./src/app/web-extension/App.scss 9.9 KiB [built] [code generated]
asset modules 210 bytes (javascript) 195 KiB (asset) 5 modules
./node_modules/elliptic/package.json 1.11 KiB [built] [code generated]
webpack 5.65.0 compiled successfully in 23401 ms

'''