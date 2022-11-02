## MyDPO web app

```
$ docker-compose up -d
[+] Running 14/14
 ⠿ postgres Pulled                                                                                                                                                              11.6s
   ⠿ 31b3f1ad4ce1 Pull complete                                                                                                                                                  3.0s
   ⠿ dc97844d0cd5 Pull complete                                                                                                                                                  4.0s
   ⠿ 9ad9b1166fde Pull complete                                                                                                                                                  4.0s
   ⠿ 286c4682b24d Pull complete                                                                                                                                                  4.1s
   ⠿ 1d3679a4a1a1 Pull complete                                                                                                                                                  4.7s
   ⠿ 5f2e6cdc8503 Pull complete                                                                                                                                                  4.8s
   ⠿ 0f7dc70f54e8 Pull complete                                                                                                                                                  4.8s
   ⠿ a090c7442692 Pull complete                                                                                                                                                  4.9s
   ⠿ 81bfe40fd0f6 Pull complete                                                                                                                                                  9.6s
   ⠿ 8ac8c22bbb38 Pull complete                                                                                                                                                  9.6s
   ⠿ 96e51d1d3c6e Pull complete                                                                                                                                                  9.7s
   ⠿ 667bd4154fa2 Pull complete                                                                                                                                                  9.7s
   ⠿ 87267fb600a9 Pull complete                                                                                                                                                  9.8s
[+] Running 2/2
 ⠿ Network mydpo_default       Created                                                                                                                                           0.0s
 ⠿ Container mydpo-postgres-1  Started
 ```
 
 ```
 $ sudo chmod 777 database -R
 ```
 
 ```
 $ yarn install && cp .env.example .env && yarn prisma:deploy && yarn dev
yarn install v1.22.19
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
warning "@emotion/react > @emotion/babel-plugin@11.10.0" has unmet peer dependency "@babel/core@^7.0.0".
warning "@emotion/react > @emotion/babel-plugin > @babel/plugin-syntax-jsx@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning " > formik-mui@5.0.0-alpha.0" has unmet peer dependency "tiny-warning@>=1.0.3".
warning "react-hot-toast > goober@2.1.10" has unmet peer dependency "csstype@^3.0.10".
warning " > @babel/preset-env@7.18.10" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/helper-compilation-targets@7.18.9" has unmet peer dependency "@babel/core@^7.0.0".
warning "@babel/preset-env > @babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@7.18.6" has unmet peer dependency "@babel/core@^7.0.0".
warning "@babel/preset-env > @babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@7.18.9" has unmet peer dependency "@babel/core@^7.13.0".
warning "@babel/preset-env > @babel/plugin-proposal-async-generator-functions@7.18.10" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-class-properties@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-class-static-block@7.18.6" has unmet peer dependency "@babel/core@^7.12.0".
warning "@babel/preset-env > @babel/plugin-proposal-dynamic-import@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-export-namespace-from@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-json-strings@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-logical-assignment-operators@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-nullish-coalescing-operator@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-numeric-separator@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-object-rest-spread@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-optional-catch-binding@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-optional-chaining@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-private-methods@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-private-property-in-object@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-unicode-property-regex@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-async-generators@7.8.4" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-class-properties@7.12.13" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-class-static-block@7.14.5" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-dynamic-import@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-export-namespace-from@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-import-assertions@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-json-strings@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-logical-assignment-operators@7.10.4" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-nullish-coalescing-operator@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-numeric-separator@7.10.4" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-object-rest-spread@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-optional-catch-binding@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-optional-chaining@7.8.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-private-property-in-object@7.14.5" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-syntax-top-level-await@7.14.5" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-arrow-functions@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-async-to-generator@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-block-scoped-functions@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-block-scoping@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-classes@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-computed-properties@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-destructuring@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-dotall-regex@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-duplicate-keys@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-exponentiation-operator@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-for-of@7.18.8" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-function-name@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-literals@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-member-expression-literals@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-modules-amd@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-modules-commonjs@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-modules-systemjs@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-modules-umd@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-named-capturing-groups-regex@7.18.6" has unmet peer dependency "@babel/core@^7.0.0".
warning "@babel/preset-env > @babel/plugin-transform-new-target@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-object-super@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-parameters@7.18.8" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-property-literals@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-regenerator@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-reserved-words@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-shorthand-properties@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-spread@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-sticky-regex@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-template-literals@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-typeof-symbol@7.18.9" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-unicode-escapes@7.18.10" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-transform-unicode-regex@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/preset-modules@0.1.5" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > babel-plugin-polyfill-corejs2@0.3.2" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > babel-plugin-polyfill-corejs3@0.5.3" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > babel-plugin-polyfill-regenerator@0.4.0" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-env > @babel/plugin-proposal-async-generator-functions > @babel/helper-remap-async-to-generator@7.18.9" has unmet peer dependency "@babel/core@^7.0.0".
warning "@babel/preset-env > @babel/plugin-proposal-class-properties > @babel/helper-create-class-features-plugin@7.18.9" has unmet peer dependency "@babel/core@^7.0.0".
warning "@babel/preset-env > @babel/plugin-proposal-unicode-property-regex > @babel/helper-create-regexp-features-plugin@7.18.6" has unmet peer dependency "@babel/core@^7.0.0".
warning "@babel/preset-env > babel-plugin-polyfill-corejs2 > @babel/helper-define-polyfill-provider@0.3.2" has unmet peer dependency "@babel/core@^7.4.0-0".
warning " > @babel/preset-typescript@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-typescript > @babel/plugin-transform-typescript@7.18.12" has unmet peer dependency "@babel/core@^7.0.0-0".
warning "@babel/preset-typescript > @babel/plugin-transform-typescript > @babel/plugin-syntax-typescript@7.18.6" has unmet peer dependency "@babel/core@^7.0.0-0".
warning " > @graphql-codegen/typescript-urql@3.6.4" has unmet peer dependency "graphql-tag@^2.0.0".
[4/4] Building fresh packages...
Done in 52.45s.
yarn run v1.22.19
$ yarn prisma migrate deploy
$ /workspace/PRIVACYMAP/mydpo/node_modules/.bin/prisma migrate deploy
Environment variables loaded from .env
Prisma schema loaded from src/server/db/schema.prisma
Datasource "db": PostgreSQL database "mydpo", schema "public" at "localhost:35432"

22 migrations found in prisma/migrations

Applying migration `20210218175246_initial_schema`
Applying migration `20211030220122_refactor_mydpo`
Applying migration `20211030220541_pseudorefactor`
Applying migration `20211101162721_ready_for_sprint`
Applying migration `20211103183232_refactor`
Applying migration `20211103183725_refactor`
Applying migration `20211106213246_refactor`
Applying migration `20211106221402_refactor`
Applying migration `20211108142701_application`
Applying migration `20211108152649_refactor`
Applying migration `20211109034032_refactor`
Applying migration `20211109034401_refactor`
Applying migration `20211109035947_refactor`
Applying migration `20211109040847_refactor`
Applying migration `20211109041229_refactor`
Applying migration `20211110152621_refactor`
Applying migration `20211110152800_refactor`
Applying migration `20211110214211_refactor`
Applying migration `20211117143630_refactor`
Applying migration `20211210124930_refactor`
Applying migration `20211210125042_refactor`
Applying migration `20211223165902_token`

The following migrations have been applied:

migrations/
  └─ 20210218175246_initial_schema/
    └─ migration.sql
  └─ 20211030220122_refactor_mydpo/
    └─ migration.sql
  └─ 20211030220541_pseudorefactor/
    └─ migration.sql
  └─ 20211101162721_ready_for_sprint/
    └─ migration.sql
  └─ 20211103183232_refactor/
    └─ migration.sql
  └─ 20211103183725_refactor/
    └─ migration.sql
  └─ 20211106213246_refactor/
    └─ migration.sql
  └─ 20211106221402_refactor/
    └─ migration.sql
  └─ 20211108142701_application/
    └─ migration.sql
  └─ 20211108152649_refactor/
    └─ migration.sql
  └─ 20211109034032_refactor/
    └─ migration.sql
  └─ 20211109034401_refactor/
    └─ migration.sql
  └─ 20211109035947_refactor/
    └─ migration.sql
  └─ 20211109040847_refactor/
    └─ migration.sql
  └─ 20211109041229_refactor/
    └─ migration.sql
  └─ 20211110152621_refactor/
    └─ migration.sql
  └─ 20211110152800_refactor/
    └─ migration.sql
  └─ 20211110214211_refactor/
    └─ migration.sql
  └─ 20211117143630_refactor/
    └─ migration.sql
  └─ 20211210124930_refactor/
    └─ migration.sql
  └─ 20211210125042_refactor/
    └─ migration.sql
  └─ 20211223165902_token/
    └─ migration.sql
      
All migrations have been successfully applied.
Done in 1.32s.
yarn run v1.22.19
$ yarn run generate
$ yarn run generate:prisma && yarn run generate:nexus && yarn run generate:graphql-codegen
$ prisma generate
Environment variables loaded from .env
Prisma schema loaded from src/server/db/schema.prisma

✔ Generated Prisma Client (4.2.0 | library) to ./node_modules/@prisma/client in 126ms
You can now start using Prisma Client in your code. Reference: https://pris.ly/d/client
```
import { PrismaClient } from '@prisma/client'
const prisma = new PrismaClient()
```

warn Versions of prisma@4.2.1 and @prisma/client@4.2.0 don't match.
This might lead to unexpected behavior.
Please make sure they have the same version.
┌─────────────────────────────────────────────────────────┐
│  Update available 4.2.1 -> 4.4.0                        │
│  Run the following to update                            │
│    yarn add --dev prisma@latest                         │
│    yarn add @prisma/client@latest                       │
└─────────────────────────────────────────────────────────┘
$ cross-env GENERATE=true cross-env DOTENV_CONFIG_PATH=.env.example ts-node --require dotenv/config --transpile-only -P nexus.tsconfig.json src/server/graphql/schema.ts
$ graphql-codegen
✔ Parse Configuration
✔ Generate outputs
$ next dev
ready - started server on 0.0.0.0:3000, url: http://localhost:3000
info  - Loaded env from /workspace/PRIVACYMAP/mydpo/.env
warn  - Invalid next.config.js options detected: 
  - The root value has an unexpected property, target, which is not in the list of allowed properties (amp, analyticsId, assetPrefix, basePath, cleanDistDir, compiler, compress, crossOrigin, devIndicators, distDir, env, eslint, excludeDefaultMomentLocales, experimental, exportPathMap, future, generateBuildId, generateEtags, headers, httpAgentOptions, i18n, images, onDemandEntries, optimizeFonts, output, outputFileTracing, pageExtensions, poweredByHeader, productionBrowserSourceMaps, publicRuntimeConfig, reactStrictMode, redirects, rewrites, sassOptions, serverRuntimeConfig, staticPageGenerationTimeout, swcMinify, trailingSlash, typescript, useFileSystemPublicRoutes, webpack).
  - The root value has an unexpected property, webpackDevMiddleware, which is not in the list of allowed properties (amp, analyticsId, assetPrefix, basePath, cleanDistDir, compiler, compress, crossOrigin, devIndicators, distDir, env, eslint, excludeDefaultMomentLocales, experimental, exportPathMap, future, generateBuildId, generateEtags, headers, httpAgentOptions, i18n, images, onDemandEntries, optimizeFonts, output, outputFileTracing, pageExtensions, poweredByHeader, productionBrowserSourceMaps, publicRuntimeConfig, reactStrictMode, redirects, rewrites, sassOptions, serverRuntimeConfig, staticPageGenerationTimeout, swcMinify, trailingSlash, typescript, useFileSystemPublicRoutes, webpack).

See more info here: https://nextjs.org/docs/messages/invalid-next-config
event - compiled client and server successfully in 2.3s (216 modules)
Attention: Next.js now collects completely anonymous telemetry regarding usage.
This information is used to shape Next.js' roadmap and prioritize features.
You can learn more, including how to opt-out if you'd not like to participate in this anonymous program, by visiting the following URL:
https://nextjs.org/telemetry
```

