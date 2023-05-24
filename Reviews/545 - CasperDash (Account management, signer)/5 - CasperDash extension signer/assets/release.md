# Release Workflow Logs

```sh
2023-04-10T02:36:37.6145764Z Requested labels: ubuntu-latest
2023-04-10T02:36:37.6145815Z Job defined at: CasperDash/useWallet/.github/workflows/release.yml@refs/heads/main
2023-04-10T02:36:37.6145846Z Waiting for a runner to pick up this job...
2023-04-10T02:36:38.2278899Z Job is waiting for a hosted runner to come online.
2023-04-10T02:36:41.7934226Z Job is about to start running on the hosted runner: GitHub Actions 2 (hosted)
2023-04-10T02:36:44.0735975Z Current runner version: '2.303.0'
2023-04-10T02:36:44.0766237Z ##[group]Operating System
2023-04-10T02:36:44.0766910Z Ubuntu
2023-04-10T02:36:44.0767292Z 22.04.2
2023-04-10T02:36:44.0767586Z LTS
2023-04-10T02:36:44.0768051Z ##[endgroup]
2023-04-10T02:36:44.0768462Z ##[group]Runner Image
2023-04-10T02:36:44.0768896Z Image: ubuntu-22.04
2023-04-10T02:36:44.0769243Z Version: 20230402.1
2023-04-10T02:36:44.0769905Z Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20230402.1/images/linux/Ubuntu2204-Readme.md
2023-04-10T02:36:44.0770699Z Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20230402.1
2023-04-10T02:36:44.0771260Z ##[endgroup]
2023-04-10T02:36:44.0771632Z ##[group]Runner Image Provisioner
2023-04-10T02:36:44.0772046Z 2.0.139.1
2023-04-10T02:36:44.0772445Z ##[endgroup]
2023-04-10T02:36:44.0773911Z ##[group]GITHUB_TOKEN Permissions
2023-04-10T02:36:44.0774696Z Actions: write
2023-04-10T02:36:44.0775037Z Checks: write
2023-04-10T02:36:44.0775818Z Contents: write
2023-04-10T02:36:44.0776313Z Deployments: write
2023-04-10T02:36:44.0776738Z Discussions: write
2023-04-10T02:36:44.0777149Z Issues: write
2023-04-10T02:36:44.0777533Z Metadata: read
2023-04-10T02:36:44.0777868Z Packages: write
2023-04-10T02:36:44.0778252Z Pages: write
2023-04-10T02:36:44.0778693Z PullRequests: write
2023-04-10T02:36:44.0779127Z RepositoryProjects: write
2023-04-10T02:36:44.0779518Z SecurityEvents: write
2023-04-10T02:36:44.0779931Z Statuses: write
2023-04-10T02:36:44.0780360Z ##[endgroup]
2023-04-10T02:36:44.0784616Z Secret source: Actions
2023-04-10T02:36:44.0785168Z Prepare workflow directory
2023-04-10T02:36:44.1740247Z Prepare all required actions
2023-04-10T02:36:44.1958377Z Getting action download info
2023-04-10T02:36:44.4431929Z Download action repository 'actions/checkout@v3' (SHA:8f4b7f84864484a7bf31766abe9204da3cbe65b3)
2023-04-10T02:36:45.1362996Z Download action repository 'pnpm/action-setup@v2.2.4' (SHA:c3b53f6a16e57305370b4ae5a540c2077a1d50dd)
2023-04-10T02:36:45.8112056Z Download action repository 'actions/setup-node@v3' (SHA:64ed1c7eab4cce3362f8c340dee64e5eaeef8f7c)
2023-04-10T02:36:46.5137284Z Download action repository 'changesets/action@v1.4.1' (SHA:e9cc34b540dd3ad1b030c57fd97269e8f6ad905a)
2023-04-10T02:36:47.2796254Z Complete job name: release (18, 7.26.3)
2023-04-10T02:36:47.3768220Z ##[group]Run actions/checkout@v3
2023-04-10T02:36:47.3768574Z with:
2023-04-10T02:36:47.3768826Z   fetch-depth: 0
2023-04-10T02:36:47.3769114Z   repository: CasperDash/useWallet
2023-04-10T02:36:47.3769645Z   token: ***
2023-04-10T02:36:47.3769897Z   ssh-strict: true
2023-04-10T02:36:47.3770174Z   persist-credentials: true
2023-04-10T02:36:47.3770454Z   clean: true
2023-04-10T02:36:47.3770671Z   lfs: false
2023-04-10T02:36:47.3770921Z   submodules: false
2023-04-10T02:36:47.3771190Z   set-safe-directory: true
2023-04-10T02:36:47.3771465Z ##[endgroup]
2023-04-10T02:36:47.7662316Z Syncing repository: CasperDash/useWallet
2023-04-10T02:36:47.7664692Z ##[group]Getting Git version info
2023-04-10T02:36:47.7665355Z Working directory is '/home/runner/work/useWallet/useWallet'
2023-04-10T02:36:47.7665995Z [command]/usr/bin/git version
2023-04-10T02:36:47.7820893Z git version 2.40.0
2023-04-10T02:36:47.7855914Z ##[endgroup]
2023-04-10T02:36:47.7876446Z Temporarily overriding HOME='/home/runner/work/_temp/34d42812-cc59-4be9-8ab1-429a397f1643' before making global git config changes
2023-04-10T02:36:47.7877034Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:36:47.7880242Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:36:47.7943812Z Deleting the contents of '/home/runner/work/useWallet/useWallet'
2023-04-10T02:36:47.7950321Z ##[group]Initializing the repository
2023-04-10T02:36:47.7954808Z [command]/usr/bin/git init /home/runner/work/useWallet/useWallet
2023-04-10T02:36:47.8044704Z hint: Using 'master' as the name for the initial branch. This default branch name
2023-04-10T02:36:47.8046067Z hint: is subject to change. To configure the initial branch name to use in all
2023-04-10T02:36:47.8047304Z hint: of your new repositories, which will suppress this warning, call:
2023-04-10T02:36:47.8047862Z hint: 
2023-04-10T02:36:47.8048779Z hint: 	git config --global init.defaultBranch <name>
2023-04-10T02:36:47.8049295Z hint: 
2023-04-10T02:36:47.8050161Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2023-04-10T02:36:47.8050917Z hint: 'development'. The just-created branch can be renamed via this command:
2023-04-10T02:36:47.8051702Z hint: 
2023-04-10T02:36:47.8052364Z hint: 	git branch -m <name>
2023-04-10T02:36:47.8059129Z Initialized empty Git repository in /home/runner/work/useWallet/useWallet/.git/
2023-04-10T02:36:47.8070264Z [command]/usr/bin/git remote add origin https://github.com/CasperDash/useWallet
2023-04-10T02:36:47.8123934Z ##[endgroup]
2023-04-10T02:36:47.8124708Z ##[group]Disabling automatic garbage collection
2023-04-10T02:36:47.8127804Z [command]/usr/bin/git config --local gc.auto 0
2023-04-10T02:36:47.8166288Z ##[endgroup]
2023-04-10T02:36:47.8166987Z ##[group]Setting up auth
2023-04-10T02:36:47.8174734Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:36:47.8215181Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:36:47.8675096Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:36:47.8704908Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:36:47.8999076Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2023-04-10T02:36:47.9036851Z ##[endgroup]
2023-04-10T02:36:47.9037558Z ##[group]Fetching the repository
2023-04-10T02:36:47.9051388Z [command]/usr/bin/git -c protocol.version=2 fetch --prune --progress --no-recurse-submodules origin +refs/heads/*:refs/remotes/origin/* +refs/tags/*:refs/tags/*
2023-04-10T02:36:48.3313668Z remote: Enumerating objects: 1571, done.        
2023-04-10T02:36:48.3314489Z remote: Counting objects:   0% (1/504)        
2023-04-10T02:36:48.3315022Z remote: Counting objects:   1% (6/504)        
2023-04-10T02:36:48.3320088Z remote: Counting objects:   2% (11/504)        
2023-04-10T02:36:48.3320988Z remote: Counting objects:   3% (16/504)        
2023-04-10T02:36:48.3321651Z remote: Counting objects:   4% (21/504)        
2023-04-10T02:36:48.3322297Z remote: Counting objects:   5% (26/504)        
2023-04-10T02:36:48.3322964Z remote: Counting objects:   6% (31/504)        
2023-04-10T02:36:48.3323603Z remote: Counting objects:   7% (36/504)        
2023-04-10T02:36:48.3324238Z remote: Counting objects:   8% (41/504)        
2023-04-10T02:36:48.3325235Z remote: Counting objects:   9% (46/504)        
2023-04-10T02:36:48.3325893Z remote: Counting objects:  10% (51/504)        
2023-04-10T02:36:48.3326513Z remote: Counting objects:  11% (56/504)        
2023-04-10T02:36:48.3327226Z remote: Counting objects:  12% (61/504)        
2023-04-10T02:36:48.3327970Z remote: Counting objects:  13% (66/504)        
2023-04-10T02:36:48.3328900Z remote: Counting objects:  14% (71/504)        
2023-04-10T02:36:48.3329774Z remote: Counting objects:  15% (76/504)        
2023-04-10T02:36:48.3330358Z remote: Counting objects:  16% (81/504)        
2023-04-10T02:36:48.3330996Z remote: Counting objects:  17% (86/504)        
2023-04-10T02:36:48.3331618Z remote: Counting objects:  18% (91/504)        
2023-04-10T02:36:48.3332056Z remote: Counting objects:  19% (96/504)        
2023-04-10T02:36:48.3332742Z remote: Counting objects:  20% (101/504)        
2023-04-10T02:36:48.3338364Z remote: Counting objects:  21% (106/504)        
2023-04-10T02:36:48.3338729Z remote: Counting objects:  22% (111/504)        
2023-04-10T02:36:48.3339325Z remote: Counting objects:  23% (116/504)        
2023-04-10T02:36:48.3339648Z remote: Counting objects:  24% (121/504)        
2023-04-10T02:36:48.3339970Z remote: Counting objects:  25% (126/504)        
2023-04-10T02:36:48.3340304Z remote: Counting objects:  26% (132/504)        
2023-04-10T02:36:48.3340609Z remote: Counting objects:  27% (137/504)        
2023-04-10T02:36:48.3340937Z remote: Counting objects:  28% (142/504)        
2023-04-10T02:36:48.3341309Z remote: Counting objects:  29% (147/504)        
2023-04-10T02:36:48.3341629Z remote: Counting objects:  30% (152/504)        
2023-04-10T02:36:48.3341934Z remote: Counting objects:  31% (157/504)        
2023-04-10T02:36:48.3342251Z remote: Counting objects:  32% (162/504)        
2023-04-10T02:36:48.3342566Z remote: Counting objects:  33% (167/504)        
2023-04-10T02:36:48.3342886Z remote: Counting objects:  34% (172/504)        
2023-04-10T02:36:48.3343184Z remote: Counting objects:  35% (177/504)        
2023-04-10T02:36:48.3343503Z remote: Counting objects:  36% (182/504)        
2023-04-10T02:36:48.3343815Z remote: Counting objects:  37% (187/504)        
2023-04-10T02:36:48.3344128Z remote: Counting objects:  38% (192/504)        
2023-04-10T02:36:48.3344431Z remote: Counting objects:  39% (197/504)        
2023-04-10T02:36:48.3344741Z remote: Counting objects:  40% (202/504)        
2023-04-10T02:36:48.3345051Z remote: Counting objects:  41% (207/504)        
2023-04-10T02:36:48.3345365Z remote: Counting objects:  42% (212/504)        
2023-04-10T02:36:48.3345661Z remote: Counting objects:  43% (217/504)        
2023-04-10T02:36:48.3345975Z remote: Counting objects:  44% (222/504)        
2023-04-10T02:36:48.3346285Z remote: Counting objects:  45% (227/504)        
2023-04-10T02:36:48.3346597Z remote: Counting objects:  46% (232/504)        
2023-04-10T02:36:48.3346893Z remote: Counting objects:  47% (237/504)        
2023-04-10T02:36:48.3347204Z remote: Counting objects:  48% (242/504)        
2023-04-10T02:36:48.3347516Z remote: Counting objects:  49% (247/504)        
2023-04-10T02:36:48.3347825Z remote: Counting objects:  50% (252/504)        
2023-04-10T02:36:48.3348135Z remote: Counting objects:  51% (258/504)        
2023-04-10T02:36:48.3348585Z remote: Counting objects:  52% (263/504)        
2023-04-10T02:36:48.3348904Z remote: Counting objects:  53% (268/504)        
2023-04-10T02:36:48.3349215Z remote: Counting objects:  54% (273/504)        
2023-04-10T02:36:48.3349534Z remote: Counting objects:  55% (278/504)        
2023-04-10T02:36:48.3349833Z remote: Counting objects:  56% (283/504)        
2023-04-10T02:36:48.3350145Z remote: Counting objects:  57% (288/504)        
2023-04-10T02:36:48.3350459Z remote: Counting objects:  58% (293/504)        
2023-04-10T02:36:48.3350773Z remote: Counting objects:  59% (298/504)        
2023-04-10T02:36:48.3351072Z remote: Counting objects:  60% (303/504)        
2023-04-10T02:36:48.3351385Z remote: Counting objects:  61% (308/504)        
2023-04-10T02:36:48.3351703Z remote: Counting objects:  62% (313/504)        
2023-04-10T02:36:48.3352016Z remote: Counting objects:  63% (318/504)        
2023-04-10T02:36:48.3352310Z remote: Counting objects:  64% (323/504)        
2023-04-10T02:36:48.3352632Z remote: Counting objects:  65% (328/504)        
2023-04-10T02:36:48.3352942Z remote: Counting objects:  66% (333/504)        
2023-04-10T02:36:48.3353269Z remote: Counting objects:  67% (338/504)        
2023-04-10T02:36:48.3353581Z remote: Counting objects:  68% (343/504)        
2023-04-10T02:36:48.3353874Z remote: Counting objects:  69% (348/504)        
2023-04-10T02:36:48.3354183Z remote: Counting objects:  70% (353/504)        
2023-04-10T02:36:48.3354493Z remote: Counting objects:  71% (358/504)        
2023-04-10T02:36:48.3354805Z remote: Counting objects:  72% (363/504)        
2023-04-10T02:36:48.3355105Z remote: Counting objects:  73% (368/504)        
2023-04-10T02:36:48.3355417Z remote: Counting objects:  74% (373/504)        
2023-04-10T02:36:48.3355880Z remote: Counting objects:  75% (378/504)        
2023-04-10T02:36:48.3356194Z remote: Counting objects:  76% (384/504)        
2023-04-10T02:36:48.3356495Z remote: Counting objects:  77% (389/504)        
2023-04-10T02:36:48.3356814Z remote: Counting objects:  78% (394/504)        
2023-04-10T02:36:48.3357128Z remote: Counting objects:  79% (399/504)        
2023-04-10T02:36:48.3357442Z remote: Counting objects:  80% (404/504)        
2023-04-10T02:36:48.3357742Z remote: Counting objects:  81% (409/504)        
2023-04-10T02:36:48.3358058Z remote: Counting objects:  82% (414/504)        
2023-04-10T02:36:48.3358372Z remote: Counting objects:  83% (419/504)        
2023-04-10T02:36:48.3358687Z remote: Counting objects:  84% (424/504)        
2023-04-10T02:36:48.3359004Z remote: Counting objects:  85% (429/504)        
2023-04-10T02:36:48.3359306Z remote: Counting objects:  86% (434/504)        
2023-04-10T02:36:48.3359621Z remote: Counting objects:  87% (439/504)        
2023-04-10T02:36:48.3359941Z remote: Counting objects:  88% (444/504)        
2023-04-10T02:36:48.3360251Z remote: Counting objects:  89% (449/504)        
2023-04-10T02:36:48.3360552Z remote: Counting objects:  90% (454/504)        
2023-04-10T02:36:48.3360862Z remote: Counting objects:  91% (459/504)        
2023-04-10T02:36:48.3361183Z remote: Counting objects:  92% (464/504)        
2023-04-10T02:36:48.3361497Z remote: Counting objects:  93% (469/504)        
2023-04-10T02:36:48.3361795Z remote: Counting objects:  94% (474/504)        
2023-04-10T02:36:48.3362105Z remote: Counting objects:  95% (479/504)        
2023-04-10T02:36:48.3362415Z remote: Counting objects:  96% (484/504)        
2023-04-10T02:36:48.3362728Z remote: Counting objects:  97% (489/504)        
2023-04-10T02:36:48.3363023Z remote: Counting objects:  98% (494/504)        
2023-04-10T02:36:48.3363331Z remote: Counting objects:  99% (499/504)        
2023-04-10T02:36:48.3363639Z remote: Counting objects: 100% (504/504)        
2023-04-10T02:36:48.3363976Z remote: Counting objects: 100% (504/504), done.        
2023-04-10T02:36:48.3364317Z remote: Compressing objects:   0% (1/292)        
2023-04-10T02:36:48.3364656Z remote: Compressing objects:   1% (3/292)        
2023-04-10T02:36:48.3365033Z remote: Compressing objects:   2% (6/292)        
2023-04-10T02:36:48.3365884Z remote: Compressing objects:   3% (9/292)        
2023-04-10T02:36:48.3366828Z remote: Compressing objects:   4% (12/292)        
2023-04-10T02:36:48.3367172Z remote: Compressing objects:   5% (15/292)        
2023-04-10T02:36:48.3367604Z remote: Compressing objects:   6% (18/292)        
2023-04-10T02:36:48.3368839Z remote: Compressing objects:   7% (21/292)        
2023-04-10T02:36:48.3369341Z remote: Compressing objects:   8% (24/292)        
2023-04-10T02:36:48.3369931Z remote: Compressing objects:   9% (27/292)        
2023-04-10T02:36:48.3370697Z remote: Compressing objects:  10% (30/292)        
2023-04-10T02:36:48.3371217Z remote: Compressing objects:  11% (33/292)        
2023-04-10T02:36:48.3371650Z remote: Compressing objects:  12% (36/292)        
2023-04-10T02:36:48.3372249Z remote: Compressing objects:  13% (38/292)        
2023-04-10T02:36:48.3372920Z remote: Compressing objects:  14% (41/292)        
2023-04-10T02:36:48.3373607Z remote: Compressing objects:  15% (44/292)        
2023-04-10T02:36:48.3374150Z remote: Compressing objects:  16% (47/292)        
2023-04-10T02:36:48.3374956Z remote: Compressing objects:  17% (50/292)        
2023-04-10T02:36:48.3375662Z remote: Compressing objects:  18% (53/292)        
2023-04-10T02:36:48.3376353Z remote: Compressing objects:  19% (56/292)        
2023-04-10T02:36:48.3377312Z remote: Compressing objects:  20% (59/292)        
2023-04-10T02:36:48.3377959Z remote: Compressing objects:  21% (62/292)        
2023-04-10T02:36:48.3378633Z remote: Compressing objects:  22% (65/292)        
2023-04-10T02:36:48.3379292Z remote: Compressing objects:  23% (68/292)        
2023-04-10T02:36:48.3379935Z remote: Compressing objects:  24% (71/292)        
2023-04-10T02:36:48.3380657Z remote: Compressing objects:  25% (73/292)        
2023-04-10T02:36:48.3381292Z remote: Compressing objects:  26% (76/292)        
2023-04-10T02:36:48.3382047Z remote: Compressing objects:  27% (79/292)        
2023-04-10T02:36:48.3382775Z remote: Compressing objects:  28% (82/292)        
2023-04-10T02:36:48.3383414Z remote: Compressing objects:  29% (85/292)        
2023-04-10T02:36:48.3384119Z remote: Compressing objects:  30% (88/292)        
2023-04-10T02:36:48.3384789Z remote: Compressing objects:  31% (91/292)        
2023-04-10T02:36:48.3385428Z remote: Compressing objects:  32% (94/292)        
2023-04-10T02:36:48.3386094Z remote: Compressing objects:  33% (97/292)        
2023-04-10T02:36:48.3386827Z remote: Compressing objects:  34% (100/292)        
2023-04-10T02:36:48.3387483Z remote: Compressing objects:  35% (103/292)        
2023-04-10T02:36:48.3388111Z remote: Compressing objects:  36% (106/292)        
2023-04-10T02:36:48.3388750Z remote: Compressing objects:  37% (109/292)        
2023-04-10T02:36:48.3389410Z remote: Compressing objects:  38% (111/292)        
2023-04-10T02:36:48.3390074Z remote: Compressing objects:  39% (114/292)        
2023-04-10T02:36:48.3390770Z remote: Compressing objects:  40% (117/292)        
2023-04-10T02:36:48.3441299Z remote: Compressing objects:  41% (120/292)        
2023-04-10T02:36:48.3441683Z remote: Compressing objects:  42% (123/292)        
2023-04-10T02:36:48.3442032Z remote: Compressing objects:  43% (126/292)        
2023-04-10T02:36:48.3442372Z remote: Compressing objects:  44% (129/292)        
2023-04-10T02:36:48.3442690Z remote: Compressing objects:  45% (132/292)        
2023-04-10T02:36:48.3443031Z remote: Compressing objects:  46% (135/292)        
2023-04-10T02:36:48.3443368Z remote: Compressing objects:  47% (138/292)        
2023-04-10T02:36:48.3443702Z remote: Compressing objects:  48% (141/292)        
2023-04-10T02:36:48.3444018Z remote: Compressing objects:  49% (144/292)        
2023-04-10T02:36:48.3444358Z remote: Compressing objects:  50% (146/292)        
2023-04-10T02:36:48.3444689Z remote: Compressing objects:  51% (149/292)        
2023-04-10T02:36:48.3445018Z remote: Compressing objects:  52% (152/292)        
2023-04-10T02:36:48.3445329Z remote: Compressing objects:  53% (155/292)        
2023-04-10T02:36:48.3445921Z remote: Compressing objects:  54% (158/292)        
2023-04-10T02:36:48.3446264Z remote: Compressing objects:  55% (161/292)        
2023-04-10T02:36:48.3446599Z remote: Compressing objects:  56% (164/292)        
2023-04-10T02:36:48.3446914Z remote: Compressing objects:  57% (167/292)        
2023-04-10T02:36:48.3447244Z remote: Compressing objects:  58% (170/292)        
2023-04-10T02:36:48.3447572Z remote: Compressing objects:  59% (173/292)        
2023-04-10T02:36:48.3447902Z remote: Compressing objects:  60% (176/292)        
2023-04-10T02:36:48.3448214Z remote: Compressing objects:  61% (179/292)        
2023-04-10T02:36:48.3448540Z remote: Compressing objects:  62% (182/292)        
2023-04-10T02:36:48.3448879Z remote: Compressing objects:  63% (184/292)        
2023-04-10T02:36:48.3449207Z remote: Compressing objects:  64% (187/292)        
2023-04-10T02:36:48.3449540Z remote: Compressing objects:  65% (190/292)        
2023-04-10T02:36:48.3449857Z remote: Compressing objects:  66% (193/292)        
2023-04-10T02:36:48.3450181Z remote: Compressing objects:  67% (196/292)        
2023-04-10T02:36:48.3450507Z remote: Compressing objects:  68% (199/292)        
2023-04-10T02:36:48.3450828Z remote: Compressing objects:  69% (202/292)        
2023-04-10T02:36:48.3451138Z remote: Compressing objects:  70% (205/292)        
2023-04-10T02:36:48.3451464Z remote: Compressing objects:  71% (208/292)        
2023-04-10T02:36:48.3451788Z remote: Compressing objects:  72% (211/292)        
2023-04-10T02:36:48.3452114Z remote: Compressing objects:  73% (214/292)        
2023-04-10T02:36:48.3452425Z remote: Compressing objects:  74% (217/292)        
2023-04-10T02:36:48.3452947Z remote: Compressing objects:  75% (219/292)        
2023-04-10T02:36:48.3453433Z remote: Compressing objects:  76% (222/292)        
2023-04-10T02:36:48.3453762Z remote: Compressing objects:  77% (225/292)        
2023-04-10T02:36:48.3454070Z remote: Compressing objects:  78% (228/292)        
2023-04-10T02:36:48.3454406Z remote: Compressing objects:  79% (231/292)        
2023-04-10T02:36:48.3454736Z remote: Compressing objects:  80% (234/292)        
2023-04-10T02:36:48.3455063Z remote: Compressing objects:  81% (237/292)        
2023-04-10T02:36:48.3455376Z remote: Compressing objects:  82% (240/292)        
2023-04-10T02:36:48.3455701Z remote: Compressing objects:  83% (243/292)        
2023-04-10T02:36:48.3456027Z remote: Compressing objects:  84% (246/292)        
2023-04-10T02:36:48.3456350Z remote: Compressing objects:  85% (249/292)        
2023-04-10T02:36:48.3456660Z remote: Compressing objects:  86% (252/292)        
2023-04-10T02:36:48.3456983Z remote: Compressing objects:  87% (255/292)        
2023-04-10T02:36:48.3457316Z remote: Compressing objects:  88% (257/292)        
2023-04-10T02:36:48.3457644Z remote: Compressing objects:  89% (260/292)        
2023-04-10T02:36:48.3457955Z remote: Compressing objects:  90% (263/292)        
2023-04-10T02:36:48.3458292Z remote: Compressing objects:  91% (266/292)        
2023-04-10T02:36:48.3458614Z remote: Compressing objects:  92% (269/292)        
2023-04-10T02:36:48.3458970Z remote: Compressing objects:  93% (272/292)        
2023-04-10T02:36:48.3459291Z remote: Compressing objects:  94% (275/292)        
2023-04-10T02:36:48.3459617Z remote: Compressing objects:  95% (278/292)        
2023-04-10T02:36:48.3459937Z remote: Compressing objects:  96% (281/292)        
2023-04-10T02:36:48.3460248Z remote: Compressing objects:  97% (284/292)        
2023-04-10T02:36:48.3468609Z remote: Compressing objects:  98% (287/292)        
2023-04-10T02:36:48.3469162Z remote: Compressing objects:  99% (290/292)        
2023-04-10T02:36:48.3469902Z remote: Compressing objects: 100% (292/292)        
2023-04-10T02:36:48.3470547Z remote: Compressing objects: 100% (292/292), done.        
2023-04-10T02:36:48.3593914Z Receiving objects:   0% (1/1571)
2023-04-10T02:36:48.3596216Z Receiving objects:   1% (16/1571)
2023-04-10T02:36:48.3598274Z Receiving objects:   2% (32/1571)
2023-04-10T02:36:48.3601596Z Receiving objects:   3% (48/1571)
2023-04-10T02:36:48.3604796Z Receiving objects:   4% (63/1571)
2023-04-10T02:36:48.3657607Z Receiving objects:   5% (79/1571)
2023-04-10T02:36:48.3659975Z Receiving objects:   6% (95/1571)
2023-04-10T02:36:48.3862742Z Receiving objects:   7% (110/1571)
2023-04-10T02:36:48.3863445Z Receiving objects:   8% (126/1571)
2023-04-10T02:36:48.3864136Z Receiving objects:   9% (142/1571)
2023-04-10T02:36:48.3864729Z Receiving objects:  10% (158/1571)
2023-04-10T02:36:48.3878182Z Receiving objects:  11% (173/1571)
2023-04-10T02:36:48.3878611Z Receiving objects:  12% (189/1571)
2023-04-10T02:36:48.3879817Z Receiving objects:  13% (205/1571)
2023-04-10T02:36:48.3882272Z Receiving objects:  14% (220/1571)
2023-04-10T02:36:48.3883882Z Receiving objects:  15% (236/1571)
2023-04-10T02:36:48.3887189Z Receiving objects:  16% (252/1571)
2023-04-10T02:36:48.3887850Z Receiving objects:  17% (268/1571)
2023-04-10T02:36:48.3888490Z Receiving objects:  18% (283/1571)
2023-04-10T02:36:48.3889478Z Receiving objects:  19% (299/1571)
2023-04-10T02:36:48.3891609Z Receiving objects:  20% (315/1571)
2023-04-10T02:36:48.3891887Z Receiving objects:  21% (330/1571)
2023-04-10T02:36:48.3896211Z Receiving objects:  22% (346/1571)
2023-04-10T02:36:48.3896896Z Receiving objects:  23% (362/1571)
2023-04-10T02:36:48.3897196Z Receiving objects:  24% (378/1571)
2023-04-10T02:36:48.3897478Z Receiving objects:  25% (393/1571)
2023-04-10T02:36:48.3897750Z Receiving objects:  26% (409/1571)
2023-04-10T02:36:48.3898036Z Receiving objects:  27% (425/1571)
2023-04-10T02:36:48.3898669Z Receiving objects:  28% (440/1571)
2023-04-10T02:36:48.3899635Z Receiving objects:  29% (456/1571)
2023-04-10T02:36:48.3977565Z Receiving objects:  30% (472/1571)
2023-04-10T02:36:48.4924803Z Receiving objects:  31% (488/1571)
2023-04-10T02:36:48.4926848Z Receiving objects:  32% (503/1571)
2023-04-10T02:36:48.4938041Z Receiving objects:  33% (519/1571)
2023-04-10T02:36:48.4951183Z Receiving objects:  34% (535/1571)
2023-04-10T02:36:48.4953713Z Receiving objects:  35% (550/1571)
2023-04-10T02:36:48.4954910Z Receiving objects:  36% (566/1571)
2023-04-10T02:36:48.4956816Z Receiving objects:  37% (582/1571)
2023-04-10T02:36:48.4959406Z Receiving objects:  38% (597/1571)
2023-04-10T02:36:48.4959969Z Receiving objects:  39% (613/1571)
2023-04-10T02:36:48.4960669Z Receiving objects:  40% (629/1571)
2023-04-10T02:36:48.4962116Z Receiving objects:  41% (645/1571)
2023-04-10T02:36:48.4964077Z Receiving objects:  42% (660/1571)
2023-04-10T02:36:48.4964623Z Receiving objects:  43% (676/1571)
2023-04-10T02:36:48.4967706Z Receiving objects:  44% (692/1571)
2023-04-10T02:36:48.4968856Z Receiving objects:  45% (707/1571)
2023-04-10T02:36:48.4971018Z Receiving objects:  46% (723/1571)
2023-04-10T02:36:48.4973302Z Receiving objects:  47% (739/1571)
2023-04-10T02:36:48.4974537Z Receiving objects:  48% (755/1571)
2023-04-10T02:36:48.4975631Z Receiving objects:  49% (770/1571)
2023-04-10T02:36:48.4977332Z Receiving objects:  50% (786/1571)
2023-04-10T02:36:48.4978902Z Receiving objects:  51% (802/1571)
2023-04-10T02:36:48.5083522Z Receiving objects:  52% (817/1571)
2023-04-10T02:36:48.5085761Z Receiving objects:  53% (833/1571)
2023-04-10T02:36:48.5086357Z Receiving objects:  54% (849/1571)
2023-04-10T02:36:48.5087096Z Receiving objects:  55% (865/1571)
2023-04-10T02:36:48.5087457Z Receiving objects:  56% (880/1571)
2023-04-10T02:36:48.5087749Z Receiving objects:  57% (896/1571)
2023-04-10T02:36:48.5091395Z Receiving objects:  58% (912/1571)
2023-04-10T02:36:48.5091978Z Receiving objects:  59% (927/1571)
2023-04-10T02:36:48.5092473Z Receiving objects:  60% (943/1571)
2023-04-10T02:36:48.5092946Z Receiving objects:  61% (959/1571)
2023-04-10T02:36:48.5098089Z Receiving objects:  62% (975/1571)
2023-04-10T02:36:48.5215853Z Receiving objects:  63% (990/1571)
2023-04-10T02:36:48.5284244Z Receiving objects:  64% (1006/1571)
2023-04-10T02:36:48.5313698Z Receiving objects:  65% (1022/1571)
2023-04-10T02:36:48.5315827Z Receiving objects:  66% (1037/1571)
2023-04-10T02:36:48.5318453Z Receiving objects:  67% (1053/1571)
2023-04-10T02:36:48.5319159Z Receiving objects:  68% (1069/1571)
2023-04-10T02:36:48.5322129Z Receiving objects:  69% (1084/1571)
2023-04-10T02:36:48.5322690Z Receiving objects:  70% (1100/1571)
2023-04-10T02:36:48.5326493Z Receiving objects:  71% (1116/1571)
2023-04-10T02:36:48.5327029Z Receiving objects:  72% (1132/1571)
2023-04-10T02:36:48.5331069Z Receiving objects:  73% (1147/1571)
2023-04-10T02:36:48.5331543Z Receiving objects:  74% (1163/1571)
2023-04-10T02:36:48.5390077Z Receiving objects:  75% (1179/1571)
2023-04-10T02:36:48.5390398Z Receiving objects:  76% (1194/1571)
2023-04-10T02:36:48.5390679Z Receiving objects:  77% (1210/1571)
2023-04-10T02:36:48.5390992Z Receiving objects:  78% (1226/1571)
2023-04-10T02:36:48.5391279Z Receiving objects:  79% (1242/1571)
2023-04-10T02:36:48.5391563Z Receiving objects:  80% (1257/1571)
2023-04-10T02:36:48.5391831Z Receiving objects:  81% (1273/1571)
2023-04-10T02:36:48.5392121Z Receiving objects:  82% (1289/1571)
2023-04-10T02:36:48.5392423Z Receiving objects:  83% (1304/1571)
2023-04-10T02:36:48.5392699Z Receiving objects:  84% (1320/1571)
2023-04-10T02:36:48.5393214Z Receiving objects:  85% (1336/1571)
2023-04-10T02:36:48.5393578Z Receiving objects:  86% (1352/1571)
2023-04-10T02:36:48.5393950Z Receiving objects:  87% (1367/1571)
2023-04-10T02:36:48.5394259Z Receiving objects:  88% (1383/1571)
2023-04-10T02:36:48.5394679Z Receiving objects:  89% (1399/1571)
2023-04-10T02:36:48.5395044Z Receiving objects:  90% (1414/1571)
2023-04-10T02:36:48.5395351Z Receiving objects:  91% (1430/1571)
2023-04-10T02:36:48.5395716Z Receiving objects:  92% (1446/1571)
2023-04-10T02:36:48.5396092Z Receiving objects:  93% (1462/1571)
2023-04-10T02:36:48.5396776Z Receiving objects:  94% (1477/1571)
2023-04-10T02:36:48.5397089Z Receiving objects:  95% (1493/1571)
2023-04-10T02:36:48.5397454Z Receiving objects:  96% (1509/1571)
2023-04-10T02:36:48.5397833Z Receiving objects:  97% (1524/1571)
2023-04-10T02:36:48.5398235Z Receiving objects:  98% (1540/1571)
2023-04-10T02:36:48.5406121Z Receiving objects:  99% (1556/1571)
2023-04-10T02:36:48.5406942Z remote: Total 1571 (delta 249), reused 407 (delta 207), pack-reused 1067        
2023-04-10T02:36:48.5430088Z Receiving objects: 100% (1571/1571)
2023-04-10T02:36:48.5454559Z Receiving objects: 100% (1571/1571), 1.67 MiB | 9.12 MiB/s, done.
2023-04-10T02:36:48.5455035Z Resolving deltas:   0% (0/784)
2023-04-10T02:36:48.5455361Z Resolving deltas:   1% (8/784)
2023-04-10T02:36:48.5465571Z Resolving deltas:   2% (16/784)
2023-04-10T02:36:48.5465992Z Resolving deltas:   3% (24/784)
2023-04-10T02:36:48.5466475Z Resolving deltas:   4% (32/784)
2023-04-10T02:36:48.5466785Z Resolving deltas:   5% (40/784)
2023-04-10T02:36:48.5467162Z Resolving deltas:   6% (48/784)
2023-04-10T02:36:48.5467527Z Resolving deltas:   7% (55/784)
2023-04-10T02:36:48.5467935Z Resolving deltas:   8% (63/784)
2023-04-10T02:36:48.5468237Z Resolving deltas:   9% (71/784)
2023-04-10T02:36:48.5468615Z Resolving deltas:  10% (79/784)
2023-04-10T02:36:48.5468986Z Resolving deltas:  11% (87/784)
2023-04-10T02:36:48.5469359Z Resolving deltas:  12% (95/784)
2023-04-10T02:36:48.5469695Z Resolving deltas:  13% (102/784)
2023-04-10T02:36:48.5470064Z Resolving deltas:  14% (110/784)
2023-04-10T02:36:48.5470426Z Resolving deltas:  15% (118/784)
2023-04-10T02:36:48.5470796Z Resolving deltas:  16% (126/784)
2023-04-10T02:36:48.5471103Z Resolving deltas:  17% (134/784)
2023-04-10T02:36:48.5471495Z Resolving deltas:  18% (142/784)
2023-04-10T02:36:48.5471860Z Resolving deltas:  19% (149/784)
2023-04-10T02:36:48.5472214Z Resolving deltas:  20% (157/784)
2023-04-10T02:36:48.5472529Z Resolving deltas:  21% (165/784)
2023-04-10T02:36:48.5472913Z Resolving deltas:  22% (173/784)
2023-04-10T02:36:48.5473280Z Resolving deltas:  23% (181/784)
2023-04-10T02:36:48.5473635Z Resolving deltas:  24% (189/784)
2023-04-10T02:36:48.5519677Z Resolving deltas:  25% (196/784)
2023-04-10T02:36:48.5520059Z Resolving deltas:  26% (204/784)
2023-04-10T02:36:48.5520818Z Resolving deltas:  27% (212/784)
2023-04-10T02:36:48.5521217Z Resolving deltas:  28% (220/784)
2023-04-10T02:36:48.5521544Z Resolving deltas:  29% (228/784)
2023-04-10T02:36:48.5521898Z Resolving deltas:  30% (236/784)
2023-04-10T02:36:48.5522304Z Resolving deltas:  31% (244/784)
2023-04-10T02:36:48.5522670Z Resolving deltas:  32% (251/784)
2023-04-10T02:36:48.5522990Z Resolving deltas:  33% (259/784)
2023-04-10T02:36:48.5523345Z Resolving deltas:  34% (267/784)
2023-04-10T02:36:48.5523699Z Resolving deltas:  35% (275/784)
2023-04-10T02:36:48.5524090Z Resolving deltas:  36% (283/784)
2023-04-10T02:36:48.5524394Z Resolving deltas:  37% (291/784)
2023-04-10T02:36:48.5524765Z Resolving deltas:  38% (298/784)
2023-04-10T02:36:48.5525132Z Resolving deltas:  39% (306/784)
2023-04-10T02:36:48.5525517Z Resolving deltas:  40% (314/784)
2023-04-10T02:36:48.5525821Z Resolving deltas:  41% (322/784)
2023-04-10T02:36:48.5526190Z Resolving deltas:  42% (330/784)
2023-04-10T02:36:48.5526545Z Resolving deltas:  43% (338/784)
2023-04-10T02:36:48.5526902Z Resolving deltas:  44% (345/784)
2023-04-10T02:36:48.5527238Z Resolving deltas:  45% (353/784)
2023-04-10T02:36:48.5527626Z Resolving deltas:  46% (361/784)
2023-04-10T02:36:48.5527978Z Resolving deltas:  47% (369/784)
2023-04-10T02:36:48.5528331Z Resolving deltas:  48% (377/784)
2023-04-10T02:36:48.5528632Z Resolving deltas:  49% (385/784)
2023-04-10T02:36:48.5529028Z Resolving deltas:  50% (392/784)
2023-04-10T02:36:48.5529383Z Resolving deltas:  51% (400/784)
2023-04-10T02:36:48.5529738Z Resolving deltas:  52% (408/784)
2023-04-10T02:36:48.5530037Z Resolving deltas:  53% (416/784)
2023-04-10T02:36:48.5530415Z Resolving deltas:  54% (424/784)
2023-04-10T02:36:48.5530790Z Resolving deltas:  55% (432/784)
2023-04-10T02:36:48.5531305Z Resolving deltas:  56% (440/784)
2023-04-10T02:36:48.5531608Z Resolving deltas:  57% (447/784)
2023-04-10T02:36:48.5531975Z Resolving deltas:  58% (455/784)
2023-04-10T02:36:48.5532364Z Resolving deltas:  59% (463/784)
2023-04-10T02:36:48.5613216Z Resolving deltas:  60% (471/784)
2023-04-10T02:36:48.5630739Z Resolving deltas:  61% (479/784)
2023-04-10T02:36:48.5635419Z Resolving deltas:  62% (487/784)
2023-04-10T02:36:48.5645906Z Resolving deltas:  63% (494/784)
2023-04-10T02:36:48.5688263Z Resolving deltas:  64% (502/784)
2023-04-10T02:36:48.5703804Z Resolving deltas:  65% (510/784)
2023-04-10T02:36:48.5746686Z Resolving deltas:  66% (518/784)
2023-04-10T02:36:48.5759222Z Resolving deltas:  67% (526/784)
2023-04-10T02:36:48.5765020Z Resolving deltas:  68% (534/784)
2023-04-10T02:36:48.5770615Z Resolving deltas:  69% (541/784)
2023-04-10T02:36:48.5772783Z Resolving deltas:  70% (549/784)
2023-04-10T02:36:48.5774066Z Resolving deltas:  71% (557/784)
2023-04-10T02:36:48.5775236Z Resolving deltas:  72% (565/784)
2023-04-10T02:36:48.5776426Z Resolving deltas:  73% (573/784)
2023-04-10T02:36:48.5777418Z Resolving deltas:  74% (581/784)
2023-04-10T02:36:48.5778482Z Resolving deltas:  75% (588/784)
2023-04-10T02:36:48.5779815Z Resolving deltas:  76% (596/784)
2023-04-10T02:36:48.5781111Z Resolving deltas:  77% (604/784)
2023-04-10T02:36:48.5782226Z Resolving deltas:  78% (612/784)
2023-04-10T02:36:48.5783313Z Resolving deltas:  79% (620/784)
2023-04-10T02:36:48.5784394Z Resolving deltas:  80% (628/784)
2023-04-10T02:36:48.5785421Z Resolving deltas:  81% (636/784)
2023-04-10T02:36:48.5786388Z Resolving deltas:  82% (643/784)
2023-04-10T02:36:48.5787340Z Resolving deltas:  83% (651/784)
2023-04-10T02:36:48.5788431Z Resolving deltas:  84% (659/784)
2023-04-10T02:36:48.5789627Z Resolving deltas:  85% (667/784)
2023-04-10T02:36:48.5790715Z Resolving deltas:  86% (675/784)
2023-04-10T02:36:48.5791857Z Resolving deltas:  87% (683/784)
2023-04-10T02:36:48.5793048Z Resolving deltas:  88% (690/784)
2023-04-10T02:36:48.5794099Z Resolving deltas:  89% (698/784)
2023-04-10T02:36:48.5796499Z Resolving deltas:  90% (706/784)
2023-04-10T02:36:48.5798871Z Resolving deltas:  91% (714/784)
2023-04-10T02:36:48.5801222Z Resolving deltas:  92% (722/784)
2023-04-10T02:36:48.5805614Z Resolving deltas:  93% (730/784)
2023-04-10T02:36:48.5809501Z Resolving deltas:  94% (737/784)
2023-04-10T02:36:48.5813035Z Resolving deltas:  95% (745/784)
2023-04-10T02:36:48.5814354Z Resolving deltas:  96% (753/784)
2023-04-10T02:36:48.5818063Z Resolving deltas:  97% (761/784)
2023-04-10T02:36:48.5838793Z Resolving deltas:  98% (769/784)
2023-04-10T02:36:48.5916466Z Resolving deltas:  99% (777/784)
2023-04-10T02:36:48.5916876Z Resolving deltas: 100% (784/784)
2023-04-10T02:36:48.5917251Z Resolving deltas: 100% (784/784), done.
2023-04-10T02:36:48.6101103Z From https://github.com/CasperDash/useWallet
2023-04-10T02:36:48.6102214Z  * [new branch]      build-core                  -> origin/build-core
2023-04-10T02:36:48.6103230Z  * [new branch]      build-react                 -> origin/build-react
2023-04-10T02:36:48.6136182Z  * [new branch]      build-react-2               -> origin/build-react-2
2023-04-10T02:36:48.6136910Z  * [new branch]      build-react-core-2          -> origin/build-react-core-2
2023-04-10T02:36:48.6137639Z  * [new branch]      build/core                  -> origin/build/core
2023-04-10T02:36:48.6138147Z  * [new branch]      build/react                 -> origin/build/react
2023-04-10T02:36:48.6138752Z  * [new branch]      chore/remove-space          -> origin/chore/remove-space
2023-04-10T02:36:48.6139317Z  * [new branch]      develop                     -> origin/develop
2023-04-10T02:36:48.6139846Z  * [new branch]      doc                         -> origin/doc
2023-04-10T02:36:48.6140461Z  * [new branch]      docs/import-wallet-on-readme -> origin/docs/import-wallet-on-readme
2023-04-10T02:36:48.6141127Z  * [new branch]      docs/update-hooks           -> origin/docs/update-hooks
2023-04-10T02:36:48.6142055Z  * [new branch]      docs/update-readme-features -> origin/docs/update-readme-features
2023-04-10T02:36:48.6142805Z  * [new branch]      feat/#36-integrate-with-ledger -> origin/feat/#36-integrate-with-ledger
2023-04-10T02:36:48.6143492Z  * [new branch]      feat/actions                -> origin/feat/actions
2023-04-10T02:36:48.6144087Z  * [new branch]      feat/casper-wallet-connector -> origin/feat/casper-wallet-connector
2023-04-10T02:36:48.6144724Z  * [new branch]      feat/connectors             -> origin/feat/connectors
2023-04-10T02:36:48.6145382Z  * [new branch]      feat/window-events-account  -> origin/feat/window-events-account
2023-04-10T02:36:48.6146035Z  * [new branch]      feature/documentation       -> origin/feature/documentation
2023-04-10T02:36:48.6146693Z  * [new branch]      fix/auto-connect            -> origin/fix/auto-connect
2023-04-10T02:36:48.6147372Z  * [new branch]      fix/onconnect-event-with-use-account -> origin/fix/onconnect-event-with-use-account
2023-04-10T02:36:48.6148140Z  * [new branch]      improvement-add-comments    -> origin/improvement-add-comments
2023-04-10T02:36:48.6148736Z  * [new branch]      main                        -> origin/main
2023-04-10T02:36:48.6149448Z  * [new branch]      refactor/rename-casper-dash-global -> origin/refactor/rename-casper-dash-global
2023-04-10T02:36:48.6153584Z  * [new branch]      release/0.0.1               -> origin/release/0.0.1
2023-04-10T02:36:48.6159013Z  * [new branch]      release/0.0.2               -> origin/release/0.0.2
2023-04-10T02:36:48.6164162Z  * [new branch]      release/0.0.3               -> origin/release/0.0.3
2023-04-10T02:36:48.6169680Z  * [new branch]      release/0.0.4               -> origin/release/0.0.4
2023-04-10T02:36:48.6175574Z  * [new branch]      test/casper-wallet-connector -> origin/test/casper-wallet-connector
2023-04-10T02:36:48.6180243Z  * [new branch]      test/use-account            -> origin/test/use-account
2023-04-10T02:36:48.6184894Z  * [new branch]      update-doc                  -> origin/update-doc
2023-04-10T02:36:48.6189391Z  * [new tag]         @casperdash/usewallet-core@0.0.1 -> @casperdash/usewallet-core@0.0.1
2023-04-10T02:36:48.6193464Z  * [new tag]         @casperdash/usewallet-core@0.0.2 -> @casperdash/usewallet-core@0.0.2
2023-04-10T02:36:48.6197778Z  * [new tag]         @casperdash/usewallet-core@0.0.3 -> @casperdash/usewallet-core@0.0.3
2023-04-10T02:36:48.6202758Z  * [new tag]         @casperdash/usewallet@0.0.1 -> @casperdash/usewallet@0.0.1
2023-04-10T02:36:48.6203360Z  * [new tag]         @casperdash/usewallet@0.0.2 -> @casperdash/usewallet@0.0.2
2023-04-10T02:36:48.6207699Z  * [new tag]         @casperdash/usewallet@0.0.3 -> @casperdash/usewallet@0.0.3
2023-04-10T02:36:48.6211903Z  * [new tag]         docs-0.0.2                  -> docs-0.0.2
2023-04-10T02:36:48.6215497Z  * [new tag]         docs-0.0.3                  -> docs-0.0.3
2023-04-10T02:36:48.6216976Z  * [new tag]         docs-0.0.4                  -> docs-0.0.4
2023-04-10T02:36:48.6217802Z  * [new tag]         docs-0.0.5                  -> docs-0.0.5
2023-04-10T02:36:48.6218510Z  * [new tag]         docs-0.0.6                  -> docs-0.0.6
2023-04-10T02:36:48.6267624Z [command]/usr/bin/git branch --list --remote origin/main
2023-04-10T02:36:48.6304166Z   origin/main
2023-04-10T02:36:48.6327834Z [command]/usr/bin/git rev-parse refs/remotes/origin/main
2023-04-10T02:36:48.6349312Z 25f8ac7a84341a7485ddf7707522bda42d38972c
2023-04-10T02:36:48.6403531Z ##[endgroup]
2023-04-10T02:36:48.6404217Z ##[group]Determining the checkout info
2023-04-10T02:36:48.6404838Z ##[endgroup]
2023-04-10T02:36:48.6405396Z ##[group]Checking out the ref
2023-04-10T02:36:48.6406172Z [command]/usr/bin/git checkout --progress --force -B main refs/remotes/origin/main
2023-04-10T02:36:48.6574916Z Switched to a new branch 'main'
2023-04-10T02:36:48.6575424Z branch 'main' set up to track 'origin/main'.
2023-04-10T02:36:48.6582947Z ##[endgroup]
2023-04-10T02:36:48.6631376Z [command]/usr/bin/git log -1 --format='%H'
2023-04-10T02:36:48.6665217Z '25f8ac7a84341a7485ddf7707522bda42d38972c'
2023-04-10T02:36:48.7026302Z ##[group]Run pnpm/action-setup@v2.2.4
2023-04-10T02:36:48.7026606Z with:
2023-04-10T02:36:48.7026837Z   version: 7.26.3
2023-04-10T02:36:48.7027075Z   dest: ~/setup-pnpm
2023-04-10T02:36:48.7027326Z   run_install: null
2023-04-10T02:36:48.7027560Z ##[endgroup]
2023-04-10T02:36:48.8404215Z ##[group]Running self-installer...
2023-04-10T02:36:49.4531944Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:36:49.4646034Z Packages: +1
2023-04-10T02:36:49.4646551Z +
2023-04-10T02:36:50.2147243Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:36:50.2148303Z   Content-addressable store is at: /home/runner/.pnpm-store/v3
2023-04-10T02:36:50.2149561Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:36:50.2460794Z 
2023-04-10T02:36:50.2461517Z dependencies:
2023-04-10T02:36:50.2462501Z + pnpm 7.26.3 (8.2.0 is available)
2023-04-10T02:36:50.2462867Z 
2023-04-10T02:36:50.4544519Z Progress: resolved 1, reused 0, downloaded 1, added 1, done
2023-04-10T02:36:50.4776479Z ##[endgroup]
2023-04-10T02:36:50.4776952Z Installation Completed!
2023-04-10T02:36:50.4917240Z ##[group]Run actions/setup-node@v3
2023-04-10T02:36:50.4917517Z with:
2023-04-10T02:36:50.4917742Z   cache: pnpm
2023-04-10T02:36:50.4917987Z   node-version: 18
2023-04-10T02:36:50.4918247Z   always-auth: false
2023-04-10T02:36:50.4918492Z   check-latest: false
2023-04-10T02:36:50.4918957Z   token: ***
2023-04-10T02:36:50.4919190Z env:
2023-04-10T02:36:50.4919497Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:50.4919797Z ##[endgroup]
2023-04-10T02:36:50.7813869Z Found in cache @ /opt/hostedtoolcache/node/18.15.0/x64
2023-04-10T02:36:50.7826372Z ##[group]Environment details
2023-04-10T02:36:51.8868375Z node: v18.15.0
2023-04-10T02:36:51.8868997Z npm: 9.5.0
2023-04-10T02:36:51.8869765Z yarn: 1.22.19
2023-04-10T02:36:51.8870755Z ##[endgroup]
2023-04-10T02:36:51.8879826Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm store path --silent
2023-04-10T02:36:52.5040527Z /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:36:52.7347622Z pnpm cache is not found
2023-04-10T02:36:52.7555256Z ##[group]Run pnpm i
2023-04-10T02:36:52.7555587Z [36;1mpnpm i[0m
2023-04-10T02:36:52.7620392Z shell: /usr/bin/bash -e {0}
2023-04-10T02:36:52.7620680Z env:
2023-04-10T02:36:52.7620984Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:52.7621308Z ##[endgroup]
2023-04-10T02:36:53.4296545Z Scope: all 5 workspace projects
2023-04-10T02:36:53.5312357Z Lockfile is up to date, resolution step is skipped
2023-04-10T02:36:53.6676198Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:36:53.9087222Z Packages: +1012
2023-04-10T02:36:53.9098576Z ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2023-04-10T02:36:54.5935762Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:36:54.5939907Z   Content-addressable store is at: /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:36:54.5940944Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:36:54.6691003Z Progress: resolved 1012, reused 0, downloaded 11, added 6
2023-04-10T02:36:55.6710530Z Progress: resolved 1012, reused 0, downloaded 69, added 62
2023-04-10T02:36:56.6737418Z Progress: resolved 1012, reused 0, downloaded 139, added 136
2023-04-10T02:36:57.6766803Z Progress: resolved 1012, reused 0, downloaded 217, added 217
2023-04-10T02:36:58.6843515Z Progress: resolved 1012, reused 0, downloaded 266, added 265
2023-04-10T02:36:59.6859803Z Progress: resolved 1012, reused 0, downloaded 333, added 330
2023-04-10T02:37:00.6918645Z Progress: resolved 1012, reused 0, downloaded 403, added 403
2023-04-10T02:37:01.6927944Z Progress: resolved 1012, reused 0, downloaded 478, added 481
2023-04-10T02:37:02.7139667Z Progress: resolved 1012, reused 0, downloaded 544, added 543
2023-04-10T02:37:03.7209198Z Progress: resolved 1012, reused 0, downloaded 616, added 613
2023-04-10T02:37:04.7213224Z Progress: resolved 1012, reused 0, downloaded 714, added 715
2023-04-10T02:37:05.7264678Z Progress: resolved 1012, reused 0, downloaded 752, added 752
2023-04-10T02:37:06.7282013Z Progress: resolved 1012, reused 0, downloaded 803, added 804
2023-04-10T02:37:07.7345707Z Progress: resolved 1012, reused 0, downloaded 889, added 892
2023-04-10T02:37:08.7356490Z Progress: resolved 1012, reused 0, downloaded 956, added 955
2023-04-10T02:37:09.7354688Z Progress: resolved 1012, reused 0, downloaded 1000, added 1004
2023-04-10T02:37:10.7349846Z Progress: resolved 1012, reused 0, downloaded 1003, added 1007
2023-04-10T02:37:11.7355676Z Progress: resolved 1012, reused 0, downloaded 1005, added 1009
2023-04-10T02:37:12.9180134Z Progress: resolved 1012, reused 0, downloaded 1006, added 1010
2023-04-10T02:37:13.9193226Z Progress: resolved 1012, reused 0, downloaded 1008, added 1011
2023-04-10T02:37:14.7822694Z .../@napi-rs/simple-git-linux-x64-gnu postinstall$ node install.js
2023-04-10T02:37:14.7833536Z .../@napi-rs/simple-git-linux-x64-musl postinstall$ node install.js
2023-04-10T02:37:14.8384153Z .../node_modules/secp256k1 install$ npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."
2023-04-10T02:37:14.8687414Z .../@napi-rs/simple-git-linux-x64-musl postinstall: Failed
2023-04-10T02:37:14.8745988Z .../keccak@3.0.3/node_modules/keccak install$ node-gyp-build || exit 0
2023-04-10T02:37:14.8755941Z .../node_modules/secp256k1 install$ node-gyp-build || exit 0
2023-04-10T02:37:14.9495350Z Progress: resolved 1012, reused 0, downloaded 1008, added 1012, done
2023-04-10T02:37:14.9496591Z .../@napi-rs/simple-git-linux-x64-gnu postinstall: Done
2023-04-10T02:37:15.2134539Z .../node_modules/secp256k1 install: Done
2023-04-10T02:37:15.2839209Z .../keccak@3.0.3/node_modules/keccak install: Done
2023-04-10T02:37:15.9417783Z .../node_modules/secp256k1 install: > secp256k1@3.7.1 rebuild
2023-04-10T02:37:15.9425947Z .../node_modules/secp256k1 install: > node-gyp rebuild
2023-04-10T02:37:16.0548064Z .../node_modules/secp256k1 install: gyp info it worked if it ends with ok
2023-04-10T02:37:16.0583171Z .../node_modules/secp256k1 install: gyp info using node-gyp@9.3.1
2023-04-10T02:37:16.0583787Z .../node_modules/secp256k1 install: gyp info using node@18.15.0 | linux | x64
2023-04-10T02:37:16.1639029Z .../node_modules/secp256k1 install: gyp info find Python using Python version 3.10.6 found at "/usr/bin/python3"
2023-04-10T02:37:16.3183286Z .../node_modules/secp256k1 install: gyp http GET https://nodejs.org/download/release/v18.15.0/node-v18.15.0-headers.tar.gz
2023-04-10T02:37:16.4312322Z .../node_modules/secp256k1 install: gyp http 200 https://nodejs.org/download/release/v18.15.0/node-v18.15.0-headers.tar.gz
2023-04-10T02:37:18.0164028Z .../node_modules/secp256k1 install: gyp http GET https://nodejs.org/download/release/v18.15.0/SHASUMS256.txt
2023-04-10T02:37:18.0445219Z .../node_modules/secp256k1 install: gyp http 200 https://nodejs.org/download/release/v18.15.0/SHASUMS256.txt
2023-04-10T02:37:18.0604377Z .../node_modules/secp256k1 install: gyp info spawn /usr/bin/python3
2023-04-10T02:37:18.0605283Z .../node_modules/secp256k1 install: gyp info spawn args [
2023-04-10T02:37:18.0606604Z .../node_modules/secp256k1 install: gyp info spawn args   '/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py',
2023-04-10T02:37:18.0607485Z .../node_modules/secp256k1 install: gyp info spawn args   'binding.gyp',
2023-04-10T02:37:18.0608200Z .../node_modules/secp256k1 install: gyp info spawn args   '-f',
2023-04-10T02:37:18.0608988Z .../node_modules/secp256k1 install: gyp info spawn args   'make',
2023-04-10T02:37:18.0609680Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:18.0610785Z .../node_modules/secp256k1 install: gyp info spawn args   '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build/config.gypi',
2023-04-10T02:37:18.0612024Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:18.0613506Z .../node_modules/secp256k1 install: gyp info spawn args   '/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/addon.gypi',
2023-04-10T02:37:18.0614325Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:18.0615247Z .../node_modules/secp256k1 install: gyp info spawn args   '/home/runner/.cache/node-gyp/18.15.0/include/node/common.gypi',
2023-04-10T02:37:18.0616098Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dlibrary=shared_library',
2023-04-10T02:37:18.0616879Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dvisibility=default',
2023-04-10T02:37:18.0617781Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_root_dir=/home/runner/.cache/node-gyp/18.15.0',
2023-04-10T02:37:18.0618885Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_gyp_dir=/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp',
2023-04-10T02:37:18.0620007Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_lib_file=/home/runner/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
2023-04-10T02:37:18.0621206Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dmodule_root_dir=/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1',
2023-04-10T02:37:18.0622091Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_engine=v8',
2023-04-10T02:37:18.0622815Z .../node_modules/secp256k1 install: gyp info spawn args   '--depth=.',
2023-04-10T02:37:18.0623550Z .../node_modules/secp256k1 install: gyp info spawn args   '--no-parallel',
2023-04-10T02:37:18.0624299Z .../node_modules/secp256k1 install: gyp info spawn args   '--generator-output',
2023-04-10T02:37:18.0625016Z .../node_modules/secp256k1 install: gyp info spawn args   'build',
2023-04-10T02:37:18.0625784Z .../node_modules/secp256k1 install: gyp info spawn args   '-Goutput_dir=.'
2023-04-10T02:37:18.0626380Z .../node_modules/secp256k1 install: gyp info spawn args ]
2023-04-10T02:37:18.2953523Z .../node_modules/secp256k1 install: gyp info spawn make
2023-04-10T02:37:18.2956182Z .../node_modules/secp256k1 install: gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
2023-04-10T02:37:18.2977586Z .../node_modules/secp256k1 install: make: Entering directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build'
2023-04-10T02:37:18.3000463Z .../node_modules/secp256k1 install:   CXX(target) Release/obj.target/secp256k1/src/addon.o
2023-04-10T02:37:19.2821974Z .../node_modules/secp256k1 install: In file included from ../src/addon.cc:2:
2023-04-10T02:37:19.2825079Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2023-04-10T02:37:19.2827917Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2298:7: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2023-04-10T02:37:19.2829582Z .../node_modules/secp256k1 install:  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2023-04-10T02:37:19.2830694Z .../node_modules/secp256k1 install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:19.2856568Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::SetAccessor(v8::Local<v8::ObjectTemplate>, v8::Local<v8::String>, Nan::GetterCallback, Nan::SetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, Nan::imp::Sig)’:
2023-04-10T02:37:19.2861287Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2536:19: warning: ‘void v8::ObjectTemplate::SetAccessor(v8::Local<v8::Name>, v8::AccessorNameGetterCallback, v8::AccessorNameSetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, v8::Local<v8::AccessorSignature>, v8::SideEffectType, v8::SideEffectType)’ is deprecated: Do signature check in accessor [-Wdeprecated-declarations]
2023-04-10T02:37:19.2864095Z .../node_modules/secp256k1 install:  2536 |   tpl->SetAccessor(
2023-04-10T02:37:19.2872093Z .../node_modules/secp256k1 install:       |   ~~~~~~~~~~~~~~~~^
2023-04-10T02:37:19.2873538Z .../node_modules/secp256k1 install:  2537 |       name
2023-04-10T02:37:19.2910822Z .../node_modules/secp256k1 install:       |       ~~~~         
2023-04-10T02:37:19.2911670Z .../node_modules/secp256k1 install:  2538 |     , getter_
2023-04-10T02:37:19.2912141Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~      
2023-04-10T02:37:19.2912612Z .../node_modules/secp256k1 install:  2539 |     , setter_
2023-04-10T02:37:19.2913069Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~      
2023-04-10T02:37:19.2913508Z .../node_modules/secp256k1 install:  2540 |     , obj
2023-04-10T02:37:19.2913974Z .../node_modules/secp256k1 install:       |     ~~~~~          
2023-04-10T02:37:19.2914425Z .../node_modules/secp256k1 install:  2541 |     , settings
2023-04-10T02:37:19.2914891Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~     
2023-04-10T02:37:19.2915340Z .../node_modules/secp256k1 install:  2542 |     , attribute
2023-04-10T02:37:19.2915804Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~~    
2023-04-10T02:37:19.2916269Z .../node_modules/secp256k1 install:  2543 |     , signature);
2023-04-10T02:37:19.2916715Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~~~   
2023-04-10T02:37:19.2917671Z .../node_modules/secp256k1 install: In file included from /home/runner/.cache/node-gyp/18.15.0/include/node/v8-function.h:15,
2023-04-10T02:37:19.2918539Z .../node_modules/secp256k1 install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/v8.h:33,
2023-04-10T02:37:19.2919380Z .../node_modules/secp256k1 install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:73,
2023-04-10T02:37:19.2919969Z .../node_modules/secp256k1 install:                  from ../src/addon.cc:1:
2023-04-10T02:37:19.2921166Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/v8-template.h:838:8: note: declared here
2023-04-10T02:37:19.2921761Z .../node_modules/secp256k1 install:   838 |   void SetAccessor(
2023-04-10T02:37:19.2922219Z .../node_modules/secp256k1 install:       |        ^~~~~~~~~~~
2023-04-10T02:37:19.2988089Z .../node_modules/secp256k1 install: In file included from ../../../../nan@2.14.0/node_modules/nan/nan.h:2884,
2023-04-10T02:37:19.2993644Z .../node_modules/secp256k1 install:                  from ../src/addon.cc:2:
2023-04-10T02:37:19.2995076Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h: In constructor ‘Nan::TypedArrayContents<T>::TypedArrayContents(v8::Local<v8::Value>)’:
2023-04-10T02:37:19.2996396Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h:34:43: error: ‘class v8::ArrayBuffer’ has no member named ‘GetContents’
2023-04-10T02:37:19.2997420Z .../node_modules/secp256k1 install:    34 |       data   = static_cast<char*>(buffer->GetContents().Data()) + byte_offset;
2023-04-10T02:37:19.2998046Z .../node_modules/secp256k1 install:       |                                           ^~~~~~~~~~~
2023-04-10T02:37:19.3020185Z .../node_modules/secp256k1 install: In file included from ../src/addon.cc:1:
2023-04-10T02:37:19.3031038Z .../node_modules/secp256k1 install: ../src/addon.cc: At global scope:
2023-04-10T02:37:19.3033192Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:978:7: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2023-04-10T02:37:19.3035260Z .../node_modules/secp256k1 install:   978 |       (node::addon_register_func) (regfunc),                          \
2023-04-10T02:37:19.3035872Z .../node_modules/secp256k1 install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:19.3036813Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:1012:3: note: in expansion of macro ‘NODE_MODULE_X’
2023-04-10T02:37:19.3037601Z .../node_modules/secp256k1 install:  1012 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2023-04-10T02:37:19.3038152Z .../node_modules/secp256k1 install:       |   ^~~~~~~~~~~~~
2023-04-10T02:37:19.3038889Z .../node_modules/secp256k1 install: ../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
2023-04-10T02:37:19.3039467Z .../node_modules/secp256k1 install:    50 | NODE_MODULE(secp256k1, Init)
2023-04-10T02:37:19.3039942Z .../node_modules/secp256k1 install:       | ^~~~~~~~~~~
2023-04-10T02:37:19.3938697Z .../node_modules/secp256k1 install: make: *** [secp256k1.target.mk:165: Release/obj.target/secp256k1/src/addon.o] Error 1
2023-04-10T02:37:19.3939428Z .../node_modules/secp256k1 install: gyp ERR! build error 
2023-04-10T02:37:19.3960942Z .../node_modules/secp256k1 install: make: Leaving directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build'
2023-04-10T02:37:19.3962048Z .../node_modules/secp256k1 install: gyp ERR! stack Error: `make` failed with exit code: 2
2023-04-10T02:37:19.3963360Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess.onExit (/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/lib/build.js:203:23)
2023-04-10T02:37:19.4010425Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
2023-04-10T02:37:19.4011194Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
2023-04-10T02:37:19.4012042Z .../node_modules/secp256k1 install: gyp ERR! System Linux 5.15.0-1035-azure
2023-04-10T02:37:19.4014128Z .../node_modules/secp256k1 install: gyp ERR! command "/opt/hostedtoolcache/node/18.15.0/x64/bin/node" "/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
2023-04-10T02:37:19.4054611Z .../node_modules/secp256k1 install: gyp ERR! cwd /home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1
2023-04-10T02:37:19.4055531Z .../node_modules/secp256k1 install: gyp ERR! node -v v18.15.0
2023-04-10T02:37:19.4056119Z .../node_modules/secp256k1 install: gyp ERR! node-gyp -v v9.3.1
2023-04-10T02:37:19.4056595Z .../node_modules/secp256k1 install: gyp ERR! not ok 
2023-04-10T02:37:19.4112250Z .../node_modules/secp256k1 install: Secp256k1 bindings compilation fail. Pure JS implementation will be used.
2023-04-10T02:37:19.4117566Z .../node_modules/secp256k1 install: Done
2023-04-10T02:37:19.4822311Z .../node_modules/@swc/core postinstall$ node postinstall.js
2023-04-10T02:37:19.5007440Z .../eccrypto@1.1.6/node_modules/eccrypto install$ node-gyp rebuild || exit 0
2023-04-10T02:37:19.5257251Z .../esbuild@0.15.18/node_modules/esbuild postinstall$ node install.js
2023-04-10T02:37:19.5259400Z .../esbuild@0.17.12/node_modules/esbuild postinstall$ node install.js
2023-04-10T02:37:19.5947225Z .../node_modules/@swc/core postinstall: Done
2023-04-10T02:37:19.6346203Z .../esbuild@0.15.18/node_modules/esbuild postinstall: Done
2023-04-10T02:37:19.7065552Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info it worked if it ends with ok
2023-04-10T02:37:19.7066580Z .../esbuild@0.17.12/node_modules/esbuild postinstall: Done
2023-04-10T02:37:19.7114806Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info using node-gyp@9.3.1
2023-04-10T02:37:19.7130453Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info using node@18.15.0 | linux | x64
2023-04-10T02:37:19.8362229Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info find Python using Python version 3.10.6 found at "/usr/bin/python3"
2023-04-10T02:37:19.9683956Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn /usr/bin/python3
2023-04-10T02:37:19.9692363Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args [
2023-04-10T02:37:19.9697449Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/gyp/gyp_main.py',
2023-04-10T02:37:19.9700243Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'binding.gyp',
2023-04-10T02:37:19.9706062Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-f',
2023-04-10T02:37:19.9709907Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'make',
2023-04-10T02:37:19.9713382Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:19.9717306Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build/config.gypi',
2023-04-10T02:37:19.9720086Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:19.9724180Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/addon.gypi',
2023-04-10T02:37:19.9727013Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:19.9730473Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/.cache/node-gyp/18.15.0/include/node/common.gypi',
2023-04-10T02:37:19.9735020Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dlibrary=shared_library',
2023-04-10T02:37:19.9738532Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dvisibility=default',
2023-04-10T02:37:19.9742151Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_root_dir=/home/runner/.cache/node-gyp/18.15.0',
2023-04-10T02:37:19.9745903Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_gyp_dir=/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp',
2023-04-10T02:37:19.9748907Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_lib_file=/home/runner/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
2023-04-10T02:37:19.9752374Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dmodule_root_dir=/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto',
2023-04-10T02:37:19.9756065Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_engine=v8',
2023-04-10T02:37:19.9759099Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--depth=.',
2023-04-10T02:37:19.9762448Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--no-parallel',
2023-04-10T02:37:19.9773651Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--generator-output',
2023-04-10T02:37:19.9774657Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'build',
2023-04-10T02:37:19.9775385Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Goutput_dir=.'
2023-04-10T02:37:19.9775956Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args ]
2023-04-10T02:37:20.1691570Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn make
2023-04-10T02:37:20.1702383Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
2023-04-10T02:37:20.1703551Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: Entering directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build'
2023-04-10T02:37:20.1715473Z .../eccrypto@1.1.6/node_modules/eccrypto install:   CXX(target) Release/obj.target/ecdh/ecdh.o
2023-04-10T02:37:20.9663666Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:2:
2023-04-10T02:37:20.9666865Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2023-04-10T02:37:20.9670039Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2298:7: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2023-04-10T02:37:20.9673516Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2023-04-10T02:37:20.9674433Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.9695307Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::SetAccessor(v8::Local<v8::ObjectTemplate>, v8::Local<v8::String>, Nan::GetterCallback, Nan::SetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, Nan::imp::Sig)’:
2023-04-10T02:37:20.9717674Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2536:19: warning: ‘void v8::ObjectTemplate::SetAccessor(v8::Local<v8::Name>, v8::AccessorNameGetterCallback, v8::AccessorNameSetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, v8::Local<v8::AccessorSignature>, v8::SideEffectType, v8::SideEffectType)’ is deprecated: Do signature check in accessor [-Wdeprecated-declarations]
2023-04-10T02:37:20.9719311Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2536 |   tpl->SetAccessor(
2023-04-10T02:37:20.9720026Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~~~~~~^
2023-04-10T02:37:20.9720705Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2537 |       name
2023-04-10T02:37:20.9722277Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ~~~~         
2023-04-10T02:37:20.9771536Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2538 |     , getter_
2023-04-10T02:37:20.9774744Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~      
2023-04-10T02:37:20.9776308Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2539 |     , setter_
2023-04-10T02:37:20.9777714Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~      
2023-04-10T02:37:20.9779105Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2540 |     , obj
2023-04-10T02:37:20.9780500Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~          
2023-04-10T02:37:20.9781893Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2541 |     , settings
2023-04-10T02:37:20.9783277Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~     
2023-04-10T02:37:20.9784670Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2542 |     , attribute
2023-04-10T02:37:20.9786115Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~~    
2023-04-10T02:37:20.9787522Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2543 |     , signature);
2023-04-10T02:37:20.9788355Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~~~   
2023-04-10T02:37:20.9789414Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from /home/runner/.cache/node-gyp/18.15.0/include/node/v8-function.h:15,
2023-04-10T02:37:20.9790454Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/v8.h:33,
2023-04-10T02:37:20.9791451Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:73,
2023-04-10T02:37:20.9792163Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from ../ecdh.cc:1:
2023-04-10T02:37:20.9793409Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/v8-template.h:838:8: note: declared here
2023-04-10T02:37:20.9794130Z .../eccrypto@1.1.6/node_modules/eccrypto install:   838 |   void SetAccessor(
2023-04-10T02:37:20.9794751Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |        ^~~~~~~~~~~
2023-04-10T02:37:20.9800122Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../../../../nan@2.14.0/node_modules/nan/nan.h:2884,
2023-04-10T02:37:20.9801361Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from ../ecdh.cc:2:
2023-04-10T02:37:20.9809343Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h: In constructor ‘Nan::TypedArrayContents<T>::TypedArrayContents(v8::Local<v8::Value>)’:
2023-04-10T02:37:20.9811421Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h:34:43: error: ‘class v8::ArrayBuffer’ has no member named ‘GetContents’
2023-04-10T02:37:20.9823352Z .../eccrypto@1.1.6/node_modules/eccrypto install:    34 |       data   = static_cast<char*>(buffer->GetContents().Data()) + byte_offset;
2023-04-10T02:37:20.9824057Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                           ^~~~~~~~~~~
2023-04-10T02:37:21.0137026Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc: In function ‘int derive(const uint8_t*, const uint8_t*, uint8_t*)’:
2023-04-10T02:37:21.0138790Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:37:41: warning: ‘EC_KEY* EC_KEY_new_by_curve_name(int)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0140027Z .../eccrypto@1.1.6/node_modules/eccrypto install:    37 |   CHECK((pkey = EC_KEY_new_by_curve_name(NID_secp256k1)) != NULL);
2023-04-10T02:37:21.0141000Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                 ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:21.0142191Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:21.0143659Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:21.0144554Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:21.0145396Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0146739Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:998:31: note: declared here
2023-04-10T02:37:21.0147852Z .../eccrypto@1.1.6/node_modules/eccrypto install:   998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
2023-04-10T02:37:21.0148818Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                               ^~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0150436Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:38:31: warning: ‘int EC_KEY_set_private_key(EC_KEY*, const BIGNUM*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0151643Z .../eccrypto@1.1.6/node_modules/eccrypto install:    38 |   CHECK(EC_KEY_set_private_key(pkey, pkey_bn) == 1);
2023-04-10T02:37:21.0152546Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:21.0153642Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:21.0154654Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:21.0155545Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:21.0156380Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0157726Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1056:27: note: declared here
2023-04-10T02:37:21.0159156Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1056 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_private_key(EC_KEY *key, const BIGNUM *prv);
2023-04-10T02:37:21.0160144Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0161767Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:40:29: warning: ‘int EVP_PKEY_set1_EC_KEY(EVP_PKEY*, ec_key_st*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0162933Z .../eccrypto@1.1.6/node_modules/eccrypto install:    40 |   CHECK(EVP_PKEY_set1_EC_KEY(evp_pkey, pkey) == 1);
2023-04-10T02:37:21.0163849Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0164972Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:21.0166000Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:21.0166900Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:21.0167731Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:3:
2023-04-10T02:37:21.0169088Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/evp.h:1370:5: note: declared here
2023-04-10T02:37:21.0170194Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1370 | int EVP_PKEY_set1_EC_KEY(EVP_PKEY *pkey, struct ec_key_st *key);
2023-04-10T02:37:21.0171060Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0172588Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:43:44: warning: ‘EC_KEY* EC_KEY_new_by_curve_name(int)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0174073Z .../eccrypto@1.1.6/node_modules/eccrypto install:    43 |   CHECK((peerkey = EC_KEY_new_by_curve_name(NID_secp256k1)) != NULL);
2023-04-10T02:37:21.0175265Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                    ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:21.0176424Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:21.0177444Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:21.0178339Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:21.0178891Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0179807Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:998:31: note: declared here
2023-04-10T02:37:21.0180574Z .../eccrypto@1.1.6/node_modules/eccrypto install:   998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
2023-04-10T02:37:21.0181238Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                               ^~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0182514Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:51:50: warning: ‘int EC_POINT_set_compressed_coordinates_GFp(const EC_GROUP*, EC_POINT*, const BIGNUM*, int, BN_CTX*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0183555Z .../eccrypto@1.1.6/node_modules/eccrypto install:    51 |     res = EC_POINT_set_compressed_coordinates_GFp(peerkey_group,
2023-04-10T02:37:21.0184240Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:21.0184865Z .../eccrypto@1.1.6/node_modules/eccrypto install:    52 |                                                  peerkey_p,
2023-04-10T02:37:21.0185631Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~
2023-04-10T02:37:21.0186255Z .../eccrypto@1.1.6/node_modules/eccrypto install:    53 |                                                  peerkey_bn,
2023-04-10T02:37:21.0186865Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~
2023-04-10T02:37:21.0187505Z .../eccrypto@1.1.6/node_modules/eccrypto install:    54 |                                                  compressed_y_bit,
2023-04-10T02:37:21.0188139Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0188745Z .../eccrypto@1.1.6/node_modules/eccrypto install:    55 |                                                  NULL);
2023-04-10T02:37:21.0189350Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~
2023-04-10T02:37:21.0189936Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0190867Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:686:27: note: declared here
2023-04-10T02:37:21.0191637Z .../eccrypto@1.1.6/node_modules/eccrypto install:   686 | OSSL_DEPRECATEDIN_3_0 int EC_POINT_set_compressed_coordinates_GFp
2023-04-10T02:37:21.0235036Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0236327Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:57:32: warning: ‘int EC_KEY_set_public_key(EC_KEY*, const EC_POINT*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0237151Z .../eccrypto@1.1.6/node_modules/eccrypto install:    57 |     res = EC_KEY_set_public_key(peerkey, peerkey_p);
2023-04-10T02:37:21.0237795Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0238396Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0239613Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1070:27: note: declared here
2023-04-10T02:37:21.0240439Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1070 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_public_key(EC_KEY *key, const EC_POINT *pub);
2023-04-10T02:37:21.0241126Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0242323Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:62:51: warning: ‘int EC_KEY_set_public_key_affine_coordinates(EC_KEY*, BIGNUM*, BIGNUM*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0243191Z .../eccrypto@1.1.6/node_modules/eccrypto install:    62 |     res = EC_KEY_set_public_key_affine_coordinates(peerkey,
2023-04-10T02:37:21.0243846Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~
2023-04-10T02:37:21.0244486Z .../eccrypto@1.1.6/node_modules/eccrypto install:    63 |                                                  peerkey_bn_x,
2023-04-10T02:37:21.0245119Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~
2023-04-10T02:37:21.0245749Z .../eccrypto@1.1.6/node_modules/eccrypto install:    64 |                                                  peerkey_bn_y);
2023-04-10T02:37:21.0246369Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~
2023-04-10T02:37:21.0246942Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0247852Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1122:27: note: declared here
2023-04-10T02:37:21.0248817Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1122 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_public_key_affine_coordinates(EC_KEY *key,
2023-04-10T02:37:21.0249505Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0250600Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:69:29: warning: ‘int EVP_PKEY_set1_EC_KEY(EVP_PKEY*, ec_key_st*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0251418Z .../eccrypto@1.1.6/node_modules/eccrypto install:    69 |   CHECK(EVP_PKEY_set1_EC_KEY(evp_peerkey, peerkey) == 1);
2023-04-10T02:37:21.0252063Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0252990Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:21.0253696Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:21.0254330Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:21.0254907Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:3:
2023-04-10T02:37:21.0255811Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/evp.h:1370:5: note: declared here
2023-04-10T02:37:21.0256572Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1370 | int EVP_PKEY_set1_EC_KEY(EVP_PKEY *pkey, struct ec_key_st *key);
2023-04-10T02:37:21.0257177Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0258186Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:82:14: warning: ‘void EC_KEY_free(EC_KEY*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0258875Z .../eccrypto@1.1.6/node_modules/eccrypto install:    82 |   EC_KEY_free(peerkey);
2023-04-10T02:37:21.0259425Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~^~~~~~~~~
2023-04-10T02:37:21.0260158Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0261074Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1003:28: note: declared here
2023-04-10T02:37:21.0261802Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1003 | OSSL_DEPRECATEDIN_3_0 void EC_KEY_free(EC_KEY *key);
2023-04-10T02:37:21.0262412Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                            ^~~~~~~~~~~
2023-04-10T02:37:21.0263406Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:90:14: warning: ‘void EC_KEY_free(EC_KEY*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:21.0264080Z .../eccrypto@1.1.6/node_modules/eccrypto install:    90 |   EC_KEY_free(pkey);
2023-04-10T02:37:21.0264628Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~^~~~~~
2023-04-10T02:37:21.0265198Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:21.0266115Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1003:28: note: declared here
2023-04-10T02:37:21.0266821Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1003 | OSSL_DEPRECATEDIN_3_0 void EC_KEY_free(EC_KEY *key);
2023-04-10T02:37:21.0267428Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                            ^~~~~~~~~~~
2023-04-10T02:37:21.0267994Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:1:
2023-04-10T02:37:21.0268558Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc: At global scope:
2023-04-10T02:37:21.0270588Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:978:7: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2023-04-10T02:37:21.0271817Z .../eccrypto@1.1.6/node_modules/eccrypto install:   978 |       (node::addon_register_func) (regfunc),                          \
2023-04-10T02:37:21.0272434Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:21.0273409Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:1012:3: note: in expansion of macro ‘NODE_MODULE_X’
2023-04-10T02:37:21.0274229Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1012 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2023-04-10T02:37:21.0274814Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ^~~~~~~~~~~~~
2023-04-10T02:37:21.0275599Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
2023-04-10T02:37:21.0276218Z .../eccrypto@1.1.6/node_modules/eccrypto install:   131 | NODE_MODULE(ecdh, InitAll)
2023-04-10T02:37:21.0276751Z .../eccrypto@1.1.6/node_modules/eccrypto install:       | ^~~~~~~~~~~
2023-04-10T02:37:21.1002206Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: *** [ecdh.target.mk:119: Release/obj.target/ecdh/ecdh.o] Error 1
2023-04-10T02:37:21.1002882Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! build error 
2023-04-10T02:37:21.1004131Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: Leaving directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build'
2023-04-10T02:37:21.1004914Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack Error: `make` failed with exit code: 2
2023-04-10T02:37:21.1006156Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess.onExit (/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/lib/build.js:203:23)
2023-04-10T02:37:21.1007378Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
2023-04-10T02:37:21.1008183Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
2023-04-10T02:37:21.1009034Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! System Linux 5.15.0-1035-azure
2023-04-10T02:37:21.1010331Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! command "/opt/hostedtoolcache/node/18.15.0/x64/bin/node" "/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
2023-04-10T02:37:21.1011354Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! cwd /home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto
2023-04-10T02:37:21.1012129Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! node -v v18.15.0
2023-04-10T02:37:21.1013008Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! node-gyp -v v9.3.1
2023-04-10T02:37:21.1013533Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! not ok 
2023-04-10T02:37:21.1052780Z .../eccrypto@1.1.6/node_modules/eccrypto install: Done
2023-04-10T02:37:21.3331062Z 
2023-04-10T02:37:21.3331969Z devDependencies:
2023-04-10T02:37:21.3332847Z + @babel/core 7.20.12
2023-04-10T02:37:21.3334364Z + @changesets/changelog-github 0.4.8
2023-04-10T02:37:21.3334897Z + @changesets/cli 2.26.0
2023-04-10T02:37:21.3335606Z + @typescript-eslint/eslint-plugin 5.48.0
2023-04-10T02:37:21.3336234Z + @typescript-eslint/parser 5.48.0
2023-04-10T02:37:21.3336784Z + @vitest/coverage-c8 0.28.3
2023-04-10T02:37:21.3337191Z + @vitest/ui 0.28.4
2023-04-10T02:37:21.3337544Z + eslint 8.31.0
2023-04-10T02:37:21.3338155Z + eslint-config-airbnb-typescript 17.0.0
2023-04-10T02:37:21.3339228Z + eslint-config-prettier 8.6.0
2023-04-10T02:37:21.3339778Z + eslint-plugin-import 2.26.0
2023-04-10T02:37:21.3340355Z + eslint-plugin-prettier 4.2.1
2023-04-10T02:37:21.3340909Z + eslint-plugin-sonar 0.9.2
2023-04-10T02:37:21.3341292Z + husky 8.0.3
2023-04-10T02:37:21.3341608Z + jsdom 20.0.3
2023-04-10T02:37:21.3342044Z + lint-staged 13.1.0
2023-04-10T02:37:21.3342403Z + prettier 2.8.1
2023-04-10T02:37:21.3342746Z + semver 7.3.8
2023-04-10T02:37:21.3343071Z + tsup 6.5.0
2023-04-10T02:37:21.3343419Z + typescript 4.9.4
2023-04-10T02:37:21.3343901Z + vite-tsconfig-paths 4.0.5
2023-04-10T02:37:21.3344285Z + vitest 0.26.3
2023-04-10T02:37:21.3344495Z 
2023-04-10T02:37:21.3348546Z . prepare$ husky install
2023-04-10T02:37:21.4129012Z . prepare: husky - Git hooks installed
2023-04-10T02:37:21.4177857Z . prepare: Done
2023-04-10T02:37:21.4199145Z Done in 28.5s
2023-04-10T02:37:21.4803098Z ##[group]Run changesets/action@v1.4.1
2023-04-10T02:37:21.4803401Z with:
2023-04-10T02:37:21.4803638Z   title: chore(version): packages
2023-04-10T02:37:21.4803952Z   commit: chore(version): packages
2023-04-10T02:37:21.4804246Z   version: pnpm changeset:version
2023-04-10T02:37:21.4804535Z   publish: pnpm changeset:release
2023-04-10T02:37:21.4804804Z   setupGitUser: true
2023-04-10T02:37:21.4805083Z   createGithubReleases: true
2023-04-10T02:37:21.4805338Z env:
2023-04-10T02:37:21.4805618Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:21.4806258Z   GITHUB_TOKEN: ***
2023-04-10T02:37:21.4806617Z   NPM_TOKEN: ***
2023-04-10T02:37:21.4806858Z ##[endgroup]
2023-04-10T02:37:21.6392819Z setting git user
2023-04-10T02:37:21.6445953Z [command]/usr/bin/git config user.name "github-actions[bot]"
2023-04-10T02:37:21.6558445Z [command]/usr/bin/git config user.email "github-actions[bot]@users.noreply.github.com"
2023-04-10T02:37:21.6597431Z setting GitHub credentials
2023-04-10T02:37:21.6638086Z No changesets found, attempting to publish any unpublished packages to npm
2023-04-10T02:37:21.6638921Z No user .npmrc file found, creating one
2023-04-10T02:37:21.6753356Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm changeset:release
2023-04-10T02:37:22.2675068Z 
2023-04-10T02:37:22.2675818Z > root@0.0.3 changeset:release /home/runner/work/useWallet/useWallet
2023-04-10T02:37:22.2676461Z > pnpm build && changeset publish
2023-04-10T02:37:22.2676675Z 
2023-04-10T02:37:22.8588135Z 
2023-04-10T02:37:22.8589281Z > root@0.0.3 build /home/runner/work/useWallet/useWallet
2023-04-10T02:37:22.8590669Z > pnpm -r --filter './packages/**' build
2023-04-10T02:37:22.8591240Z 
2023-04-10T02:37:23.5006919Z Scope: 2 of 5 workspace projects
2023-04-10T02:37:23.5045391Z packages/core build$ tsup src/index.ts
2023-04-10T02:37:23.7854546Z packages/core build: CLI Building entry: src/index.ts
2023-04-10T02:37:23.7863503Z packages/core build: CLI Using tsconfig: ../../tsconfig.json
2023-04-10T02:37:23.7869473Z packages/core build: CLI tsup v6.5.0
2023-04-10T02:37:23.7877292Z packages/core build: CLI Using tsup config: /home/runner/work/useWallet/useWallet/packages/core/tsup.config.js
2023-04-10T02:37:23.7908102Z packages/core build: CLI Target: es2021
2023-04-10T02:37:23.7954928Z packages/core build: CLI Cleaning output folder
2023-04-10T02:37:23.7978182Z packages/core build: IIFE Build start
2023-04-10T02:37:23.7987175Z packages/core build: CJS Build start
2023-04-10T02:37:23.7997100Z packages/core build: ESM Build start
2023-04-10T02:37:24.1023343Z packages/core build: ESM dist/index.js     22.78 KB
2023-04-10T02:37:24.1031103Z packages/core build: ESM dist/index.js.map 58.70 KB
2023-04-10T02:37:24.1041324Z packages/core build: ESM ⚡️ Build success in 304ms
2023-04-10T02:37:24.1122758Z packages/core build: CJS dist/index.cjs     24.99 KB
2023-04-10T02:37:24.1148279Z packages/core build: CJS dist/index.cjs.map 59.07 KB
2023-04-10T02:37:24.1149413Z packages/core build: CJS ⚡️ Build success in 315ms
2023-04-10T02:37:24.3333411Z packages/core build: IIFE dist/index.global.js     1.63 MB
2023-04-10T02:37:24.3334362Z packages/core build: IIFE dist/index.global.js.map 2.17 MB
2023-04-10T02:37:24.3335825Z packages/core build: IIFE ⚡️ Build success in 534ms
2023-04-10T02:37:24.3411531Z packages/core build: DTS Build start
2023-04-10T02:37:27.2795527Z packages/core build: DTS ⚡️ Build success in 2934ms
2023-04-10T02:37:27.2806784Z packages/core build: DTS dist/index.d.ts 19.81 KB
2023-04-10T02:37:27.3210586Z packages/core build: Done
2023-04-10T02:37:27.3224511Z packages/react build$ tsup src/index.ts
2023-04-10T02:37:27.5883583Z packages/react build: CLI Building entry: src/index.ts
2023-04-10T02:37:27.5884153Z packages/react build: CLI Using tsconfig: ../../tsconfig.json
2023-04-10T02:37:27.5884600Z packages/react build: CLI tsup v6.5.0
2023-04-10T02:37:27.5885243Z packages/react build: CLI Using tsup config: /home/runner/work/useWallet/useWallet/packages/react/tsup.config.js
2023-04-10T02:37:27.5935829Z packages/react build: CLI Target: es2021
2023-04-10T02:37:27.5982709Z packages/react build: CLI Cleaning output folder
2023-04-10T02:37:27.5992493Z packages/react build: IIFE Build start
2023-04-10T02:37:27.5995783Z packages/react build: CJS Build start
2023-04-10T02:37:27.6016370Z packages/react build: ESM Build start
2023-04-10T02:37:27.7654632Z packages/react build: ESM dist/index.js     8.31 KB
2023-04-10T02:37:27.7655569Z packages/react build: ESM dist/index.js.map 17.20 KB
2023-04-10T02:37:27.7657024Z packages/react build: ESM ⚡️ Build success in 162ms
2023-04-10T02:37:27.8327329Z packages/react build: CJS dist/index.cjs     10.60 KB
2023-04-10T02:37:27.8328225Z packages/react build: CJS dist/index.cjs.map 17.54 KB
2023-04-10T02:37:27.8329417Z packages/react build: CJS ⚡️ Build success in 233ms
2023-04-10T02:37:28.1741128Z packages/react build: DTS Build start
2023-04-10T02:37:28.2968946Z packages/react build: IIFE dist/index.global.js     1.79 MB
2023-04-10T02:37:28.2975330Z packages/react build: IIFE dist/index.global.js.map 2.48 MB
2023-04-10T02:37:28.2976209Z packages/react build: IIFE ⚡️ Build success in 698ms
2023-04-10T02:37:31.3783683Z packages/react build: DTS ⚡️ Build success in 3203ms
2023-04-10T02:37:31.3798679Z packages/react build: DTS dist/index.d.ts 4.15 KB
2023-04-10T02:37:31.4121916Z packages/react build: Done
2023-04-10T02:37:31.9490487Z 🦋  info npm info @casperdash/usewallet-core
2023-04-10T02:37:31.9548848Z 🦋  info npm info @casperdash/usewallet
2023-04-10T02:37:33.5665383Z 🦋  info @casperdash/usewallet-core is being published because our local version (0.0.4) has not been published on npm
2023-04-10T02:37:33.5667653Z 🦋  info @casperdash/usewallet is being published because our local version (0.0.4) has not been published on npm
2023-04-10T02:37:33.5668619Z 🦋  info Publishing "@casperdash/usewallet-core" at "0.0.4"
2023-04-10T02:37:33.5673057Z 🦋  info Publishing "@casperdash/usewallet" at "0.0.4"
2023-04-10T02:37:37.1348121Z 🦋  success packages published successfully:
2023-04-10T02:37:37.1349178Z 🦋  @casperdash/usewallet-core@0.0.4
2023-04-10T02:37:37.1350629Z 🦋  @casperdash/usewallet@0.0.4
2023-04-10T02:37:37.1351292Z 🦋  Creating git tags...
2023-04-10T02:37:37.1351958Z 🦋  New tag:  @casperdash/usewallet-core@0.0.4
2023-04-10T02:37:37.1426655Z 🦋  New tag:  @casperdash/usewallet@0.0.4
2023-04-10T02:37:37.1747992Z [command]/usr/bin/git push origin --tags
2023-04-10T02:37:38.2234500Z To https://github.com/CasperDash/useWallet
2023-04-10T02:37:38.2242051Z  * [new tag]         @casperdash/usewallet-core@0.0.4 -> @casperdash/usewallet-core@0.0.4
2023-04-10T02:37:38.2243189Z  * [new tag]         @casperdash/usewallet@0.0.4 -> @casperdash/usewallet@0.0.4
2023-04-10T02:37:38.2671397Z Post job cleanup.
2023-04-10T02:37:38.4582031Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm store path --silent
2023-04-10T02:37:39.0491171Z /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:37:39.0812183Z [command]/usr/bin/tar --posix -z -cf cache.tgz --exclude cache.tgz -P -C /home/runner/work/useWallet/useWallet --files-from manifest.txt
2023-04-10T02:38:18.3320237Z Cache Size: ~166 MB (173941030 B)
2023-04-10T02:38:18.4478411Z Cache saved successfully
2023-04-10T02:38:18.4771284Z Cache saved with the key: node-cache-Linux-pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:38:18.4876142Z Post job cleanup.
2023-04-10T02:38:18.6267036Z Pruning is unnecessary.
2023-04-10T02:38:18.6401030Z Post job cleanup.
2023-04-10T02:38:18.8241031Z [command]/usr/bin/git version
2023-04-10T02:38:18.8304426Z git version 2.40.0
2023-04-10T02:38:18.8362316Z Temporarily overriding HOME='/home/runner/work/_temp/55caf8df-39aa-4935-8c30-a84911d8fd27' before making global git config changes
2023-04-10T02:38:18.8363879Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:38:18.8371220Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:38:18.8427927Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:38:18.8478049Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:38:18.8766467Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:38:18.8787322Z http.https://github.com/.extraheader
2023-04-10T02:38:18.8805992Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2023-04-10T02:38:18.8857260Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:38:18.9375642Z Cleaning up orphan processes
```