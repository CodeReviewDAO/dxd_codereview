```
foc@192:~/dev/proposals/casperdash-client/client$ yarn build-extension-mainnet
yarn run v1.22.10
$ rimraf -r build_extension && webpack --env=type=extension --mode development --env=network=mainnet
{
  output: {
    filename: 'static/js/[name].js',
    assetModuleFilename: 'assets/images/[name][ext][query]',
    chunkFilename: 'static/js/[name].js',
    path: '/home/faruk/dev/proposals/casperdash-client/client/build_extension'
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
          '/home/faruk/dev/proposals/casperdash-client/client/node_modules/mini-css-extract-plugin/dist/loader.js',
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
        'process.env': '{"REACT_APP_API_ROOT":"https://api.casperdash.io","REACT_APP_NETWORK_NAME":"casper","REACT_APP_AUCTION_HASH":"ccb576d6ce6dec84a551e48f0d0b7af89ddba44c7390b690036257a04a3ae9ea","REACT_APP_VERSION":"1.3.2","APP_ENVIRONMENT":"prod"}'
      }
    },
    HtmlWebpackPlugin {
      userOptions: {
        template: '/home/faruk/dev/proposals/casperdash-client/client/template/extension/popup.html',
        filename: 'popup.html',
        chunks: [ 'popup' ],
        cache: false
      },
      version: 5
    },
    HtmlWebpackPlugin {
      userOptions: {
        template: '/home/faruk/dev/proposals/casperdash-client/client/template/extension/popup.html',
        filename: 'home.html',
        chunks: [ 'popup' ],
        cache: false
      },
      version: 5
    },
    CopyPlugin {
      patterns: [
        {
          from: 'template/extension/manifest.json',
          to: '/home/faruk/dev/proposals/casperdash-client/client/build_extension',
          force: true
        }
      ],
      options: {}
    },
    CopyPlugin {
      patterns: [
        {
          from: 'template/extension/512.png',
          to: '/home/faruk/dev/proposals/casperdash-client/client/build_extension',
          force: true
        }
      ],
      options: {}
    },
    CopyPlugin {
      patterns: [
        {
          from: 'src/assets/image/',
          to: '/home/faruk/dev/proposals/casperdash-client/client/build_extension/assets/images/',
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
      '@cd/assets': '/home/faruk/dev/proposals/casperdash-client/client/src/assets',
      '@cd/actions': '/home/faruk/dev/proposals/casperdash-client/client/src/actions',
      '@cd/helpers': '/home/faruk/dev/proposals/casperdash-client/client/src/helpers',
      '@cd/selectors': '/home/faruk/dev/proposals/casperdash-client/client/src/selectors',
      '@cd/services': '/home/faruk/dev/proposals/casperdash-client/client/src/services',
      '@cd/shared': '/home/faruk/dev/proposals/casperdash-client/client/src/shared',
      '@cd/store': '/home/faruk/dev/proposals/casperdash-client/client/src/store',
      '@cd/config': '/home/faruk/dev/proposals/casperdash-client/client/src/config',
      '@cd/constants': '/home/faruk/dev/proposals/casperdash-client/client/src/constants',
      '@cd/common': '/home/faruk/dev/proposals/casperdash-client/client/src/components/Common',
      '@cd/hooks': '/home/faruk/dev/proposals/casperdash-client/client/src/components/hooks',
      '@cd/hocs': '/home/faruk/dev/proposals/casperdash-client/client/src/components/hocs',
      '@cd/web': '/home/faruk/dev/proposals/casperdash-client/client/src/components/web',
      '@cd/web-extension': '/home/faruk/dev/proposals/casperdash-client/client/src/components/web-extension',
      '@cd/components': '/home/faruk/dev/proposals/casperdash-client/client/src/components'
    },
    fallback: {
      stream: '/home/faruk/dev/proposals/casperdash-client/client/node_modules/stream-browserify/index.js'
    }
  },
  entry: {
    popup: '/home/faruk/dev/proposals/casperdash-client/client/src/app/web-extension/index.js',
    'sw/service-worker': '/home/faruk/dev/proposals/casperdash-client/client/src/services/ServiceWorker/serviceWorker.js',
    'scripts/content/content': '/home/faruk/dev/proposals/casperdash-client/client/src/content/content.js',
    'scripts/content/inpage': '/home/faruk/dev/proposals/casperdash-client/client/src/content/inpage.js'
  },
  devtool: 'inline-source-map'
}
34% building 2/4 entries 112/254 dependencies 7/87 modules[BABEL] Note: The code generator has deoptimised the styling of /home/faruk/dev/proposals/casperdash-client/client/node_modules/casper-js-sdk/dist/lib.js as it exceeds the max of 500KB.
37% building 2/4 entries 173/263 dependencies 8/132 modules[BABEL] Note: The code generator has deoptimised the styling of /home/faruk/dev/proposals/casperdash-client/client/node_modules/react-dom/cjs/react-dom.development.js as it exceeds the max of 500KB.
37% building 2/4 entries 4770/4804 dependencies 856/1600 modules[BABEL] Note: The code generator has deoptimised the styling of /home/faruk/dev/proposals/casperdash-client/client/node_modules/apexcharts/dist/apexcharts.common.js as it exceeds the max of 500KB.
assets by path assets/images/*.svg 71.7 KiB 52 assets
assets by path assets/images/*.png 501 KiB
  assets by chunk 195 KiB (auxiliary name: popup) 5 assets
  + 12 assets
assets by path static/js/ 29.8 MiB 5 assets
assets by path assets/images/token-icons/*.png 5.76 KiB
  asset assets/images/token-icons/cspr.png 3.1 KiB [emitted] [from: src/assets/image/token-icons/cspr.png] [copied]
  asset assets/images/token-icons/question-icon.png 2.66 KiB [emitted] [from: src/assets/image/token-icons/question-icon.png] [copied]
assets by path *.html 3.61 KiB
  asset home.html 1.8 KiB [emitted]
  asset popup.html 1.8 KiB [emitted]
asset assets/css/popup.css 814 KiB [emitted] (name: popup)
asset 512.png 20.7 KiB [emitted] [from: template/extension/512.png] [copied]
asset manifest.json 752 bytes [emitted] [from: template/extension/manifest.json] [copied]
Entrypoint popup 22.4 MiB (195 KiB) = assets/css/popup.css 814 KiB static/js/popup.js 21.6 MiB 5 auxiliary assets
Entrypoint sw/service-worker 8 MiB = static/js/sw/service-worker.js
Entrypoint scripts/content/content 128 KiB = static/js/scripts/content/content.js
Entrypoint scripts/content/inpage 8.24 KiB = static/js/scripts/content/inpage.js
orphan modules 1.37 MiB (javascript) 1.01 KiB (runtime) [orphan] 657 modules
runtime modules 78.1 KiB 301 modules
javascript modules 5.22 MiB 1209 modules
css modules 305 KiB
  modules by path ./src/components/web-extension/ 47.9 KiB 60 modules
  modules by path ./src/components/Common/ 1.47 KiB 7 modules
  modules by path ./node_modules/ 245 KiB 2 modules
  + 1 module
asset modules 210 bytes (javascript) 195 KiB (asset)
  ./src/assets/image/nft-header.png 42 bytes (javascript) 121 KiB (asset) [built] [code generated]
  ./src/assets/image/ic-version.png 42 bytes (javascript) 1.6 KiB (asset) [built] [code generated]
  ./src/assets/image/ic-backup.png 42 bytes (javascript) 1.14 KiB (asset) [built] [code generated]
  + 2 modules
./node_modules/elliptic/package.json 1.11 KiB [built] [code generated]
webpack 5.84.1 compiled successfully in 21823 ms
Done in 23.39s.
foc@192:~/dev/proposals/casperdash-client/client$
```