```
2022-08-05T13:25:59.8999089Z Requested labels: ubuntu-latest
2022-08-05T13:25:59.8999141Z Job defined at: make-software/dao-contracts/.github/workflows/ci-casper-js-client.yml@refs/pull/81/merge
2022-08-05T13:25:59.8999167Z Waiting for a runner to pick up this job...
2022-08-05T13:26:00.7359854Z Job is waiting for a hosted runner to come online.
2022-08-05T13:26:04.4200917Z Job is about to start running on the hosted runner: GitHub Actions 2 (hosted)
2022-08-05T13:26:08.3088263Z Current runner version: '2.294.0'
2022-08-05T13:26:08.3115883Z ##[group]Operating System
2022-08-05T13:26:08.3116415Z Ubuntu
2022-08-05T13:26:08.3116705Z 20.04.4
2022-08-05T13:26:08.3117060Z LTS
2022-08-05T13:26:08.3117327Z ##[endgroup]
2022-08-05T13:26:08.3117681Z ##[group]Virtual Environment
2022-08-05T13:26:08.3118066Z Environment: ubuntu-20.04
2022-08-05T13:26:08.3118378Z Version: 20220729.1
2022-08-05T13:26:08.3118960Z Included Software: https://github.com/actions/virtual-environments/blob/ubuntu20/20220729.1/images/linux/Ubuntu2004-Readme.md
2022-08-05T13:26:08.3119718Z Image Release: https://github.com/actions/virtual-environments/releases/tag/ubuntu20%2F20220729.1
2022-08-05T13:26:08.3120168Z ##[endgroup]
2022-08-05T13:26:08.3120541Z ##[group]Virtual Environment Provisioner
2022-08-05T13:26:08.3120943Z 1.0.0.0-main-20220725-1
2022-08-05T13:26:08.3121308Z ##[endgroup]
2022-08-05T13:26:08.3122311Z ##[group]GITHUB_TOKEN Permissions
2022-08-05T13:26:08.3122934Z Actions: write
2022-08-05T13:26:08.3123447Z Checks: write
2022-08-05T13:26:08.3123800Z Contents: write
2022-08-05T13:26:08.3124139Z Deployments: write
2022-08-05T13:26:08.3124482Z Discussions: write
2022-08-05T13:26:08.3124766Z Issues: write
2022-08-05T13:26:08.3125117Z Metadata: read
2022-08-05T13:26:08.3125437Z Packages: write
2022-08-05T13:26:08.3125707Z Pages: write
2022-08-05T13:26:08.3126034Z PullRequests: write
2022-08-05T13:26:08.3126426Z RepositoryProjects: write
2022-08-05T13:26:08.3126786Z SecurityEvents: write
2022-08-05T13:26:08.3127129Z Statuses: write
2022-08-05T13:26:08.3127451Z ##[endgroup]
2022-08-05T13:26:08.3131081Z Secret source: Actions
2022-08-05T13:26:08.3131729Z Prepare workflow directory
2022-08-05T13:26:08.4598599Z Prepare all required actions
2022-08-05T13:26:08.4783797Z Getting action download info
2022-08-05T13:26:08.7623641Z Download action repository 'actions/checkout@v2' (SHA:7884fcad6b5d53d10323aee724dc68d8b9096a2e)
2022-08-05T13:26:09.9134171Z Download action repository 'actions/setup-node@v2' (SHA:1f8c6b94b26d0feae1e387ca63ccbdc44d27b561)
2022-08-05T13:26:11.2929717Z ##[group]Checking docker version
2022-08-05T13:26:11.2946551Z ##[command]/usr/bin/docker version --format '{{.Server.APIVersion}}'
2022-08-05T13:26:11.4572195Z '1.41'
2022-08-05T13:26:11.4595141Z Docker daemon API version: '1.41'
2022-08-05T13:26:11.4595520Z ##[command]/usr/bin/docker version --format '{{.Client.APIVersion}}'
2022-08-05T13:26:11.4958860Z '1.41'
2022-08-05T13:26:11.4985768Z Docker client API version: '1.41'
2022-08-05T13:26:11.4993379Z ##[endgroup]
2022-08-05T13:26:11.4996877Z ##[group]Clean up resources from previous jobs
2022-08-05T13:26:11.5002893Z ##[command]/usr/bin/docker ps --all --quiet --no-trunc --filter "label=4cd98f"
2022-08-05T13:26:11.5327320Z ##[command]/usr/bin/docker network prune --force --filter "label=4cd98f"
2022-08-05T13:26:11.5621241Z ##[endgroup]
2022-08-05T13:26:11.5621570Z ##[group]Create local container network
2022-08-05T13:26:11.5633094Z ##[command]/usr/bin/docker network create --label 4cd98f github_network_245660b484a946a1a9d939397e5f343c
2022-08-05T13:26:11.6389012Z cd29dd4088ddbabd64fc92a7653a88985c948ad66f22bd15a01ecc09feed39c8
2022-08-05T13:26:11.6409587Z ##[endgroup]
2022-08-05T13:26:11.6502615Z ##[group]Starting casper-nctl service container
2022-08-05T13:26:11.6524036Z ##[command]/usr/bin/docker pull makesoftware/casper-nctl:v144-220303
2022-08-05T13:26:13.2310874Z v144-220303: Pulling from makesoftware/casper-nctl
2022-08-05T13:26:13.2316390Z 08c01a0ec47e: Pulling fs layer
2022-08-05T13:26:13.2316716Z b25a0d084e6c: Pulling fs layer
2022-08-05T13:26:13.2316985Z 8a8b8c037d14: Pulling fs layer
2022-08-05T13:26:13.2317238Z 3e4ad4f1a5f6: Pulling fs layer
2022-08-05T13:26:13.2317504Z 4f4fb700ef54: Pulling fs layer
2022-08-05T13:26:13.2317768Z 63769906b684: Pulling fs layer
2022-08-05T13:26:13.2318012Z 4d4354bdcee9: Pulling fs layer
2022-08-05T13:26:13.2318271Z 7b9a538e3db9: Pulling fs layer
2022-08-05T13:26:13.2318561Z 282a27f7e8a5: Pulling fs layer
2022-08-05T13:26:13.2318931Z cd3342f6c0ba: Pulling fs layer
2022-08-05T13:26:13.2319545Z ca0f8fe31cc0: Pulling fs layer
2022-08-05T13:26:13.2319815Z 8b5d6530e04c: Pulling fs layer
2022-08-05T13:26:13.2320046Z 3e4ad4f1a5f6: Waiting
2022-08-05T13:26:13.2320283Z 4f4fb700ef54: Waiting
2022-08-05T13:26:13.2320514Z 63769906b684: Waiting
2022-08-05T13:26:13.2320724Z 4d4354bdcee9: Waiting
2022-08-05T13:26:13.2320965Z 7b9a538e3db9: Waiting
2022-08-05T13:26:13.2321191Z 282a27f7e8a5: Waiting
2022-08-05T13:26:13.2321403Z cd3342f6c0ba: Waiting
2022-08-05T13:26:13.2321637Z ca0f8fe31cc0: Waiting
2022-08-05T13:26:13.2321893Z 8b5d6530e04c: Waiting
2022-08-05T13:26:13.7957309Z 8a8b8c037d14: Verifying Checksum
2022-08-05T13:26:13.7957841Z 8a8b8c037d14: Download complete
2022-08-05T13:26:14.0664269Z 08c01a0ec47e: Verifying Checksum
2022-08-05T13:26:14.0667755Z 08c01a0ec47e: Download complete
2022-08-05T13:26:14.3413333Z 3e4ad4f1a5f6: Verifying Checksum
2022-08-05T13:26:14.3413637Z 3e4ad4f1a5f6: Download complete
2022-08-05T13:26:14.4535340Z 4f4fb700ef54: Verifying Checksum
2022-08-05T13:26:14.4535714Z 4f4fb700ef54: Download complete
2022-08-05T13:26:14.8984253Z 63769906b684: Verifying Checksum
2022-08-05T13:26:14.8985863Z 63769906b684: Download complete
2022-08-05T13:26:15.1782686Z 08c01a0ec47e: Pull complete
2022-08-05T13:26:15.2570651Z 4d4354bdcee9: Verifying Checksum
2022-08-05T13:26:15.2573139Z 4d4354bdcee9: Download complete
2022-08-05T13:26:15.7650151Z 282a27f7e8a5: Download complete
2022-08-05T13:26:16.3583668Z cd3342f6c0ba: Verifying Checksum
2022-08-05T13:26:16.3595103Z cd3342f6c0ba: Download complete
2022-08-05T13:26:16.5020793Z b25a0d084e6c: Verifying Checksum
2022-08-05T13:26:16.5021114Z b25a0d084e6c: Download complete
2022-08-05T13:26:16.9561771Z ca0f8fe31cc0: Verifying Checksum
2022-08-05T13:26:16.9562085Z ca0f8fe31cc0: Download complete
2022-08-05T13:26:17.0020021Z 7b9a538e3db9: Verifying Checksum
2022-08-05T13:26:17.0020920Z 7b9a538e3db9: Download complete
2022-08-05T13:26:17.3062138Z 8b5d6530e04c: Verifying Checksum
2022-08-05T13:26:17.3062399Z 8b5d6530e04c: Download complete
2022-08-05T13:26:22.8643303Z b25a0d084e6c: Pull complete
2022-08-05T13:26:22.9286085Z 8a8b8c037d14: Pull complete
2022-08-05T13:26:22.9924013Z 3e4ad4f1a5f6: Pull complete
2022-08-05T13:26:23.0498906Z 4f4fb700ef54: Pull complete
2022-08-05T13:26:23.1245010Z 63769906b684: Pull complete
2022-08-05T13:26:23.2683890Z 4d4354bdcee9: Pull complete
2022-08-05T13:26:24.7496997Z 7b9a538e3db9: Pull complete
2022-08-05T13:26:24.8148282Z 282a27f7e8a5: Pull complete
2022-08-05T13:26:24.8737784Z cd3342f6c0ba: Pull complete
2022-08-05T13:26:24.9330892Z ca0f8fe31cc0: Pull complete
2022-08-05T13:26:24.9963490Z 8b5d6530e04c: Pull complete
2022-08-05T13:26:25.0018291Z Digest: sha256:87fc1759c9a7239594b9ea574d048f92925919a8a0fc168b5e230e75aa8b892c
2022-08-05T13:26:25.0038641Z Status: Downloaded newer image for makesoftware/casper-nctl:v144-220303
2022-08-05T13:26:25.0057803Z docker.io/makesoftware/casper-nctl:v144-220303
2022-08-05T13:26:25.0145053Z ##[command]/usr/bin/docker create --name e3bbe42de4f541f0a2fc53325e822296_makesoftwarecaspernctlv144220303_c1c81f --label 4cd98f --network github_network_245660b484a946a1a9d939397e5f343c --network-alias casper-nctl -p 11101:11101 -p 14101:14101 -p 18101:18101 --name casper-nctl -e "PREDEFINED_ACCOUNTS=true" -e "MINIMUM_ROUND_EXPONENT=12" -e "MAXIMUM_ROUND_EXPONENT=13" -e "DEPLOY_DELAY=2sec" -e GITHUB_ACTIONS=true -e CI=true -v "/tmp":"/home/casper/casper-node/utils/nctl/assets" makesoftware/casper-nctl:v144-220303
2022-08-05T13:26:25.0685698Z 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:25.0718390Z ##[command]/usr/bin/docker start 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:25.5125328Z 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:25.5152327Z ##[command]/usr/bin/docker ps --all --filter id=694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b --filter status=running --no-trunc --format "{{.ID}} {{.Status}}"
2022-08-05T13:26:25.5513516Z 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b Up Less than a second (health: starting)
2022-08-05T13:26:25.5543197Z ##[command]/usr/bin/docker port 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:25.5861918Z 14101/tcp -> 0.0.0.0:14101
2022-08-05T13:26:25.5862581Z 14101/tcp -> :::14101
2022-08-05T13:26:25.5863524Z 18101/tcp -> 0.0.0.0:18101
2022-08-05T13:26:25.5863853Z 18101/tcp -> :::18101
2022-08-05T13:26:25.5864205Z 11101/tcp -> 0.0.0.0:11101
2022-08-05T13:26:25.5864648Z 11101/tcp -> :::11101
2022-08-05T13:26:25.5957814Z ##[endgroup]
2022-08-05T13:26:25.5958171Z ##[group]Waiting for all services to be ready
2022-08-05T13:26:25.6000022Z ##[command]/usr/bin/docker inspect --format="{{if .Config.Healthcheck}}{{print .State.Health.Status}}{{end}}" 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:25.6311189Z starting
2022-08-05T13:26:25.6339111Z casper-nctl service is starting, waiting 2 seconds before checking again.
2022-08-05T13:26:27.6353505Z ##[command]/usr/bin/docker inspect --format="{{if .Config.Healthcheck}}{{print .State.Health.Status}}{{end}}" 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:27.6723808Z starting
2022-08-05T13:26:27.6741439Z casper-nctl service is starting, waiting 4 seconds before checking again.
2022-08-05T13:26:31.8534182Z ##[command]/usr/bin/docker inspect --format="{{if .Config.Healthcheck}}{{print .State.Health.Status}}{{end}}" 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:31.8908566Z starting
2022-08-05T13:26:31.8926260Z casper-nctl service is starting, waiting 7 seconds before checking again.
2022-08-05T13:26:39.3942342Z ##[command]/usr/bin/docker inspect --format="{{if .Config.Healthcheck}}{{print .State.Health.Status}}{{end}}" 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:39.4272948Z starting
2022-08-05T13:26:39.4287552Z casper-nctl service is starting, waiting 13 seconds before checking again.
2022-08-05T13:26:53.0905172Z ##[command]/usr/bin/docker inspect --format="{{if .Config.Healthcheck}}{{print .State.Health.Status}}{{end}}" 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:26:53.1207818Z starting
2022-08-05T13:26:53.1223412Z casper-nctl service is starting, waiting 32 seconds before checking again.
2022-08-05T13:27:25.1213683Z ##[command]/usr/bin/docker inspect --format="{{if .Config.Healthcheck}}{{print .State.Health.Status}}{{end}}" 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:27:25.1523835Z healthy
2022-08-05T13:27:25.1541723Z casper-nctl service is healthy.
2022-08-05T13:27:25.1542413Z ##[endgroup]
2022-08-05T13:27:25.1863887Z ##[group]Run sudo chown runner $NCTL_USERS_FOLDER_PATH/*/*
2022-08-05T13:27:25.1864295Z [36;1msudo chown runner $NCTL_USERS_FOLDER_PATH/*/*[0m
2022-08-05T13:27:25.1923817Z shell: /usr/bin/bash -e {0}
2022-08-05T13:27:25.1924069Z env:
2022-08-05T13:27:25.1924252Z   NODE_ENV: ci
2022-08-05T13:27:25.1924553Z   WASM_RELEASE_PATH: /home/runner/work/dao-contracts/dao-contracts/client/wasm
2022-08-05T13:27:25.1924893Z   NCTL_USERS_FOLDER_PATH: /tmp/net-1/users
2022-08-05T13:27:25.1925131Z   CHAIN_NAME: casper-net-1
2022-08-05T13:27:25.1925407Z   NODE_ADDRESS: http://localhost:11101/rpc
2022-08-05T13:27:25.1925710Z   EVENT_STREAM_ADDRESS: http://localhost:18101/events/main
2022-08-05T13:27:25.1925979Z   INSTALL_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:25.1926225Z   DEPLOY_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:25.1926455Z ##[endgroup]
2022-08-05T13:27:25.2426757Z ##[group]Run actions/checkout@v2
2022-08-05T13:27:25.2427039Z with:
2022-08-05T13:27:25.2427286Z   repository: make-software/dao-contracts
2022-08-05T13:27:25.2427686Z   token: ***
2022-08-05T13:27:25.2427889Z   ssh-strict: true
2022-08-05T13:27:25.2428129Z   persist-credentials: true
2022-08-05T13:27:25.2428341Z   clean: true
2022-08-05T13:27:25.2428611Z   fetch-depth: 1
2022-08-05T13:27:25.2428809Z   lfs: false
2022-08-05T13:27:25.2428992Z   submodules: false
2022-08-05T13:27:25.2429440Z   set-safe-directory: true
2022-08-05T13:27:25.2429666Z env:
2022-08-05T13:27:25.2429839Z   NODE_ENV: ci
2022-08-05T13:27:25.2430134Z   WASM_RELEASE_PATH: /home/runner/work/dao-contracts/dao-contracts/client/wasm
2022-08-05T13:27:25.2430458Z   NCTL_USERS_FOLDER_PATH: /tmp/net-1/users
2022-08-05T13:27:25.2430694Z   CHAIN_NAME: casper-net-1
2022-08-05T13:27:25.2430972Z   NODE_ADDRESS: http://localhost:11101/rpc
2022-08-05T13:27:25.2431308Z   EVENT_STREAM_ADDRESS: http://localhost:18101/events/main
2022-08-05T13:27:25.2431589Z   INSTALL_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:25.2431822Z   DEPLOY_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:25.2432051Z ##[endgroup]
2022-08-05T13:27:25.4962052Z Syncing repository: make-software/dao-contracts
2022-08-05T13:27:25.4963739Z ##[group]Getting Git version info
2022-08-05T13:27:25.4964247Z Working directory is '/home/runner/work/dao-contracts/dao-contracts'
2022-08-05T13:27:25.4964770Z [command]/usr/bin/git version
2022-08-05T13:27:25.5085036Z git version 2.37.1
2022-08-05T13:27:25.5106967Z ##[endgroup]
2022-08-05T13:27:25.5125380Z Temporarily overriding HOME='/home/runner/work/_temp/fe1f17e1-9d3c-4027-8d15-ec708f8040fe' before making global git config changes
2022-08-05T13:27:25.5126227Z Adding repository directory to the temporary git global config as a safe directory
2022-08-05T13:27:25.5127129Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/dao-contracts/dao-contracts
2022-08-05T13:27:25.5219550Z Deleting the contents of '/home/runner/work/dao-contracts/dao-contracts'
2022-08-05T13:27:25.5225000Z ##[group]Initializing the repository
2022-08-05T13:27:25.5229743Z [command]/usr/bin/git init /home/runner/work/dao-contracts/dao-contracts
2022-08-05T13:27:25.5307870Z hint: Using 'master' as the name for the initial branch. This default branch name
2022-08-05T13:27:25.5308976Z hint: is subject to change. To configure the initial branch name to use in all
2022-08-05T13:27:25.5309607Z hint: of your new repositories, which will suppress this warning, call:
2022-08-05T13:27:25.5310842Z hint: 
2022-08-05T13:27:25.5311724Z hint: 	git config --global init.defaultBranch <name>
2022-08-05T13:27:25.5312069Z hint: 
2022-08-05T13:27:25.5312869Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2022-08-05T13:27:25.5313424Z hint: 'development'. The just-created branch can be renamed via this command:
2022-08-05T13:27:25.5313763Z hint: 
2022-08-05T13:27:25.5314473Z hint: 	git branch -m <name>
2022-08-05T13:27:25.5316916Z Initialized empty Git repository in /home/runner/work/dao-contracts/dao-contracts/.git/
2022-08-05T13:27:25.5326378Z [command]/usr/bin/git remote add origin https://github.com/make-software/dao-contracts
2022-08-05T13:27:25.5371401Z ##[endgroup]
2022-08-05T13:27:25.5371972Z ##[group]Disabling automatic garbage collection
2022-08-05T13:27:25.5377970Z [command]/usr/bin/git config --local gc.auto 0
2022-08-05T13:27:25.5411543Z ##[endgroup]
2022-08-05T13:27:25.5412102Z ##[group]Setting up auth
2022-08-05T13:27:25.5422192Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2022-08-05T13:27:25.5458428Z [command]/usr/bin/git submodule foreach --recursive git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :
2022-08-05T13:27:25.5836624Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2022-08-05T13:27:25.5857954Z [command]/usr/bin/git submodule foreach --recursive git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :
2022-08-05T13:27:25.6096013Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2022-08-05T13:27:25.6284586Z ##[endgroup]
2022-08-05T13:27:25.6285031Z ##[group]Fetching the repository
2022-08-05T13:27:25.6285982Z [command]/usr/bin/git -c protocol.version=2 fetch --no-tags --prune --progress --no-recurse-submodules --depth=1 origin +9856e76ddea88902a5c3897fe622852d01d36295:refs/remotes/pull/81/merge
2022-08-05T13:27:26.2519187Z remote: Enumerating objects: 186, done.        
2022-08-05T13:27:26.2532526Z remote: Counting objects:   0% (1/186)        
2022-08-05T13:27:26.2533162Z remote: Counting objects:   1% (2/186)        
2022-08-05T13:27:26.2533777Z remote: Counting objects:   2% (4/186)        
2022-08-05T13:27:26.2534362Z remote: Counting objects:   3% (6/186)        
2022-08-05T13:27:26.2534970Z remote: Counting objects:   4% (8/186)        
2022-08-05T13:27:26.2535542Z remote: Counting objects:   5% (10/186)        
2022-08-05T13:27:26.2536128Z remote: Counting objects:   6% (12/186)        
2022-08-05T13:27:26.2536708Z remote: Counting objects:   7% (14/186)        
2022-08-05T13:27:26.2537285Z remote: Counting objects:   8% (15/186)        
2022-08-05T13:27:26.2537845Z remote: Counting objects:   9% (17/186)        
2022-08-05T13:27:26.2538430Z remote: Counting objects:  10% (19/186)        
2022-08-05T13:27:26.2539033Z remote: Counting objects:  11% (21/186)        
2022-08-05T13:27:26.2539606Z remote: Counting objects:  12% (23/186)        
2022-08-05T13:27:26.2540740Z remote: Counting objects:  13% (25/186)        
2022-08-05T13:27:26.2541405Z remote: Counting objects:  14% (27/186)        
2022-08-05T13:27:26.2545085Z remote: Counting objects:  15% (28/186)        
2022-08-05T13:27:26.2545592Z remote: Counting objects:  16% (30/186)        
2022-08-05T13:27:26.2546193Z remote: Counting objects:  17% (32/186)        
2022-08-05T13:27:26.2546776Z remote: Counting objects:  18% (34/186)        
2022-08-05T13:27:26.2547349Z remote: Counting objects:  19% (36/186)        
2022-08-05T13:27:26.2547904Z remote: Counting objects:  20% (38/186)        
2022-08-05T13:27:26.2548483Z remote: Counting objects:  21% (40/186)        
2022-08-05T13:27:26.2549061Z remote: Counting objects:  22% (41/186)        
2022-08-05T13:27:26.2549622Z remote: Counting objects:  23% (43/186)        
2022-08-05T13:27:26.2550205Z remote: Counting objects:  24% (45/186)        
2022-08-05T13:27:26.2550783Z remote: Counting objects:  25% (47/186)        
2022-08-05T13:27:26.2551352Z remote: Counting objects:  26% (49/186)        
2022-08-05T13:27:26.2551908Z remote: Counting objects:  27% (51/186)        
2022-08-05T13:27:26.2552473Z remote: Counting objects:  28% (53/186)        
2022-08-05T13:27:26.2553047Z remote: Counting objects:  29% (54/186)        
2022-08-05T13:27:26.2553986Z remote: Counting objects:  30% (56/186)        
2022-08-05T13:27:26.2554473Z remote: Counting objects:  31% (58/186)        
2022-08-05T13:27:26.2584452Z remote: Counting objects:  32% (60/186)        
2022-08-05T13:27:26.2585101Z remote: Counting objects:  33% (62/186)        
2022-08-05T13:27:26.2585697Z remote: Counting objects:  34% (64/186)        
2022-08-05T13:27:26.2586255Z remote: Counting objects:  35% (66/186)        
2022-08-05T13:27:26.2586829Z remote: Counting objects:  36% (67/186)        
2022-08-05T13:27:26.2587406Z remote: Counting objects:  37% (69/186)        
2022-08-05T13:27:26.2587999Z remote: Counting objects:  38% (71/186)        
2022-08-05T13:27:26.2588554Z remote: Counting objects:  39% (73/186)        
2022-08-05T13:27:26.2589131Z remote: Counting objects:  40% (75/186)        
2022-08-05T13:27:26.2589708Z remote: Counting objects:  41% (77/186)        
2022-08-05T13:27:26.2590283Z remote: Counting objects:  42% (79/186)        
2022-08-05T13:27:26.2590838Z remote: Counting objects:  43% (80/186)        
2022-08-05T13:27:26.2591791Z remote: Counting objects:  44% (82/186)        
2022-08-05T13:27:26.2592303Z remote: Counting objects:  45% (84/186)        
2022-08-05T13:27:26.2592883Z remote: Counting objects:  46% (86/186)        
2022-08-05T13:27:26.2593609Z remote: Counting objects:  47% (88/186)        
2022-08-05T13:27:26.2594190Z remote: Counting objects:  48% (90/186)        
2022-08-05T13:27:26.2594993Z remote: Counting objects:  49% (92/186)        
2022-08-05T13:27:26.2595490Z remote: Counting objects:  50% (93/186)        
2022-08-05T13:27:26.2596234Z remote: Counting objects:  51% (95/186)        
2022-08-05T13:27:26.2597002Z remote: Counting objects:  52% (97/186)        
2022-08-05T13:27:26.2597435Z remote: Counting objects:  53% (99/186)        
2022-08-05T13:27:26.2597953Z remote: Counting objects:  54% (101/186)        
2022-08-05T13:27:26.2598457Z remote: Counting objects:  55% (103/186)        
2022-08-05T13:27:26.2598975Z remote: Counting objects:  56% (105/186)        
2022-08-05T13:27:26.2599493Z remote: Counting objects:  57% (107/186)        
2022-08-05T13:27:26.2600006Z remote: Counting objects:  58% (108/186)        
2022-08-05T13:27:26.2600501Z remote: Counting objects:  59% (110/186)        
2022-08-05T13:27:26.2601007Z remote: Counting objects:  60% (112/186)        
2022-08-05T13:27:26.2601514Z remote: Counting objects:  61% (114/186)        
2022-08-05T13:27:26.2602004Z remote: Counting objects:  62% (116/186)        
2022-08-05T13:27:26.2602506Z remote: Counting objects:  63% (118/186)        
2022-08-05T13:27:26.2603023Z remote: Counting objects:  64% (120/186)        
2022-08-05T13:27:26.2603534Z remote: Counting objects:  65% (121/186)        
2022-08-05T13:27:26.2604026Z remote: Counting objects:  66% (123/186)        
2022-08-05T13:27:26.2604536Z remote: Counting objects:  67% (125/186)        
2022-08-05T13:27:26.2605057Z remote: Counting objects:  68% (127/186)        
2022-08-05T13:27:26.2605564Z remote: Counting objects:  69% (129/186)        
2022-08-05T13:27:26.2606059Z remote: Counting objects:  70% (131/186)        
2022-08-05T13:27:26.2606567Z remote: Counting objects:  71% (133/186)        
2022-08-05T13:27:26.2607190Z remote: Counting objects:  72% (134/186)        
2022-08-05T13:27:26.2641119Z remote: Counting objects:  73% (136/186)        
2022-08-05T13:27:26.2641998Z remote: Counting objects:  74% (138/186)        
2022-08-05T13:27:26.2642364Z remote: Counting objects:  75% (140/186)        
2022-08-05T13:27:26.2642638Z remote: Counting objects:  76% (142/186)        
2022-08-05T13:27:26.2642913Z remote: Counting objects:  77% (144/186)        
2022-08-05T13:27:26.2643429Z remote: Counting objects:  78% (146/186)        
2022-08-05T13:27:26.2643950Z remote: Counting objects:  79% (147/186)        
2022-08-05T13:27:26.2644462Z remote: Counting objects:  80% (149/186)        
2022-08-05T13:27:26.2644962Z remote: Counting objects:  81% (151/186)        
2022-08-05T13:27:26.2645465Z remote: Counting objects:  82% (153/186)        
2022-08-05T13:27:26.2646004Z remote: Counting objects:  83% (155/186)        
2022-08-05T13:27:26.2646511Z remote: Counting objects:  84% (157/186)        
2022-08-05T13:27:26.2647265Z remote: Counting objects:  85% (159/186)        
2022-08-05T13:27:26.2648618Z remote: Counting objects:  86% (160/186)        
2022-08-05T13:27:26.2649038Z remote: Counting objects:  87% (162/186)        
2022-08-05T13:27:26.2649861Z remote: Counting objects:  88% (164/186)        
2022-08-05T13:27:26.2650533Z remote: Counting objects:  89% (166/186)        
2022-08-05T13:27:26.2651196Z remote: Counting objects:  90% (168/186)        
2022-08-05T13:27:26.2651734Z remote: Counting objects:  91% (170/186)        
2022-08-05T13:27:26.2652253Z remote: Counting objects:  92% (172/186)        
2022-08-05T13:27:26.2652920Z remote: Counting objects:  93% (173/186)        
2022-08-05T13:27:26.2653450Z remote: Counting objects:  94% (175/186)        
2022-08-05T13:27:26.2653968Z remote: Counting objects:  95% (177/186)        
2022-08-05T13:27:26.2654793Z remote: Counting objects:  96% (179/186)        
2022-08-05T13:27:26.2655247Z remote: Counting objects:  97% (181/186)        
2022-08-05T13:27:26.2655771Z remote: Counting objects:  98% (183/186)        
2022-08-05T13:27:26.2656462Z remote: Counting objects:  99% (185/186)        
2022-08-05T13:27:26.2657189Z remote: Counting objects: 100% (186/186)        
2022-08-05T13:27:26.2657844Z remote: Counting objects: 100% (186/186), done.        
2022-08-05T13:27:26.2658576Z remote: Compressing objects:   0% (1/169)        
2022-08-05T13:27:26.2659146Z remote: Compressing objects:   1% (2/169)        
2022-08-05T13:27:26.2659683Z remote: Compressing objects:   2% (4/169)        
2022-08-05T13:27:26.2660350Z remote: Compressing objects:   3% (6/169)        
2022-08-05T13:27:26.3142635Z remote: Compressing objects:   4% (7/169)        
2022-08-05T13:27:26.3143016Z remote: Compressing objects:   5% (9/169)        
2022-08-05T13:27:26.3143342Z remote: Compressing objects:   6% (11/169)        
2022-08-05T13:27:26.3143679Z remote: Compressing objects:   7% (12/169)        
2022-08-05T13:27:26.3143985Z remote: Compressing objects:   8% (14/169)        
2022-08-05T13:27:26.3144304Z remote: Compressing objects:   9% (16/169)        
2022-08-05T13:27:26.3144622Z remote: Compressing objects:  10% (17/169)        
2022-08-05T13:27:26.3144926Z remote: Compressing objects:  11% (19/169)        
2022-08-05T13:27:26.3145241Z remote: Compressing objects:  12% (21/169)        
2022-08-05T13:27:26.3145549Z remote: Compressing objects:  13% (22/169)        
2022-08-05T13:27:26.3145860Z remote: Compressing objects:  14% (24/169)        
2022-08-05T13:27:26.3146174Z remote: Compressing objects:  15% (26/169)        
2022-08-05T13:27:26.3146490Z remote: Compressing objects:  16% (28/169)        
2022-08-05T13:27:26.3146807Z remote: Compressing objects:  17% (29/169)        
2022-08-05T13:27:26.3147103Z remote: Compressing objects:  18% (31/169)        
2022-08-05T13:27:26.3147419Z remote: Compressing objects:  19% (33/169)        
2022-08-05T13:27:26.3147736Z remote: Compressing objects:  20% (34/169)        
2022-08-05T13:27:26.3148036Z remote: Compressing objects:  21% (36/169)        
2022-08-05T13:27:26.3148353Z remote: Compressing objects:  22% (38/169)        
2022-08-05T13:27:26.3148691Z remote: Compressing objects:  23% (39/169)        
2022-08-05T13:27:26.3149000Z remote: Compressing objects:  24% (41/169)        
2022-08-05T13:27:26.3149313Z remote: Compressing objects:  25% (43/169)        
2022-08-05T13:27:26.3149851Z remote: Compressing objects:  26% (44/169)        
2022-08-05T13:27:26.3151023Z remote: Compressing objects:  27% (46/169)        
2022-08-05T13:27:26.3151722Z remote: Compressing objects:  28% (48/169)        
2022-08-05T13:27:26.3152326Z remote: Compressing objects:  29% (50/169)        
2022-08-05T13:27:26.3152902Z remote: Compressing objects:  30% (51/169)        
2022-08-05T13:27:26.3153493Z remote: Compressing objects:  31% (53/169)        
2022-08-05T13:27:26.3154089Z remote: Compressing objects:  32% (55/169)        
2022-08-05T13:27:26.3154680Z remote: Compressing objects:  33% (56/169)        
2022-08-05T13:27:26.3155491Z remote: Compressing objects:  34% (58/169)        
2022-08-05T13:27:26.3161559Z remote: Compressing objects:  35% (60/169)        
2022-08-05T13:27:26.3162122Z remote: Compressing objects:  36% (61/169)        
2022-08-05T13:27:26.3162733Z remote: Compressing objects:  37% (63/169)        
2022-08-05T13:27:26.3163324Z remote: Compressing objects:  38% (65/169)        
2022-08-05T13:27:26.3163925Z remote: Compressing objects:  39% (66/169)        
2022-08-05T13:27:26.3164535Z remote: Compressing objects:  40% (68/169)        
2022-08-05T13:27:26.3165127Z remote: Compressing objects:  41% (70/169)        
2022-08-05T13:27:26.3165708Z remote: Compressing objects:  42% (71/169)        
2022-08-05T13:27:26.3166299Z remote: Compressing objects:  43% (73/169)        
2022-08-05T13:27:26.3166893Z remote: Compressing objects:  44% (75/169)        
2022-08-05T13:27:26.3167493Z remote: Compressing objects:  45% (77/169)        
2022-08-05T13:27:26.3168459Z remote: Compressing objects:  46% (78/169)        
2022-08-05T13:27:26.3168990Z remote: Compressing objects:  47% (80/169)        
2022-08-05T13:27:26.3169586Z remote: Compressing objects:  48% (82/169)        
2022-08-05T13:27:26.3170178Z remote: Compressing objects:  49% (83/169)        
2022-08-05T13:27:26.3170761Z remote: Compressing objects:  50% (85/169)        
2022-08-05T13:27:26.3171358Z remote: Compressing objects:  51% (87/169)        
2022-08-05T13:27:26.3171992Z remote: Compressing objects:  52% (88/169)        
2022-08-05T13:27:26.3172865Z remote: Compressing objects:  53% (90/169)        
2022-08-05T13:27:26.3173464Z remote: Compressing objects:  54% (92/169)        
2022-08-05T13:27:26.3174054Z remote: Compressing objects:  55% (93/169)        
2022-08-05T13:27:26.3174644Z remote: Compressing objects:  56% (95/169)        
2022-08-05T13:27:26.3175224Z remote: Compressing objects:  57% (97/169)        
2022-08-05T13:27:26.3175819Z remote: Compressing objects:  58% (99/169)        
2022-08-05T13:27:26.3176422Z remote: Compressing objects:  59% (100/169)        
2022-08-05T13:27:26.3177029Z remote: Compressing objects:  60% (102/169)        
2022-08-05T13:27:26.3177853Z remote: Compressing objects:  61% (104/169)        
2022-08-05T13:27:26.3178450Z remote: Compressing objects:  62% (105/169)        
2022-08-05T13:27:26.3179046Z remote: Compressing objects:  63% (107/169)        
2022-08-05T13:27:26.3179644Z remote: Compressing objects:  64% (109/169)        
2022-08-05T13:27:26.3180230Z remote: Compressing objects:  65% (110/169)        
2022-08-05T13:27:26.3180827Z remote: Compressing objects:  66% (112/169)        
2022-08-05T13:27:26.3181431Z remote: Compressing objects:  67% (114/169)        
2022-08-05T13:27:26.3182028Z remote: Compressing objects:  68% (115/169)        
2022-08-05T13:27:26.3182611Z remote: Compressing objects:  69% (117/169)        
2022-08-05T13:27:26.3183209Z remote: Compressing objects:  70% (119/169)        
2022-08-05T13:27:26.3183806Z remote: Compressing objects:  71% (120/169)        
2022-08-05T13:27:26.3184399Z remote: Compressing objects:  72% (122/169)        
2022-08-05T13:27:26.3184974Z remote: Compressing objects:  73% (124/169)        
2022-08-05T13:27:26.3185561Z remote: Compressing objects:  74% (126/169)        
2022-08-05T13:27:26.3186200Z remote: Compressing objects:  75% (127/169)        
2022-08-05T13:27:26.3186803Z remote: Compressing objects:  76% (129/169)        
2022-08-05T13:27:26.3187395Z remote: Compressing objects:  77% (131/169)        
2022-08-05T13:27:26.3187992Z remote: Compressing objects:  78% (132/169)        
2022-08-05T13:27:26.3188586Z remote: Compressing objects:  79% (134/169)        
2022-08-05T13:27:26.3189174Z remote: Compressing objects:  80% (136/169)        
2022-08-05T13:27:26.3189751Z remote: Compressing objects:  81% (137/169)        
2022-08-05T13:27:26.3190353Z remote: Compressing objects:  82% (139/169)        
2022-08-05T13:27:26.3190951Z remote: Compressing objects:  83% (141/169)        
2022-08-05T13:27:26.3191554Z remote: Compressing objects:  84% (142/169)        
2022-08-05T13:27:26.3192128Z remote: Compressing objects:  85% (144/169)        
2022-08-05T13:27:26.3192716Z remote: Compressing objects:  86% (146/169)        
2022-08-05T13:27:26.3193312Z remote: Compressing objects:  87% (148/169)        
2022-08-05T13:27:26.3193906Z remote: Compressing objects:  88% (149/169)        
2022-08-05T13:27:26.3194483Z remote: Compressing objects:  89% (151/169)        
2022-08-05T13:27:26.3195072Z remote: Compressing objects:  90% (153/169)        
2022-08-05T13:27:26.3195742Z remote: Compressing objects:  91% (154/169)        
2022-08-05T13:27:26.3196327Z remote: Compressing objects:  92% (156/169)        
2022-08-05T13:27:26.3196904Z remote: Compressing objects:  93% (158/169)        
2022-08-05T13:27:26.3197487Z remote: Compressing objects:  94% (159/169)        
2022-08-05T13:27:26.3198074Z remote: Compressing objects:  95% (161/169)        
2022-08-05T13:27:26.3198648Z remote: Compressing objects:  96% (163/169)        
2022-08-05T13:27:26.3199464Z remote: Compressing objects:  97% (164/169)        
2022-08-05T13:27:26.3199982Z remote: Compressing objects:  98% (166/169)        
2022-08-05T13:27:26.3200577Z remote: Compressing objects:  99% (168/169)        
2022-08-05T13:27:26.3201153Z remote: Compressing objects: 100% (169/169)        
2022-08-05T13:27:26.3201798Z remote: Compressing objects: 100% (169/169), done.        
2022-08-05T13:27:26.3285620Z Receiving objects:   0% (1/186)
2022-08-05T13:27:26.3285910Z Receiving objects:   1% (2/186)
2022-08-05T13:27:26.3286374Z Receiving objects:   2% (4/186)
2022-08-05T13:27:26.3286609Z Receiving objects:   3% (6/186)
2022-08-05T13:27:26.3290184Z Receiving objects:   4% (8/186)
2022-08-05T13:27:26.3932775Z Receiving objects:   5% (10/186)
2022-08-05T13:27:26.3933280Z Receiving objects:   6% (12/186)
2022-08-05T13:27:26.3933525Z Receiving objects:   7% (14/186)
2022-08-05T13:27:26.3933769Z Receiving objects:   8% (15/186)
2022-08-05T13:27:26.3936460Z Receiving objects:   9% (17/186)
2022-08-05T13:27:26.3937056Z Receiving objects:  10% (19/186)
2022-08-05T13:27:26.3937344Z Receiving objects:  11% (21/186)
2022-08-05T13:27:26.3937585Z Receiving objects:  12% (23/186)
2022-08-05T13:27:26.3937823Z Receiving objects:  13% (25/186)
2022-08-05T13:27:26.3938044Z Receiving objects:  14% (27/186)
2022-08-05T13:27:26.3938276Z Receiving objects:  15% (28/186)
2022-08-05T13:27:26.3938512Z Receiving objects:  16% (30/186)
2022-08-05T13:27:26.4013692Z Receiving objects:  17% (32/186)
2022-08-05T13:27:26.4014105Z Receiving objects:  18% (34/186)
2022-08-05T13:27:26.4014345Z Receiving objects:  19% (36/186)
2022-08-05T13:27:26.4687291Z Receiving objects:  20% (38/186)
2022-08-05T13:27:26.4689709Z Receiving objects:  21% (40/186)
2022-08-05T13:27:26.4690604Z Receiving objects:  22% (41/186)
2022-08-05T13:27:26.4691422Z Receiving objects:  23% (43/186)
2022-08-05T13:27:26.4691734Z Receiving objects:  24% (45/186)
2022-08-05T13:27:26.4692013Z Receiving objects:  25% (47/186)
2022-08-05T13:27:26.4694638Z Receiving objects:  26% (49/186)
2022-08-05T13:27:26.4695150Z Receiving objects:  27% (51/186)
2022-08-05T13:27:26.4696267Z Receiving objects:  28% (53/186)
2022-08-05T13:27:26.4697434Z Receiving objects:  29% (54/186)
2022-08-05T13:27:26.4698943Z Receiving objects:  30% (56/186)
2022-08-05T13:27:26.4776607Z Receiving objects:  31% (58/186)
2022-08-05T13:27:26.4778898Z Receiving objects:  32% (60/186)
2022-08-05T13:27:26.4780564Z Receiving objects:  33% (62/186)
2022-08-05T13:27:26.4781775Z Receiving objects:  34% (64/186)
2022-08-05T13:27:26.4784111Z Receiving objects:  35% (66/186)
2022-08-05T13:27:26.4786245Z Receiving objects:  36% (67/186)
2022-08-05T13:27:26.4794073Z Receiving objects:  37% (69/186)
2022-08-05T13:27:26.4795659Z Receiving objects:  38% (71/186)
2022-08-05T13:27:26.4795907Z Receiving objects:  39% (73/186)
2022-08-05T13:27:26.4796130Z Receiving objects:  40% (75/186)
2022-08-05T13:27:26.4796446Z Receiving objects:  41% (77/186)
2022-08-05T13:27:26.4796690Z Receiving objects:  42% (79/186)
2022-08-05T13:27:26.4796924Z Receiving objects:  43% (80/186)
2022-08-05T13:27:26.4797151Z Receiving objects:  44% (82/186)
2022-08-05T13:27:26.4797382Z Receiving objects:  45% (84/186)
2022-08-05T13:27:26.4798172Z Receiving objects:  46% (86/186)
2022-08-05T13:27:26.4800537Z Receiving objects:  47% (88/186)
2022-08-05T13:27:26.4801524Z Receiving objects:  48% (90/186)
2022-08-05T13:27:26.4802652Z Receiving objects:  49% (92/186)
2022-08-05T13:27:26.4803523Z Receiving objects:  50% (93/186)
2022-08-05T13:27:26.4803957Z Receiving objects:  51% (95/186)
2022-08-05T13:27:26.4806126Z Receiving objects:  52% (97/186)
2022-08-05T13:27:26.4806546Z Receiving objects:  53% (99/186)
2022-08-05T13:27:26.4808432Z Receiving objects:  54% (101/186)
2022-08-05T13:27:26.4809557Z Receiving objects:  55% (103/186)
2022-08-05T13:27:26.4810832Z Receiving objects:  56% (105/186)
2022-08-05T13:27:26.4811740Z Receiving objects:  57% (107/186)
2022-08-05T13:27:26.4812773Z Receiving objects:  58% (108/186)
2022-08-05T13:27:26.4813902Z Receiving objects:  59% (110/186)
2022-08-05T13:27:26.4815058Z Receiving objects:  60% (112/186)
2022-08-05T13:27:26.4816477Z Receiving objects:  61% (114/186)
2022-08-05T13:27:26.4818716Z Receiving objects:  62% (116/186)
2022-08-05T13:27:26.4819530Z Receiving objects:  63% (118/186)
2022-08-05T13:27:26.4820856Z Receiving objects:  64% (120/186)
2022-08-05T13:27:26.4822110Z Receiving objects:  65% (121/186)
2022-08-05T13:27:26.4822343Z Receiving objects:  66% (123/186)
2022-08-05T13:27:26.4824670Z Receiving objects:  67% (125/186)
2022-08-05T13:27:26.4825100Z Receiving objects:  68% (127/186)
2022-08-05T13:27:26.4825341Z Receiving objects:  69% (129/186)
2022-08-05T13:27:26.4827756Z Receiving objects:  70% (131/186)
2022-08-05T13:27:26.4828202Z Receiving objects:  71% (133/186)
2022-08-05T13:27:26.4831053Z Receiving objects:  72% (134/186)
2022-08-05T13:27:26.4832328Z Receiving objects:  73% (136/186)
2022-08-05T13:27:26.4833977Z Receiving objects:  74% (138/186)
2022-08-05T13:27:26.4834775Z Receiving objects:  75% (140/186)
2022-08-05T13:27:26.4835569Z Receiving objects:  76% (142/186)
2022-08-05T13:27:26.4838049Z Receiving objects:  77% (144/186)
2022-08-05T13:27:26.4838286Z Receiving objects:  78% (146/186)
2022-08-05T13:27:26.4839253Z Receiving objects:  79% (147/186)
2022-08-05T13:27:26.4840219Z Receiving objects:  80% (149/186)
2022-08-05T13:27:26.4841513Z Receiving objects:  81% (151/186)
2022-08-05T13:27:26.4842436Z Receiving objects:  82% (153/186)
2022-08-05T13:27:26.4843624Z Receiving objects:  83% (155/186)
2022-08-05T13:27:26.4844858Z Receiving objects:  84% (157/186)
2022-08-05T13:27:26.4845652Z Receiving objects:  85% (159/186)
2022-08-05T13:27:26.4846532Z Receiving objects:  86% (160/186)
2022-08-05T13:27:26.5479773Z Receiving objects:  87% (162/186)
2022-08-05T13:27:26.5480467Z remote: Total 186 (delta 13), reused 91 (delta 7), pack-reused 0        
2022-08-05T13:27:26.5480764Z Receiving objects:  88% (164/186)
2022-08-05T13:27:26.5481050Z Receiving objects:  89% (166/186)
2022-08-05T13:27:26.5481290Z Receiving objects:  90% (168/186)
2022-08-05T13:27:26.5481538Z Receiving objects:  91% (170/186)
2022-08-05T13:27:26.5481775Z Receiving objects:  92% (172/186)
2022-08-05T13:27:26.5482044Z Receiving objects:  93% (173/186)
2022-08-05T13:27:26.5482263Z Receiving objects:  94% (175/186)
2022-08-05T13:27:26.5482493Z Receiving objects:  95% (177/186)
2022-08-05T13:27:26.5482723Z Receiving objects:  96% (179/186)
2022-08-05T13:27:26.5482940Z Receiving objects:  97% (181/186)
2022-08-05T13:27:26.5483185Z Receiving objects:  98% (183/186)
2022-08-05T13:27:26.5483415Z Receiving objects:  99% (185/186)
2022-08-05T13:27:26.5483631Z Receiving objects: 100% (186/186)
2022-08-05T13:27:26.5483899Z Receiving objects: 100% (186/186), 164.18 KiB | 753.00 KiB/s, done.
2022-08-05T13:27:26.5484165Z Resolving deltas:   0% (0/13)
2022-08-05T13:27:26.5484617Z Resolving deltas:   7% (1/13)
2022-08-05T13:27:26.5484926Z Resolving deltas:  15% (2/13)
2022-08-05T13:27:26.5485179Z Resolving deltas:  23% (3/13)
2022-08-05T13:27:26.5485503Z Resolving deltas:  30% (4/13)
2022-08-05T13:27:26.5485827Z Resolving deltas:  38% (5/13)
2022-08-05T13:27:26.5486115Z Resolving deltas:  46% (6/13)
2022-08-05T13:27:26.5486424Z Resolving deltas:  53% (7/13)
2022-08-05T13:27:26.5486726Z Resolving deltas:  61% (8/13)
2022-08-05T13:27:26.5486979Z Resolving deltas:  69% (9/13)
2022-08-05T13:27:26.5487291Z Resolving deltas:  76% (10/13)
2022-08-05T13:27:26.5487638Z Resolving deltas:  84% (11/13)
2022-08-05T13:27:26.5487892Z Resolving deltas:  92% (12/13)
2022-08-05T13:27:26.5488203Z Resolving deltas: 100% (13/13)
2022-08-05T13:27:26.5488519Z Resolving deltas: 100% (13/13), done.
2022-08-05T13:27:26.5554727Z From https://github.com/make-software/dao-contracts
2022-08-05T13:27:26.5555622Z  * [new ref]         9856e76ddea88902a5c3897fe622852d01d36295 -> pull/81/merge
2022-08-05T13:27:26.5581630Z ##[endgroup]
2022-08-05T13:27:26.5582483Z ##[group]Determining the checkout info
2022-08-05T13:27:26.5583699Z ##[endgroup]
2022-08-05T13:27:26.5584660Z ##[group]Checking out the ref
2022-08-05T13:27:26.5588889Z [command]/usr/bin/git checkout --progress --force refs/remotes/pull/81/merge
2022-08-05T13:27:26.5705643Z Note: switching to 'refs/remotes/pull/81/merge'.
2022-08-05T13:27:26.5705950Z 
2022-08-05T13:27:26.5706276Z You are in 'detached HEAD' state. You can look around, make experimental
2022-08-05T13:27:26.5706733Z changes and commit them, and you can discard any commits you make in this
2022-08-05T13:27:26.5707171Z state without impacting any branches by switching back to a branch.
2022-08-05T13:27:26.5707612Z 
2022-08-05T13:27:26.5707765Z If you want to create a new branch to retain commits you create, you may
2022-08-05T13:27:26.5708278Z do so (now or later) by using -c with the switch command. Example:
2022-08-05T13:27:26.5708505Z 
2022-08-05T13:27:26.5708711Z   git switch -c <new-branch-name>
2022-08-05T13:27:26.5708903Z 
2022-08-05T13:27:26.5709041Z Or undo this operation with:
2022-08-05T13:27:26.5709300Z 
2022-08-05T13:27:26.5709375Z   git switch -
2022-08-05T13:27:26.5709562Z 
2022-08-05T13:27:26.5709776Z Turn off this advice by setting config variable advice.detachedHead to false
2022-08-05T13:27:26.5710023Z 
2022-08-05T13:27:26.5710282Z HEAD is now at 9856e76 Merge d8ccb703efbe46694c18cbb2614a781126d67d83 into aeab969856b797e19fa3bf951bd363d6b3bdce1e
2022-08-05T13:27:26.5719349Z ##[endgroup]
2022-08-05T13:27:26.5774038Z [command]/usr/bin/git log -1 --format='%H'
2022-08-05T13:27:26.5805726Z '9856e76ddea88902a5c3897fe622852d01d36295'
2022-08-05T13:27:26.5966501Z ##[group]Run actions/setup-node@v2
2022-08-05T13:27:26.5967576Z with:
2022-08-05T13:27:26.5967862Z   node-version: 14
2022-08-05T13:27:26.5968203Z   always-auth: false
2022-08-05T13:27:26.5968446Z   check-latest: false
2022-08-05T13:27:26.5968874Z   token: ***
2022-08-05T13:27:26.5969140Z env:
2022-08-05T13:27:26.5969422Z   NODE_ENV: ci
2022-08-05T13:27:26.5969744Z   WASM_RELEASE_PATH: /home/runner/work/dao-contracts/dao-contracts/client/wasm
2022-08-05T13:27:26.5970141Z   NCTL_USERS_FOLDER_PATH: /tmp/net-1/users
2022-08-05T13:27:26.5970458Z   CHAIN_NAME: casper-net-1
2022-08-05T13:27:26.5970759Z   NODE_ADDRESS: http://localhost:11101/rpc
2022-08-05T13:27:26.5971171Z   EVENT_STREAM_ADDRESS: http://localhost:18101/events/main
2022-08-05T13:27:26.5971526Z   INSTALL_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:26.5971794Z   DEPLOY_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:26.5972104Z ##[endgroup]
2022-08-05T13:27:26.7641682Z Found in cache @ /opt/hostedtoolcache/node/14.20.0/x64
2022-08-05T13:27:26.7734638Z ##[group]Run cd client && npm install
2022-08-05T13:27:26.7735015Z [36;1mcd client && npm install[0m
2022-08-05T13:27:26.7792455Z shell: /usr/bin/bash -e {0}
2022-08-05T13:27:26.7792762Z env:
2022-08-05T13:27:26.7793022Z   NODE_ENV: ci
2022-08-05T13:27:26.7793370Z   WASM_RELEASE_PATH: /home/runner/work/dao-contracts/dao-contracts/client/wasm
2022-08-05T13:27:26.7793865Z   NCTL_USERS_FOLDER_PATH: /tmp/net-1/users
2022-08-05T13:27:26.7794191Z   CHAIN_NAME: casper-net-1
2022-08-05T13:27:26.7794538Z   NODE_ADDRESS: http://localhost:11101/rpc
2022-08-05T13:27:26.7794877Z   EVENT_STREAM_ADDRESS: http://localhost:18101/events/main
2022-08-05T13:27:26.7795260Z   INSTALL_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:26.7795582Z   DEPLOY_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:26.7795830Z ##[endgroup]
2022-08-05T13:27:35.6937733Z 
2022-08-05T13:27:35.6950448Z > secp256k1@4.0.3 install /home/runner/work/dao-contracts/dao-contracts/client/node_modules/ethereum-cryptography/node_modules/secp256k1
2022-08-05T13:27:35.6951244Z > node-gyp-build || exit 0
2022-08-05T13:27:35.6951385Z 
2022-08-05T13:27:35.8093849Z 
2022-08-05T13:27:35.8095546Z > secp256k1@3.7.1 install /home/runner/work/dao-contracts/dao-contracts/client/node_modules/secp256k1
2022-08-05T13:27:35.8096187Z > npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."
2022-08-05T13:27:35.8096435Z 
2022-08-05T13:27:36.0254446Z 
2022-08-05T13:27:36.0255944Z > secp256k1@3.7.1 rebuild /home/runner/work/dao-contracts/dao-contracts/client/node_modules/secp256k1
2022-08-05T13:27:36.0256642Z > node-gyp rebuild
2022-08-05T13:27:36.0256787Z 
2022-08-05T13:27:38.1573356Z make: Entering directory '/home/runner/work/dao-contracts/dao-contracts/client/node_modules/secp256k1/build'
2022-08-05T13:27:38.1665237Z   CXX(target) Release/obj.target/secp256k1/src/addon.o
2022-08-05T13:27:40.6622346Z In file included from ../src/addon.cc:2:
2022-08-05T13:27:40.6624552Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:40.6627502Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:40.6628386Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:40.6629221Z       |                                                              ^
2022-08-05T13:27:40.6782077Z In file included from ../src/addon.cc:1:
2022-08-05T13:27:40.6782706Z ../src/addon.cc: At global scope:
2022-08-05T13:27:40.6784883Z /home/runner/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2022-08-05T13:27:40.6785796Z   793 |       (node::addon_register_func) (regfunc),                          \
2022-08-05T13:27:40.6786511Z       |                                           ^
2022-08-05T13:27:40.6787302Z /home/runner/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
2022-08-05T13:27:40.6788321Z   827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2022-08-05T13:27:40.6788780Z       |   ^~~~~~~~~~~~~
2022-08-05T13:27:40.6789616Z ../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
2022-08-05T13:27:40.6790106Z    50 | NODE_MODULE(secp256k1, Init)
2022-08-05T13:27:40.6790669Z       | ^~~~~~~~~~~
2022-08-05T13:27:41.4439654Z   CXX(target) Release/obj.target/secp256k1/src/privatekey.o
2022-08-05T13:27:41.9190412Z In file included from ../src/privatekey.cc:2:
2022-08-05T13:27:41.9191778Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:41.9193361Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:41.9194081Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:41.9194527Z       |                                                              ^
2022-08-05T13:27:42.0153135Z ../src/privatekey.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE privateKeyNegate(Nan::NAN_METHOD_ARGS_TYPE)’:
2022-08-05T13:27:42.0154773Z ../src/privatekey.cc:73:30: warning: ignoring return value of ‘int secp256k1_ec_privkey_negate(const secp256k1_context*, unsigned char*)’, declared with attribute warn_unused_result [-Wunused-result]
2022-08-05T13:27:42.0155532Z    73 |   secp256k1_ec_privkey_negate(secp256k1ctx, &private_key[0]);
2022-08-05T13:27:42.0156054Z       |   ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2022-08-05T13:27:42.2511262Z   CXX(target) Release/obj.target/secp256k1/src/publickey.o
2022-08-05T13:27:42.7247823Z In file included from ../src/publickey.cc:3:
2022-08-05T13:27:42.7249354Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:42.7257371Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:42.7258079Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:42.7258522Z       |                                                              ^
2022-08-05T13:27:43.0430926Z   CXX(target) Release/obj.target/secp256k1/src/signature.o
2022-08-05T13:27:43.5142741Z In file included from ../src/signature.cc:2:
2022-08-05T13:27:43.5144321Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:43.5145876Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:43.5147352Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:43.5150099Z       |                                                              ^
2022-08-05T13:27:43.7006064Z   CXX(target) Release/obj.target/secp256k1/src/ecdsa.o
2022-08-05T13:27:44.1739571Z In file included from ../src/ecdsa.cc:2:
2022-08-05T13:27:44.1741306Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:44.1742910Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:44.1745908Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:44.1746533Z       |                                                              ^
2022-08-05T13:27:44.1913539Z ../src/ecdsa.cc: In function ‘Nan::NAN_METHOD_RETURN_TYPE sign(Nan::NAN_METHOD_ARGS_TYPE)’:
2022-08-05T13:27:44.1915337Z ../src/ecdsa.cc:88:131: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
2022-08-05T13:27:44.1916526Z    88 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("signature").ToLocalChecked(), COPY_BUFFER(&output[0], 64));
2022-08-05T13:27:44.1917635Z       |                                                                                                                                   ^
2022-08-05T13:27:44.1918324Z In file included from /home/runner/.cache/node-gyp/14.20.0/include/node/node.h:67,
2022-08-05T13:27:44.1969575Z                  from ../src/ecdsa.cc:1:
2022-08-05T13:27:44.1970234Z /home/runner/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
2022-08-05T13:27:44.1970975Z  3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
2022-08-05T13:27:44.1971312Z       |                                     ^~~
2022-08-05T13:27:44.1972828Z ../src/ecdsa.cc:89:130: warning: ignoring return value of ‘v8::Maybe<bool> v8::Object::Set(v8::Local<v8::Context>, v8::Local<v8::Value>, v8::Local<v8::Value>)’, declared with attribute warn_unused_result [-Wunused-result]
2022-08-05T13:27:44.1973721Z    89 |   obj->Set(info.GetIsolate()->GetCurrentContext(), Nan::New<v8::String>("recovery").ToLocalChecked(), Nan::New<v8::Number>(recid));
2022-08-05T13:27:44.1974218Z       |                                                                                                                                  ^
2022-08-05T13:27:44.1974758Z In file included from /home/runner/.cache/node-gyp/14.20.0/include/node/node.h:67,
2022-08-05T13:27:44.1975099Z                  from ../src/ecdsa.cc:1:
2022-08-05T13:27:44.1975613Z /home/runner/.cache/node-gyp/14.20.0/include/node/v8.h:3670:37: note: declared here
2022-08-05T13:27:44.1976027Z  3670 |   V8_WARN_UNUSED_RESULT Maybe<bool> Set(Local<Context> context,
2022-08-05T13:27:44.1976347Z       |                                     ^~~
2022-08-05T13:27:44.4434431Z   CXX(target) Release/obj.target/secp256k1/src/ecdh.o
2022-08-05T13:27:44.9181769Z In file included from ../src/ecdh.cc:2:
2022-08-05T13:27:44.9183243Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:44.9184646Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:44.9185433Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:44.9186630Z       |                                                              ^
2022-08-05T13:27:45.0991926Z   CC(target) Release/obj.target/secp256k1/src/secp256k1-src/src/secp256k1.o
2022-08-05T13:27:46.7199923Z   CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_parsing.o
2022-08-05T13:27:46.8025474Z   CC(target) Release/obj.target/secp256k1/src/secp256k1-src/contrib/lax_der_privatekey_parsing.o
2022-08-05T13:27:46.8658950Z   SOLINK_MODULE(target) Release/obj.target/secp256k1.node
2022-08-05T13:27:46.9467924Z   COPY Release/secp256k1.node
2022-08-05T13:27:46.9547121Z make: Leaving directory '/home/runner/work/dao-contracts/dao-contracts/client/node_modules/secp256k1/build'
2022-08-05T13:27:46.9709472Z 
2022-08-05T13:27:46.9710817Z > eccrypto@1.1.6 install /home/runner/work/dao-contracts/dao-contracts/client/node_modules/eccrypto
2022-08-05T13:27:46.9711649Z > node-gyp rebuild || exit 0
2022-08-05T13:27:46.9712022Z 
2022-08-05T13:27:47.3775712Z make: Entering directory '/home/runner/work/dao-contracts/dao-contracts/client/node_modules/eccrypto/build'
2022-08-05T13:27:47.3789851Z   CXX(target) Release/obj.target/ecdh/ecdh.o
2022-08-05T13:27:47.8620886Z In file included from ../ecdh.cc:2:
2022-08-05T13:27:47.8622475Z ../../nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2022-08-05T13:27:47.8624010Z ../../nan/nan.h:2298:62: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2022-08-05T13:27:47.8624995Z  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2022-08-05T13:27:47.8625901Z       |                                                              ^
2022-08-05T13:27:47.9018433Z In file included from ../ecdh.cc:1:
2022-08-05T13:27:47.9019348Z ../ecdh.cc: At global scope:
2022-08-05T13:27:47.9021686Z /home/runner/.cache/node-gyp/14.20.0/include/node/node.h:793:43: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2022-08-05T13:27:47.9035197Z   793 |       (node::addon_register_func) (regfunc),                          \
2022-08-05T13:27:47.9035892Z       |                                           ^
2022-08-05T13:27:47.9036966Z /home/runner/.cache/node-gyp/14.20.0/include/node/node.h:827:3: note: in expansion of macro ‘NODE_MODULE_X’
2022-08-05T13:27:47.9037751Z   827 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2022-08-05T13:27:47.9038658Z       |   ^~~~~~~~~~~~~
2022-08-05T13:27:47.9039447Z ../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
2022-08-05T13:27:47.9039781Z   131 | NODE_MODULE(ecdh, InitAll)
2022-08-05T13:27:47.9039998Z       | ^~~~~~~~~~~
2022-08-05T13:27:48.0748437Z   SOLINK_MODULE(target) Release/obj.target/ecdh.node
2022-08-05T13:27:48.1106670Z   COPY Release/ecdh.node
2022-08-05T13:27:48.1168790Z make: Leaving directory '/home/runner/work/dao-contracts/dao-contracts/client/node_modules/eccrypto/build'
2022-08-05T13:27:48.1260955Z 
2022-08-05T13:27:48.1262251Z > keccak@3.0.2 install /home/runner/work/dao-contracts/dao-contracts/client/node_modules/keccak
2022-08-05T13:27:48.1265598Z > node-gyp-build || exit 0
2022-08-05T13:27:48.1266068Z 
2022-08-05T13:27:48.3460423Z npm notice created a lockfile as package-lock.json. You should commit this file.
2022-08-05T13:27:48.3554401Z npm WARN eslint-plugin-prettier@3.4.1 requires a peer of eslint@>=5.0.0 but none is installed. You must install peer dependencies yourself.
2022-08-05T13:27:48.3635796Z npm WARN eslint-plugin-prettier@3.4.1 requires a peer of prettier@>=1.13.0 but none is installed. You must install peer dependencies yourself.
2022-08-05T13:27:48.3726001Z npm WARN acorn-import-assertions@1.8.0 requires a peer of acorn@^8 but none is installed. You must install peer dependencies yourself.
2022-08-05T13:27:48.3788755Z npm WARN dao-contracts-js-client@0.1.0 No repository field.
2022-08-05T13:27:48.3791747Z 
2022-08-05T13:27:48.3820494Z added 190 packages from 280 contributors and audited 192 packages in 19.5s
2022-08-05T13:27:48.4468512Z 
2022-08-05T13:27:48.4469255Z 14 packages are looking for funding
2022-08-05T13:27:48.4470029Z   run `npm fund` for details
2022-08-05T13:27:48.4470398Z 
2022-08-05T13:27:48.4475602Z found 0 vulnerabilities
2022-08-05T13:27:48.4475918Z 
2022-08-05T13:27:48.4674384Z ##[group]Run cd client && NODE_ENV=ci npm run e2e:generic-client
2022-08-05T13:27:48.4674768Z [36;1mcd client && NODE_ENV=ci npm run e2e:generic-client[0m
2022-08-05T13:27:48.4729367Z shell: /usr/bin/bash -e {0}
2022-08-05T13:27:48.4729601Z env:
2022-08-05T13:27:48.4729787Z   NODE_ENV: ci
2022-08-05T13:27:48.4730088Z   WASM_RELEASE_PATH: /home/runner/work/dao-contracts/dao-contracts/client/wasm
2022-08-05T13:27:48.4730417Z   NCTL_USERS_FOLDER_PATH: /tmp/net-1/users
2022-08-05T13:27:48.4730665Z   CHAIN_NAME: casper-net-1
2022-08-05T13:27:48.4730929Z   NODE_ADDRESS: http://localhost:11101/rpc
2022-08-05T13:27:48.4731235Z   EVENT_STREAM_ADDRESS: http://localhost:18101/events/main
2022-08-05T13:27:48.4731516Z   INSTALL_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:48.4731750Z   DEPLOY_PAYMENT_AMOUNT: 200000000000
2022-08-05T13:27:48.4731985Z ##[endgroup]
2022-08-05T13:27:48.6770595Z 
2022-08-05T13:27:48.6771851Z > dao-contracts-js-client@0.1.0 e2e:generic-client /home/runner/work/dao-contracts/dao-contracts/client
2022-08-05T13:27:48.6773068Z > ts-node ./e2e/e2e-generic-client.ts
2022-08-05T13:27:48.6773227Z 
2022-08-05T13:27:51.4987416Z testing env variables {
2022-08-05T13:27:51.4988034Z   NODE_ENV: 'ci',
2022-08-05T13:27:51.4988384Z   CHAIN_NAME: 'casper-net-1',
2022-08-05T13:27:51.4988794Z   NODE_ADDRESS: 'http://localhost:11101/rpc',
2022-08-05T13:27:51.4989225Z   EVENT_STREAM_ADDRESS: 'http://localhost:18101/events/main',
2022-08-05T13:27:51.4989750Z   WASM_RELEASE_PATH: '/home/runner/work/dao-contracts/dao-contracts/client/wasm',
2022-08-05T13:27:51.4990185Z   NCTL_USERS_FOLDER_PATH: '/tmp/net-1/users',
2022-08-05T13:27:51.4990610Z   INSTALL_PAYMENT_AMOUNT: '200000000000',
2022-08-05T13:27:51.4990944Z   DEPLOY_PAYMENT_AMOUNT: '200000000000'
2022-08-05T13:27:51.4991175Z }
2022-08-05T13:27:51.5012141Z 
2022-08-05T13:27:51.5012154Z 
2022-08-05T13:27:51.5014056Z ... Testing install ...
2022-08-05T13:27:51.5014461Z 
2022-08-05T13:27:51.5014658Z 
2022-08-05T13:27:51.6439673Z ... Contract deploy is pending, waiting for next block finalisation (deployHash: b3c86e9449de318daad998b9a3264ce60ae0e41665ec618e5cc5cf3179878bd7) ...
2022-08-05T13:28:00.7743953Z ... Contract installed successfully.
2022-08-05T13:28:00.7745316Z  - Contract Package Hash: hash-258cd5808f8eae77a9bdc1866f22460264c9b345e349689fee6cc11e81056e51
2022-08-05T13:28:00.7800143Z  - Contract Hash: hash-55ab3ec9cc4e24a7e03f6fd1e9fe66c321d186d3f18de027cbdeeab29626b80b
2022-08-05T13:28:00.7966589Z 
2022-08-05T13:28:00.7967067Z 
2022-08-05T13:28:00.7968113Z ... Testing deploys ...
2022-08-05T13:28:00.7968354Z 
2022-08-05T13:28:00.7968366Z 
2022-08-05T13:28:00.7968962Z  - Trying to create and send a mint deploy
2022-08-05T13:28:00.8243104Z ... Contract deploy is pending, waiting for next block finalisation (deployHash: 483c83154f9b7403e7566f34702b45a20bdce4fba98166a619c60545dd647d9c) ...
2022-08-05T13:28:09.8563616Z  - Requested Mint Amount:  200000000000
2022-08-05T13:28:09.8564035Z  - Total Supply After Mint:  200000000000
2022-08-05T13:28:09.8564408Z  - Total supply equals mint: SUCCESS!
2022-08-05T13:28:09.8564918Z 
2022-08-05T13:28:09.8564926Z 
2022-08-05T13:28:09.8565190Z  - Trying to create and send a add to whitelist deploy
2022-08-05T13:28:09.8609311Z  - Whitelist Value Before Deploy: undefined
2022-08-05T13:28:09.8889515Z ... Contract deploy is pending, waiting for next block finalisation (deployHash: b15660068ddcf3ace449efb79053e711470d509900e1ad83726bfd3a92ce23e9) ...
2022-08-05T13:28:18.9334807Z  - Whitelist Value After Deploy: true
2022-08-05T13:28:18.9336748Z  - Recipient is added to the whitelist: SUCCESS!
2022-08-05T13:28:18.9554208Z Post job cleanup.
2022-08-05T13:28:19.0959874Z Post job cleanup.
2022-08-05T13:28:19.2225103Z [command]/usr/bin/git version
2022-08-05T13:28:19.2278232Z git version 2.37.1
2022-08-05T13:28:19.2326661Z Temporarily overriding HOME='/home/runner/work/_temp/82d33b6b-8bd4-410c-9365-7e14c479515f' before making global git config changes
2022-08-05T13:28:19.2329124Z Adding repository directory to the temporary git global config as a safe directory
2022-08-05T13:28:19.2336495Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/dao-contracts/dao-contracts
2022-08-05T13:28:19.2384594Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2022-08-05T13:28:19.2426304Z [command]/usr/bin/git submodule foreach --recursive git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :
2022-08-05T13:28:19.2703569Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2022-08-05T13:28:19.2738240Z http.https://github.com/.extraheader
2022-08-05T13:28:19.2750135Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2022-08-05T13:28:19.2794062Z [command]/usr/bin/git submodule foreach --recursive git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :
2022-08-05T13:28:19.3210808Z Print service container logs: e3bbe42de4f541f0a2fc53325e822296_makesoftwarecaspernctlv144220303_c1c81f
2022-08-05T13:28:19.3216890Z ##[command]/usr/bin/docker logs --details 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:28:19.3551193Z  2022-08-05T13:26:25.526970 [INFO] [1] NCTL :: asset tear-down begins ... please wait
2022-08-05T13:28:19.3551918Z  2022-08-05T13:26:27.548598 [INFO] [1] NCTL :: asset tear-down complete
2022-08-05T13:28:19.3552785Z  2022-08-05T13:26:27.564681 [INFO] [1] NCTL :: asset setup begins ... please wait
2022-08-05T13:28:19.3553143Z  2022-08-05T13:26:27.565837 [INFO] [1] NCTL :: ... setting directories
2022-08-05T13:28:19.3553461Z  2022-08-05T13:26:27.673902 [INFO] [1] NCTL :: ... setting binaries
2022-08-05T13:28:19.3553792Z  2022-08-05T13:26:28.040562 [INFO] [1] NCTL :: ... setting cryptographic keys
2022-08-05T13:28:19.3554108Z  2022-08-05T13:26:28.190456 [INFO] [1] NCTL :: ... setting daemon config
2022-08-05T13:28:19.3554494Z  2022-08-05T13:26:28.308092 [INFO] [1] NCTL :: ... setting chainspec.toml
2022-08-05T13:28:19.3554812Z  2022-08-05T13:26:28.344919 [INFO] [1] NCTL :: ... setting accounts.toml
2022-08-05T13:28:19.3555116Z  2022-08-05T13:26:28.411751 [INFO] [1] NCTL :: ... setting node configs
2022-08-05T13:28:19.3555516Z  2022-08-05T13:26:28.872387 [INFO] [1] NCTL :: asset setup complete
2022-08-05T13:28:19.3555756Z  ./
2022-08-05T13:28:19.3555930Z  ./chainspec/
2022-08-05T13:28:19.3556154Z  ./chainspec/accounts.toml
2022-08-05T13:28:19.3556373Z  ./faucet/
2022-08-05T13:28:19.3556564Z  ./faucet/public_key.pem
2022-08-05T13:28:19.3556798Z  ./faucet/public_key_hex
2022-08-05T13:28:19.3557022Z  ./faucet/secret_key.pem
2022-08-05T13:28:19.3557227Z  ./nodes/
2022-08-05T13:28:19.3557405Z  ./nodes/node-1/
2022-08-05T13:28:19.3557624Z  ./nodes/node-1/config/
2022-08-05T13:28:19.3557854Z  ./nodes/node-1/config/1_0_0/
2022-08-05T13:28:19.3558110Z  ./nodes/node-1/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3558339Z  ./nodes/node-1/keys/
2022-08-05T13:28:19.3558575Z  ./nodes/node-1/keys/public_key.pem
2022-08-05T13:28:19.3558827Z  ./nodes/node-1/keys/public_key_hex
2022-08-05T13:28:19.3559080Z  ./nodes/node-1/keys/secret_key.pem
2022-08-05T13:28:19.3559295Z  ./nodes/node-10/
2022-08-05T13:28:19.3559511Z  ./nodes/node-10/config/
2022-08-05T13:28:19.3559749Z  ./nodes/node-10/config/1_0_0/
2022-08-05T13:28:19.3560063Z  ./nodes/node-10/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3560307Z  ./nodes/node-10/keys/
2022-08-05T13:28:19.3560531Z  ./nodes/node-10/keys/public_key.pem
2022-08-05T13:28:19.3560785Z  ./nodes/node-10/keys/public_key_hex
2022-08-05T13:28:19.3561034Z  ./nodes/node-10/keys/secret_key.pem
2022-08-05T13:28:19.3561248Z  ./nodes/node-2/
2022-08-05T13:28:19.3561455Z  ./nodes/node-2/config/
2022-08-05T13:28:19.3561975Z  ./nodes/node-2/config/1_0_0/
2022-08-05T13:28:19.3562231Z  ./nodes/node-2/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3562456Z  ./nodes/node-2/keys/
2022-08-05T13:28:19.3562696Z  ./nodes/node-2/keys/public_key.pem
2022-08-05T13:28:19.3562949Z  ./nodes/node-2/keys/public_key_hex
2022-08-05T13:28:19.3563199Z  ./nodes/node-2/keys/secret_key.pem
2022-08-05T13:28:19.3563410Z  ./nodes/node-3/
2022-08-05T13:28:19.3563620Z  ./nodes/node-3/config/
2022-08-05T13:28:19.3563846Z  ./nodes/node-3/config/1_0_0/
2022-08-05T13:28:19.3564100Z  ./nodes/node-3/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3564335Z  ./nodes/node-3/keys/
2022-08-05T13:28:19.3564567Z  ./nodes/node-3/keys/public_key.pem
2022-08-05T13:28:19.3564819Z  ./nodes/node-3/keys/public_key_hex
2022-08-05T13:28:19.3565062Z  ./nodes/node-3/keys/secret_key.pem
2022-08-05T13:28:19.3565272Z  ./nodes/node-4/
2022-08-05T13:28:19.3565484Z  ./nodes/node-4/config/
2022-08-05T13:28:19.3565707Z  ./nodes/node-4/config/1_0_0/
2022-08-05T13:28:19.3565965Z  ./nodes/node-4/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3566203Z  ./nodes/node-4/keys/
2022-08-05T13:28:19.3566442Z  ./nodes/node-4/keys/public_key.pem
2022-08-05T13:28:19.3566860Z  ./nodes/node-4/keys/public_key_hex
2022-08-05T13:28:19.3567131Z  ./nodes/node-4/keys/secret_key.pem
2022-08-05T13:28:19.3567339Z  ./nodes/node-5/
2022-08-05T13:28:19.3567553Z  ./nodes/node-5/config/
2022-08-05T13:28:19.3567776Z  ./nodes/node-5/config/1_0_0/
2022-08-05T13:28:19.3568017Z  ./nodes/node-5/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3568260Z  ./nodes/node-5/keys/
2022-08-05T13:28:19.3568497Z  ./nodes/node-5/keys/public_key.pem
2022-08-05T13:28:19.3568752Z  ./nodes/node-5/keys/public_key_hex
2022-08-05T13:28:19.3568986Z  ./nodes/node-5/keys/secret_key.pem
2022-08-05T13:28:19.3569217Z  ./nodes/node-6/
2022-08-05T13:28:19.3569429Z  ./nodes/node-6/config/
2022-08-05T13:28:19.3569650Z  ./nodes/node-6/config/1_0_0/
2022-08-05T13:28:19.3569885Z  ./nodes/node-6/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3570129Z  ./nodes/node-6/keys/
2022-08-05T13:28:19.3570364Z  ./nodes/node-6/keys/public_key.pem
2022-08-05T13:28:19.3570608Z  ./nodes/node-6/keys/public_key_hex
2022-08-05T13:28:19.3570840Z  ./nodes/node-6/keys/secret_key.pem
2022-08-05T13:28:19.3571079Z  ./nodes/node-7/
2022-08-05T13:28:19.3571299Z  ./nodes/node-7/config/
2022-08-05T13:28:19.3571524Z  ./nodes/node-7/config/1_0_0/
2022-08-05T13:28:19.3571764Z  ./nodes/node-7/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3572007Z  ./nodes/node-7/keys/
2022-08-05T13:28:19.3572239Z  ./nodes/node-7/keys/public_key.pem
2022-08-05T13:28:19.3572706Z  ./nodes/node-7/keys/public_key_hex
2022-08-05T13:28:19.3572942Z  ./nodes/node-7/keys/secret_key.pem
2022-08-05T13:28:19.3573166Z  ./nodes/node-8/
2022-08-05T13:28:19.3573372Z  ./nodes/node-8/config/
2022-08-05T13:28:19.3573584Z  ./nodes/node-8/config/1_0_0/
2022-08-05T13:28:19.3573832Z  ./nodes/node-8/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3574075Z  ./nodes/node-8/keys/
2022-08-05T13:28:19.3574306Z  ./nodes/node-8/keys/public_key.pem
2022-08-05T13:28:19.3574548Z  ./nodes/node-8/keys/public_key_hex
2022-08-05T13:28:19.3574797Z  ./nodes/node-8/keys/secret_key.pem
2022-08-05T13:28:19.3575087Z  ./nodes/node-9/
2022-08-05T13:28:19.3575309Z  ./nodes/node-9/config/
2022-08-05T13:28:19.3575537Z  ./nodes/node-9/config/1_0_0/
2022-08-05T13:28:19.3575774Z  ./nodes/node-9/config/1_0_0/accounts.toml
2022-08-05T13:28:19.3576022Z  ./nodes/node-9/keys/
2022-08-05T13:28:19.3576257Z  ./nodes/node-9/keys/public_key.pem
2022-08-05T13:28:19.3576524Z  ./nodes/node-9/keys/public_key_hex
2022-08-05T13:28:19.3576764Z  ./nodes/node-9/keys/secret_key.pem
2022-08-05T13:28:19.3576983Z  ./users/
2022-08-05T13:28:19.3577178Z  ./users/user-1/
2022-08-05T13:28:19.3577398Z  ./users/user-1/public_key.pem
2022-08-05T13:28:19.3577622Z  ./users/user-1/public_key_hex
2022-08-05T13:28:19.3577861Z  ./users/user-1/secret_key.pem
2022-08-05T13:28:19.3578084Z  ./users/user-10/
2022-08-05T13:28:19.3578289Z  ./users/user-10/public_key.pem
2022-08-05T13:28:19.3578648Z  ./users/user-10/public_key_hex
2022-08-05T13:28:19.3578884Z  ./users/user-10/secret_key.pem
2022-08-05T13:28:19.3579108Z  ./users/user-2/
2022-08-05T13:28:19.3579310Z  ./users/user-2/public_key.pem
2022-08-05T13:28:19.3579550Z  ./users/user-2/public_key_hex
2022-08-05T13:28:19.3579789Z  ./users/user-2/secret_key.pem
2022-08-05T13:28:19.3580008Z  ./users/user-3/
2022-08-05T13:28:19.3580216Z  ./users/user-3/public_key.pem
2022-08-05T13:28:19.3580450Z  ./users/user-3/public_key_hex
2022-08-05T13:28:19.3580685Z  ./users/user-3/secret_key.pem
2022-08-05T13:28:19.3580906Z  ./users/user-4/
2022-08-05T13:28:19.3581111Z  ./users/user-4/public_key.pem
2022-08-05T13:28:19.3581345Z  ./users/user-4/public_key_hex
2022-08-05T13:28:19.3581578Z  ./users/user-4/secret_key.pem
2022-08-05T13:28:19.3581795Z  ./users/user-5/
2022-08-05T13:28:19.3582002Z  ./users/user-5/public_key.pem
2022-08-05T13:28:19.3582237Z  ./users/user-5/public_key_hex
2022-08-05T13:28:19.3582467Z  ./users/user-5/secret_key.pem
2022-08-05T13:28:19.3582691Z  ./users/user-6/
2022-08-05T13:28:19.3582892Z  ./users/user-6/public_key.pem
2022-08-05T13:28:19.3583127Z  ./users/user-6/public_key_hex
2022-08-05T13:28:19.3583360Z  ./users/user-6/secret_key.pem
2022-08-05T13:28:19.3583697Z  ./users/user-7/
2022-08-05T13:28:19.3583925Z  ./users/user-7/public_key.pem
2022-08-05T13:28:19.3584163Z  ./users/user-7/public_key_hex
2022-08-05T13:28:19.3584395Z  ./users/user-7/secret_key.pem
2022-08-05T13:28:19.3584597Z  ./users/user-8/
2022-08-05T13:28:19.3584811Z  ./users/user-8/public_key.pem
2022-08-05T13:28:19.3585045Z  ./users/user-8/public_key_hex
2022-08-05T13:28:19.3585279Z  ./users/user-8/secret_key.pem
2022-08-05T13:28:19.3585488Z  ./users/user-9/
2022-08-05T13:28:19.3585704Z  ./users/user-9/public_key.pem
2022-08-05T13:28:19.3585943Z  ./users/user-9/public_key_hex
2022-08-05T13:28:19.3586179Z  ./users/user-9/secret_key.pem
2022-08-05T13:28:19.3586461Z  2022-08-05T13:26:28.886790 [INFO] [1] NCTL :: starting node(s) begins ... please wait
2022-08-05T13:28:19.3586796Z  2022-08-05T13:26:28.891376 [INFO] [1] NCTL :: ... starting supervisord
2022-08-05T13:28:19.3587133Z  2022-08-05T13:26:31.038539 [INFO] [1] NCTL :: ... starting nodes: genesis bootstraps
2022-08-05T13:28:19.3587484Z  2022-08-05T13:26:32.211181 [INFO] [1] NCTL :: ... starting nodes: genesis non-bootstraps
2022-08-05T13:28:19.3587801Z  2022-08-05T13:26:33.370708 [INFO] [1] NCTL :: starting node(s) complete
2022-08-05T13:28:19.3588148Z  validators-1:casper-net-1-node-1    RUNNING   pid 728, uptime 0:00:03
2022-08-05T13:28:19.3588522Z  validators-1:casper-net-1-node-2    RUNNING   pid 729, uptime 0:00:03
2022-08-05T13:28:19.3588882Z  validators-1:casper-net-1-node-3    RUNNING   pid 730, uptime 0:00:03
2022-08-05T13:28:19.3589238Z  validators-2:casper-net-1-node-4    RUNNING   pid 753, uptime 0:00:02
2022-08-05T13:28:19.3589583Z  validators-2:casper-net-1-node-5    RUNNING   pid 754, uptime 0:00:02
2022-08-05T13:28:19.3589945Z  validators-3:casper-net-1-node-10   STOPPED   Not started
2022-08-05T13:28:19.3590291Z  validators-3:casper-net-1-node-6    STOPPED   Not started
2022-08-05T13:28:19.3590619Z  validators-3:casper-net-1-node-7    STOPPED   Not started
2022-08-05T13:28:19.3590932Z  validators-3:casper-net-1-node-8    STOPPED   Not started
2022-08-05T13:28:19.3591262Z  validators-3:casper-net-1-node-9    STOPPED   Not started
2022-08-05T13:28:19.3599847Z Stop and remove container: e3bbe42de4f541f0a2fc53325e822296_makesoftwarecaspernctlv144220303_c1c81f
2022-08-05T13:28:19.3607107Z ##[command]/usr/bin/docker rm --force 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:28:19.6084710Z 694d14168f87c366fbb9c78cbd9b3a6dfc9273e4f3390d5ed3a71dfb1255c73b
2022-08-05T13:28:19.6117930Z Remove container network: github_network_245660b484a946a1a9d939397e5f343c
2022-08-05T13:28:19.6123923Z ##[command]/usr/bin/docker network rm github_network_245660b484a946a1a9d939397e5f343c
2022-08-05T13:28:19.7177191Z github_network_245660b484a946a1a9d939397e5f343c
2022-08-05T13:28:19.7324336Z Cleaning up orphan processes
```