## MyDPO api

```
$ yarn install && yarn dev
yarn install v1.22.19
info No lockfile found.
[1/4] Resolving packages...
[2/4] Fetching packages...
[3/4] Linking dependencies...
[4/4] Building fresh packages...
success Saved lockfile.
Done in 16.30s.
yarn run v1.22.19
$ yarn nodemon src/index.ts
$ /workspace/PRIVACYMAP/api/node_modules/.bin/nodemon src/index.ts
[nodemon] 2.0.20
[nodemon] to restart at any time, enter `rs`
[nodemon] watching path(s): *.*
[nodemon] watching extensions: ts,json
[nodemon] starting `ts-node src/index.ts`
Server running on 9999
```

## Setup

### Add firm and user to db

```
$ docker exec -it mydpo-postgres-1 psql -U postgres -W postgres
Password: 
psql (14.5 (Debian 14.5-1.pgdg110+1))
Type "help" for help.

postgres=# \c mydpo
Password: 
You are now connected to database "mydpo" as user "postgres".
mydpo=# INSERT INTO "ConsultancyFirm" (id, name, slug) VALUES ('ckvjuluhp000008l40bgq5x3y', 'MyDPO', 'MyDPO-ckvjuluhp000008l40bgq5x3y');
INSERT 0 1
mydpo=# INSERT INTO "User" (id, email, name, "consultancyFirmId") VALUES ('ckvsahypo000008l990jp8f8z', 'jmorello@kreitech.com.uy', 'Juano Morello', 'ckvjuluhp000008l40bgq5x3y');
INSERT 0 1
mydpo=# INSERT INTO "User" (id, email, name, "consultancyFirmId") VALUES ('ckvsahypo000008l990jp8f8x', 'kiligim528@ishyp.com', 'Juano Morello', 'ckvjuluhp000008l40bgq5x3y');
INSERT 0 1
mydpo=#
```
