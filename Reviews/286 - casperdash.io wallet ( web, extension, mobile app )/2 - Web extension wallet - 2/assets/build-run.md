```

yusuf@ubuntu:~/286-2/casperdash-client$ ls
client   package.json              README.md    yarn.lock
LICENSE  pull_request_template.md  SECURITY.md
yusuf@ubuntu:~/286-2/casperdash-client$ cd client/
yusuf@ubuntu:~/286-2/casperdash-client/client$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
yusuf@ubuntu:~/286-2/casperdash-client/client$ yarn install
yarn install v1.22.18
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
warning " > @babel/plugin-transform-runtime@7.16.7" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/plugin-transform-runtime > babel-plugin-polyfill-corejs2@0.3.0" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/plugin-transform-runtime > babel-plugin-polyfill-corejs3@0.4.0" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/plugin-transform-runtime > babel-plugin-polyfill-regenerator@0.3.0" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/plugin-transform-runtime > babel-plugin-polyfill-corejs2 > @babel/helper-define-polyfill-provider@0.3.0" has unmet peer dependency "@babel/core@^7.4.0-0".
warning "@babel/plugin-transform-runtime > babel-plugin-polyfill-corejs2 > @babel/helper-define-polyfill-provider > @babel/helper-compilation-targets@7.16.3" has unmet peer dependency "@babel/core@^7.0.0".
warning " > @testing-library/user-event@7.2.1" has unmet peer dependency "@testing-library/dom@>=5".
warning " > bootstrap@5.1.3" has unmet peer dependency "@popperjs/core@^2.10.2".
warning "casper-js-sdk > eslint-plugin-prettier@3.4.1" has unmet peer dependency "eslint@>=5.0.0".
warning "casper-js-sdk > eslint-plugin-prettier@3.4.1" has unmet peer dependency "prettier@>=1.13.0".
warning "react-scripts > @typescript-eslint/eslint-plugin > tsutils@3.21.0" has unmet peer dependency "typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta".
warning " > react-snapshot@1.3.0" has incorrect peer dependency "react@^15.3.0 || ^16.0.0".
warning " > react-snapshot@1.3.0" has incorrect peer dependency "react-dom@^15.3.0 || ^16.0.0".
warning " > babel-loader@8.2.3" has unmet peer dependency "@babel/core@^7.0.0".
warning " > extract-text-webpack-plugin@3.0.2" has incorrect peer dependency "webpack@^3.1.0".
[4/4] Building fresh packages...
Done in 22.53s.


yusuf@ubuntu:~/286-2/casperdash-client/client$ yarn dev-extension-testnet
yarn run v1.22.18
$ webpack --mode development --env=type=extension --env=network=testnet --watch
{
  output: {
    filename: 'static/js/[name].js',
    assetModuleFilename: 'assets/images/[name][ext][query]',
    chunkFilename: 'static/js/[name].js',
    path: '/home/yusuf/286-2/casperdash-client/client/build_extension'
  },
  module: {
    rules: [
      { test: /\.(js|jsx)$/, use: [ 'babel-loader' ] },
      {
        test: /\.(css|scss)$/,
        use: [
          '/home/yusuf/286-2/casperdash-client/client/node_modules/mini-css-extract-plugin/dist/loader.js',
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
        'process.env': '{"GJS_DEBUG_TOPICS":"JS ERROR;JS LOG","LESSOPEN":"| /usr/bin/lesspipe %s","npm_package_dependencies__babel_plugin_transform_runtime":"^7.16.7","npm_package_devDependencies_babel_core":"^6.26.3","npm_package_devDependencies__svgr_webpack":"^6.1.2","npm_package_scripts_build_testnet":"webpack --mode production  --env=network=testnet && react-snapshot","npm_package_dependencies_apexcharts":"^3.30.0","USER":"yusuf","LC_TIME":"en_IE.UTF-8","npm_package_devDependencies_webpack_cli":"^4.9.1","npm_package_devDependencies_webpack_bundle_analyzer":"^4.5.0","npm_package_dependencies_react_toastify":"^8.1.0","npm_config_version_commit_hooks":"true","npm_config_user_agent":"yarn/1.22.18 npm/? node/v16.14.2 linux x64","npm_package_dependencies_formik":"^2.2.9","npm_config_bin_links":"true","SSH_AGENT_PID":"1758","XDG_SESSION_TYPE":"x11","npm_node_execpath":"/usr/bin/node","npm_package_scripts_start_mainnet":"webpack-dev-server --mode development --env=network=mainnet","npm_package_dependencies_identicon_js":"^2.3.3","npm_config_init_version":"1.0.0","SHLVL":"1","npm_package_scripts_build_extension_mainnet":"webpack --mode production --env=type=extension --env=network=mainnet","npm_package_dependencies_bootstrap_icons":"^1.5.0","npm_package_dependencies__zondax_ledger_casper":"^0.0.1","HOME":"/home/yusuf","OLDPWD":"/home/yusuf/286-2/casperdash-client","npm_package_browserslist_production_0":">0.2%","npm_package_scripts_dev_extension":"webpack --mode development --env=type=extension --watch","DESKTOP_SESSION":"ubuntu","npm_package_browserslist_production_1":"not dead","npm_package_browserslist_production_2":"not op_mini all","npm_config_init_license":"MIT","GNOME_SHELL_SESSION_MODE":"ubuntu","GTK_MODULES":"gail:atk-bridge","YARN_WRAP_OUTPUT":"false","npm_config_version_tag_prefix":"v","LC_MONETARY":"en_IE.UTF-8","MANAGERPID":"1586","npm_package_dependencies_redux_thunk":"^2.3.0","DBUS_SESSION_BUS_ADDRESS":"unix:path=/run/user/1000/bus","npm_package_devDependencies_css_minimizer_webpack_plugin":"^3.2.0","npm_package_dependencies_dotenv":"^10.0.0","npm_package_dependencies_dayjs":"^1.8.29","COLORTERM":"truecolor","npm_package_devDependencies_babel_loader":"^8.2.3","npm_package_dependencies_react_scripts":"^4.0.3","npm_package_dependencies_react_router_dom":"^6.1.1","npm_package_dependencies_qs":"^6.9.4","npm_package_description":"CasperDash Client","npm_package_scripts_test_ci":"CODECOV_TOKEN=f53cf772-9742-494e-af36-d84321b726dc SKIP_PREFLIGHT_CHECK=true CI=true react-scripts test --coverage","npm_package_scripts_build_mainnet":"webpack --mode production --env=network=mainnet && react-snapshot","npm_package_reactSnapshot_exclude_0":"/dashboard/**","npm_package_dependencies__testing_library_react":"^9.5.0","IM_CONFIG_PHASE":"1","npm_package_scripts_dev":"webpack-dev-server --mode development","LOGNAME":"yusuf","npm_package_jest_collectCoverageFrom_0":"src/**/*.{js,jsx,ts,tsx}","npm_package_dependencies_reselect":"^4.0.0","JOURNAL_STREAM":"8:49567","_":"/usr/bin/yarn","npm_package_jest_collectCoverageFrom_1":"!<rootDir>/node_modules/","npm_package_dependencies_big_js":"^6.1.1","npm_package_private":"false","XDG_SESSION_CLASS":"user","npm_config_registry":"https://registry.yarnpkg.com","USERNAME":"yusuf","TERM":"xterm-256color","npm_package_scripts_dev_extension_testnet":"webpack --mode development --env=type=extension --env=network=testnet --watch","GNOME_DESKTOP_SESSION_ID":"this-is-deprecated","npm_package_devDependencies_html_webpack_plugin":"^5.5.0","npm_config_ignore_scripts":"","WINDOWPATH":"2","npm_package_devDependencies_esbuild_loader":"^2.17.0","npm_package_browserslist_development_0":"last 1 chrome version","npm_package_dependencies_axios":"^0.24.0","PATH":"/tmp/yarn--1649534792212-0.8208584780997332:/home/yusuf/286-2/casperdash-client/client/node_modules/.bin:/home/yusuf/.config/yarn/link/node_modules/.bin:/home/yusuf/.yarn/bin:/usr/libexec/lib/node_modules/npm/bin/node-gyp-bin:/usr/lib/node_modules/npm/bin/node-gyp-bin:/usr/bin/node_modules/npm/bin/node-gyp-bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin","NODE":"/usr/bin/node","SESSION_MANAGER":"local/ubuntu:@/tmp/.ICE-unix/1794,unix/ubuntu:/tmp/.ICE-unix/1794","INVOCATION_ID":"03e1eb08341a4f8d9437d5bf7787a367","PAPERSIZE":"a4","npm_package_browserslist_development_1":"last 1 firefox version","npm_package_name":"casperdash_client","XDG_MENU_PREFIX":"gnome-","LC_ADDRESS":"en_IE.UTF-8","GNOME_TERMINAL_SCREEN":"/org/gnome/Terminal/screen/ab5a3a7a_ba12_416f_bf13_65c1f372cba1","XDG_RUNTIME_DIR":"/run/user/1000","npm_package_browserslist_development_2":"last 1 safari version","npm_package_dependencies_react_redux":"^7.2.0","DISPLAY":":0","npm_package_devDependencies_webpack_merge":"^5.8.0","npm_package_jest_resetMocks":"false","npm_package_dependencies_memoize_one":"^6.0.0","npm_package_dependencies_browserslist":"^4.13.0","LANG":"en_US.UTF-8","XDG_CURRENT_DESKTOP":"ubuntu:GNOME","LC_TELEPHONE":"en_IE.UTF-8","npm_package_devDependencies_webpack":"^5.65.0","npm_package_devDependencies_react_select_event":"^5.3.0","npm_package_jest_moduleNameMapper__assets_____":"<rootDir>/src/assets$1","npm_package_dependencies_redux":"^4.0.5","npm_package_dependencies_react_dom":"^17.0.2","npm_package_dependencies_casper_js_sdk":"^2.7.3","XMODIFIERS":"@im=ibus","XDG_SESSION_DESKTOP":"ubuntu","XAUTHORITY":"/run/user/1000/gdm/Xauthority","LS_COLORS":"rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:","GNOME_TERMINAL_SERVICE":":1.113","npm_lifecycle_script":"webpack --mode development --env=type=extension --env=network=testnet --watch","npm_package_devDependencies_html_loader":"^3.0.1","npm_package_devDependencies_copy_webpack_plugin":"^10.2.0","SSH_AUTH_SOCK":"/run/user/1000/keyring/ssh","npm_package_devDependencies_webpack_dev_server":"^4.6.0","npm_package_scripts_test":"react-scripts test --coverage --watchAll ","npm_config_version_git_message":"v%s","SHELL":"/bin/bash","LC_NAME":"en_IE.UTF-8","npm_lifecycle_event":"dev-extension-testnet","npm_package_dependencies__testing_library_jest_dom":"^4.2.4","npm_package_dependencies__redux_requests_core":"^1.6.2","npm_package_version":"1.1.2","QT_ACCESSIBILITY":"1","GDMSESSION":"ubuntu","npm_config_argv":"{\\"remain\\":[],\\"cooked\\":[\\"run\\",\\"dev-extension-testnet\\"],\\"original\\":[\\"dev-extension-testnet\\"]}","npm_package_dependencies_react_top_loading_bar":"^2.0.1","npm_package_dependencies_lodash_es":"^4.17.21","npm_package_dependencies_fuse_js":"^6.5.3","npm_package_dependencies_cookie":"^0.4.1","npm_package_dependencies__testing_library_user_event":"^7.2.1","LESSCLOSE":"/usr/bin/lesspipe %s %s","LC_MEASUREMENT":"en_IE.UTF-8","npm_package_devDependencies_sass_loader":"^12.4.0","npm_package_scripts_dev_extension_mainnet":"webpack --mode development --env=type=extension --env=network=mainnet --watch","npm_package_dependencies_qrcode_react":"^1.0.1","npm_config_version_git_tag":"true","npm_config_version_git_sign":"","GPG_AGENT_INFO":"/run/user/1000/gnupg/S.gpg-agent:0:1","GJS_DEBUG_OUTPUT":"stderr","LC_IDENTIFICATION":"en_IE.UTF-8","npm_package_scripts_start_testnet":"webpack-dev-server --mode development --env=network=testnet","npm_package_dependencies_sass":"^1.26.10","npm_package_dependencies_react_bootstrap":"^2.0.3","npm_package_license":"MIT","npm_config_strict_ssl":"true","QT_IM_MODULE":"ibus","npm_package_devDependencies_style_loader":"^3.3.1","npm_package_scripts_build_extension_testnet":"webpack --mode production --env=type=extension --env=network=testnet","npm_package_dependencies_react_select":"^5.2.1","PWD":"/home/yusuf/286-2/casperdash-client/client","npm_execpath":"/usr/share/yarn/bin/yarn.js","npm_package_jest_moduleNameMapper_______css_scss__":"<rootDir>/src/__mocks__/styleMock.js","npm_package_dependencies_bootstrap":"^5.1.3","npm_package_dependencies__redux_requests_axios":"^1.1.1","XDG_CONFIG_DIRS":"/etc/xdg/xdg-ubuntu:/etc/xdg","XDG_DATA_DIRS":"/usr/share/ubuntu:/usr/local/share/:/usr/share/:/var/lib/snapd/desktop","npm_package_devDependencies_css_loader":"^6.5.1","npm_package_author_name":"CasperDash","LC_NUMERIC":"en_IE.UTF-8","npm_package_devDependencies_extract_text_webpack_plugin":"^3.0.2","npm_package_devDependencies_babel_preset_env":"^1.7.0","npm_config_save_prefix":"^","npm_config_ignore_optional":"","LC_PAPER":"en_IE.UTF-8","npm_package_devDependencies_mini_css_extract_plugin":"^2.4.5","VTE_VERSION":"6003","npm_package_dependencies__ledgerhq_hw_transport_webusb":"^6.20.0","INIT_CWD":"/home/yusuf/286-2/casperdash-client/client","npm_package_dev'... 470 more characters
      }
    },
    HtmlWebpackPlugin {
      userOptions: {
        template: '/home/yusuf/286-2/casperdash-client/client/template/extension/popup.html',
        filename: 'popup.html'
      },
      version: 5
    },
    HtmlWebpackPlugin {
      userOptions: {
        template: '/home/yusuf/286-2/casperdash-client/client/template/extension/popup.html',
        filename: 'home.html'
      },
      version: 5
    },
    CopyPlugin {
      patterns: [
        {
          from: 'template/extension/manifest.json',
          to: '/home/yusuf/286-2/casperdash-client/client/build_extension',
          force: true
        }
      ],
      options: {}
    },
    CopyPlugin {
      patterns: [
        {
          from: 'template/extension/512.png',
          to: '/home/yusuf/286-2/casperdash-client/client/build_extension',
          force: true
        }
      ],
      options: {}
    },
    CopyPlugin {
      patterns: [
        {
          from: 'src/assets/image/',
          to: '/home/yusuf/286-2/casperdash-client/client/build_extension/assets/images/',
          force: true
        }
      ],
      options: {}
    }
  ],
  resolve: {
    extensions: [ '.js', '.jsx' ],
    alias: { assets: '/home/yusuf/286-2/casperdash-client/client/src/assets' }
  },
  entry: '/home/yusuf/286-2/casperdash-client/client/src/app/web-extension/index.js',
  devtool: 'inline-source-map'
}
10% building 0/1 entries 639/781 dependencies 65/300 modules[BABEL] Note: The code generator has deoptimised the styling of /home/yusuf/286-2/casperdash-client/client/node_modules/react-dom/cjs/react-dom.development.js as it exceeds the max of 500KB.
10% building 0/1 entries 848/1000 dependencies 86/406 modules[BABEL] Note: The code generator has deoptimised the styling of /home/yusuf/286-2/casperdash-client/client/node_modules/casper-js-sdk/dist/lib.js as it exceeds the max of 500KB.
assets by path assets/images/ 554 KiB
  assets by path assets/images/*.svg 51.8 KiB 33 assets
  assets by path assets/images/*.png 496 KiB
    assets by chunk 191 KiB (auxiliary name: main) 2 assets
  assets by path assets/images/token-icons/*.png 5.76 KiB
    asset assets/images/token-icons/cspr.png 3.1 KiB [emitted] [from: src/assets/image/token-icons/cspr.png] [copied]
    asset assets/images/token-icons/question-icon.png 2.66 KiB [emitted] [from: src/assets/image/token-icons/question-icon.png] [copied]
assets by chunk 18.3 MiB (name: main)
  asset static/js/main.js 17.6 MiB [emitted] (name: main)
  asset assets/css/main.css 661 KiB [emitted] (name: main)
assets by path *.html 3.62 KiB
  asset home.html 1.81 KiB [emitted]
  asset popup.html 1.81 KiB [emitted]
asset 512.png 20.7 KiB [emitted] [from: template/extension/512.png] [copied]
asset manifest.json 262 bytes [emitted] [from: template/extension/manifest.json] [copied]
Entrypoint main 18.3 MiB (191 KiB) = assets/css/main.css 661 KiB static/js/main.js 17.6 MiB 2 auxiliary assets
orphan modules 819 KiB (javascript) 997 bytes (runtime) [orphan] 208 modules
runtime modules 37.2 KiB 151 modules
javascript modules 4.11 MiB
  modules by path ./node_modules/ 3.86 MiB 516 modules
  modules by path ./src/ 247 KiB 158 modules
  buffer (ignored) 15 bytes [optional] [built] [code generated]
css modules 251 KiB
  modules by path ./src/components/web-extension/ 25.8 KiB 19 modules
  modules by path ./src/components/Common/ 784 bytes 5 modules
  modules by path ./node_modules/ 215 KiB 2 modules
  css ./node_modules/css-loader/dist/cjs.js!./node_modules/sass-loader/dist/cjs.js!./src/app/web-extension/App.scss 9.69 KiB [built] [code generated]
asset modules 84 bytes (javascript) 191 KiB (asset)
  ./src/assets/image/nft-header.png 42 bytes (javascript) 121 KiB (asset) [built] [code generated]
  ./src/assets/image/cd-nft-empty.png 42 bytes (javascript) 70.2 KiB (asset) [built] [code generated]
webpack 5.65.0 compiled successfully in 14347 ms


```
