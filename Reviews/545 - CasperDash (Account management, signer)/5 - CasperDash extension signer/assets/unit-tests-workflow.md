# Unit Tests Workflow Logs

```sh
2023-04-10T02:38:16.9355173Z Requested labels: ubuntu-latest
2023-04-10T02:38:16.9355237Z Job defined at: CasperDash/useWallet/.github/workflows/main.yml@refs/heads/main
2023-04-10T02:38:16.9355266Z Waiting for a runner to pick up this job...
2023-04-10T02:38:17.1545390Z Job is waiting for a hosted runner to come online.
2023-04-10T02:38:19.9090613Z Job is about to start running on the hosted runner: GitHub Actions 4 (hosted)
2023-04-10T02:38:22.2429799Z Current runner version: '2.303.0'
2023-04-10T02:38:22.2460217Z ##[group]Operating System
2023-04-10T02:38:22.2460725Z Ubuntu
2023-04-10T02:38:22.2461016Z 22.04.2
2023-04-10T02:38:22.2461299Z LTS
2023-04-10T02:38:22.2461640Z ##[endgroup]
2023-04-10T02:38:22.2461972Z ##[group]Runner Image
2023-04-10T02:38:22.2462320Z Image: ubuntu-22.04
2023-04-10T02:38:22.2462592Z Version: 20230402.1
2023-04-10T02:38:22.2463091Z Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20230402.1/images/linux/Ubuntu2204-Readme.md
2023-04-10T02:38:22.2463760Z Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20230402.1
2023-04-10T02:38:22.2464216Z ##[endgroup]
2023-04-10T02:38:22.2464509Z ##[group]Runner Image Provisioner
2023-04-10T02:38:22.2464844Z 2.0.139.1
2023-04-10T02:38:22.2465185Z ##[endgroup]
2023-04-10T02:38:22.2466190Z ##[group]GITHUB_TOKEN Permissions
2023-04-10T02:38:22.2466794Z Actions: write
2023-04-10T02:38:22.2467109Z Checks: write
2023-04-10T02:38:22.2467637Z Contents: write
2023-04-10T02:38:22.2468102Z Deployments: write
2023-04-10T02:38:22.2468385Z Discussions: write
2023-04-10T02:38:22.2468722Z Issues: write
2023-04-10T02:38:22.2469035Z Metadata: read
2023-04-10T02:38:22.2469355Z Packages: write
2023-04-10T02:38:22.2469623Z Pages: write
2023-04-10T02:38:22.2469950Z PullRequests: write
2023-04-10T02:38:22.2470348Z RepositoryProjects: write
2023-04-10T02:38:22.2470660Z SecurityEvents: write
2023-04-10T02:38:22.2470986Z Statuses: write
2023-04-10T02:38:22.2471323Z ##[endgroup]
2023-04-10T02:38:22.2475179Z Secret source: Actions
2023-04-10T02:38:22.2475731Z Prepare workflow directory
2023-04-10T02:38:22.3301454Z Prepare all required actions
2023-04-10T02:38:22.3495887Z Getting action download info
2023-04-10T02:38:22.8226136Z Download action repository 'actions/checkout@v3' (SHA:8f4b7f84864484a7bf31766abe9204da3cbe65b3)
2023-04-10T02:38:23.1396642Z Download action repository 'pnpm/action-setup@v2.2.4' (SHA:c3b53f6a16e57305370b4ae5a540c2077a1d50dd)
2023-04-10T02:38:23.4125932Z Download action repository 'actions/setup-node@v3' (SHA:64ed1c7eab4cce3362f8c340dee64e5eaeef8f7c)
2023-04-10T02:38:23.6933726Z Download action repository 'actions/cache@v3' (SHA:88522ab9f39a2ea568f7027eddc7d8d8bc9d59c8)
2023-04-10T02:38:23.9489828Z Download action repository 'codecov/codecov-action@v3' (SHA:d9f34f8cd5cb3b3eb79b3e4b5dae3a16df499a70)
2023-04-10T02:38:24.2762719Z Complete job name: Test (18, 7.19)
2023-04-10T02:38:24.3568165Z ##[group]Run actions/checkout@v3
2023-04-10T02:38:24.3568458Z with:
2023-04-10T02:38:24.3568706Z   repository: CasperDash/useWallet
2023-04-10T02:38:24.3569194Z   token: ***
2023-04-10T02:38:24.3569416Z   ssh-strict: true
2023-04-10T02:38:24.3569643Z   persist-credentials: true
2023-04-10T02:38:24.3569888Z   clean: true
2023-04-10T02:38:24.3570093Z   fetch-depth: 1
2023-04-10T02:38:24.3570304Z   lfs: false
2023-04-10T02:38:24.3570517Z   submodules: false
2023-04-10T02:38:24.3570753Z   set-safe-directory: true
2023-04-10T02:38:24.3570974Z ##[endgroup]
2023-04-10T02:38:24.6904071Z Syncing repository: CasperDash/useWallet
2023-04-10T02:38:24.6905755Z ##[group]Getting Git version info
2023-04-10T02:38:24.6906252Z Working directory is '/home/runner/work/useWallet/useWallet'
2023-04-10T02:38:24.6906769Z [command]/usr/bin/git version
2023-04-10T02:38:24.7045470Z git version 2.40.0
2023-04-10T02:38:24.7072689Z ##[endgroup]
2023-04-10T02:38:24.7091942Z Temporarily overriding HOME='/home/runner/work/_temp/971f9612-a355-44ed-9d2a-5f5a803c32cc' before making global git config changes
2023-04-10T02:38:24.7092434Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:38:24.7097474Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:38:24.7150689Z Deleting the contents of '/home/runner/work/useWallet/useWallet'
2023-04-10T02:38:24.7156161Z ##[group]Initializing the repository
2023-04-10T02:38:24.7159806Z [command]/usr/bin/git init /home/runner/work/useWallet/useWallet
2023-04-10T02:38:24.7246453Z hint: Using 'master' as the name for the initial branch. This default branch name
2023-04-10T02:38:24.7247021Z hint: is subject to change. To configure the initial branch name to use in all
2023-04-10T02:38:24.7247536Z hint: of your new repositories, which will suppress this warning, call:
2023-04-10T02:38:24.7247909Z hint: 
2023-04-10T02:38:24.7248342Z hint: 	git config --global init.defaultBranch <name>
2023-04-10T02:38:24.7248714Z hint: 
2023-04-10T02:38:24.7249170Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2023-04-10T02:38:24.7249726Z hint: 'development'. The just-created branch can be renamed via this command:
2023-04-10T02:38:24.7250091Z hint: 
2023-04-10T02:38:24.7250440Z hint: 	git branch -m <name>
2023-04-10T02:38:24.7258093Z Initialized empty Git repository in /home/runner/work/useWallet/useWallet/.git/
2023-04-10T02:38:24.7267615Z [command]/usr/bin/git remote add origin https://github.com/CasperDash/useWallet
2023-04-10T02:38:24.7310075Z ##[endgroup]
2023-04-10T02:38:24.7310654Z ##[group]Disabling automatic garbage collection
2023-04-10T02:38:24.7313705Z [command]/usr/bin/git config --local gc.auto 0
2023-04-10T02:38:24.7346798Z ##[endgroup]
2023-04-10T02:38:24.7347321Z ##[group]Setting up auth
2023-04-10T02:38:24.7354009Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:38:24.7387984Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:38:24.7803004Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:38:24.7831393Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:38:24.8069438Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2023-04-10T02:38:24.8107955Z ##[endgroup]
2023-04-10T02:38:24.8108588Z ##[group]Fetching the repository
2023-04-10T02:38:24.8117100Z [command]/usr/bin/git -c protocol.version=2 fetch --no-tags --prune --progress --no-recurse-submodules --depth=1 origin +25f8ac7a84341a7485ddf7707522bda42d38972c:refs/remotes/origin/main
2023-04-10T02:38:25.0341180Z remote: Enumerating objects: 169, done.        
2023-04-10T02:38:25.0347402Z remote: Counting objects:   0% (1/169)        
2023-04-10T02:38:25.0351866Z remote: Counting objects:   1% (2/169)        
2023-04-10T02:38:25.0355117Z remote: Counting objects:   2% (4/169)        
2023-04-10T02:38:25.0357428Z remote: Counting objects:   3% (6/169)        
2023-04-10T02:38:25.0359701Z remote: Counting objects:   4% (7/169)        
2023-04-10T02:38:25.0362197Z remote: Counting objects:   5% (9/169)        
2023-04-10T02:38:25.0365194Z remote: Counting objects:   6% (11/169)        
2023-04-10T02:38:25.0368322Z remote: Counting objects:   7% (12/169)        
2023-04-10T02:38:25.0371315Z remote: Counting objects:   8% (14/169)        
2023-04-10T02:38:25.0375637Z remote: Counting objects:   9% (16/169)        
2023-04-10T02:38:25.0378920Z remote: Counting objects:  10% (17/169)        
2023-04-10T02:38:25.0381971Z remote: Counting objects:  11% (19/169)        
2023-04-10T02:38:25.0384360Z remote: Counting objects:  12% (21/169)        
2023-04-10T02:38:25.0387090Z remote: Counting objects:  13% (22/169)        
2023-04-10T02:38:25.0389496Z remote: Counting objects:  14% (24/169)        
2023-04-10T02:38:25.0392453Z remote: Counting objects:  15% (26/169)        
2023-04-10T02:38:25.0394608Z remote: Counting objects:  16% (28/169)        
2023-04-10T02:38:25.0396633Z remote: Counting objects:  17% (29/169)        
2023-04-10T02:38:25.0399714Z remote: Counting objects:  18% (31/169)        
2023-04-10T02:38:25.0403078Z remote: Counting objects:  19% (33/169)        
2023-04-10T02:38:25.0407685Z remote: Counting objects:  20% (34/169)        
2023-04-10T02:38:25.0411414Z remote: Counting objects:  21% (36/169)        
2023-04-10T02:38:25.0413823Z remote: Counting objects:  22% (38/169)        
2023-04-10T02:38:25.0416160Z remote: Counting objects:  23% (39/169)        
2023-04-10T02:38:25.0418476Z remote: Counting objects:  24% (41/169)        
2023-04-10T02:38:25.0420766Z remote: Counting objects:  25% (43/169)        
2023-04-10T02:38:25.0423067Z remote: Counting objects:  26% (44/169)        
2023-04-10T02:38:25.0425358Z remote: Counting objects:  27% (46/169)        
2023-04-10T02:38:25.0427701Z remote: Counting objects:  28% (48/169)        
2023-04-10T02:38:25.0430026Z remote: Counting objects:  29% (50/169)        
2023-04-10T02:38:25.0432292Z remote: Counting objects:  30% (51/169)        
2023-04-10T02:38:25.0433917Z remote: Counting objects:  31% (53/169)        
2023-04-10T02:38:25.0435484Z remote: Counting objects:  32% (55/169)        
2023-04-10T02:38:25.0437032Z remote: Counting objects:  33% (56/169)        
2023-04-10T02:38:25.0438591Z remote: Counting objects:  34% (58/169)        
2023-04-10T02:38:25.0440243Z remote: Counting objects:  35% (60/169)        
2023-04-10T02:38:25.0442079Z remote: Counting objects:  36% (61/169)        
2023-04-10T02:38:25.0443653Z remote: Counting objects:  37% (63/169)        
2023-04-10T02:38:25.0445222Z remote: Counting objects:  38% (65/169)        
2023-04-10T02:38:25.0446769Z remote: Counting objects:  39% (66/169)        
2023-04-10T02:38:25.0448439Z remote: Counting objects:  40% (68/169)        
2023-04-10T02:38:25.0450051Z remote: Counting objects:  41% (70/169)        
2023-04-10T02:38:25.0452407Z remote: Counting objects:  42% (71/169)        
2023-04-10T02:38:25.0454080Z remote: Counting objects:  43% (73/169)        
2023-04-10T02:38:25.0456162Z remote: Counting objects:  44% (75/169)        
2023-04-10T02:38:25.0458627Z remote: Counting objects:  45% (77/169)        
2023-04-10T02:38:25.0461088Z remote: Counting objects:  46% (78/169)        
2023-04-10T02:38:25.0462768Z remote: Counting objects:  47% (80/169)        
2023-04-10T02:38:25.0465107Z remote: Counting objects:  48% (82/169)        
2023-04-10T02:38:25.0466728Z remote: Counting objects:  49% (83/169)        
2023-04-10T02:38:25.0468282Z remote: Counting objects:  50% (85/169)        
2023-04-10T02:38:25.0469851Z remote: Counting objects:  51% (87/169)        
2023-04-10T02:38:25.0471630Z remote: Counting objects:  52% (88/169)        
2023-04-10T02:38:25.0473372Z remote: Counting objects:  53% (90/169)        
2023-04-10T02:38:25.0474979Z remote: Counting objects:  54% (92/169)        
2023-04-10T02:38:25.0476592Z remote: Counting objects:  55% (93/169)        
2023-04-10T02:38:25.0480232Z remote: Counting objects:  56% (95/169)        
2023-04-10T02:38:25.0482069Z remote: Counting objects:  57% (97/169)        
2023-04-10T02:38:25.0487746Z remote: Counting objects:  58% (99/169)        
2023-04-10T02:38:25.0488036Z remote: Counting objects:  59% (100/169)        
2023-04-10T02:38:25.0488309Z remote: Counting objects:  60% (102/169)        
2023-04-10T02:38:25.0488601Z remote: Counting objects:  61% (104/169)        
2023-04-10T02:38:25.0488859Z remote: Counting objects:  62% (105/169)        
2023-04-10T02:38:25.0489130Z remote: Counting objects:  63% (107/169)        
2023-04-10T02:38:25.0489538Z remote: Counting objects:  64% (109/169)        
2023-04-10T02:38:25.0489807Z remote: Counting objects:  65% (110/169)        
2023-04-10T02:38:25.0490066Z remote: Counting objects:  66% (112/169)        
2023-04-10T02:38:25.0490326Z remote: Counting objects:  67% (114/169)        
2023-04-10T02:38:25.0490592Z remote: Counting objects:  68% (115/169)        
2023-04-10T02:38:25.0490841Z remote: Counting objects:  69% (117/169)        
2023-04-10T02:38:25.0491099Z remote: Counting objects:  70% (119/169)        
2023-04-10T02:38:25.0491368Z remote: Counting objects:  71% (120/169)        
2023-04-10T02:38:25.0491632Z remote: Counting objects:  72% (122/169)        
2023-04-10T02:38:25.0491880Z remote: Counting objects:  73% (124/169)        
2023-04-10T02:38:25.0492374Z remote: Counting objects:  74% (126/169)        
2023-04-10T02:38:25.0492636Z remote: Counting objects:  75% (127/169)        
2023-04-10T02:38:25.0492885Z remote: Counting objects:  76% (129/169)        
2023-04-10T02:38:25.0493149Z remote: Counting objects:  77% (131/169)        
2023-04-10T02:38:25.0493412Z remote: Counting objects:  78% (132/169)        
2023-04-10T02:38:25.0493666Z remote: Counting objects:  79% (134/169)        
2023-04-10T02:38:25.0493930Z remote: Counting objects:  80% (136/169)        
2023-04-10T02:38:25.0494198Z remote: Counting objects:  81% (137/169)        
2023-04-10T02:38:25.0494445Z remote: Counting objects:  82% (139/169)        
2023-04-10T02:38:25.0494709Z remote: Counting objects:  83% (141/169)        
2023-04-10T02:38:25.0494969Z remote: Counting objects:  84% (142/169)        
2023-04-10T02:38:25.0495234Z remote: Counting objects:  85% (144/169)        
2023-04-10T02:38:25.0495484Z remote: Counting objects:  86% (146/169)        
2023-04-10T02:38:25.0495756Z remote: Counting objects:  87% (148/169)        
2023-04-10T02:38:25.0496019Z remote: Counting objects:  88% (149/169)        
2023-04-10T02:38:25.0496267Z remote: Counting objects:  89% (151/169)        
2023-04-10T02:38:25.0496533Z remote: Counting objects:  90% (153/169)        
2023-04-10T02:38:25.0496801Z remote: Counting objects:  91% (154/169)        
2023-04-10T02:38:25.0497055Z remote: Counting objects:  92% (156/169)        
2023-04-10T02:38:25.0497318Z remote: Counting objects:  93% (158/169)        
2023-04-10T02:38:25.0497585Z remote: Counting objects:  94% (159/169)        
2023-04-10T02:38:25.0497829Z remote: Counting objects:  95% (161/169)        
2023-04-10T02:38:25.0498096Z remote: Counting objects:  96% (163/169)        
2023-04-10T02:38:25.0498361Z remote: Counting objects:  97% (164/169)        
2023-04-10T02:38:25.0498624Z remote: Counting objects:  98% (166/169)        
2023-04-10T02:38:25.0498871Z remote: Counting objects:  99% (168/169)        
2023-04-10T02:38:25.0499143Z remote: Counting objects: 100% (169/169)        
2023-04-10T02:38:25.0499422Z remote: Counting objects: 100% (169/169), done.        
2023-04-10T02:38:25.0499706Z remote: Compressing objects:   0% (1/151)        
2023-04-10T02:38:25.0499995Z remote: Compressing objects:   1% (2/151)        
2023-04-10T02:38:25.0500277Z remote: Compressing objects:   2% (4/151)        
2023-04-10T02:38:25.0500675Z remote: Compressing objects:   3% (5/151)        
2023-04-10T02:38:25.0500955Z remote: Compressing objects:   4% (7/151)        
2023-04-10T02:38:25.0501226Z remote: Compressing objects:   5% (8/151)        
2023-04-10T02:38:25.0501494Z remote: Compressing objects:   6% (10/151)        
2023-04-10T02:38:25.0501775Z remote: Compressing objects:   7% (11/151)        
2023-04-10T02:38:25.0502059Z remote: Compressing objects:   8% (13/151)        
2023-04-10T02:38:25.0502345Z remote: Compressing objects:   9% (14/151)        
2023-04-10T02:38:25.0502607Z remote: Compressing objects:  10% (16/151)        
2023-04-10T02:38:25.0502893Z remote: Compressing objects:  11% (17/151)        
2023-04-10T02:38:25.0503169Z remote: Compressing objects:  12% (19/151)        
2023-04-10T02:38:25.0503432Z remote: Compressing objects:  13% (20/151)        
2023-04-10T02:38:25.0503711Z remote: Compressing objects:  14% (22/151)        
2023-04-10T02:38:25.0503987Z remote: Compressing objects:  15% (23/151)        
2023-04-10T02:38:25.0504254Z remote: Compressing objects:  16% (25/151)        
2023-04-10T02:38:25.0504532Z remote: Compressing objects:  17% (26/151)        
2023-04-10T02:38:25.0504814Z remote: Compressing objects:  18% (28/151)        
2023-04-10T02:38:25.0549068Z remote: Compressing objects:  19% (29/151)        
2023-04-10T02:38:25.0549390Z remote: Compressing objects:  20% (31/151)        
2023-04-10T02:38:25.0549661Z remote: Compressing objects:  21% (32/151)        
2023-04-10T02:38:25.0549970Z remote: Compressing objects:  22% (34/151)        
2023-04-10T02:38:25.0550249Z remote: Compressing objects:  23% (35/151)        
2023-04-10T02:38:25.0550725Z remote: Compressing objects:  24% (37/151)        
2023-04-10T02:38:25.0551005Z remote: Compressing objects:  25% (38/151)        
2023-04-10T02:38:25.0551283Z remote: Compressing objects:  26% (40/151)        
2023-04-10T02:38:25.0551545Z remote: Compressing objects:  27% (41/151)        
2023-04-10T02:38:25.0552881Z remote: Compressing objects:  28% (43/151)        
2023-04-10T02:38:25.0553182Z remote: Compressing objects:  29% (44/151)        
2023-04-10T02:38:25.0553456Z remote: Compressing objects:  30% (46/151)        
2023-04-10T02:38:25.0553717Z remote: Compressing objects:  31% (47/151)        
2023-04-10T02:38:25.0553995Z remote: Compressing objects:  32% (49/151)        
2023-04-10T02:38:25.0554270Z remote: Compressing objects:  33% (50/151)        
2023-04-10T02:38:25.0554530Z remote: Compressing objects:  34% (52/151)        
2023-04-10T02:38:25.0554805Z remote: Compressing objects:  35% (53/151)        
2023-04-10T02:38:25.0555076Z remote: Compressing objects:  36% (55/151)        
2023-04-10T02:38:25.0555342Z remote: Compressing objects:  37% (56/151)        
2023-04-10T02:38:25.0555617Z remote: Compressing objects:  38% (58/151)        
2023-04-10T02:38:25.0555891Z remote: Compressing objects:  39% (59/151)        
2023-04-10T02:38:25.0556153Z remote: Compressing objects:  40% (61/151)        
2023-04-10T02:38:25.0556432Z remote: Compressing objects:  41% (62/151)        
2023-04-10T02:38:25.0556703Z remote: Compressing objects:  42% (64/151)        
2023-04-10T02:38:25.0556978Z remote: Compressing objects:  43% (65/151)        
2023-04-10T02:38:25.0557234Z remote: Compressing objects:  44% (67/151)        
2023-04-10T02:38:25.0557512Z remote: Compressing objects:  45% (68/151)        
2023-04-10T02:38:25.0557782Z remote: Compressing objects:  46% (70/151)        
2023-04-10T02:38:25.0559605Z remote: Compressing objects:  47% (71/151)        
2023-04-10T02:38:25.0559895Z remote: Compressing objects:  48% (73/151)        
2023-04-10T02:38:25.0560180Z remote: Compressing objects:  49% (74/151)        
2023-04-10T02:38:25.0560441Z remote: Compressing objects:  50% (76/151)        
2023-04-10T02:38:25.0560822Z remote: Compressing objects:  51% (78/151)        
2023-04-10T02:38:25.0561106Z remote: Compressing objects:  52% (79/151)        
2023-04-10T02:38:25.0561380Z remote: Compressing objects:  53% (81/151)        
2023-04-10T02:38:25.0561849Z remote: Compressing objects:  54% (82/151)        
2023-04-10T02:38:25.0562134Z remote: Compressing objects:  55% (84/151)        
2023-04-10T02:38:25.0562409Z remote: Compressing objects:  56% (85/151)        
2023-04-10T02:38:25.0562668Z remote: Compressing objects:  57% (87/151)        
2023-04-10T02:38:25.0562945Z remote: Compressing objects:  58% (88/151)        
2023-04-10T02:38:25.0563226Z remote: Compressing objects:  59% (90/151)        
2023-04-10T02:38:25.0563490Z remote: Compressing objects:  60% (91/151)        
2023-04-10T02:38:25.0563764Z remote: Compressing objects:  61% (93/151)        
2023-04-10T02:38:25.0564042Z remote: Compressing objects:  62% (94/151)        
2023-04-10T02:38:25.0564301Z remote: Compressing objects:  63% (96/151)        
2023-04-10T02:38:25.0564572Z remote: Compressing objects:  64% (97/151)        
2023-04-10T02:38:25.0564843Z remote: Compressing objects:  65% (99/151)        
2023-04-10T02:38:25.0565122Z remote: Compressing objects:  66% (100/151)        
2023-04-10T02:38:25.0565396Z remote: Compressing objects:  67% (102/151)        
2023-04-10T02:38:25.0565679Z remote: Compressing objects:  68% (103/151)        
2023-04-10T02:38:25.0565959Z remote: Compressing objects:  69% (105/151)        
2023-04-10T02:38:25.0566222Z remote: Compressing objects:  70% (106/151)        
2023-04-10T02:38:25.0566544Z remote: Compressing objects:  71% (108/151)        
2023-04-10T02:38:25.0566821Z remote: Compressing objects:  72% (109/151)        
2023-04-10T02:38:25.0567090Z remote: Compressing objects:  73% (111/151)        
2023-04-10T02:38:25.0567400Z remote: Compressing objects:  74% (112/151)        
2023-04-10T02:38:25.0567792Z remote: Compressing objects:  75% (114/151)        
2023-04-10T02:38:25.0568071Z remote: Compressing objects:  76% (115/151)        
2023-04-10T02:38:25.0568339Z remote: Compressing objects:  77% (117/151)        
2023-04-10T02:38:25.0568619Z remote: Compressing objects:  78% (118/151)        
2023-04-10T02:38:25.0568912Z remote: Compressing objects:  79% (120/151)        
2023-04-10T02:38:25.0569174Z remote: Compressing objects:  80% (121/151)        
2023-04-10T02:38:25.0569450Z remote: Compressing objects:  81% (123/151)        
2023-04-10T02:38:25.0569725Z remote: Compressing objects:  82% (124/151)        
2023-04-10T02:38:25.0569989Z remote: Compressing objects:  83% (126/151)        
2023-04-10T02:38:25.0570271Z remote: Compressing objects:  84% (127/151)        
2023-04-10T02:38:25.0570543Z remote: Compressing objects:  85% (129/151)        
2023-04-10T02:38:25.0570814Z remote: Compressing objects:  86% (130/151)        
2023-04-10T02:38:25.0571077Z remote: Compressing objects:  87% (132/151)        
2023-04-10T02:38:25.0571362Z remote: Compressing objects:  88% (133/151)        
2023-04-10T02:38:25.0571640Z remote: Compressing objects:  89% (135/151)        
2023-04-10T02:38:25.0571930Z remote: Compressing objects:  90% (136/151)        
2023-04-10T02:38:25.0572208Z remote: Compressing objects:  91% (138/151)        
2023-04-10T02:38:25.0572478Z remote: Compressing objects:  92% (139/151)        
2023-04-10T02:38:25.0572759Z remote: Compressing objects:  93% (141/151)        
2023-04-10T02:38:25.0573080Z remote: Compressing objects:  94% (142/151)        
2023-04-10T02:38:25.0573374Z remote: Compressing objects:  95% (144/151)        
2023-04-10T02:38:25.0573650Z remote: Compressing objects:  96% (145/151)        
2023-04-10T02:38:25.0573925Z remote: Compressing objects:  97% (147/151)        
2023-04-10T02:38:25.0574190Z remote: Compressing objects:  98% (148/151)        
2023-04-10T02:38:25.0574475Z remote: Compressing objects:  99% (150/151)        
2023-04-10T02:38:25.0574754Z remote: Compressing objects: 100% (151/151)        
2023-04-10T02:38:25.0575098Z remote: Compressing objects: 100% (151/151), done.        
2023-04-10T02:38:25.0609154Z Receiving objects:   0% (1/169)
2023-04-10T02:38:25.0611262Z Receiving objects:   1% (2/169)
2023-04-10T02:38:25.0613229Z Receiving objects:   2% (4/169)
2023-04-10T02:38:25.0615011Z Receiving objects:   3% (6/169)
2023-04-10T02:38:25.0617177Z Receiving objects:   4% (7/169)
2023-04-10T02:38:25.0619160Z Receiving objects:   5% (9/169)
2023-04-10T02:38:25.0621001Z Receiving objects:   6% (11/169)
2023-04-10T02:38:25.0622866Z Receiving objects:   7% (12/169)
2023-04-10T02:38:25.0624786Z Receiving objects:   8% (14/169)
2023-04-10T02:38:25.0626552Z Receiving objects:   9% (16/169)
2023-04-10T02:38:25.0628366Z Receiving objects:  10% (17/169)
2023-04-10T02:38:25.0630170Z Receiving objects:  11% (19/169)
2023-04-10T02:38:25.0631845Z Receiving objects:  12% (21/169)
2023-04-10T02:38:25.0634517Z Receiving objects:  13% (22/169)
2023-04-10T02:38:25.0638112Z Receiving objects:  14% (24/169)
2023-04-10T02:38:25.0640162Z Receiving objects:  15% (26/169)
2023-04-10T02:38:25.0642232Z Receiving objects:  16% (28/169)
2023-04-10T02:38:25.0644279Z Receiving objects:  17% (29/169)
2023-04-10T02:38:25.0646248Z Receiving objects:  18% (31/169)
2023-04-10T02:38:25.0648095Z Receiving objects:  19% (33/169)
2023-04-10T02:38:25.0650073Z Receiving objects:  20% (34/169)
2023-04-10T02:38:25.0652066Z Receiving objects:  21% (36/169)
2023-04-10T02:38:25.0654072Z Receiving objects:  22% (38/169)
2023-04-10T02:38:25.0656095Z Receiving objects:  23% (39/169)
2023-04-10T02:38:25.0659041Z Receiving objects:  24% (41/169)
2023-04-10T02:38:25.0661191Z Receiving objects:  25% (43/169)
2023-04-10T02:38:25.0663317Z Receiving objects:  26% (44/169)
2023-04-10T02:38:25.0665237Z Receiving objects:  27% (46/169)
2023-04-10T02:38:25.0667082Z Receiving objects:  28% (48/169)
2023-04-10T02:38:25.0668800Z Receiving objects:  29% (50/169)
2023-04-10T02:38:25.0673299Z Receiving objects:  30% (51/169)
2023-04-10T02:38:25.0675688Z Receiving objects:  31% (53/169)
2023-04-10T02:38:25.0677932Z Receiving objects:  32% (55/169)
2023-04-10T02:38:25.0679843Z Receiving objects:  33% (56/169)
2023-04-10T02:38:25.0865015Z Receiving objects:  34% (58/169)
2023-04-10T02:38:25.0867488Z Receiving objects:  35% (60/169)
2023-04-10T02:38:25.0869791Z Receiving objects:  36% (61/169)
2023-04-10T02:38:25.0872164Z Receiving objects:  37% (63/169)
2023-04-10T02:38:25.0874506Z Receiving objects:  38% (65/169)
2023-04-10T02:38:25.0876851Z Receiving objects:  39% (66/169)
2023-04-10T02:38:25.0879404Z Receiving objects:  40% (68/169)
2023-04-10T02:38:25.0881959Z Receiving objects:  41% (70/169)
2023-04-10T02:38:25.0885674Z Receiving objects:  42% (71/169)
2023-04-10T02:38:25.0888237Z Receiving objects:  43% (73/169)
2023-04-10T02:38:25.0900295Z Receiving objects:  44% (75/169)
2023-04-10T02:38:25.0902615Z Receiving objects:  45% (77/169)
2023-04-10T02:38:25.0904939Z Receiving objects:  46% (78/169)
2023-04-10T02:38:25.0920636Z Receiving objects:  47% (80/169)
2023-04-10T02:38:25.0923064Z Receiving objects:  48% (82/169)
2023-04-10T02:38:25.0927536Z Receiving objects:  49% (83/169)
2023-04-10T02:38:25.0930185Z Receiving objects:  50% (85/169)
2023-04-10T02:38:25.0933373Z Receiving objects:  51% (87/169)
2023-04-10T02:38:25.0935641Z Receiving objects:  52% (88/169)
2023-04-10T02:38:25.0937905Z Receiving objects:  53% (90/169)
2023-04-10T02:38:25.0940247Z Receiving objects:  54% (92/169)
2023-04-10T02:38:25.0942724Z Receiving objects:  55% (93/169)
2023-04-10T02:38:25.0944936Z Receiving objects:  56% (95/169)
2023-04-10T02:38:25.0947474Z Receiving objects:  57% (97/169)
2023-04-10T02:38:25.0950828Z Receiving objects:  58% (99/169)
2023-04-10T02:38:25.0953480Z Receiving objects:  59% (100/169)
2023-04-10T02:38:25.0956200Z Receiving objects:  60% (102/169)
2023-04-10T02:38:25.0958411Z Receiving objects:  61% (104/169)
2023-04-10T02:38:25.0961146Z Receiving objects:  62% (105/169)
2023-04-10T02:38:25.0964209Z Receiving objects:  63% (107/169)
2023-04-10T02:38:25.0966379Z Receiving objects:  64% (109/169)
2023-04-10T02:38:25.0968824Z Receiving objects:  65% (110/169)
2023-04-10T02:38:25.0971220Z Receiving objects:  66% (112/169)
2023-04-10T02:38:25.0973288Z Receiving objects:  67% (114/169)
2023-04-10T02:38:25.0975837Z Receiving objects:  68% (115/169)
2023-04-10T02:38:25.0979524Z Receiving objects:  69% (117/169)
2023-04-10T02:38:25.0982283Z Receiving objects:  70% (119/169)
2023-04-10T02:38:25.0985384Z Receiving objects:  71% (120/169)
2023-04-10T02:38:25.0988997Z Receiving objects:  72% (122/169)
2023-04-10T02:38:25.0991360Z Receiving objects:  73% (124/169)
2023-04-10T02:38:25.0993387Z Receiving objects:  74% (126/169)
2023-04-10T02:38:25.0995580Z Receiving objects:  75% (127/169)
2023-04-10T02:38:25.0997819Z Receiving objects:  76% (129/169)
2023-04-10T02:38:25.0999802Z Receiving objects:  77% (131/169)
2023-04-10T02:38:25.1024638Z Receiving objects:  78% (132/169)
2023-04-10T02:38:25.1027636Z Receiving objects:  79% (134/169)
2023-04-10T02:38:25.1028948Z Receiving objects:  80% (136/169)
2023-04-10T02:38:25.1031743Z Receiving objects:  81% (137/169)
2023-04-10T02:38:25.1035960Z Receiving objects:  82% (139/169)
2023-04-10T02:38:25.1038870Z Receiving objects:  83% (141/169)
2023-04-10T02:38:25.1041837Z Receiving objects:  84% (142/169)
2023-04-10T02:38:25.1044756Z Receiving objects:  85% (144/169)
2023-04-10T02:38:25.1048637Z Receiving objects:  86% (146/169)
2023-04-10T02:38:25.1048907Z Receiving objects:  87% (148/169)
2023-04-10T02:38:25.1050996Z Receiving objects:  88% (149/169)
2023-04-10T02:38:25.1054142Z Receiving objects:  89% (151/169)
2023-04-10T02:38:25.1056387Z Receiving objects:  90% (153/169)
2023-04-10T02:38:25.1058686Z Receiving objects:  91% (154/169)
2023-04-10T02:38:25.1061241Z Receiving objects:  92% (156/169)
2023-04-10T02:38:25.1063204Z Receiving objects:  93% (158/169)
2023-04-10T02:38:25.1066095Z Receiving objects:  94% (159/169)
2023-04-10T02:38:25.1069434Z Receiving objects:  95% (161/169)
2023-04-10T02:38:25.1069931Z Receiving objects:  96% (163/169)
2023-04-10T02:38:25.1084678Z Receiving objects:  97% (164/169)
2023-04-10T02:38:25.1085551Z remote: Total 169 (delta 18), reused 115 (delta 7), pack-reused 0        
2023-04-10T02:38:25.1107731Z Receiving objects:  98% (166/169)
2023-04-10T02:38:25.1110731Z Receiving objects:  99% (168/169)
2023-04-10T02:38:25.1113864Z Receiving objects: 100% (169/169)
2023-04-10T02:38:25.1114385Z Receiving objects: 100% (169/169), 993.20 KiB | 19.47 MiB/s, done.
2023-04-10T02:38:25.1119102Z Resolving deltas:   0% (0/18)
2023-04-10T02:38:25.1121292Z Resolving deltas:   5% (1/18)
2023-04-10T02:38:25.1123407Z Resolving deltas:  11% (2/18)
2023-04-10T02:38:25.1125123Z Resolving deltas:  16% (3/18)
2023-04-10T02:38:25.1126758Z Resolving deltas:  22% (4/18)
2023-04-10T02:38:25.1128336Z Resolving deltas:  27% (5/18)
2023-04-10T02:38:25.1128958Z Resolving deltas:  33% (6/18)
2023-04-10T02:38:25.1130222Z Resolving deltas:  38% (7/18)
2023-04-10T02:38:25.1131755Z Resolving deltas:  44% (8/18)
2023-04-10T02:38:25.1134746Z Resolving deltas:  50% (9/18)
2023-04-10T02:38:25.1135227Z Resolving deltas:  55% (10/18)
2023-04-10T02:38:25.1137487Z Resolving deltas:  61% (11/18)
2023-04-10T02:38:25.1138152Z Resolving deltas:  66% (12/18)
2023-04-10T02:38:25.1139698Z Resolving deltas:  72% (13/18)
2023-04-10T02:38:25.1140223Z Resolving deltas:  77% (14/18)
2023-04-10T02:38:25.1143222Z Resolving deltas:  83% (15/18)
2023-04-10T02:38:25.1145896Z Resolving deltas:  88% (16/18)
2023-04-10T02:38:25.1147027Z Resolving deltas:  94% (17/18)
2023-04-10T02:38:25.1147624Z Resolving deltas: 100% (18/18)
2023-04-10T02:38:25.1148233Z Resolving deltas: 100% (18/18), done.
2023-04-10T02:38:25.1240743Z From https://github.com/CasperDash/useWallet
2023-04-10T02:38:25.1241870Z  * [new ref]         25f8ac7a84341a7485ddf7707522bda42d38972c -> origin/main
2023-04-10T02:38:25.1281912Z ##[endgroup]
2023-04-10T02:38:25.1282593Z ##[group]Determining the checkout info
2023-04-10T02:38:25.1283126Z ##[endgroup]
2023-04-10T02:38:25.1283727Z ##[group]Checking out the ref
2023-04-10T02:38:25.1284355Z [command]/usr/bin/git checkout --progress --force -B main refs/remotes/origin/main
2023-04-10T02:38:25.1446051Z Switched to a new branch 'main'
2023-04-10T02:38:25.1447736Z branch 'main' set up to track 'origin/main'.
2023-04-10T02:38:25.1455245Z ##[endgroup]
2023-04-10T02:38:25.1498534Z [command]/usr/bin/git log -1 --format='%H'
2023-04-10T02:38:25.1529346Z '25f8ac7a84341a7485ddf7707522bda42d38972c'
2023-04-10T02:38:25.1836255Z ##[group]Run pnpm/action-setup@v2.2.4
2023-04-10T02:38:25.1836592Z with:
2023-04-10T02:38:25.1836910Z   version: 7.19
2023-04-10T02:38:25.1837152Z   dest: ~/setup-pnpm
2023-04-10T02:38:25.1837451Z   run_install: null
2023-04-10T02:38:25.1837725Z ##[endgroup]
2023-04-10T02:38:25.3071737Z ##[group]Running self-installer...
2023-04-10T02:38:25.7896441Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:38:25.7976971Z Packages: +1
2023-04-10T02:38:25.7977373Z +
2023-04-10T02:38:26.4468796Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:38:26.4469915Z   Content-addressable store is at: /home/runner/.pnpm-store/v3
2023-04-10T02:38:26.4470753Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:38:26.4735618Z 
2023-04-10T02:38:26.4736331Z dependencies:
2023-04-10T02:38:26.4736993Z + pnpm 7.19.0 (8.2.0 is available)
2023-04-10T02:38:26.4737427Z 
2023-04-10T02:38:26.7897005Z Progress: resolved 1, reused 0, downloaded 1, added 1, done
2023-04-10T02:38:26.8103990Z ##[endgroup]
2023-04-10T02:38:26.8107151Z Installation Completed!
2023-04-10T02:38:26.8285068Z ##[group]Run actions/setup-node@v3
2023-04-10T02:38:26.8285313Z with:
2023-04-10T02:38:26.8285499Z   node-version: 18
2023-04-10T02:38:26.8285710Z   always-auth: false
2023-04-10T02:38:26.8285923Z   check-latest: false
2023-04-10T02:38:26.8286364Z   token: ***
2023-04-10T02:38:26.8286546Z env:
2023-04-10T02:38:26.8286800Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:38:26.8287266Z ##[endgroup]
2023-04-10T02:38:27.0345407Z Found in cache @ /opt/hostedtoolcache/node/18.15.0/x64
2023-04-10T02:38:27.0356759Z ##[group]Environment details
2023-04-10T02:38:33.6890994Z node: v18.15.0
2023-04-10T02:38:33.6891838Z npm: 9.5.0
2023-04-10T02:38:33.6892441Z yarn: 1.22.19
2023-04-10T02:38:33.6893326Z ##[endgroup]
2023-04-10T02:38:33.7777590Z ##[group]Run actions/cache@v3
2023-04-10T02:38:33.7777821Z with:
2023-04-10T02:38:33.7778124Z   path: node_modules
docs/node_modules
examples/**/node_modules
packages/**/node_modules
packages/**/dist

2023-04-10T02:38:33.7778552Z   key: modules-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:38:33.7778886Z   enableCrossOsArchive: false
2023-04-10T02:38:33.7779121Z   fail-on-cache-miss: false
2023-04-10T02:38:33.7779348Z   lookup-only: false
2023-04-10T02:38:33.7779544Z env:
2023-04-10T02:38:33.7779783Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:38:33.7780038Z ##[endgroup]
2023-04-10T02:38:35.0160924Z Received 144507044 of 148701348 (97.2%), 137.7 MBs/sec
2023-04-10T02:38:35.0342001Z Received 148701348 of 148701348 (100.0%), 139.0 MBs/sec
2023-04-10T02:38:35.0346367Z Cache Size: ~142 MB (148701348 B)
2023-04-10T02:38:35.0393064Z [command]/usr/bin/tar -xf /home/runner/work/_temp/69483b6c-01e4-4060-b81d-7266fc8c239a/cache.tzst -P -C /home/runner/work/useWallet/useWallet --use-compress-program unzstd
2023-04-10T02:38:36.8564915Z Cache restored successfully
2023-04-10T02:38:36.9596511Z Cache restored from key: modules-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:38:36.9811889Z ##[group]Run pnpm i
2023-04-10T02:38:36.9812188Z [36;1mpnpm i[0m
2023-04-10T02:38:36.9870082Z shell: /usr/bin/bash -e {0}
2023-04-10T02:38:36.9870330Z env:
2023-04-10T02:38:36.9870606Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:38:36.9870865Z ##[endgroup]
2023-04-10T02:38:37.6706974Z Scope: all 5 workspace projects
2023-04-10T02:38:37.8442772Z Lockfile is up to date, resolution step is skipped
2023-04-10T02:38:37.9987024Z Already up to date
2023-04-10T02:38:38.6740198Z 
2023-04-10T02:38:38.6756241Z . prepare$ husky install
2023-04-10T02:38:38.8140196Z . prepare: husky - Git hooks installed
2023-04-10T02:38:38.8207282Z . prepare: Done
2023-04-10T02:38:38.8230253Z Done in 1.7s
2023-04-10T02:38:38.8444956Z ##[group]Run pnpm test:coverage
2023-04-10T02:38:38.8445248Z [36;1mpnpm test:coverage[0m
2023-04-10T02:38:38.8505686Z shell: /usr/bin/bash -e {0}
2023-04-10T02:38:38.8505920Z env:
2023-04-10T02:38:38.8506189Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:38:38.8506446Z ##[endgroup]
2023-04-10T02:38:39.3791069Z 
2023-04-10T02:38:39.3818021Z > root@0.0.3 test:coverage /home/runner/work/useWallet/useWallet
2023-04-10T02:38:39.3818804Z > vitest run --coverage
2023-04-10T02:38:39.3819038Z 
2023-04-10T02:38:39.9258223Z 
2023-04-10T02:38:39.9262579Z [7m[1m[36m RUN [39m[22m[27m [36mv0.26.3[39m [90m/home/runner/work/useWallet/useWallet[39m
2023-04-10T02:38:39.9265115Z [2m      Coverage enabled with [22m[33mc8[39m
2023-04-10T02:38:39.9266972Z 
2023-04-10T02:38:41.8926355Z [90mstdout[2m | packages/core/src/connectors/casperWallet.test.ts[2m > [22m[2mCasperWalletConnector[2m > [22m[2mconnect[2m > [22m[2msign[2m > [22m[2mshould sign the deploy using the provider[22m[39m
2023-04-10T02:38:41.8927308Z signedDeploy:  [90mundefined[39m
2023-04-10T02:38:41.8927475Z 
2023-04-10T02:38:42.0326669Z  [32m✓[39m packages/core/src/connectors/casperWallet.test.ts [2m ([22m[2m23 tests[22m[2m)[22m[90m 58[2mms[22m[39m
2023-04-10T02:38:43.2013957Z [90mstderr[2m | packages/core/src/connectors/casperDash.test.ts[2m > [22m[2mCasperDashConnector[2m > [22m[2misConnected[2m > [22m[2mreturns false if there is an error[22m[39m
2023-04-10T02:38:43.2014471Z Error: 
2023-04-10T02:38:43.2015093Z     at [90m/home/runner/work/useWallet/useWallet/[39mpackages/core/src/connectors/casperDash.test.ts:193:46
2023-04-10T02:38:43.2016471Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2294:13
2023-04-10T02:38:43.2017447Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2171:26
2023-04-10T02:38:43.2018456Z     at runTest [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:381:42[90m)[39m
2023-04-10T02:38:43.2019474Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:43.2020474Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:43.2021503Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:43.2022490Z     at runFiles [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:614:5[90m)[39m
2023-04-10T02:38:43.2023513Z     at startTestsNode [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:632:3[90m)[39m
2023-04-10T02:38:43.2024412Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/entry.js:103:11
2023-04-10T02:38:43.2024723Z 
2023-04-10T02:38:43.3686930Z  [32m✓[39m packages/core/src/connectors/casperDash.test.ts [2m ([22m[2m23 tests[22m[2m)[22m[90m 69[2mms[22m[39m
2023-04-10T02:38:44.5909917Z  [32m✓[39m packages/core/src/connectors/casperSigner.test.ts [2m ([22m[2m23 tests[22m[2m)[22m[90m 30[2mms[22m[39m
2023-04-10T02:38:45.8021640Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:45.8022449Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:45.8022918Z 
2023-04-10T02:38:45.9046125Z [90mstderr[2m | packages/core/src/utils/client.test.ts[2m > [22m[2mClient[2m > [22m[2mconstructor[2m > [22m[2mshould set status to CONNECTING[22m[39m
2023-04-10T02:38:45.9055297Z ConnectorNotFoundError: Connector not found
2023-04-10T02:38:45.9056390Z     at CasperDashConnector.getProvider [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/connectors/casperDash.ts:67:13[90m)[39m
2023-04-10T02:38:45.9057509Z     at CasperDashConnector.isConnected [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/connectors/casperDash.ts:96:29[90m)[39m
2023-04-10T02:38:45.9058447Z     at Client.autoConnect [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/utils/client.ts:132:57[90m)[39m
2023-04-10T02:38:45.9059247Z     at [90m/home/runner/work/useWallet/useWallet/[39mpackages/core/src/utils/client.test.ts:76:19
2023-04-10T02:38:45.9060681Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2294:13
2023-04-10T02:38:45.9061693Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2171:26
2023-04-10T02:38:45.9062695Z     at runTest [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:381:42[90m)[39m
2023-04-10T02:38:45.9064154Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:45.9065173Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:45.9066160Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:45.9066537Z 
2023-04-10T02:38:45.9099789Z [90mstderr[2m | packages/core/src/utils/client.test.ts[2m > [22m[2mClient[2m > [22m[2mconstructor[2m > [22m[2mshould set status to DISCONNECTED when no connector is connected[22m[39m
2023-04-10T02:38:45.9102279Z ConnectorNotFoundError: Connector not found
2023-04-10T02:38:45.9103049Z     at CasperDashConnector.getProvider [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/connectors/casperDash.ts:67:13[90m)[39m
2023-04-10T02:38:45.9103873Z     at CasperDashConnector.isConnected [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/connectors/casperDash.ts:96:29[90m)[39m
2023-04-10T02:38:45.9104596Z     at Client.autoConnect [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/utils/client.ts:132:57[90m)[39m
2023-04-10T02:38:45.9105207Z     at [90m/home/runner/work/useWallet/useWallet/[39mpackages/core/src/utils/client.test.ts:84:20
2023-04-10T02:38:45.9106051Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2294:13
2023-04-10T02:38:45.9107013Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2171:26
2023-04-10T02:38:45.9108282Z     at runTest [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:381:42[90m)[39m
2023-04-10T02:38:45.9109303Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:45.9110302Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:45.9111312Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:45.9111681Z 
2023-04-10T02:38:46.0886541Z  [32m✓[39m packages/core/src/utils/client.test.ts [2m ([22m[2m18 tests[22m[2m)[22m[90m 52[2mms[22m[39m
2023-04-10T02:38:47.7045103Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:47.7082030Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:47.7082848Z 
2023-04-10T02:38:48.1212768Z  [32m✓[39m packages/react/src/hooks/useSign.test.ts [2m ([22m[2m6 tests[22m[2m)[22m[90m 141[2mms[22m[39m
2023-04-10T02:38:49.4054857Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:49.4055478Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:49.4055759Z 
2023-04-10T02:38:49.5963238Z  [32m✓[39m packages/core/src/actions/account/connect.test.ts [2m ([22m[2m4 tests[22m[2m)[22m[90m 10[2mms[22m[39m
2023-04-10T02:38:51.1182384Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:51.1183201Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:51.1183566Z 
2023-04-10T02:38:51.4584578Z  [32m✓[39m packages/react/src/hooks/useSignMessage.test.ts [2m ([22m[2m4 tests[22m[2m)[22m[90m 135[2mms[22m[39m
2023-04-10T02:38:52.4834195Z [90mstderr[2m | packages/core/src/actions/signing/sign.test.ts[2m > [22m[2msign[2m > [22m[2mshould return undefined if the connector is not available[22m[39m
2023-04-10T02:38:52.4851727Z ConnectorNotFoundError: Connector not found
2023-04-10T02:38:52.4852751Z     at Module.sign [90m(/home/runner/work/useWallet/useWallet/[39mpackages/core/src/actions/signing/sign.ts:24:13[90m)[39m
2023-04-10T02:38:52.4853571Z     at [90m/home/runner/work/useWallet/useWallet/[39mpackages/core/src/actions/signing/sign.test.ts:50:26
2023-04-10T02:38:52.4855094Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2294:13
2023-04-10T02:38:52.4856172Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-chain.f51aa930.js:2171:26
2023-04-10T02:38:52.4857174Z     at runTest [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:381:42[90m)[39m
2023-04-10T02:38:52.4858190Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:52.4859202Z     at runSuite [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:479:15[90m)[39m
2023-04-10T02:38:52.4860207Z     at runFiles [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:614:5[90m)[39m
2023-04-10T02:38:52.4861618Z     at startTestsNode [90m(/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/chunk-runtime-setup.a06d5c72.js:632:3[90m)[39m
2023-04-10T02:38:52.4862547Z     at [90m/home/runner/work/useWallet/useWallet/[39mnode_modules/[4m.pnpm[24m/vitest@0.26.3_fgccqoxlrfh5cn2u2i6rmljy2e/node_modules/[4mvitest[24m/dist/entry.js:103:11
2023-04-10T02:38:52.4862855Z 
2023-04-10T02:38:52.6059588Z  [32m✓[39m packages/core/src/actions/signing/sign.test.ts [2m ([22m[2m3 tests[22m[2m)[22m[90m 16[2mms[22m[39m
2023-04-10T02:38:53.8062484Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:53.8063101Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:53.8063362Z 
2023-04-10T02:38:53.9926102Z  [32m✓[39m packages/core/src/actions/account/getActivePublicKey.test.ts [2m ([22m[2m3 tests[22m[2m)[22m[90m 8[2mms[22m[39m
2023-04-10T02:38:55.4687442Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:55.4687907Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:55.4688104Z 
2023-04-10T02:38:55.8746276Z  [32m✓[39m packages/react/src/hooks/useConnect.test.ts [2m ([22m[2m4 tests[22m[2m)[22m[90m 137[2mms[22m[39m
2023-04-10T02:38:57.0807049Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:57.0807865Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:57.0808486Z 
2023-04-10T02:38:57.2685185Z  [32m✓[39m packages/core/src/actions/account/isConnected.test.ts [2m ([22m[2m4 tests[22m[2m)[22m[90m 9[2mms[22m[39m
2023-04-10T02:38:58.4155555Z  [32m✓[39m packages/core/src/actions/signing/signMessage.test.ts [2m ([22m[2m3 tests[22m[2m)[22m[90m 8[2mms[22m[39m
2023-04-10T02:38:59.9373987Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:38:59.9376151Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:38:59.9376437Z 
2023-04-10T02:39:00.2775498Z  [32m✓[39m packages/react/src/hooks/useDisconnect.test.ts [2m ([22m[2m3 tests[22m[2m)[22m[90m 132[2mms[22m[39m
2023-04-10T02:39:01.4871912Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:39:01.4872682Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:39:01.4873102Z 
2023-04-10T02:39:01.6645634Z  [32m✓[39m packages/core/src/actions/account/getAccount.test.ts [2m ([22m[2m3 tests[22m[2m)[22m[90m 8[2mms[22m[39m
2023-04-10T02:39:02.8974729Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:39:02.8975479Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:39:02.8975972Z 
2023-04-10T02:39:03.0565932Z  [32m✓[39m packages/core/src/actions/account/disconnect.test.ts [2m ([22m[2m2 tests[22m[2m)[22m[90m 9[2mms[22m[39m
2023-04-10T02:39:04.2275740Z  [32m✓[39m packages/core/src/utils/deepEqual.test.ts [2m ([22m[2m9 tests[22m[2m)[22m[90m 9[2mms[22m[39m
2023-04-10T02:39:05.6125024Z  [32m✓[39m packages/react/src/hooks/useAccount.test.ts [2m ([22m[2m1 test[22m[2m)[22m[90m 19[2mms[22m[39m
2023-04-10T02:39:06.8494025Z [90mstdout[2m | unknown test[22m[39m
2023-04-10T02:39:06.8496195Z secp256k1 unavailable, reverting to browser version
2023-04-10T02:39:06.8496708Z 
2023-04-10T02:39:07.1872106Z  [32m✓[39m packages/core/src/actions/account/watchAccount.test.ts [2m ([22m[2m1 test[22m[2m)[22m[90m 6[2mms[22m[39m
2023-04-10T02:39:07.1903275Z 
2023-04-10T02:39:07.1923926Z [2m Test Files [22m [1m[32m18 passed[39m[22m[90m (18)[39m
2023-04-10T02:39:07.1926966Z [2m      Tests [22m [1m[32m137 passed[39m[22m[90m (137)[39m
2023-04-10T02:39:07.1930871Z [2m   Start at [22m 02:38:39
2023-04-10T02:39:07.1933591Z [2m   Duration [22m 27.26s[2m (transform 951ms, setup 6ms, collect 4.99s, tests 856ms)[22m
2023-04-10T02:39:07.1935076Z 
2023-04-10T02:39:07.1936783Z [34m % [39m[2mCoverage report from [22m[33mc8[39m
2023-04-10T02:39:09.9904657Z ------------------------------------|---------|----------|---------|---------|----------------------
2023-04-10T02:39:09.9906031Z File                                | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s    
2023-04-10T02:39:09.9907211Z ------------------------------------|---------|----------|---------|---------|----------------------
2023-04-10T02:39:09.9907904Z All files                           |   88.15 |    85.64 |   80.18 |   88.15 |                      
2023-04-10T02:39:09.9908690Z  core/src                           |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9909215Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9909936Z  core/src/actions/account           |   93.49 |    83.33 |      80 |   93.49 |                      
2023-04-10T02:39:09.9910646Z   connect.ts                        |   84.37 |    71.42 |     100 |   84.37 | 16-19,59-68,75       
2023-04-10T02:39:09.9911385Z   disconnect.ts                     |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9911899Z   getAccount.ts                     |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9912639Z   getActivePublicKey.ts             |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9913197Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9913911Z   isConnected.ts                    |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9914436Z   watchAccount.ts                   |    98.3 |    66.66 |      50 |    98.3 | 48                   
2023-04-10T02:39:09.9915151Z  core/src/actions/signing           |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9915926Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9916634Z   sign.ts                           |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9917166Z   signMessage.ts                    |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9917917Z  core/src/connectors                |   93.97 |    90.16 |   91.48 |   93.97 |                      
2023-04-10T02:39:09.9918570Z   base.ts                           |   68.42 |      100 |   66.66 |   68.42 | 40-57                
2023-04-10T02:39:09.9919287Z   casperDash.ts                     |     100 |       95 |     100 |     100 | 47                   
2023-04-10T02:39:09.9919940Z   casperSigner.ts                   |    97.2 |       90 |   93.33 |    97.2 | 78-79,212-215        
2023-04-10T02:39:09.9921077Z   casperWallet.ts                   |   91.91 |    84.21 |   86.66 |   91.91 | ...3,194-195,232-235 
2023-04-10T02:39:09.9921618Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9922348Z  core/src/enums                     |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9922853Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9923541Z   status.ts                         |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9924048Z  core/src/errors                    |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9924766Z   ClientNotFoundError.ts            |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9925365Z   ConnectorAlreadyConnectedError.ts |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9926138Z   ConnectorNotFoundError.ts         |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9926673Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9927568Z  core/src/utils                     |   67.57 |    72.46 |    60.6 |   67.57 |                      
2023-04-10T02:39:09.9928229Z   client.ts                         |   66.22 |    78.26 |   73.91 |   66.22 | ...9,276-278,283-288 
2023-04-10T02:39:09.9929067Z   deepEqual.ts                      |   84.09 |    63.15 |     100 |   84.09 | 16-20,25,44          
2023-04-10T02:39:09.9929591Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9930415Z   parser.ts                         |   28.57 |      100 |       0 |   28.57 | 3-7                  
2023-04-10T02:39:09.9931047Z   storage.ts                        |    65.3 |       50 |      25 |    65.3 | ...32-34,37-46,48-49 
2023-04-10T02:39:09.9931780Z  react/src                          |   82.79 |      100 |      50 |   82.79 |                      
2023-04-10T02:39:09.9932278Z   client.ts                         |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9933043Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9933682Z   provider.ts                       |   69.23 |      100 |      40 |   69.23 | 12,15-21,45-52       
2023-04-10T02:39:09.9935206Z  react/src/enums                    |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9935704Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9936201Z   mutationKeys.ts                   |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9936935Z   queryKeys.ts                      |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9937682Z  react/src/hooks                    |   93.83 |      100 |     100 |   93.83 |                      
2023-04-10T02:39:09.9938168Z   index.ts                          |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9939030Z   useAccount.ts                     |   64.61 |      100 |     100 |   64.61 | 38-60                
2023-04-10T02:39:09.9939557Z   useConnect.ts                     |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9940270Z   useDisconnect.ts                  |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9940786Z   useSign.ts                        |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9941495Z   useSignMessage.ts                 |     100 |      100 |     100 |     100 |                      
2023-04-10T02:39:09.9942289Z ------------------------------------|---------|----------|---------|---------|----------------------
2023-04-10T02:39:10.1581207Z ##[group]Run codecov/codecov-action@v3
2023-04-10T02:39:10.1581456Z with:
2023-04-10T02:39:10.1581643Z env:
2023-04-10T02:39:10.1581902Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:39:10.1582175Z ##[endgroup]
2023-04-10T02:39:10.3090279Z ==> linux OS detected
2023-04-10T02:39:10.6454110Z https://uploader.codecov.io/latest/linux/codecov.SHA256SUM
2023-04-10T02:39:10.7320045Z ==> SHASUM file signed by key id 806bb28aed779869
2023-04-10T02:39:10.9226981Z ==> Uploader SHASUM verified (32cb14b5f3aaacd67f4c1ff55d82f037d3cd10c8e7b69c051f27391d2e66e15c  codecov)
2023-04-10T02:39:10.9230474Z ==> Running version latest
2023-04-10T02:39:11.0024377Z ==> Running version v0.4.1
2023-04-10T02:39:11.0044987Z [command]/home/runner/work/_actions/codecov/codecov-action/v3/dist/codecov -n  -Q github-action-3.1.1
2023-04-10T02:39:11.2204145Z [2023-04-10T02:39:11.218Z] ['info'] 
2023-04-10T02:39:11.2208056Z      _____          _
2023-04-10T02:39:11.2208854Z     / ____|        | |
2023-04-10T02:39:11.2209285Z    | |     ___   __| | ___  ___ _____   __
2023-04-10T02:39:11.2209889Z    | |    / _ \ / _` |/ _ \/ __/ _ \ \ / /
2023-04-10T02:39:11.2210307Z    | |___| (_) | (_| |  __/ (_| (_) \ V /
2023-04-10T02:39:11.2210915Z     \_____\___/ \__,_|\___|\___\___/ \_/
2023-04-10T02:39:11.2211211Z 
2023-04-10T02:39:11.2211689Z   Codecov report uploader 0.4.1
2023-04-10T02:39:11.2267834Z [2023-04-10T02:39:11.226Z] ['info'] => Project root located at: /home/runner/work/useWallet/useWallet
2023-04-10T02:39:11.2281124Z [2023-04-10T02:39:11.227Z] ['info'] -> No token specified or token is empty
2023-04-10T02:39:11.2357723Z [2023-04-10T02:39:11.235Z] ['info'] Searching for coverage files...
2023-04-10T02:39:11.3411539Z [2023-04-10T02:39:11.340Z] ['info'] Warning: Some files located via search were excluded from upload.
2023-04-10T02:39:11.3420898Z [2023-04-10T02:39:11.341Z] ['info'] If Codecov did not locate your files, please review https://docs.codecov.com/docs/supported-report-formats
2023-04-10T02:39:11.3428288Z [2023-04-10T02:39:11.342Z] ['info'] => Found 2 possible coverage files:
2023-04-10T02:39:11.3429050Z   coverage/coverage-final.json
2023-04-10T02:39:11.3430144Z   coverage/tmp/coverage-1802-1681094350098-19.json
2023-04-10T02:39:11.3434332Z [2023-04-10T02:39:11.343Z] ['info'] Processing /home/runner/work/useWallet/useWallet/coverage/coverage-final.json...
2023-04-10T02:39:11.3460897Z [2023-04-10T02:39:11.345Z] ['info'] Processing /home/runner/work/useWallet/useWallet/coverage/tmp/coverage-1802-1681094350098-19.json...
2023-04-10T02:39:11.4555031Z [2023-04-10T02:39:11.454Z] ['info'] Detected GitHub Actions as the CI provider.
2023-04-10T02:39:11.7607595Z [2023-04-10T02:39:11.759Z] ['info'] Pinging Codecov: https://codecov.io/upload/v4?package=github-action-3.1.1-uploader-0.4.1&token=*******&branch=main&build=4653946868&build_url=https%3A%2F%2Fgithub.com%2FCasperDash%2FuseWallet%2Factions%2Fruns%2F4653946868&commit=25f8ac7a84341a7485ddf7707522bda42d38972c&job=Main&pr=&service=github-actions&slug=CasperDash%2FuseWallet&name=&tag=&flags=&parent=
2023-04-10T02:39:12.0432184Z [2023-04-10T02:39:12.042Z] ['error'] There was an error running the uploader: Error uploading to https://codecov.io: Error: There was an error fetching the storage URL during POST: 404 - {'detail': ErrorDetail(string='Could not find a repository, try using repo upload token', code='not_found')}
2023-04-10T02:39:12.1519028Z Post job cleanup.
2023-04-10T02:39:12.2956165Z Cache hit occurred on the primary key modules-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8, not saving cache.
2023-04-10T02:39:12.3051255Z Post job cleanup.
2023-04-10T02:39:12.4735430Z Post job cleanup.
2023-04-10T02:39:12.5897212Z Pruning is unnecessary.
2023-04-10T02:39:12.6006178Z Post job cleanup.
2023-04-10T02:39:12.7385591Z [command]/usr/bin/git version
2023-04-10T02:39:12.7435266Z git version 2.40.0
2023-04-10T02:39:12.7483307Z Temporarily overriding HOME='/home/runner/work/_temp/ac0333d0-fbc2-4455-a9ac-b8d3329b7d21' before making global git config changes
2023-04-10T02:39:12.7484288Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:39:12.7489892Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:39:12.7535523Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:39:12.7574681Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:39:12.7865441Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:39:12.7897667Z http.https://github.com/.extraheader
2023-04-10T02:39:12.7910595Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2023-04-10T02:39:12.7950104Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:39:12.8381352Z Cleaning up orphan processes
```