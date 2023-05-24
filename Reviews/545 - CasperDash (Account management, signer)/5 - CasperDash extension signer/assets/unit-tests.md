```sh
gitpod /workspace/useWallet (main) $ pnpm test

> root@0.0.2-beta.1 test /workspace/useWallet
> vitest


 DEV  v0.26.3 /workspace/useWallet

 ✓ packages/core/src/connectors/casperDash.test.ts (23)
 ✓ packages/core/src/connectors/casperSigner.test.ts (23)
 ✓ packages/core/src/actions/signing/sign.test.ts (3)
 ✓ packages/core/src/utils/client.test.ts (18)
 ✓ packages/core/src/actions/account/getActivePublicKey.test.ts (3)
 ✓ packages/core/src/actions/account/connect.test.ts (4)
 ✓ packages/react/src/hooks/useSign.test.ts (6) 565ms
 ✓ packages/react/src/hooks/useSignMessage.test.ts (4) 500ms
 ✓ packages/core/src/actions/signing/signMessage.test.ts (3)
 ✓ packages/core/src/actions/account/getAccount.test.ts (3)
 ✓ packages/core/src/actions/account/isConnected.test.ts (4)
 ✓ packages/core/src/actions/account/disconnect.test.ts (2)
 ✓ packages/react/src/hooks/useConnect.test.ts (4)
 ✓ packages/core/src/utils/deepEqual.test.ts (9)
 ✓ packages/react/src/hooks/useDisconnect.test.ts (3)
 ✓ packages/react/src/hooks/useAccount.test.ts (1)
 ✓ packages/core/src/actions/account/watchAccount.test.ts (1)

 Test Files  17 passed (17)
      Tests  114 passed (114)
   Start at  07:30:49
   Duration  11.17s (transform 2.39s, setup 10ms, collect 8.95s, tests 2.56s)


 PASS  Waiting for file changes...
       press h to show help, press q to quit
gitpod /workspace/useWallet (main) $
```