# Linting Workflow Logs

```sh
2023-04-10T02:36:38.3552818Z Requested labels: ubuntu-latest
2023-04-10T02:36:38.3552862Z Job defined at: CasperDash/useWallet/.github/workflows/main.yml@refs/heads/main
2023-04-10T02:36:38.3552887Z Waiting for a runner to pick up this job...
2023-04-10T02:36:38.5077613Z Job is waiting for a hosted runner to come online.
2023-04-10T02:36:42.0207829Z Job is about to start running on the hosted runner: GitHub Actions 4 (hosted)
2023-04-10T02:36:44.5160914Z Current runner version: '2.303.0'
2023-04-10T02:36:44.5191626Z ##[group]Operating System
2023-04-10T02:36:44.5192205Z Ubuntu
2023-04-10T02:36:44.5192559Z 22.04.2
2023-04-10T02:36:44.5193003Z LTS
2023-04-10T02:36:44.5193314Z ##[endgroup]
2023-04-10T02:36:44.5193716Z ##[group]Runner Image
2023-04-10T02:36:44.5194136Z Image: ubuntu-22.04
2023-04-10T02:36:44.5194470Z Version: 20230402.1
2023-04-10T02:36:44.5195130Z Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20230402.1/images/linux/Ubuntu2204-Readme.md
2023-04-10T02:36:44.5195916Z Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20230402.1
2023-04-10T02:36:44.5196442Z ##[endgroup]
2023-04-10T02:36:44.5196801Z ##[group]Runner Image Provisioner
2023-04-10T02:36:44.5197200Z 2.0.139.1
2023-04-10T02:36:44.5197601Z ##[endgroup]
2023-04-10T02:36:44.5198727Z ##[group]GITHUB_TOKEN Permissions
2023-04-10T02:36:44.5199432Z Actions: write
2023-04-10T02:36:44.5199814Z Checks: write
2023-04-10T02:36:44.5200425Z Contents: write
2023-04-10T02:36:44.5200917Z Deployments: write
2023-04-10T02:36:44.5201382Z Discussions: write
2023-04-10T02:36:44.5201734Z Issues: write
2023-04-10T02:36:44.5202110Z Metadata: read
2023-04-10T02:36:44.5202495Z Packages: write
2023-04-10T02:36:44.5202817Z Pages: write
2023-04-10T02:36:44.5203250Z PullRequests: write
2023-04-10T02:36:44.5203681Z RepositoryProjects: write
2023-04-10T02:36:44.5204059Z SecurityEvents: write
2023-04-10T02:36:44.5204454Z Statuses: write
2023-04-10T02:36:44.5204827Z ##[endgroup]
2023-04-10T02:36:44.5209087Z Secret source: Actions
2023-04-10T02:36:44.5209706Z Prepare workflow directory
2023-04-10T02:36:44.6172804Z Prepare all required actions
2023-04-10T02:36:44.6391241Z Getting action download info
2023-04-10T02:36:45.0105127Z Download action repository 'actions/checkout@v3' (SHA:8f4b7f84864484a7bf31766abe9204da3cbe65b3)
2023-04-10T02:36:45.4164701Z Download action repository 'pnpm/action-setup@v2.2.4' (SHA:c3b53f6a16e57305370b4ae5a540c2077a1d50dd)
2023-04-10T02:36:45.7087330Z Download action repository 'actions/setup-node@v3' (SHA:64ed1c7eab4cce3362f8c340dee64e5eaeef8f7c)
2023-04-10T02:36:45.9839154Z Download action repository 'actions/cache@v3' (SHA:88522ab9f39a2ea568f7027eddc7d8d8bc9d59c8)
2023-04-10T02:36:46.4458353Z Complete job name: Lint (18, 7.26.3)
2023-04-10T02:36:46.5402645Z ##[group]Run actions/checkout@v3
2023-04-10T02:36:46.5403006Z with:
2023-04-10T02:36:46.5403269Z   repository: CasperDash/useWallet
2023-04-10T02:36:46.5403814Z   token: ***
2023-04-10T02:36:46.5404064Z   ssh-strict: true
2023-04-10T02:36:46.5404400Z   persist-credentials: true
2023-04-10T02:36:46.5404670Z   clean: true
2023-04-10T02:36:46.5404914Z   fetch-depth: 1
2023-04-10T02:36:46.5405139Z   lfs: false
2023-04-10T02:36:46.5405389Z   submodules: false
2023-04-10T02:36:46.5405664Z   set-safe-directory: true
2023-04-10T02:36:46.5405925Z ##[endgroup]
2023-04-10T02:36:46.9602769Z Syncing repository: CasperDash/useWallet
2023-04-10T02:36:46.9604749Z ##[group]Getting Git version info
2023-04-10T02:36:46.9605385Z Working directory is '/home/runner/work/useWallet/useWallet'
2023-04-10T02:36:46.9608374Z [command]/usr/bin/git version
2023-04-10T02:36:46.9625627Z git version 2.40.0
2023-04-10T02:36:46.9656421Z ##[endgroup]
2023-04-10T02:36:46.9677830Z Temporarily overriding HOME='/home/runner/work/_temp/7b10b005-6411-494d-827d-2ab1397f8056' before making global git config changes
2023-04-10T02:36:46.9678418Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:36:46.9683952Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:36:46.9748147Z Deleting the contents of '/home/runner/work/useWallet/useWallet'
2023-04-10T02:36:46.9754814Z ##[group]Initializing the repository
2023-04-10T02:36:46.9759031Z [command]/usr/bin/git init /home/runner/work/useWallet/useWallet
2023-04-10T02:36:46.9909560Z hint: Using 'master' as the name for the initial branch. This default branch name
2023-04-10T02:36:46.9910914Z hint: is subject to change. To configure the initial branch name to use in all
2023-04-10T02:36:46.9912404Z hint: of your new repositories, which will suppress this warning, call:
2023-04-10T02:36:46.9913011Z hint: 
2023-04-10T02:36:46.9913948Z hint: 	git config --global init.defaultBranch <name>
2023-04-10T02:36:46.9914500Z hint: 
2023-04-10T02:36:46.9915373Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2023-04-10T02:36:46.9916208Z hint: 'development'. The just-created branch can be renamed via this command:
2023-04-10T02:36:46.9916980Z hint: 
2023-04-10T02:36:46.9917511Z hint: 	git branch -m <name>
2023-04-10T02:36:46.9922192Z Initialized empty Git repository in /home/runner/work/useWallet/useWallet/.git/
2023-04-10T02:36:46.9937837Z [command]/usr/bin/git remote add origin https://github.com/CasperDash/useWallet
2023-04-10T02:36:46.9988628Z ##[endgroup]
2023-04-10T02:36:46.9989411Z ##[group]Disabling automatic garbage collection
2023-04-10T02:36:46.9993277Z [command]/usr/bin/git config --local gc.auto 0
2023-04-10T02:36:47.0032587Z ##[endgroup]
2023-04-10T02:36:47.0033321Z ##[group]Setting up auth
2023-04-10T02:36:47.0040701Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:36:47.0080794Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:36:47.0566832Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:36:47.0597201Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:36:47.0895770Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2023-04-10T02:36:47.0943395Z ##[endgroup]
2023-04-10T02:36:47.0944308Z ##[group]Fetching the repository
2023-04-10T02:36:47.0954166Z [command]/usr/bin/git -c protocol.version=2 fetch --no-tags --prune --progress --no-recurse-submodules --depth=1 origin +25f8ac7a84341a7485ddf7707522bda42d38972c:refs/remotes/origin/main
2023-04-10T02:36:47.3486739Z remote: Enumerating objects: 169, done.        
2023-04-10T02:36:47.3492124Z remote: Counting objects:   0% (1/169)        
2023-04-10T02:36:47.3493383Z remote: Counting objects:   1% (2/169)        
2023-04-10T02:36:47.3494020Z remote: Counting objects:   2% (4/169)        
2023-04-10T02:36:47.3494784Z remote: Counting objects:   3% (6/169)        
2023-04-10T02:36:47.3495308Z remote: Counting objects:   4% (7/169)        
2023-04-10T02:36:47.3496095Z remote: Counting objects:   5% (9/169)        
2023-04-10T02:36:47.3496620Z remote: Counting objects:   6% (11/169)        
2023-04-10T02:36:47.3497491Z remote: Counting objects:   7% (12/169)        
2023-04-10T02:36:47.3498059Z remote: Counting objects:   8% (14/169)        
2023-04-10T02:36:47.3498836Z remote: Counting objects:   9% (16/169)        
2023-04-10T02:36:47.3500188Z remote: Counting objects:  10% (17/169)        
2023-04-10T02:36:47.3500739Z remote: Counting objects:  11% (19/169)        
2023-04-10T02:36:47.3501529Z remote: Counting objects:  12% (21/169)        
2023-04-10T02:36:47.3502083Z remote: Counting objects:  13% (22/169)        
2023-04-10T02:36:47.3502812Z remote: Counting objects:  14% (24/169)        
2023-04-10T02:36:47.3503356Z remote: Counting objects:  15% (26/169)        
2023-04-10T02:36:47.3504125Z remote: Counting objects:  16% (28/169)        
2023-04-10T02:36:47.3504670Z remote: Counting objects:  17% (29/169)        
2023-04-10T02:36:47.3505745Z remote: Counting objects:  18% (31/169)        
2023-04-10T02:36:47.3506315Z remote: Counting objects:  19% (33/169)        
2023-04-10T02:36:47.3507118Z remote: Counting objects:  20% (34/169)        
2023-04-10T02:36:47.3507655Z remote: Counting objects:  21% (36/169)        
2023-04-10T02:36:47.3509151Z remote: Counting objects:  22% (38/169)        
2023-04-10T02:36:47.3510073Z remote: Counting objects:  23% (39/169)        
2023-04-10T02:36:47.3510862Z remote: Counting objects:  24% (41/169)        
2023-04-10T02:36:47.3511400Z remote: Counting objects:  25% (43/169)        
2023-04-10T02:36:47.3512161Z remote: Counting objects:  26% (44/169)        
2023-04-10T02:36:47.3512729Z remote: Counting objects:  27% (46/169)        
2023-04-10T02:36:47.3513565Z remote: Counting objects:  28% (48/169)        
2023-04-10T02:36:47.3514112Z remote: Counting objects:  29% (50/169)        
2023-04-10T02:36:47.3514857Z remote: Counting objects:  30% (51/169)        
2023-04-10T02:36:47.3515406Z remote: Counting objects:  31% (53/169)        
2023-04-10T02:36:47.3516148Z remote: Counting objects:  32% (55/169)        
2023-04-10T02:36:47.3516653Z remote: Counting objects:  33% (56/169)        
2023-04-10T02:36:47.3517425Z remote: Counting objects:  34% (58/169)        
2023-04-10T02:36:47.3517941Z remote: Counting objects:  35% (60/169)        
2023-04-10T02:36:47.3518685Z remote: Counting objects:  36% (61/169)        
2023-04-10T02:36:47.3519234Z remote: Counting objects:  37% (63/169)        
2023-04-10T02:36:47.3519972Z remote: Counting objects:  38% (65/169)        
2023-04-10T02:36:47.3520503Z remote: Counting objects:  39% (66/169)        
2023-04-10T02:36:47.3521254Z remote: Counting objects:  40% (68/169)        
2023-04-10T02:36:47.3521766Z remote: Counting objects:  41% (70/169)        
2023-04-10T02:36:47.3522502Z remote: Counting objects:  42% (71/169)        
2023-04-10T02:36:47.3523049Z remote: Counting objects:  43% (73/169)        
2023-04-10T02:36:47.3523775Z remote: Counting objects:  44% (75/169)        
2023-04-10T02:36:47.3524291Z remote: Counting objects:  45% (77/169)        
2023-04-10T02:36:47.3525092Z remote: Counting objects:  46% (78/169)        
2023-04-10T02:36:47.3525630Z remote: Counting objects:  47% (80/169)        
2023-04-10T02:36:47.3526373Z remote: Counting objects:  48% (82/169)        
2023-04-10T02:36:47.3526900Z remote: Counting objects:  49% (83/169)        
2023-04-10T02:36:47.3527655Z remote: Counting objects:  50% (85/169)        
2023-04-10T02:36:47.3528180Z remote: Counting objects:  51% (87/169)        
2023-04-10T02:36:47.3529145Z remote: Counting objects:  52% (88/169)        
2023-04-10T02:36:47.3529691Z remote: Counting objects:  53% (90/169)        
2023-04-10T02:36:47.3530438Z remote: Counting objects:  54% (92/169)        
2023-04-10T02:36:47.3530937Z remote: Counting objects:  55% (93/169)        
2023-04-10T02:36:47.3531671Z remote: Counting objects:  56% (95/169)        
2023-04-10T02:36:47.3532218Z remote: Counting objects:  57% (97/169)        
2023-04-10T02:36:47.3532954Z remote: Counting objects:  58% (99/169)        
2023-04-10T02:36:47.3533604Z remote: Counting objects:  59% (100/169)        
2023-04-10T02:36:47.3534374Z remote: Counting objects:  60% (102/169)        
2023-04-10T02:36:47.3534903Z remote: Counting objects:  61% (104/169)        
2023-04-10T02:36:47.3535690Z remote: Counting objects:  62% (105/169)        
2023-04-10T02:36:47.3536236Z remote: Counting objects:  63% (107/169)        
2023-04-10T02:36:47.3537337Z remote: Counting objects:  64% (109/169)        
2023-04-10T02:36:47.3538176Z remote: Counting objects:  65% (110/169)        
2023-04-10T02:36:47.3538521Z remote: Counting objects:  66% (112/169)        
2023-04-10T02:36:47.3538833Z remote: Counting objects:  67% (114/169)        
2023-04-10T02:36:47.3539155Z remote: Counting objects:  68% (115/169)        
2023-04-10T02:36:47.3539481Z remote: Counting objects:  69% (117/169)        
2023-04-10T02:36:47.3540279Z remote: Counting objects:  70% (119/169)        
2023-04-10T02:36:47.3540606Z remote: Counting objects:  71% (120/169)        
2023-04-10T02:36:47.3540925Z remote: Counting objects:  72% (122/169)        
2023-04-10T02:36:47.3541587Z remote: Counting objects:  73% (124/169)        
2023-04-10T02:36:47.3542614Z remote: Counting objects:  74% (126/169)        
2023-04-10T02:36:47.3543317Z remote: Counting objects:  75% (127/169)        
2023-04-10T02:36:47.3544228Z remote: Counting objects:  76% (129/169)        
2023-04-10T02:36:47.3544893Z remote: Counting objects:  77% (131/169)        
2023-04-10T02:36:47.3548710Z remote: Counting objects:  78% (132/169)        
2023-04-10T02:36:47.3549086Z remote: Counting objects:  79% (134/169)        
2023-04-10T02:36:47.3549421Z remote: Counting objects:  80% (136/169)        
2023-04-10T02:36:47.3549731Z remote: Counting objects:  81% (137/169)        
2023-04-10T02:36:47.3550052Z remote: Counting objects:  82% (139/169)        
2023-04-10T02:36:47.3550381Z remote: Counting objects:  83% (141/169)        
2023-04-10T02:36:47.3550687Z remote: Counting objects:  84% (142/169)        
2023-04-10T02:36:47.3551006Z remote: Counting objects:  85% (144/169)        
2023-04-10T02:36:47.3551747Z remote: Counting objects:  86% (146/169)        
2023-04-10T02:36:47.3552071Z remote: Counting objects:  87% (148/169)        
2023-04-10T02:36:47.3552380Z remote: Counting objects:  88% (149/169)        
2023-04-10T02:36:47.3552710Z remote: Counting objects:  89% (151/169)        
2023-04-10T02:36:47.3553029Z remote: Counting objects:  90% (153/169)        
2023-04-10T02:36:47.3553336Z remote: Counting objects:  91% (154/169)        
2023-04-10T02:36:47.3553663Z remote: Counting objects:  92% (156/169)        
2023-04-10T02:36:47.3553984Z remote: Counting objects:  93% (158/169)        
2023-04-10T02:36:47.3554288Z remote: Counting objects:  94% (159/169)        
2023-04-10T02:36:47.3554606Z remote: Counting objects:  95% (161/169)        
2023-04-10T02:36:47.3554924Z remote: Counting objects:  96% (163/169)        
2023-04-10T02:36:47.3555232Z remote: Counting objects:  97% (164/169)        
2023-04-10T02:36:47.3555554Z remote: Counting objects:  98% (166/169)        
2023-04-10T02:36:47.3555868Z remote: Counting objects:  99% (168/169)        
2023-04-10T02:36:47.3556187Z remote: Counting objects: 100% (169/169)        
2023-04-10T02:36:47.3556508Z remote: Counting objects: 100% (169/169), done.        
2023-04-10T02:36:47.3556877Z remote: Compressing objects:   0% (1/151)        
2023-04-10T02:36:47.3557223Z remote: Compressing objects:   1% (2/151)        
2023-04-10T02:36:47.3557547Z remote: Compressing objects:   2% (4/151)        
2023-04-10T02:36:47.3558131Z remote: Compressing objects:   3% (5/151)        
2023-04-10T02:36:47.3558474Z remote: Compressing objects:   4% (7/151)        
2023-04-10T02:36:47.3558794Z remote: Compressing objects:   5% (8/151)        
2023-04-10T02:36:47.3559137Z remote: Compressing objects:   6% (10/151)        
2023-04-10T02:36:47.3559484Z remote: Compressing objects:   7% (11/151)        
2023-04-10T02:36:47.3559811Z remote: Compressing objects:   8% (13/151)        
2023-04-10T02:36:47.3560152Z remote: Compressing objects:   9% (14/151)        
2023-04-10T02:36:47.3560494Z remote: Compressing objects:  10% (16/151)        
2023-04-10T02:36:47.3560832Z remote: Compressing objects:  11% (17/151)        
2023-04-10T02:36:47.3561150Z remote: Compressing objects:  12% (19/151)        
2023-04-10T02:36:47.3561499Z remote: Compressing objects:  13% (20/151)        
2023-04-10T02:36:47.3561839Z remote: Compressing objects:  14% (22/151)        
2023-04-10T02:36:47.3562160Z remote: Compressing objects:  15% (23/151)        
2023-04-10T02:36:47.3562502Z remote: Compressing objects:  16% (25/151)        
2023-04-10T02:36:47.3562839Z remote: Compressing objects:  17% (26/151)        
2023-04-10T02:36:47.3563934Z remote: Compressing objects:  18% (28/151)        
2023-04-10T02:36:47.3564261Z remote: Compressing objects:  19% (29/151)        
2023-04-10T02:36:47.3564596Z remote: Compressing objects:  20% (31/151)        
2023-04-10T02:36:47.3564930Z remote: Compressing objects:  21% (32/151)        
2023-04-10T02:36:47.3565246Z remote: Compressing objects:  22% (34/151)        
2023-04-10T02:36:47.3565583Z remote: Compressing objects:  23% (35/151)        
2023-04-10T02:36:47.3565916Z remote: Compressing objects:  24% (37/151)        
2023-04-10T02:36:47.3566397Z remote: Compressing objects:  25% (38/151)        
2023-04-10T02:36:47.3566715Z remote: Compressing objects:  26% (40/151)        
2023-04-10T02:36:47.3567050Z remote: Compressing objects:  27% (41/151)        
2023-04-10T02:36:47.3567393Z remote: Compressing objects:  28% (43/151)        
2023-04-10T02:36:47.3567710Z remote: Compressing objects:  29% (44/151)        
2023-04-10T02:36:47.3568075Z remote: Compressing objects:  30% (46/151)        
2023-04-10T02:36:47.3568410Z remote: Compressing objects:  31% (47/151)        
2023-04-10T02:36:47.3568727Z remote: Compressing objects:  32% (49/151)        
2023-04-10T02:36:47.3569066Z remote: Compressing objects:  33% (50/151)        
2023-04-10T02:36:47.3569399Z remote: Compressing objects:  34% (52/151)        
2023-04-10T02:36:47.3569717Z remote: Compressing objects:  35% (53/151)        
2023-04-10T02:36:47.3570048Z remote: Compressing objects:  36% (55/151)        
2023-04-10T02:36:47.3570384Z remote: Compressing objects:  37% (56/151)        
2023-04-10T02:36:47.3570723Z remote: Compressing objects:  38% (58/151)        
2023-04-10T02:36:47.3571038Z remote: Compressing objects:  39% (59/151)        
2023-04-10T02:36:47.3571371Z remote: Compressing objects:  40% (61/151)        
2023-04-10T02:36:47.3571708Z remote: Compressing objects:  41% (62/151)        
2023-04-10T02:36:47.3572027Z remote: Compressing objects:  42% (64/151)        
2023-04-10T02:36:47.3572363Z remote: Compressing objects:  43% (65/151)        
2023-04-10T02:36:47.3572694Z remote: Compressing objects:  44% (67/151)        
2023-04-10T02:36:47.3573014Z remote: Compressing objects:  45% (68/151)        
2023-04-10T02:36:47.3573616Z remote: Compressing objects:  46% (70/151)        
2023-04-10T02:36:47.3573955Z remote: Compressing objects:  47% (71/151)        
2023-04-10T02:36:47.3574288Z remote: Compressing objects:  48% (73/151)        
2023-04-10T02:36:47.3574605Z remote: Compressing objects:  49% (74/151)        
2023-04-10T02:36:47.3574939Z remote: Compressing objects:  50% (76/151)        
2023-04-10T02:36:47.3575288Z remote: Compressing objects:  51% (78/151)        
2023-04-10T02:36:47.3575610Z remote: Compressing objects:  52% (79/151)        
2023-04-10T02:36:47.3575945Z remote: Compressing objects:  53% (81/151)        
2023-04-10T02:36:47.3576427Z remote: Compressing objects:  54% (82/151)        
2023-04-10T02:36:47.3576750Z remote: Compressing objects:  55% (84/151)        
2023-04-10T02:36:47.3577087Z remote: Compressing objects:  56% (85/151)        
2023-04-10T02:36:47.3577422Z remote: Compressing objects:  57% (87/151)        
2023-04-10T02:36:47.3577738Z remote: Compressing objects:  58% (88/151)        
2023-04-10T02:36:47.3578074Z remote: Compressing objects:  59% (90/151)        
2023-04-10T02:36:47.3578411Z remote: Compressing objects:  60% (91/151)        
2023-04-10T02:36:47.3578747Z remote: Compressing objects:  61% (93/151)        
2023-04-10T02:36:47.3579060Z remote: Compressing objects:  62% (94/151)        
2023-04-10T02:36:47.3579397Z remote: Compressing objects:  63% (96/151)        
2023-04-10T02:36:47.3579739Z remote: Compressing objects:  64% (97/151)        
2023-04-10T02:36:47.3580056Z remote: Compressing objects:  65% (99/151)        
2023-04-10T02:36:47.3580398Z remote: Compressing objects:  66% (100/151)        
2023-04-10T02:36:47.3580755Z remote: Compressing objects:  67% (102/151)        
2023-04-10T02:36:47.3581087Z remote: Compressing objects:  68% (103/151)        
2023-04-10T02:36:47.3597247Z remote: Compressing objects:  69% (105/151)        
2023-04-10T02:36:47.3597608Z remote: Compressing objects:  70% (106/151)        
2023-04-10T02:36:47.3600241Z remote: Compressing objects:  71% (108/151)        
2023-04-10T02:36:47.3600572Z remote: Compressing objects:  72% (109/151)        
2023-04-10T02:36:47.3600913Z remote: Compressing objects:  73% (111/151)        
2023-04-10T02:36:47.3602609Z remote: Compressing objects:  74% (112/151)        
2023-04-10T02:36:47.3602943Z remote: Compressing objects:  75% (114/151)        
2023-04-10T02:36:47.3604489Z remote: Compressing objects:  76% (115/151)        
2023-04-10T02:36:47.3605443Z remote: Compressing objects:  77% (117/151)        
2023-04-10T02:36:47.3605796Z remote: Compressing objects:  78% (118/151)        
2023-04-10T02:36:47.3606487Z remote: Compressing objects:  79% (120/151)        
2023-04-10T02:36:47.3607667Z remote: Compressing objects:  80% (121/151)        
2023-04-10T02:36:47.3608013Z remote: Compressing objects:  81% (123/151)        
2023-04-10T02:36:47.3608337Z remote: Compressing objects:  82% (124/151)        
2023-04-10T02:36:47.3609041Z remote: Compressing objects:  83% (126/151)        
2023-04-10T02:36:47.3609383Z remote: Compressing objects:  84% (127/151)        
2023-04-10T02:36:47.3610169Z remote: Compressing objects:  85% (129/151)        
2023-04-10T02:36:47.3610495Z remote: Compressing objects:  86% (130/151)        
2023-04-10T02:36:47.3610831Z remote: Compressing objects:  87% (132/151)        
2023-04-10T02:36:47.3611172Z remote: Compressing objects:  88% (133/151)        
2023-04-10T02:36:47.3611502Z remote: Compressing objects:  89% (135/151)        
2023-04-10T02:36:47.3611837Z remote: Compressing objects:  90% (136/151)        
2023-04-10T02:36:47.3612187Z remote: Compressing objects:  91% (138/151)        
2023-04-10T02:36:47.3612528Z remote: Compressing objects:  92% (139/151)        
2023-04-10T02:36:47.3612861Z remote: Compressing objects:  93% (141/151)        
2023-04-10T02:36:47.3613304Z remote: Compressing objects:  94% (142/151)        
2023-04-10T02:36:47.3613643Z remote: Compressing objects:  95% (144/151)        
2023-04-10T02:36:47.3613979Z remote: Compressing objects:  96% (145/151)        
2023-04-10T02:36:47.3614317Z remote: Compressing objects:  97% (147/151)        
2023-04-10T02:36:47.3614637Z remote: Compressing objects:  98% (148/151)        
2023-04-10T02:36:47.3614974Z remote: Compressing objects:  99% (150/151)        
2023-04-10T02:36:47.3615309Z remote: Compressing objects: 100% (151/151)        
2023-04-10T02:36:47.3615645Z remote: Compressing objects: 100% (151/151), done.        
2023-04-10T02:36:47.3662348Z Receiving objects:   0% (1/169)
2023-04-10T02:36:47.3662951Z Receiving objects:   1% (2/169)
2023-04-10T02:36:47.3665048Z Receiving objects:   2% (4/169)
2023-04-10T02:36:47.3665643Z Receiving objects:   3% (6/169)
2023-04-10T02:36:47.3667909Z Receiving objects:   4% (7/169)
2023-04-10T02:36:47.3691102Z Receiving objects:   5% (9/169)
2023-04-10T02:36:47.3691690Z Receiving objects:   6% (11/169)
2023-04-10T02:36:47.3692447Z Receiving objects:   7% (12/169)
2023-04-10T02:36:47.3692942Z Receiving objects:   8% (14/169)
2023-04-10T02:36:47.3693881Z Receiving objects:   9% (16/169)
2023-04-10T02:36:47.3694359Z Receiving objects:  10% (17/169)
2023-04-10T02:36:47.3695071Z Receiving objects:  11% (19/169)
2023-04-10T02:36:47.3695552Z Receiving objects:  12% (21/169)
2023-04-10T02:36:47.3696242Z Receiving objects:  13% (22/169)
2023-04-10T02:36:47.3696725Z Receiving objects:  14% (24/169)
2023-04-10T02:36:47.3697427Z Receiving objects:  15% (26/169)
2023-04-10T02:36:47.3697922Z Receiving objects:  16% (28/169)
2023-04-10T02:36:47.4025627Z Receiving objects:  17% (29/169)
2023-04-10T02:36:47.4026234Z Receiving objects:  18% (31/169)
2023-04-10T02:36:47.4027062Z Receiving objects:  19% (33/169)
2023-04-10T02:36:47.4027565Z Receiving objects:  20% (34/169)
2023-04-10T02:36:47.4030242Z Receiving objects:  21% (36/169)
2023-04-10T02:36:47.4030794Z Receiving objects:  22% (38/169)
2023-04-10T02:36:47.4031522Z Receiving objects:  23% (39/169)
2023-04-10T02:36:47.4032002Z Receiving objects:  24% (41/169)
2023-04-10T02:36:47.4032754Z Receiving objects:  25% (43/169)
2023-04-10T02:36:47.4036394Z Receiving objects:  26% (44/169)
2023-04-10T02:36:47.4039571Z Receiving objects:  27% (46/169)
2023-04-10T02:36:47.4042337Z Receiving objects:  28% (48/169)
2023-04-10T02:36:47.4042903Z Receiving objects:  29% (50/169)
2023-04-10T02:36:47.4044709Z Receiving objects:  30% (51/169)
2023-04-10T02:36:47.4056970Z Receiving objects:  31% (53/169)
2023-04-10T02:36:47.4057590Z Receiving objects:  32% (55/169)
2023-04-10T02:36:47.4072219Z Receiving objects:  33% (56/169)
2023-04-10T02:36:47.4072813Z Receiving objects:  34% (58/169)
2023-04-10T02:36:47.4073880Z Receiving objects:  35% (60/169)
2023-04-10T02:36:47.4076213Z Receiving objects:  36% (61/169)
2023-04-10T02:36:47.4077719Z Receiving objects:  37% (63/169)
2023-04-10T02:36:47.4082084Z Receiving objects:  38% (65/169)
2023-04-10T02:36:47.4082727Z Receiving objects:  39% (66/169)
2023-04-10T02:36:47.4085588Z Receiving objects:  40% (68/169)
2023-04-10T02:36:47.4086201Z Receiving objects:  41% (70/169)
2023-04-10T02:36:47.4087763Z Receiving objects:  42% (71/169)
2023-04-10T02:36:47.4088292Z Receiving objects:  43% (73/169)
2023-04-10T02:36:47.4092173Z Receiving objects:  44% (75/169)
2023-04-10T02:36:47.4092700Z Receiving objects:  45% (77/169)
2023-04-10T02:36:47.4096398Z Receiving objects:  46% (78/169)
2023-04-10T02:36:47.4096990Z Receiving objects:  47% (80/169)
2023-04-10T02:36:47.4097797Z Receiving objects:  48% (82/169)
2023-04-10T02:36:47.4098321Z Receiving objects:  49% (83/169)
2023-04-10T02:36:47.4099128Z Receiving objects:  50% (85/169)
2023-04-10T02:36:47.4099647Z Receiving objects:  51% (87/169)
2023-04-10T02:36:47.4100375Z Receiving objects:  52% (88/169)
2023-04-10T02:36:47.4100898Z Receiving objects:  53% (90/169)
2023-04-10T02:36:47.4101634Z Receiving objects:  54% (92/169)
2023-04-10T02:36:47.4102164Z Receiving objects:  55% (93/169)
2023-04-10T02:36:47.4102868Z Receiving objects:  56% (95/169)
2023-04-10T02:36:47.4103345Z Receiving objects:  57% (97/169)
2023-04-10T02:36:47.4104045Z Receiving objects:  58% (99/169)
2023-04-10T02:36:47.4104597Z Receiving objects:  59% (100/169)
2023-04-10T02:36:47.4105322Z Receiving objects:  60% (102/169)
2023-04-10T02:36:47.4105805Z Receiving objects:  61% (104/169)
2023-04-10T02:36:47.4106508Z Receiving objects:  62% (105/169)
2023-04-10T02:36:47.4106973Z Receiving objects:  63% (107/169)
2023-04-10T02:36:47.4107674Z Receiving objects:  64% (109/169)
2023-04-10T02:36:47.4108154Z Receiving objects:  65% (110/169)
2023-04-10T02:36:47.4108862Z Receiving objects:  66% (112/169)
2023-04-10T02:36:47.4109442Z Receiving objects:  67% (114/169)
2023-04-10T02:36:47.4110090Z Receiving objects:  68% (115/169)
2023-04-10T02:36:47.4110535Z Receiving objects:  69% (117/169)
2023-04-10T02:36:47.4111425Z Receiving objects:  70% (119/169)
2023-04-10T02:36:47.4111910Z Receiving objects:  71% (120/169)
2023-04-10T02:36:47.4112565Z Receiving objects:  72% (122/169)
2023-04-10T02:36:47.4113012Z Receiving objects:  73% (124/169)
2023-04-10T02:36:47.4113643Z Receiving objects:  74% (126/169)
2023-04-10T02:36:47.4114084Z Receiving objects:  75% (127/169)
2023-04-10T02:36:47.4114730Z Receiving objects:  76% (129/169)
2023-04-10T02:36:47.4115156Z Receiving objects:  77% (131/169)
2023-04-10T02:36:47.4115814Z Receiving objects:  78% (132/169)
2023-04-10T02:36:47.4116254Z Receiving objects:  79% (134/169)
2023-04-10T02:36:47.4116899Z Receiving objects:  80% (136/169)
2023-04-10T02:36:47.4117326Z Receiving objects:  81% (137/169)
2023-04-10T02:36:47.4117981Z Receiving objects:  82% (139/169)
2023-04-10T02:36:47.4118426Z Receiving objects:  83% (141/169)
2023-04-10T02:36:47.4119067Z Receiving objects:  84% (142/169)
2023-04-10T02:36:47.4119684Z Receiving objects:  85% (144/169)
2023-04-10T02:36:47.4120418Z Receiving objects:  86% (146/169)
2023-04-10T02:36:47.4120896Z Receiving objects:  87% (148/169)
2023-04-10T02:36:47.4121576Z Receiving objects:  88% (149/169)
2023-04-10T02:36:47.4122065Z Receiving objects:  89% (151/169)
2023-04-10T02:36:47.4122759Z Receiving objects:  90% (153/169)
2023-04-10T02:36:47.4123235Z Receiving objects:  91% (154/169)
2023-04-10T02:36:47.4123911Z Receiving objects:  92% (156/169)
2023-04-10T02:36:47.4124384Z Receiving objects:  93% (158/169)
2023-04-10T02:36:47.4125091Z Receiving objects:  94% (159/169)
2023-04-10T02:36:47.4125550Z Receiving objects:  95% (161/169)
2023-04-10T02:36:47.4126253Z Receiving objects:  96% (163/169)
2023-04-10T02:36:47.4129736Z Receiving objects:  97% (164/169)
2023-04-10T02:36:47.4130895Z remote: Total 169 (delta 18), reused 115 (delta 7), pack-reused 0        
2023-04-10T02:36:47.4170874Z Receiving objects:  98% (166/169)
2023-04-10T02:36:47.4175738Z Receiving objects:  99% (168/169)
2023-04-10T02:36:47.4176392Z Receiving objects: 100% (169/169)
2023-04-10T02:36:47.4178600Z Receiving objects: 100% (169/169), 993.20 KiB | 19.10 MiB/s, done.
2023-04-10T02:36:47.4183337Z Resolving deltas:   0% (0/18)
2023-04-10T02:36:47.4183913Z Resolving deltas:   5% (1/18)
2023-04-10T02:36:47.4185056Z Resolving deltas:  11% (2/18)
2023-04-10T02:36:47.4186172Z Resolving deltas:  16% (3/18)
2023-04-10T02:36:47.4188127Z Resolving deltas:  22% (4/18)
2023-04-10T02:36:47.4188579Z Resolving deltas:  27% (5/18)
2023-04-10T02:36:47.4189423Z Resolving deltas:  33% (6/18)
2023-04-10T02:36:47.4190211Z Resolving deltas:  38% (7/18)
2023-04-10T02:36:47.4190920Z Resolving deltas:  44% (8/18)
2023-04-10T02:36:47.4191524Z Resolving deltas:  50% (9/18)
2023-04-10T02:36:47.4192225Z Resolving deltas:  55% (10/18)
2023-04-10T02:36:47.4192819Z Resolving deltas:  61% (11/18)
2023-04-10T02:36:47.4193548Z Resolving deltas:  66% (12/18)
2023-04-10T02:36:47.4194346Z Resolving deltas:  72% (13/18)
2023-04-10T02:36:47.4194952Z Resolving deltas:  77% (14/18)
2023-04-10T02:36:47.4195632Z Resolving deltas:  83% (15/18)
2023-04-10T02:36:47.4196326Z Resolving deltas:  88% (16/18)
2023-04-10T02:36:47.4196937Z Resolving deltas:  94% (17/18)
2023-04-10T02:36:47.4197537Z Resolving deltas: 100% (18/18)
2023-04-10T02:36:47.4198254Z Resolving deltas: 100% (18/18), done.
2023-04-10T02:36:47.4297249Z From https://github.com/CasperDash/useWallet
2023-04-10T02:36:47.4299192Z  * [new ref]         25f8ac7a84341a7485ddf7707522bda42d38972c -> origin/main
2023-04-10T02:36:47.4323739Z ##[endgroup]
2023-04-10T02:36:47.4324735Z ##[group]Determining the checkout info
2023-04-10T02:36:47.4325409Z ##[endgroup]
2023-04-10T02:36:47.4326045Z ##[group]Checking out the ref
2023-04-10T02:36:47.4331026Z [command]/usr/bin/git checkout --progress --force -B main refs/remotes/origin/main
2023-04-10T02:36:47.4561212Z Switched to a new branch 'main'
2023-04-10T02:36:47.4627176Z branch 'main' set up to track 'origin/main'.
2023-04-10T02:36:47.4628322Z ##[endgroup]
2023-04-10T02:36:47.4639657Z [command]/usr/bin/git log -1 --format='%H'
2023-04-10T02:36:47.4673320Z '25f8ac7a84341a7485ddf7707522bda42d38972c'
2023-04-10T02:36:47.5046607Z ##[group]Run pnpm/action-setup@v2.2.4
2023-04-10T02:36:47.5046931Z with:
2023-04-10T02:36:47.5047147Z   version: 7.26.3
2023-04-10T02:36:47.5047398Z   dest: ~/setup-pnpm
2023-04-10T02:36:47.5047650Z   run_install: null
2023-04-10T02:36:47.5047874Z ##[endgroup]
2023-04-10T02:36:47.6513368Z ##[group]Running self-installer...
2023-04-10T02:36:48.1751684Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:36:48.1883869Z Packages: +1
2023-04-10T02:36:48.1885068Z +
2023-04-10T02:36:48.9697326Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:36:48.9698035Z   Content-addressable store is at: /home/runner/.pnpm-store/v3
2023-04-10T02:36:48.9698447Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:36:49.0037746Z 
2023-04-10T02:36:49.0038097Z dependencies:
2023-04-10T02:36:49.0038414Z + pnpm 7.26.3 (8.2.0 is available)
2023-04-10T02:36:49.0038593Z 
2023-04-10T02:36:49.1828436Z Progress: resolved 1, reused 0, downloaded 1, added 1, done
2023-04-10T02:36:49.1924935Z ##[endgroup]
2023-04-10T02:36:49.1929157Z Installation Completed!
2023-04-10T02:36:49.2083666Z ##[group]Run actions/setup-node@v3
2023-04-10T02:36:49.2083952Z with:
2023-04-10T02:36:49.2084175Z   cache: pnpm
2023-04-10T02:36:49.2084401Z   node-version: 18
2023-04-10T02:36:49.2084650Z   always-auth: false
2023-04-10T02:36:49.2084907Z   check-latest: false
2023-04-10T02:36:49.2085380Z   token: ***
2023-04-10T02:36:49.2085597Z env:
2023-04-10T02:36:49.2085900Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:49.2086207Z ##[endgroup]
2023-04-10T02:36:49.4558643Z Found in cache @ /opt/hostedtoolcache/node/18.15.0/x64
2023-04-10T02:36:49.4562088Z ##[group]Environment details
2023-04-10T02:36:50.4949866Z node: v18.15.0
2023-04-10T02:36:50.4950604Z npm: 9.5.0
2023-04-10T02:36:50.4951512Z yarn: 1.22.19
2023-04-10T02:36:50.4952574Z ##[endgroup]
2023-04-10T02:36:50.4965788Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm store path --silent
2023-04-10T02:36:51.0801190Z /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:36:51.1847426Z pnpm cache is not found
2023-04-10T02:36:51.3003803Z ##[group]Run actions/cache@v3
2023-04-10T02:36:51.3004089Z with:
2023-04-10T02:36:51.3004327Z   path: ~/.pnpm-store
2023-04-10T02:36:51.3004683Z   key: pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:36:51.3005048Z   restore-keys: pnpm-
2023-04-10T02:36:51.3005332Z   enableCrossOsArchive: false
2023-04-10T02:36:51.3005614Z   fail-on-cache-miss: false
2023-04-10T02:36:51.3005886Z   lookup-only: false
2023-04-10T02:36:51.3006117Z env:
2023-04-10T02:36:51.3006432Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:51.3006724Z ##[endgroup]
2023-04-10T02:36:51.5506370Z Cache not found for input keys: pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8, pnpm-
2023-04-10T02:36:51.6485599Z ##[group]Run actions/cache@v3
2023-04-10T02:36:51.6486026Z with:
2023-04-10T02:36:51.6486438Z   path: node_modules
docs/node_modules
examples/**/node_modules
packages/**/node_modules
packages/**/dist

2023-04-10T02:36:51.6487045Z   key: modules-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:36:51.6487525Z   enableCrossOsArchive: false
2023-04-10T02:36:51.6487843Z   fail-on-cache-miss: false
2023-04-10T02:36:51.6488227Z   lookup-only: false
2023-04-10T02:36:51.6488552Z env:
2023-04-10T02:36:51.6488928Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:51.6489262Z ##[endgroup]
2023-04-10T02:36:51.8920546Z Cache not found for input keys: modules-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:36:51.9099630Z ##[group]Run pnpm i
2023-04-10T02:36:51.9100064Z [36;1mpnpm i[0m
2023-04-10T02:36:51.9165780Z shell: /usr/bin/bash -e {0}
2023-04-10T02:36:51.9166092Z env:
2023-04-10T02:36:51.9166499Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:51.9167006Z ##[endgroup]
2023-04-10T02:36:52.5719395Z Scope: all 5 workspace projects
2023-04-10T02:36:52.6723274Z Lockfile is up to date, resolution step is skipped
2023-04-10T02:36:52.7931439Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:36:53.0783948Z Packages: +1012
2023-04-10T02:36:53.0784847Z ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2023-04-10T02:36:53.6733051Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:36:53.6735288Z   Content-addressable store is at: /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:36:53.6735927Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:36:53.7961388Z Progress: resolved 1012, reused 0, downloaded 11, added 4
2023-04-10T02:36:54.7971326Z Progress: resolved 1012, reused 0, downloaded 67, added 62
2023-04-10T02:36:55.7969713Z Progress: resolved 1012, reused 0, downloaded 137, added 134
2023-04-10T02:36:56.8034720Z Progress: resolved 1012, reused 0, downloaded 216, added 216
2023-04-10T02:36:57.8059715Z Progress: resolved 1012, reused 0, downloaded 268, added 265
2023-04-10T02:36:58.8211066Z Progress: resolved 1012, reused 0, downloaded 333, added 331
2023-04-10T02:36:59.8200296Z Progress: resolved 1012, reused 0, downloaded 401, added 399
2023-04-10T02:37:00.8201042Z Progress: resolved 1012, reused 0, downloaded 477, added 477
2023-04-10T02:37:01.8259708Z Progress: resolved 1012, reused 0, downloaded 522, added 520
2023-04-10T02:37:02.8260651Z Progress: resolved 1012, reused 0, downloaded 579, added 581
2023-04-10T02:37:03.8358357Z Progress: resolved 1012, reused 0, downloaded 671, added 674
2023-04-10T02:37:04.8404906Z Progress: resolved 1012, reused 0, downloaded 730, added 731
2023-04-10T02:37:05.8433094Z Progress: resolved 1012, reused 0, downloaded 806, added 806
2023-04-10T02:37:06.8497562Z Progress: resolved 1012, reused 0, downloaded 889, added 888
2023-04-10T02:37:07.8528817Z Progress: resolved 1012, reused 0, downloaded 960, added 960
2023-04-10T02:37:08.8540317Z Progress: resolved 1012, reused 0, downloaded 1000, added 1004
2023-04-10T02:37:09.8574363Z Progress: resolved 1012, reused 0, downloaded 1002, added 1006
2023-04-10T02:37:10.9050094Z Progress: resolved 1012, reused 0, downloaded 1003, added 1007
2023-04-10T02:37:11.9058354Z Progress: resolved 1012, reused 0, downloaded 1005, added 1009
2023-04-10T02:37:13.1549358Z Progress: resolved 1012, reused 0, downloaded 1006, added 1010
2023-04-10T02:37:14.1751471Z Progress: resolved 1012, reused 0, downloaded 1008, added 1012, done
2023-04-10T02:37:14.8064412Z .../@napi-rs/simple-git-linux-x64-gnu postinstall$ node install.js
2023-04-10T02:37:14.8069673Z .../@napi-rs/simple-git-linux-x64-musl postinstall$ node install.js
2023-04-10T02:37:14.8532610Z .../node_modules/secp256k1 install$ npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."
2023-04-10T02:37:14.8816107Z .../keccak@3.0.3/node_modules/keccak install$ node-gyp-build || exit 0
2023-04-10T02:37:14.8832895Z .../node_modules/secp256k1 install$ node-gyp-build || exit 0
2023-04-10T02:37:14.9070824Z .../@napi-rs/simple-git-linux-x64-gnu postinstall: Done
2023-04-10T02:37:14.9851326Z .../@napi-rs/simple-git-linux-x64-musl postinstall: Failed
2023-04-10T02:37:15.2375873Z .../keccak@3.0.3/node_modules/keccak install: Done
2023-04-10T02:37:15.2553994Z .../node_modules/secp256k1 install: Done
2023-04-10T02:37:15.5186305Z .../node_modules/secp256k1 install: > secp256k1@3.7.1 rebuild
2023-04-10T02:37:15.5187837Z .../node_modules/secp256k1 install: > node-gyp rebuild
2023-04-10T02:37:15.6397639Z .../node_modules/secp256k1 install: gyp info it worked if it ends with ok
2023-04-10T02:37:15.6420070Z .../node_modules/secp256k1 install: gyp info using node-gyp@9.3.1
2023-04-10T02:37:15.6420929Z .../node_modules/secp256k1 install: gyp info using node@18.15.0 | linux | x64
2023-04-10T02:37:15.7636318Z .../node_modules/secp256k1 install: gyp info find Python using Python version 3.10.6 found at "/usr/bin/python3"
2023-04-10T02:37:15.9223912Z .../node_modules/secp256k1 install: gyp http GET https://nodejs.org/download/release/v18.15.0/node-v18.15.0-headers.tar.gz
2023-04-10T02:37:16.0175975Z .../node_modules/secp256k1 install: gyp http 200 https://nodejs.org/download/release/v18.15.0/node-v18.15.0-headers.tar.gz
2023-04-10T02:37:17.7836378Z .../node_modules/secp256k1 install: gyp http GET https://nodejs.org/download/release/v18.15.0/SHASUMS256.txt
2023-04-10T02:37:17.8018780Z .../node_modules/secp256k1 install: gyp http 200 https://nodejs.org/download/release/v18.15.0/SHASUMS256.txt
2023-04-10T02:37:17.8085078Z .../node_modules/secp256k1 install: gyp info spawn /usr/bin/python3
2023-04-10T02:37:17.8112912Z .../node_modules/secp256k1 install: gyp info spawn args [
2023-04-10T02:37:17.8114211Z .../node_modules/secp256k1 install: gyp info spawn args   '/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py',
2023-04-10T02:37:17.8115090Z .../node_modules/secp256k1 install: gyp info spawn args   'binding.gyp',
2023-04-10T02:37:17.8115791Z .../node_modules/secp256k1 install: gyp info spawn args   '-f',
2023-04-10T02:37:17.8116478Z .../node_modules/secp256k1 install: gyp info spawn args   'make',
2023-04-10T02:37:17.8117150Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:17.8118234Z .../node_modules/secp256k1 install: gyp info spawn args   '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build/config.gypi',
2023-04-10T02:37:17.8119065Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:17.8120121Z .../node_modules/secp256k1 install: gyp info spawn args   '/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/addon.gypi',
2023-04-10T02:37:17.8121312Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:17.8122232Z .../node_modules/secp256k1 install: gyp info spawn args   '/home/runner/.cache/node-gyp/18.15.0/include/node/common.gypi',
2023-04-10T02:37:17.8123069Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dlibrary=shared_library',
2023-04-10T02:37:17.8123848Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dvisibility=default',
2023-04-10T02:37:17.8124710Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_root_dir=/home/runner/.cache/node-gyp/18.15.0',
2023-04-10T02:37:17.8125790Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_gyp_dir=/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp',
2023-04-10T02:37:17.8126846Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_lib_file=/home/runner/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
2023-04-10T02:37:17.8128008Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dmodule_root_dir=/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1',
2023-04-10T02:37:17.8128872Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_engine=v8',
2023-04-10T02:37:17.8129581Z .../node_modules/secp256k1 install: gyp info spawn args   '--depth=.',
2023-04-10T02:37:17.8130295Z .../node_modules/secp256k1 install: gyp info spawn args   '--no-parallel',
2023-04-10T02:37:17.8131026Z .../node_modules/secp256k1 install: gyp info spawn args   '--generator-output',
2023-04-10T02:37:17.8131728Z .../node_modules/secp256k1 install: gyp info spawn args   'build',
2023-04-10T02:37:17.8132437Z .../node_modules/secp256k1 install: gyp info spawn args   '-Goutput_dir=.'
2023-04-10T02:37:17.8133013Z .../node_modules/secp256k1 install: gyp info spawn args ]
2023-04-10T02:37:18.0513092Z .../node_modules/secp256k1 install: gyp info spawn make
2023-04-10T02:37:18.0521496Z .../node_modules/secp256k1 install: gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
2023-04-10T02:37:18.0527543Z .../node_modules/secp256k1 install: make: Entering directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build'
2023-04-10T02:37:18.0548436Z .../node_modules/secp256k1 install:   CXX(target) Release/obj.target/secp256k1/src/addon.o
2023-04-10T02:37:19.1308491Z .../node_modules/secp256k1 install: In file included from ../src/addon.cc:2:
2023-04-10T02:37:19.1311186Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2023-04-10T02:37:19.1313050Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2298:7: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2023-04-10T02:37:19.1314125Z .../node_modules/secp256k1 install:  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2023-04-10T02:37:19.1314837Z .../node_modules/secp256k1 install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:19.1335378Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::SetAccessor(v8::Local<v8::ObjectTemplate>, v8::Local<v8::String>, Nan::GetterCallback, Nan::SetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, Nan::imp::Sig)’:
2023-04-10T02:37:19.1342148Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2536:19: warning: ‘void v8::ObjectTemplate::SetAccessor(v8::Local<v8::Name>, v8::AccessorNameGetterCallback, v8::AccessorNameSetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, v8::Local<v8::AccessorSignature>, v8::SideEffectType, v8::SideEffectType)’ is deprecated: Do signature check in accessor [-Wdeprecated-declarations]
2023-04-10T02:37:19.1346580Z .../node_modules/secp256k1 install:  2536 |   tpl->SetAccessor(
2023-04-10T02:37:19.1349444Z .../node_modules/secp256k1 install:       |   ~~~~~~~~~~~~~~~~^
2023-04-10T02:37:19.1352315Z .../node_modules/secp256k1 install:  2537 |       name
2023-04-10T02:37:19.1354951Z .../node_modules/secp256k1 install:       |       ~~~~         
2023-04-10T02:37:19.1357530Z .../node_modules/secp256k1 install:  2538 |     , getter_
2023-04-10T02:37:19.1360019Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~      
2023-04-10T02:37:19.1362687Z .../node_modules/secp256k1 install:  2539 |     , setter_
2023-04-10T02:37:19.1365212Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~      
2023-04-10T02:37:19.1367666Z .../node_modules/secp256k1 install:  2540 |     , obj
2023-04-10T02:37:19.1370175Z .../node_modules/secp256k1 install:       |     ~~~~~          
2023-04-10T02:37:19.1372753Z .../node_modules/secp256k1 install:  2541 |     , settings
2023-04-10T02:37:19.1375555Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~     
2023-04-10T02:37:19.1378033Z .../node_modules/secp256k1 install:  2542 |     , attribute
2023-04-10T02:37:19.1380498Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~~    
2023-04-10T02:37:19.1382965Z .../node_modules/secp256k1 install:  2543 |     , signature);
2023-04-10T02:37:19.1386451Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~~~   
2023-04-10T02:37:19.1390967Z .../node_modules/secp256k1 install: In file included from /home/runner/.cache/node-gyp/18.15.0/include/node/v8-function.h:15,
2023-04-10T02:37:19.1394846Z .../node_modules/secp256k1 install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/v8.h:33,
2023-04-10T02:37:19.1398197Z .../node_modules/secp256k1 install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:73,
2023-04-10T02:37:19.1401199Z .../node_modules/secp256k1 install:                  from ../src/addon.cc:1:
2023-04-10T02:37:19.1405157Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/v8-template.h:838:8: note: declared here
2023-04-10T02:37:19.1408195Z .../node_modules/secp256k1 install:   838 |   void SetAccessor(
2023-04-10T02:37:19.1410823Z .../node_modules/secp256k1 install:       |        ^~~~~~~~~~~
2023-04-10T02:37:19.1451374Z .../node_modules/secp256k1 install: In file included from ../../../../nan@2.14.0/node_modules/nan/nan.h:2884,
2023-04-10T02:37:19.1455160Z .../node_modules/secp256k1 install:                  from ../src/addon.cc:2:
2023-04-10T02:37:19.1458927Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h: In constructor ‘Nan::TypedArrayContents<T>::TypedArrayContents(v8::Local<v8::Value>)’:
2023-04-10T02:37:19.1462972Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h:34:43: error: ‘class v8::ArrayBuffer’ has no member named ‘GetContents’
2023-04-10T02:37:19.1466710Z .../node_modules/secp256k1 install:    34 |       data   = static_cast<char*>(buffer->GetContents().Data()) + byte_offset;
2023-04-10T02:37:19.1469631Z .../node_modules/secp256k1 install:       |                                           ^~~~~~~~~~~
2023-04-10T02:37:19.1484135Z .../node_modules/secp256k1 install: In file included from ../src/addon.cc:1:
2023-04-10T02:37:19.1484813Z .../node_modules/secp256k1 install: ../src/addon.cc: At global scope:
2023-04-10T02:37:19.1486883Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:978:7: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2023-04-10T02:37:19.1488005Z .../node_modules/secp256k1 install:   978 |       (node::addon_register_func) (regfunc),                          \
2023-04-10T02:37:19.1489026Z .../node_modules/secp256k1 install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:19.1490025Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:1012:3: note: in expansion of macro ‘NODE_MODULE_X’
2023-04-10T02:37:19.1490875Z .../node_modules/secp256k1 install:  1012 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2023-04-10T02:37:19.1491502Z .../node_modules/secp256k1 install:       |   ^~~~~~~~~~~~~
2023-04-10T02:37:19.1492297Z .../node_modules/secp256k1 install: ../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
2023-04-10T02:37:19.1493430Z .../node_modules/secp256k1 install:    50 | NODE_MODULE(secp256k1, Init)
2023-04-10T02:37:19.1494024Z .../node_modules/secp256k1 install:       | ^~~~~~~~~~~
2023-04-10T02:37:19.2414940Z .../node_modules/secp256k1 install: make: *** [secp256k1.target.mk:165: Release/obj.target/secp256k1/src/addon.o] Error 1
2023-04-10T02:37:19.2417452Z .../node_modules/secp256k1 install: gyp ERR! build error 
2023-04-10T02:37:19.2418073Z .../node_modules/secp256k1 install: gyp ERR! stack Error: `make` failed with exit code: 2
2023-04-10T02:37:19.2419367Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess.onExit (/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/lib/build.js:203:23)
2023-04-10T02:37:19.2420142Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
2023-04-10T02:37:19.2420863Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
2023-04-10T02:37:19.2421573Z .../node_modules/secp256k1 install: gyp ERR! System Linux 5.15.0-1035-azure
2023-04-10T02:37:19.2422706Z .../node_modules/secp256k1 install: gyp ERR! command "/opt/hostedtoolcache/node/18.15.0/x64/bin/node" "/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
2023-04-10T02:37:19.2424253Z .../node_modules/secp256k1 install: gyp ERR! cwd /home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1
2023-04-10T02:37:19.2424965Z .../node_modules/secp256k1 install: gyp ERR! node -v v18.15.0
2023-04-10T02:37:19.2425549Z .../node_modules/secp256k1 install: gyp ERR! node-gyp -v v9.3.1
2023-04-10T02:37:19.2426011Z .../node_modules/secp256k1 install: gyp ERR! not ok 
2023-04-10T02:37:19.2426943Z .../node_modules/secp256k1 install: make: Leaving directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build'
2023-04-10T02:37:19.2551195Z .../node_modules/secp256k1 install: Secp256k1 bindings compilation fail. Pure JS implementation will be used.
2023-04-10T02:37:19.2558860Z .../node_modules/secp256k1 install: Done
2023-04-10T02:37:19.3418259Z .../node_modules/@swc/core postinstall$ node postinstall.js
2023-04-10T02:37:19.3606359Z .../eccrypto@1.1.6/node_modules/eccrypto install$ node-gyp rebuild || exit 0
2023-04-10T02:37:19.3666998Z .../esbuild@0.15.18/node_modules/esbuild postinstall$ node install.js
2023-04-10T02:37:19.3991232Z .../esbuild@0.17.12/node_modules/esbuild postinstall$ node install.js
2023-04-10T02:37:19.4698346Z .../node_modules/@swc/core postinstall: Done
2023-04-10T02:37:19.4986680Z .../esbuild@0.17.12/node_modules/esbuild postinstall: Done
2023-04-10T02:37:19.5637736Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info it worked if it ends with ok
2023-04-10T02:37:19.5644369Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info using node-gyp@9.3.1
2023-04-10T02:37:19.5656347Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info using node@18.15.0 | linux | x64
2023-04-10T02:37:19.5760133Z .../esbuild@0.15.18/node_modules/esbuild postinstall: Done
2023-04-10T02:37:19.6739816Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info find Python using Python version 3.10.6 found at "/usr/bin/python3"
2023-04-10T02:37:19.8102587Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn /usr/bin/python3
2023-04-10T02:37:19.8103970Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args [
2023-04-10T02:37:19.8105628Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/gyp/gyp_main.py',
2023-04-10T02:37:19.8106727Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'binding.gyp',
2023-04-10T02:37:19.8107547Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-f',
2023-04-10T02:37:19.8162025Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'make',
2023-04-10T02:37:19.8162726Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:19.8163798Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build/config.gypi',
2023-04-10T02:37:19.8164614Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:19.8165683Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/addon.gypi',
2023-04-10T02:37:19.8166468Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:19.8167346Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/.cache/node-gyp/18.15.0/include/node/common.gypi',
2023-04-10T02:37:19.8168154Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dlibrary=shared_library',
2023-04-10T02:37:19.8168901Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dvisibility=default',
2023-04-10T02:37:19.8169766Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_root_dir=/home/runner/.cache/node-gyp/18.15.0',
2023-04-10T02:37:19.8171166Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_gyp_dir=/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp',
2023-04-10T02:37:19.8172242Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_lib_file=/home/runner/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
2023-04-10T02:37:19.8173523Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dmodule_root_dir=/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto',
2023-04-10T02:37:19.8174373Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_engine=v8',
2023-04-10T02:37:19.8175065Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--depth=.',
2023-04-10T02:37:19.8175770Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--no-parallel',
2023-04-10T02:37:19.8176495Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--generator-output',
2023-04-10T02:37:19.8177204Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'build',
2023-04-10T02:37:19.8177897Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Goutput_dir=.'
2023-04-10T02:37:19.8178447Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args ]
2023-04-10T02:37:19.9958290Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn make
2023-04-10T02:37:19.9966204Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: Entering directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build'
2023-04-10T02:37:19.9974849Z .../eccrypto@1.1.6/node_modules/eccrypto install:   CXX(target) Release/obj.target/ecdh/ecdh.o
2023-04-10T02:37:19.9981900Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
2023-04-10T02:37:20.7901965Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:2:
2023-04-10T02:37:20.7904506Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2023-04-10T02:37:20.7955447Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2298:7: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2023-04-10T02:37:20.7956418Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2023-04-10T02:37:20.7957099Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.7958790Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::SetAccessor(v8::Local<v8::ObjectTemplate>, v8::Local<v8::String>, Nan::GetterCallback, Nan::SetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, Nan::imp::Sig)’:
2023-04-10T02:37:20.7961295Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2536:19: warning: ‘void v8::ObjectTemplate::SetAccessor(v8::Local<v8::Name>, v8::AccessorNameGetterCallback, v8::AccessorNameSetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, v8::Local<v8::AccessorSignature>, v8::SideEffectType, v8::SideEffectType)’ is deprecated: Do signature check in accessor [-Wdeprecated-declarations]
2023-04-10T02:37:20.7978752Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2536 |   tpl->SetAccessor(
2023-04-10T02:37:20.7979299Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~~~~~~^
2023-04-10T02:37:20.7979805Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2537 |       name
2023-04-10T02:37:20.7980319Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ~~~~         
2023-04-10T02:37:20.7981179Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2538 |     , getter_
2023-04-10T02:37:20.7981678Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~      
2023-04-10T02:37:20.7982184Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2539 |     , setter_
2023-04-10T02:37:20.7982701Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~      
2023-04-10T02:37:20.7983195Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2540 |     , obj
2023-04-10T02:37:20.7983706Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~          
2023-04-10T02:37:20.7984196Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2541 |     , settings
2023-04-10T02:37:20.7984707Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~     
2023-04-10T02:37:20.7985212Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2542 |     , attribute
2023-04-10T02:37:20.7985723Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~~    
2023-04-10T02:37:20.7986233Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2543 |     , signature);
2023-04-10T02:37:20.7986747Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~~~   
2023-04-10T02:37:20.7987633Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from /home/runner/.cache/node-gyp/18.15.0/include/node/v8-function.h:15,
2023-04-10T02:37:20.7988552Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/v8.h:33,
2023-04-10T02:37:20.7989437Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:73,
2023-04-10T02:37:20.7990031Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from ../ecdh.cc:1:
2023-04-10T02:37:20.7990923Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/v8-template.h:838:8: note: declared here
2023-04-10T02:37:20.7991716Z .../eccrypto@1.1.6/node_modules/eccrypto install:   838 |   void SetAccessor(
2023-04-10T02:37:20.7992243Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |        ^~~~~~~~~~~
2023-04-10T02:37:20.8057326Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../../../../nan@2.14.0/node_modules/nan/nan.h:2884,
2023-04-10T02:37:20.8063857Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from ../ecdh.cc:2:
2023-04-10T02:37:20.8071888Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h: In constructor ‘Nan::TypedArrayContents<T>::TypedArrayContents(v8::Local<v8::Value>)’:
2023-04-10T02:37:20.8073474Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h:34:43: error: ‘class v8::ArrayBuffer’ has no member named ‘GetContents’
2023-04-10T02:37:20.8088790Z .../eccrypto@1.1.6/node_modules/eccrypto install:    34 |       data   = static_cast<char*>(buffer->GetContents().Data()) + byte_offset;
2023-04-10T02:37:20.8089563Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                           ^~~~~~~~~~~
2023-04-10T02:37:20.8393912Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc: In function ‘int derive(const uint8_t*, const uint8_t*, uint8_t*)’:
2023-04-10T02:37:20.8395484Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:37:41: warning: ‘EC_KEY* EC_KEY_new_by_curve_name(int)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8396417Z .../eccrypto@1.1.6/node_modules/eccrypto install:    37 |   CHECK((pkey = EC_KEY_new_by_curve_name(NID_secp256k1)) != NULL);
2023-04-10T02:37:20.8397170Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                 ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:20.8398057Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:20.8399288Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:20.8399996Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:20.8400689Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8401714Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:998:31: note: declared here
2023-04-10T02:37:20.8402579Z .../eccrypto@1.1.6/node_modules/eccrypto install:   998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
2023-04-10T02:37:20.8403318Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                               ^~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8406597Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:38:31: warning: ‘int EC_KEY_set_private_key(EC_KEY*, const BIGNUM*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8407561Z .../eccrypto@1.1.6/node_modules/eccrypto install:    38 |   CHECK(EC_KEY_set_private_key(pkey, pkey_bn) == 1);
2023-04-10T02:37:20.8408242Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:20.8409110Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:20.8409889Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:20.8410563Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:20.8411197Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8412219Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1056:27: note: declared here
2023-04-10T02:37:20.8415059Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1056 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_private_key(EC_KEY *key, const BIGNUM *prv);
2023-04-10T02:37:20.8416178Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8419766Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:40:29: warning: ‘int EVP_PKEY_set1_EC_KEY(EVP_PKEY*, ec_key_st*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8420690Z .../eccrypto@1.1.6/node_modules/eccrypto install:    40 |   CHECK(EVP_PKEY_set1_EC_KEY(evp_pkey, pkey) == 1);
2023-04-10T02:37:20.8421406Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8422257Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:20.8423041Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:20.8423758Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:20.8424400Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:3:
2023-04-10T02:37:20.8425431Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/evp.h:1370:5: note: declared here
2023-04-10T02:37:20.8426275Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1370 | int EVP_PKEY_set1_EC_KEY(EVP_PKEY *pkey, struct ec_key_st *key);
2023-04-10T02:37:20.8426952Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8428118Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:43:44: warning: ‘EC_KEY* EC_KEY_new_by_curve_name(int)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8431476Z .../eccrypto@1.1.6/node_modules/eccrypto install:    43 |   CHECK((peerkey = EC_KEY_new_by_curve_name(NID_secp256k1)) != NULL);
2023-04-10T02:37:20.8432443Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                    ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:20.8433276Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:20.8433971Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:20.8434573Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:20.8435138Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8436050Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:998:31: note: declared here
2023-04-10T02:37:20.8436779Z .../eccrypto@1.1.6/node_modules/eccrypto install:   998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
2023-04-10T02:37:20.8437951Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                               ^~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8440107Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:51:50: warning: ‘int EC_POINT_set_compressed_coordinates_GFp(const EC_GROUP*, EC_POINT*, const BIGNUM*, int, BN_CTX*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8441061Z .../eccrypto@1.1.6/node_modules/eccrypto install:    51 |     res = EC_POINT_set_compressed_coordinates_GFp(peerkey_group,
2023-04-10T02:37:20.8441741Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:20.8445176Z .../eccrypto@1.1.6/node_modules/eccrypto install:    52 |                                                  peerkey_p,
2023-04-10T02:37:20.8445823Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~
2023-04-10T02:37:20.8446452Z .../eccrypto@1.1.6/node_modules/eccrypto install:    53 |                                                  peerkey_bn,
2023-04-10T02:37:20.8447344Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~
2023-04-10T02:37:20.8447972Z .../eccrypto@1.1.6/node_modules/eccrypto install:    54 |                                                  compressed_y_bit,
2023-04-10T02:37:20.8448606Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8449220Z .../eccrypto@1.1.6/node_modules/eccrypto install:    55 |                                                  NULL);
2023-04-10T02:37:20.8449825Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~
2023-04-10T02:37:20.8502858Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8503953Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:686:27: note: declared here
2023-04-10T02:37:20.8504755Z .../eccrypto@1.1.6/node_modules/eccrypto install:   686 | OSSL_DEPRECATEDIN_3_0 int EC_POINT_set_compressed_coordinates_GFp
2023-04-10T02:37:20.8505447Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8506557Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:57:32: warning: ‘int EC_KEY_set_public_key(EC_KEY*, const EC_POINT*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8507365Z .../eccrypto@1.1.6/node_modules/eccrypto install:    57 |     res = EC_KEY_set_public_key(peerkey, peerkey_p);
2023-04-10T02:37:20.8507997Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8508572Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8509764Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1070:27: note: declared here
2023-04-10T02:37:20.8510571Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1070 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_public_key(EC_KEY *key, const EC_POINT *pub);
2023-04-10T02:37:20.8511228Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8512452Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:62:51: warning: ‘int EC_KEY_set_public_key_affine_coordinates(EC_KEY*, BIGNUM*, BIGNUM*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8513292Z .../eccrypto@1.1.6/node_modules/eccrypto install:    62 |     res = EC_KEY_set_public_key_affine_coordinates(peerkey,
2023-04-10T02:37:20.8513946Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~
2023-04-10T02:37:20.8514587Z .../eccrypto@1.1.6/node_modules/eccrypto install:    63 |                                                  peerkey_bn_x,
2023-04-10T02:37:20.8515192Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~
2023-04-10T02:37:20.8515820Z .../eccrypto@1.1.6/node_modules/eccrypto install:    64 |                                                  peerkey_bn_y);
2023-04-10T02:37:20.8516443Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~
2023-04-10T02:37:20.8517019Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8517920Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1122:27: note: declared here
2023-04-10T02:37:20.8518719Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1122 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_public_key_affine_coordinates(EC_KEY *key,
2023-04-10T02:37:20.8519560Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8520656Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:69:29: warning: ‘int EVP_PKEY_set1_EC_KEY(EVP_PKEY*, ec_key_st*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8521866Z .../eccrypto@1.1.6/node_modules/eccrypto install:    69 |   CHECK(EVP_PKEY_set1_EC_KEY(evp_peerkey, peerkey) == 1);
2023-04-10T02:37:20.8522550Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8523342Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:20.8524020Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:20.8526248Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:20.8526835Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:3:
2023-04-10T02:37:20.8527773Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/evp.h:1370:5: note: declared here
2023-04-10T02:37:20.8528528Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1370 | int EVP_PKEY_set1_EC_KEY(EVP_PKEY *pkey, struct ec_key_st *key);
2023-04-10T02:37:20.8529113Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8530119Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:82:14: warning: ‘void EC_KEY_free(EC_KEY*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8530795Z .../eccrypto@1.1.6/node_modules/eccrypto install:    82 |   EC_KEY_free(peerkey);
2023-04-10T02:37:20.8531330Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~^~~~~~~~~
2023-04-10T02:37:20.8557072Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8558129Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1003:28: note: declared here
2023-04-10T02:37:20.8558848Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1003 | OSSL_DEPRECATEDIN_3_0 void EC_KEY_free(EC_KEY *key);
2023-04-10T02:37:20.8559466Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                            ^~~~~~~~~~~
2023-04-10T02:37:20.8560478Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:90:14: warning: ‘void EC_KEY_free(EC_KEY*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:20.8561152Z .../eccrypto@1.1.6/node_modules/eccrypto install:    90 |   EC_KEY_free(pkey);
2023-04-10T02:37:20.8561683Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~^~~~~~
2023-04-10T02:37:20.8562236Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:20.8563218Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1003:28: note: declared here
2023-04-10T02:37:20.8563940Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1003 | OSSL_DEPRECATEDIN_3_0 void EC_KEY_free(EC_KEY *key);
2023-04-10T02:37:20.8564543Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                            ^~~~~~~~~~~
2023-04-10T02:37:20.8565108Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:1:
2023-04-10T02:37:20.8565654Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc: At global scope:
2023-04-10T02:37:20.8570892Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:978:7: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2023-04-10T02:37:20.8572317Z .../eccrypto@1.1.6/node_modules/eccrypto install:   978 |       (node::addon_register_func) (regfunc),                          \
2023-04-10T02:37:20.8573374Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:20.8574418Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:1012:3: note: in expansion of macro ‘NODE_MODULE_X’
2023-04-10T02:37:20.8575230Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1012 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2023-04-10T02:37:20.8576536Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ^~~~~~~~~~~~~
2023-04-10T02:37:20.8577394Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
2023-04-10T02:37:20.8578038Z .../eccrypto@1.1.6/node_modules/eccrypto install:   131 | NODE_MODULE(ecdh, InitAll)
2023-04-10T02:37:20.8578565Z .../eccrypto@1.1.6/node_modules/eccrypto install:       | ^~~~~~~~~~~
2023-04-10T02:37:20.9309400Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: *** [ecdh.target.mk:119: Release/obj.target/ecdh/ecdh.o] Error 1
2023-04-10T02:37:20.9310101Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! build error 
2023-04-10T02:37:20.9314626Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack Error: `make` failed with exit code: 2
2023-04-10T02:37:20.9319796Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess.onExit (/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/lib/build.js:203:23)
2023-04-10T02:37:20.9323428Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
2023-04-10T02:37:20.9327083Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
2023-04-10T02:37:20.9330659Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! System Linux 5.15.0-1035-azure
2023-04-10T02:37:20.9335110Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! command "/opt/hostedtoolcache/node/18.15.0/x64/bin/node" "/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
2023-04-10T02:37:20.9356753Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! cwd /home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto
2023-04-10T02:37:20.9357647Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! node -v v18.15.0
2023-04-10T02:37:20.9358315Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! node-gyp -v v9.3.1
2023-04-10T02:37:20.9358827Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! not ok 
2023-04-10T02:37:20.9359921Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: Leaving directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build'
2023-04-10T02:37:20.9361360Z .../eccrypto@1.1.6/node_modules/eccrypto install: Done
2023-04-10T02:37:21.1740094Z 
2023-04-10T02:37:21.1740990Z devDependencies:
2023-04-10T02:37:21.1741857Z + @babel/core 7.20.12
2023-04-10T02:37:21.1742703Z + @changesets/changelog-github 0.4.8
2023-04-10T02:37:21.1743468Z + @changesets/cli 2.26.0
2023-04-10T02:37:21.1744142Z + @typescript-eslint/eslint-plugin 5.48.0
2023-04-10T02:37:21.1745025Z + @typescript-eslint/parser 5.48.0
2023-04-10T02:37:21.1745611Z + @vitest/coverage-c8 0.28.3
2023-04-10T02:37:21.1746292Z + @vitest/ui 0.28.4
2023-04-10T02:37:21.1746725Z + eslint 8.31.0
2023-04-10T02:37:21.1747574Z + eslint-config-airbnb-typescript 17.0.0
2023-04-10T02:37:21.1748222Z + eslint-config-prettier 8.6.0
2023-04-10T02:37:21.1749018Z + eslint-plugin-import 2.26.0
2023-04-10T02:37:21.1749634Z + eslint-plugin-prettier 4.2.1
2023-04-10T02:37:21.1751478Z + eslint-plugin-sonar 0.9.2
2023-04-10T02:37:21.1751966Z + husky 8.0.3
2023-04-10T02:37:21.1754944Z + jsdom 20.0.3
2023-04-10T02:37:21.1755538Z + lint-staged 13.1.0
2023-04-10T02:37:21.1756237Z + prettier 2.8.1
2023-04-10T02:37:21.1756672Z + semver 7.3.8
2023-04-10T02:37:21.1757312Z + tsup 6.5.0
2023-04-10T02:37:21.1757741Z + typescript 4.9.4
2023-04-10T02:37:21.1758512Z + vite-tsconfig-paths 4.0.5
2023-04-10T02:37:21.1758979Z + vitest 0.26.3
2023-04-10T02:37:21.1759521Z 
2023-04-10T02:37:21.1759934Z . prepare$ husky install
2023-04-10T02:37:21.2582792Z . prepare: husky - Git hooks installed
2023-04-10T02:37:21.2653700Z . prepare: Done
2023-04-10T02:37:21.2677960Z Done in 29.2s
2023-04-10T02:37:21.3261643Z ##[group]Run pnpm lint
2023-04-10T02:37:21.3262044Z [36;1mpnpm lint[0m
2023-04-10T02:37:21.3340545Z shell: /usr/bin/bash -e {0}
2023-04-10T02:37:21.3340804Z env:
2023-04-10T02:37:21.3341115Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:21.3341446Z ##[endgroup]
2023-04-10T02:37:21.9261005Z 
2023-04-10T02:37:21.9261495Z > root@0.0.3 lint /home/runner/work/useWallet/useWallet
2023-04-10T02:37:21.9262105Z > eslint . --cache
2023-04-10T02:37:21.9262274Z 
2023-04-10T02:37:30.8289108Z 
2023-04-10T02:37:30.8290425Z /home/runner/work/useWallet/useWallet/examples/example-react/src/App.tsx
2023-04-10T02:37:30.8362144Z ##[warning]  1:54  warning  'useSignMessage' is defined but never used  @typescript-eslint/no-unused-vars
2023-04-10T02:37:30.8370738Z 
2023-04-10T02:37:30.8371340Z ✖ 1 problem (0 errors, 1 warning)
2023-04-10T02:37:30.8371558Z 
2023-04-10T02:37:31.0007279Z Post job cleanup.
2023-04-10T02:37:31.6554158Z [command]/usr/bin/tar --posix -cf cache.tzst --exclude cache.tzst -P -C /home/runner/work/useWallet/useWallet --files-from manifest.txt --use-compress-program zstdmt
2023-04-10T02:37:37.9740824Z Cache Size: ~142 MB (148701348 B)
2023-04-10T02:37:38.0817523Z Cache saved successfully
2023-04-10T02:37:38.1158175Z Cache saved with key: modules-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:37:38.2169620Z Post job cleanup.
2023-04-10T02:37:38.4073424Z [command]/usr/bin/tar --posix -cf cache.tzst --exclude cache.tzst -P -C /home/runner/work/useWallet/useWallet --files-from manifest.txt --use-compress-program zstdmt
2023-04-10T02:37:38.9448134Z Cache Size: ~3 MB (3413482 B)
2023-04-10T02:37:39.0106197Z Cache saved successfully
2023-04-10T02:37:39.0126755Z Cache saved with key: pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8
2023-04-10T02:37:39.0298364Z Post job cleanup.
2023-04-10T02:37:39.2294706Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm store path --silent
2023-04-10T02:37:39.8654778Z /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:37:39.8982572Z [command]/usr/bin/tar --posix -z -cf cache.tgz --exclude cache.tgz -P -C /home/runner/work/useWallet/useWallet --files-from manifest.txt
2023-04-10T02:38:14.8467573Z Failed to save: Unable to reserve cache with key node-cache-Linux-pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8, another job may be creating this cache. More details: Cache already exists. Scope: refs/heads/main, Key: node-cache-Linux-pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8, Version: 5e34942b09d60f26936dbe01f6e5a1104cb7cc62c7c0c778bb12993b02ca0328
2023-04-10T02:38:14.8913885Z Post job cleanup.
2023-04-10T02:38:15.0358061Z Pruning is unnecessary.
2023-04-10T02:38:15.0517328Z Post job cleanup.
2023-04-10T02:38:15.2240331Z [command]/usr/bin/git version
2023-04-10T02:38:15.2304180Z git version 2.40.0
2023-04-10T02:38:15.2381003Z Temporarily overriding HOME='/home/runner/work/_temp/94c3e8b7-c14d-466f-96a7-8a25fd080d28' before making global git config changes
2023-04-10T02:38:15.2387277Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:38:15.2398101Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:38:15.2461079Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:38:15.2510426Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:38:15.2811235Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:38:15.2839910Z http.https://github.com/.extraheader
2023-04-10T02:38:15.2854959Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2023-04-10T02:38:15.2899662Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:38:15.3450747Z Cleaning up orphan processes
```