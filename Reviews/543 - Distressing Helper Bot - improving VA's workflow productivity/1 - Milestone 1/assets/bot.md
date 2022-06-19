## Bot running locally

```sh
> helperbot@1.0.0 start:pm2
> NODE_ENV=production npm run build && pm2 start ./dist/index.js --exp-backoff-restart-delay 3000 --kill-timeout 2000 && pm2 status && pm2 logs all


> helperbot@1.0.0 build
> npx tsc


                        -------------

__/\\\\\\\\\\\\\____/\\\\____________/\\\\____/\\\\\\\\\_____
 _\/\\\/////////\\\_\/\\\\\\________/\\\\\\__/\\\///////\\\___
  _\/\\\_______\/\\\_\/\\\//\\\____/\\\//\\\_\///______\//\\\__
   _\/\\\\\\\\\\\\\/__\/\\\\///\\\/\\\/_\/\\\___________/\\\/___
    _\/\\\/////////____\/\\\__\///\\\/___\/\\\________/\\\//_____
     _\/\\\_____________\/\\\____\///_____\/\\\_____/\\\//________
      _\/\\\_____________\/\\\_____________\/\\\___/\\\/___________
       _\/\\\_____________\/\\\_____________\/\\\__/\\\\\\\\\\\\\\\_
        _\///______________\///______________\///__\///////////////__


                          Runtime Edition

        PM2 is a Production Process Manager for Node.js applications
                     with a built-in Load Balancer.

                Start and Daemonize any application:
                $ pm2 start app.js

                Load Balance 4 instances of api.js:
                $ pm2 start api.js -i 4

                Monitor in production:
                $ pm2 monitor

                Make pm2 auto-boot at server restart:
                $ pm2 startup

                To go further checkout:
                http://pm2.io/


                        -------------

[PM2] Spawning PM2 daemon with pm2_home=/home/gitpod/.pm2
[PM2] PM2 Successfully daemonized
[PM2] Starting /workspace/helperbot/dist/index.js in fork_mode (1 instance)
[PM2] Done.
┌─────┬──────────┬─────────────┬─────────┬─────────┬──────────┬────────┬──────┬───────────┬──────────┬──────────┬──────────┬──────────┐
│ id  │ name     │ namespace   │ version │ mode    │ pid      │ uptime │ ↺    │ status    │ cpu      │ mem      │ user     │ watching │
├─────┼──────────┼─────────────┼─────────┼─────────┼──────────┼────────┼──────┼───────────┼──────────┼──────────┼──────────┼──────────┤
│ 0   │ index    │ default     │ 1.0.0   │ fork    │ 1527     │ 0s     │ 0    │ online    │ 0%       │ 31.8mb   │ gitpod   │ disabled │
└─────┴──────────┴─────────────┴─────────┴─────────┴──────────┴────────┴──────┴───────────┴──────────┴──────────┴──────────┴──────────┘
┌─────┬──────────┬─────────────┬─────────┬─────────┬──────────┬────────┬──────┬───────────┬──────────┬──────────┬──────────┬──────────┐
│ id  │ name     │ namespace   │ version │ mode    │ pid      │ uptime │ ↺    │ status    │ cpu      │ mem      │ user     │ watching │
├─────┼──────────┼─────────────┼─────────┼─────────┼──────────┼────────┼──────┼───────────┼──────────┼──────────┼──────────┼──────────┤
│ 0   │ index    │ default     │ 1.0.0   │ fork    │ 1527     │ 0s     │ 0    │ online    │ 0%       │ 53.2mb   │ gitpod   │ disabled │
└─────┴──────────┴─────────────┴─────────┴─────────┴──────────┴────────┴──────┴───────────┴──────────┴──────────┴──────────┴──────────┘
[TAILING] Tailing last 15 lines for [all] processes (change the value with --lines option)
/home/gitpod/.pm2/pm2.log last 15 lines:
PM2        | 2022-06-19T19:43:46: PM2 log: PM2 version          : 5.2.0
PM2        | 2022-06-19T19:43:46: PM2 log: Node.js version      : 16.15.1
PM2        | 2022-06-19T19:43:46: PM2 log: Current arch         : x64
PM2        | 2022-06-19T19:43:46: PM2 log: PM2 home             : /home/gitpod/.pm2
PM2        | 2022-06-19T19:43:46: PM2 log: PM2 PID file         : /home/gitpod/.pm2/pm2.pid
PM2        | 2022-06-19T19:43:46: PM2 log: RPC socket file      : /home/gitpod/.pm2/rpc.sock
PM2        | 2022-06-19T19:43:46: PM2 log: BUS socket file      : /home/gitpod/.pm2/pub.sock
PM2        | 2022-06-19T19:43:46: PM2 log: Application log path : /home/gitpod/.pm2/logs
PM2        | 2022-06-19T19:43:46: PM2 log: Worker Interval      : 30000
PM2        | 2022-06-19T19:43:46: PM2 log: Process dump file    : /home/gitpod/.pm2/dump.pm2
PM2        | 2022-06-19T19:43:46: PM2 log: Concurrent actions   : 2
PM2        | 2022-06-19T19:43:46: PM2 log: SIGTERM timeout      : 1600
PM2        | 2022-06-19T19:43:46: PM2 log: ===============================================================================
PM2        | 2022-06-19T19:43:46: PM2 log: App [index:0] starting in -fork mode-
PM2        | 2022-06-19T19:43:46: PM2 log: App [index:0] online

/home/gitpod/.pm2/logs/index-out.log last 15 lines:
/home/gitpod/.pm2/logs/index-error.log last 15 lines:
0|index  | TelegramError: 401: Unauthorized
0|index  |     at Telegram.callApi (/workspace/helperbot/node_modules/telegraf/lib/core/network/client.js:264:19)
0|index  |     at processTicksAndRejections (node:internal/process/task_queues:96:5)
0|index  |     at Telegraf.launch (/workspace/helperbot/node_modules/telegraf/lib/telegraf.js:100:78) {
0|index  |   response: { ok: false, error_code: 401, description: 'Unauthorized' },
0|index  |   on: { method: 'getMe', payload: {} }
0|index  | }
PM2      | App [index:0] exited with code [0] via signal [SIGINT]
PM2      | App [index:0] will restart in 3000ms
PM2      | App [index:0] starting in -fork mode-
PM2      | App [index:0] online
0|index  | TelegramError: 401: Unauthorized
0|index  |     at Telegram.callApi (/workspace/helperbot/node_modules/telegraf/lib/core/network/client.js:264:19)
0|index  |     at processTicksAndRejections (node:internal/process/task_queues:96:5)
0|index  |     at Telegraf.launch (/workspace/helperbot/node_modules/telegraf/lib/telegraf.js:100:78) {
0|index  |   response: { ok: false, error_code: 401, description: 'Unauthorized' },
0|index  |   on: { method: 'getMe', payload: {} }
0|index  | }
PM2      | App [index:0] exited with code [0] via signal [SIGINT]
PM2      | App [index:0] will restart in 4500ms
PM2      | App [index:0] starting in -fork mode-
PM2      | App [index:0] online
0|index  | TelegramError: 401: Unauthorized
0|index  |     at Telegram.callApi (/workspace/helperbot/node_modules/telegraf/lib/core/network/client.js:264:19)
0|index  |     at processTicksAndRejections (node:internal/process/task_queues:96:5)
0|index  |     at Telegraf.launch (/workspace/helperbot/node_modules/telegraf/lib/telegraf.js:100:78) {
0|index  |   response: { ok: false, error_code: 401, description: 'Unauthorized' },
0|index  |   on: { method: 'getMe', payload: {} }
0|index  | }
PM2      | App [index:0] exited with code [0] via signal [SIGINT]
PM2      | App [index:0] will restart in 6750ms
PM2      | App [index:0] starting in -fork mode-
PM2      | App [index:0] online
0|index  | TelegramError: 401: Unauthorized
0|index  |     at Telegram.callApi (/workspace/helperbot/node_modules/telegraf/lib/core/network/client.js:264:19)
0|index  |     at processTicksAndRejections (node:internal/process/task_queues:96:5)
0|index  |     at Telegraf.launch (/workspace/helperbot/node_modules/telegraf/lib/telegraf.js:100:78) {
0|index  |   response: { ok: false, error_code: 401, description: 'Unauthorized' },
0|index  |   on: { method: 'getMe', payload: {} }
0|index  | }
PM2      | App [index:0] exited with code [0] via signal [SIGINT]
PM2      | App [index:0] will restart in 10125ms
```
