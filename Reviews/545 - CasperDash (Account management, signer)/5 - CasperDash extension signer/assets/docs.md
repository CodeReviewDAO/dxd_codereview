# Documentation Workflow Logs

```sh
2023-04-10T02:36:37.6150862Z Requested labels: ubuntu-latest
2023-04-10T02:36:37.6150924Z Job defined at: CasperDash/useWallet/.github/workflows/publish-docs.yml@refs/heads/main
2023-04-10T02:36:37.6150953Z Waiting for a runner to pick up this job...
2023-04-10T02:36:38.2042987Z Job is waiting for a hosted runner to come online.
2023-04-10T02:36:40.2845787Z Job is about to start running on the hosted runner: GitHub Actions 3 (hosted)
2023-04-10T02:36:42.4982501Z Current runner version: '2.303.0'
2023-04-10T02:36:42.5012477Z ##[group]Operating System
2023-04-10T02:36:42.5013145Z Ubuntu
2023-04-10T02:36:42.5013465Z 22.04.2
2023-04-10T02:36:42.5013783Z LTS
2023-04-10T02:36:42.5014052Z ##[endgroup]
2023-04-10T02:36:42.5014394Z ##[group]Runner Image
2023-04-10T02:36:42.5014808Z Image: ubuntu-22.04
2023-04-10T02:36:42.5015162Z Version: 20230402.1
2023-04-10T02:36:42.5015726Z Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20230402.1/images/linux/Ubuntu2204-Readme.md
2023-04-10T02:36:42.5016391Z Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20230402.1
2023-04-10T02:36:42.5016894Z ##[endgroup]
2023-04-10T02:36:42.5017276Z ##[group]Runner Image Provisioner
2023-04-10T02:36:42.5017641Z 2.0.139.1
2023-04-10T02:36:42.5017906Z ##[endgroup]
2023-04-10T02:36:42.5018946Z ##[group]GITHUB_TOKEN Permissions
2023-04-10T02:36:42.5019632Z Actions: write
2023-04-10T02:36:42.5019975Z Checks: write
2023-04-10T02:36:42.5020541Z Contents: write
2023-04-10T02:36:42.5021016Z Deployments: write
2023-04-10T02:36:42.5021325Z Discussions: write
2023-04-10T02:36:42.5021721Z Issues: write
2023-04-10T02:36:42.5022065Z Metadata: read
2023-04-10T02:36:42.5022372Z Packages: write
2023-04-10T02:36:42.5022711Z Pages: write
2023-04-10T02:36:42.5023087Z PullRequests: write
2023-04-10T02:36:42.5023488Z RepositoryProjects: write
2023-04-10T02:36:42.5023873Z SecurityEvents: write
2023-04-10T02:36:42.5024233Z Statuses: write
2023-04-10T02:36:42.5024599Z ##[endgroup]
2023-04-10T02:36:42.5028601Z Secret source: Actions
2023-04-10T02:36:42.5029085Z Prepare workflow directory
2023-04-10T02:36:42.5841248Z Prepare all required actions
2023-04-10T02:36:42.6027961Z Getting action download info
2023-04-10T02:36:42.8860784Z Download action repository 'actions/checkout@v3' (SHA:8f4b7f84864484a7bf31766abe9204da3cbe65b3)
2023-04-10T02:36:43.2433774Z Download action repository 'pnpm/action-setup@v2.2.4' (SHA:c3b53f6a16e57305370b4ae5a540c2077a1d50dd)
2023-04-10T02:36:43.5392946Z Download action repository 'actions/setup-node@v3' (SHA:64ed1c7eab4cce3362f8c340dee64e5eaeef8f7c)
2023-04-10T02:36:43.8293841Z Download action repository 'aws-actions/configure-aws-credentials@v1' (SHA:67fbcbb121271f7775d2e7715933280b06314838)
2023-04-10T02:36:44.0733486Z Download action repository 'eisberg-labs/static-website-to-s3@main' (SHA:24e0c4837f0c2df9f4048bfe089c60bd529dda8a)
2023-04-10T02:36:44.5022354Z Getting action download info
2023-04-10T02:36:44.6175403Z Download action repository 'unfor19/install-aws-cli-action@v1' (SHA:457b7980b125044247e455d87b9a26fc2299b787)
2023-04-10T02:36:44.8029104Z Complete job name: publish-docs (18, 7.26.3)
2023-04-10T02:36:44.8860918Z ##[group]Run actions/checkout@v3
2023-04-10T02:36:44.8861236Z with:
2023-04-10T02:36:44.8861458Z   fetch-depth: 0
2023-04-10T02:36:44.8861727Z   repository: CasperDash/useWallet
2023-04-10T02:36:44.8862231Z   token: ***
2023-04-10T02:36:44.8862450Z   ssh-strict: true
2023-04-10T02:36:44.8862713Z   persist-credentials: true
2023-04-10T02:36:44.8862967Z   clean: true
2023-04-10T02:36:44.8863164Z   lfs: false
2023-04-10T02:36:44.8863378Z   submodules: false
2023-04-10T02:36:44.8863626Z   set-safe-directory: true
2023-04-10T02:36:44.8863868Z ##[endgroup]
2023-04-10T02:36:45.2138995Z Syncing repository: CasperDash/useWallet
2023-04-10T02:36:45.2140903Z ##[group]Getting Git version info
2023-04-10T02:36:45.2141444Z Working directory is '/home/runner/work/useWallet/useWallet'
2023-04-10T02:36:45.2142913Z [command]/usr/bin/git version
2023-04-10T02:36:45.2251592Z git version 2.40.0
2023-04-10T02:36:45.2284773Z ##[endgroup]
2023-04-10T02:36:45.2300509Z Temporarily overriding HOME='/home/runner/work/_temp/9279afa2-7716-415b-a1a1-c634e85265c0' before making global git config changes
2023-04-10T02:36:45.2301019Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:36:45.2302276Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:36:45.2360879Z Deleting the contents of '/home/runner/work/useWallet/useWallet'
2023-04-10T02:36:45.2366395Z ##[group]Initializing the repository
2023-04-10T02:36:45.2370237Z [command]/usr/bin/git init /home/runner/work/useWallet/useWallet
2023-04-10T02:36:45.2457508Z hint: Using 'master' as the name for the initial branch. This default branch name
2023-04-10T02:36:45.2458202Z hint: is subject to change. To configure the initial branch name to use in all
2023-04-10T02:36:45.2459017Z hint: of your new repositories, which will suppress this warning, call:
2023-04-10T02:36:45.2459486Z hint: 
2023-04-10T02:36:45.2460540Z hint: 	git config --global init.defaultBranch <name>
2023-04-10T02:36:45.2461036Z hint: 
2023-04-10T02:36:45.2461790Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2023-04-10T02:36:45.2462467Z hint: 'development'. The just-created branch can be renamed via this command:
2023-04-10T02:36:45.2463139Z hint: 
2023-04-10T02:36:45.2463580Z hint: 	git branch -m <name>
2023-04-10T02:36:45.2470113Z Initialized empty Git repository in /home/runner/work/useWallet/useWallet/.git/
2023-04-10T02:36:45.2479353Z [command]/usr/bin/git remote add origin https://github.com/CasperDash/useWallet
2023-04-10T02:36:45.2524646Z ##[endgroup]
2023-04-10T02:36:45.2525360Z ##[group]Disabling automatic garbage collection
2023-04-10T02:36:45.2527916Z [command]/usr/bin/git config --local gc.auto 0
2023-04-10T02:36:45.2560638Z ##[endgroup]
2023-04-10T02:36:45.2561310Z ##[group]Setting up auth
2023-04-10T02:36:45.2567253Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:36:45.2601535Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:36:45.2992372Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:36:45.3023913Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:36:45.3255608Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2023-04-10T02:36:45.3294875Z ##[endgroup]
2023-04-10T02:36:45.3295717Z ##[group]Fetching the repository
2023-04-10T02:36:45.3304306Z [command]/usr/bin/git -c protocol.version=2 fetch --prune --progress --no-recurse-submodules origin +refs/heads/*:refs/remotes/origin/* +refs/tags/*:refs/tags/*
2023-04-10T02:36:45.6191647Z remote: Enumerating objects: 1571, done.        
2023-04-10T02:36:45.6248447Z remote: Counting objects:   0% (1/510)        
2023-04-10T02:36:45.6248788Z remote: Counting objects:   1% (6/510)        
2023-04-10T02:36:45.6249082Z remote: Counting objects:   2% (11/510)        
2023-04-10T02:36:45.6249373Z remote: Counting objects:   3% (16/510)        
2023-04-10T02:36:45.6249658Z remote: Counting objects:   4% (21/510)        
2023-04-10T02:36:45.6249956Z remote: Counting objects:   5% (26/510)        
2023-04-10T02:36:45.6250234Z remote: Counting objects:   6% (31/510)        
2023-04-10T02:36:45.6250512Z remote: Counting objects:   7% (36/510)        
2023-04-10T02:36:45.6250777Z remote: Counting objects:   8% (41/510)        
2023-04-10T02:36:45.6251050Z remote: Counting objects:   9% (46/510)        
2023-04-10T02:36:45.6251328Z remote: Counting objects:  10% (51/510)        
2023-04-10T02:36:45.6251602Z remote: Counting objects:  11% (57/510)        
2023-04-10T02:36:45.6251875Z remote: Counting objects:  12% (62/510)        
2023-04-10T02:36:45.6252170Z remote: Counting objects:  13% (67/510)        
2023-04-10T02:36:45.6252440Z remote: Counting objects:  14% (72/510)        
2023-04-10T02:36:45.6252714Z remote: Counting objects:  15% (77/510)        
2023-04-10T02:36:45.6252984Z remote: Counting objects:  16% (82/510)        
2023-04-10T02:36:45.6253242Z remote: Counting objects:  17% (87/510)        
2023-04-10T02:36:45.6253790Z remote: Counting objects:  18% (92/510)        
2023-04-10T02:36:45.6254066Z remote: Counting objects:  19% (97/510)        
2023-04-10T02:36:45.6254347Z remote: Counting objects:  20% (102/510)        
2023-04-10T02:36:45.6254634Z remote: Counting objects:  21% (108/510)        
2023-04-10T02:36:45.6254917Z remote: Counting objects:  22% (113/510)        
2023-04-10T02:36:45.6255196Z remote: Counting objects:  23% (118/510)        
2023-04-10T02:36:45.6255477Z remote: Counting objects:  24% (123/510)        
2023-04-10T02:36:45.6255752Z remote: Counting objects:  25% (128/510)        
2023-04-10T02:36:45.6256037Z remote: Counting objects:  26% (133/510)        
2023-04-10T02:36:45.6256299Z remote: Counting objects:  27% (138/510)        
2023-04-10T02:36:45.6256585Z remote: Counting objects:  28% (143/510)        
2023-04-10T02:36:45.6256861Z remote: Counting objects:  29% (148/510)        
2023-04-10T02:36:45.6257135Z remote: Counting objects:  30% (153/510)        
2023-04-10T02:36:45.6257414Z remote: Counting objects:  31% (159/510)        
2023-04-10T02:36:45.6257688Z remote: Counting objects:  32% (164/510)        
2023-04-10T02:36:45.6257961Z remote: Counting objects:  33% (169/510)        
2023-04-10T02:36:45.6258399Z remote: Counting objects:  34% (174/510)        
2023-04-10T02:36:45.6258705Z remote: Counting objects:  35% (179/510)        
2023-04-10T02:36:45.6259050Z remote: Counting objects:  36% (184/510)        
2023-04-10T02:36:45.6259398Z remote: Counting objects:  37% (189/510)        
2023-04-10T02:36:45.6259751Z remote: Counting objects:  38% (194/510)        
2023-04-10T02:36:45.6260174Z remote: Counting objects:  39% (199/510)        
2023-04-10T02:36:45.6260516Z remote: Counting objects:  40% (204/510)        
2023-04-10T02:36:45.6260865Z remote: Counting objects:  41% (210/510)        
2023-04-10T02:36:45.6261218Z remote: Counting objects:  42% (215/510)        
2023-04-10T02:36:45.6261618Z remote: Counting objects:  43% (220/510)        
2023-04-10T02:36:45.6261920Z remote: Counting objects:  44% (225/510)        
2023-04-10T02:36:45.6262264Z remote: Counting objects:  45% (230/510)        
2023-04-10T02:36:45.6262620Z remote: Counting objects:  46% (235/510)        
2023-04-10T02:36:45.6262999Z remote: Counting objects:  47% (240/510)        
2023-04-10T02:36:45.6263351Z remote: Counting objects:  48% (245/510)        
2023-04-10T02:36:45.6263699Z remote: Counting objects:  49% (250/510)        
2023-04-10T02:36:45.6264060Z remote: Counting objects:  50% (255/510)        
2023-04-10T02:36:45.6264437Z remote: Counting objects:  51% (261/510)        
2023-04-10T02:36:45.6265114Z remote: Counting objects:  52% (266/510)        
2023-04-10T02:36:45.6265487Z remote: Counting objects:  53% (271/510)        
2023-04-10T02:36:45.6265791Z remote: Counting objects:  54% (276/510)        
2023-04-10T02:36:45.6266171Z remote: Counting objects:  55% (281/510)        
2023-04-10T02:36:45.6266553Z remote: Counting objects:  56% (286/510)        
2023-04-10T02:36:45.6266919Z remote: Counting objects:  57% (291/510)        
2023-04-10T02:36:45.6267267Z remote: Counting objects:  58% (296/510)        
2023-04-10T02:36:45.6267619Z remote: Counting objects:  59% (301/510)        
2023-04-10T02:36:45.6267996Z remote: Counting objects:  60% (306/510)        
2023-04-10T02:36:45.6268355Z remote: Counting objects:  61% (312/510)        
2023-04-10T02:36:45.6268700Z remote: Counting objects:  62% (317/510)        
2023-04-10T02:36:45.6269050Z remote: Counting objects:  63% (322/510)        
2023-04-10T02:36:45.6269375Z remote: Counting objects:  64% (327/510)        
2023-04-10T02:36:45.6269923Z remote: Counting objects:  65% (332/510)        
2023-04-10T02:36:45.6270507Z remote: Counting objects:  66% (337/510)        
2023-04-10T02:36:45.6270813Z remote: Counting objects:  67% (342/510)        
2023-04-10T02:36:45.6271198Z remote: Counting objects:  68% (347/510)        
2023-04-10T02:36:45.6271556Z remote: Counting objects:  69% (352/510)        
2023-04-10T02:36:45.6271905Z remote: Counting objects:  70% (357/510)        
2023-04-10T02:36:45.6272759Z remote: Counting objects:  71% (363/510)        
2023-04-10T02:36:45.6273946Z remote: Counting objects:  72% (368/510)        
2023-04-10T02:36:45.6275572Z remote: Counting objects:  73% (373/510)        
2023-04-10T02:36:45.6276350Z remote: Counting objects:  74% (378/510)        
2023-04-10T02:36:45.6276719Z remote: Counting objects:  75% (383/510)        
2023-04-10T02:36:45.6277142Z remote: Counting objects:  76% (388/510)        
2023-04-10T02:36:45.6277537Z remote: Counting objects:  77% (393/510)        
2023-04-10T02:36:45.6277902Z remote: Counting objects:  78% (398/510)        
2023-04-10T02:36:45.6278334Z remote: Counting objects:  79% (403/510)        
2023-04-10T02:36:45.6278727Z remote: Counting objects:  80% (408/510)        
2023-04-10T02:36:45.6279571Z remote: Counting objects:  81% (414/510)        
2023-04-10T02:36:45.6279988Z remote: Counting objects:  82% (419/510)        
2023-04-10T02:36:45.6280357Z remote: Counting objects:  83% (424/510)        
2023-04-10T02:36:45.6280889Z remote: Counting objects:  84% (429/510)        
2023-04-10T02:36:45.6281244Z remote: Counting objects:  85% (434/510)        
2023-04-10T02:36:45.6281614Z remote: Counting objects:  86% (439/510)        
2023-04-10T02:36:45.6282076Z remote: Counting objects:  87% (444/510)        
2023-04-10T02:36:45.6282522Z remote: Counting objects:  88% (449/510)        
2023-04-10T02:36:45.6282831Z remote: Counting objects:  89% (454/510)        
2023-04-10T02:36:45.6283184Z remote: Counting objects:  90% (459/510)        
2023-04-10T02:36:45.6283647Z remote: Counting objects:  91% (465/510)        
2023-04-10T02:36:45.6284016Z remote: Counting objects:  92% (470/510)        
2023-04-10T02:36:45.6284397Z remote: Counting objects:  93% (475/510)        
2023-04-10T02:36:45.6284841Z remote: Counting objects:  94% (480/510)        
2023-04-10T02:36:45.6285265Z remote: Counting objects:  95% (485/510)        
2023-04-10T02:36:45.6285614Z remote: Counting objects:  96% (490/510)        
2023-04-10T02:36:45.6286004Z remote: Counting objects:  97% (495/510)        
2023-04-10T02:36:45.6286304Z remote: Counting objects:  98% (500/510)        
2023-04-10T02:36:45.6286663Z remote: Counting objects:  99% (505/510)        
2023-04-10T02:36:45.6287167Z remote: Counting objects: 100% (510/510)        
2023-04-10T02:36:45.6287603Z remote: Counting objects: 100% (510/510), done.        
2023-04-10T02:36:45.6287983Z remote: Compressing objects:   0% (1/294)        
2023-04-10T02:36:45.6288383Z remote: Compressing objects:   1% (3/294)        
2023-04-10T02:36:45.6288750Z remote: Compressing objects:   2% (6/294)        
2023-04-10T02:36:45.6289369Z remote: Compressing objects:   3% (9/294)        
2023-04-10T02:36:45.6289866Z remote: Compressing objects:   4% (12/294)        
2023-04-10T02:36:45.6290241Z remote: Compressing objects:   5% (15/294)        
2023-04-10T02:36:45.6290564Z remote: Compressing objects:   6% (18/294)        
2023-04-10T02:36:45.6291036Z remote: Compressing objects:   7% (21/294)        
2023-04-10T02:36:45.6291453Z remote: Compressing objects:   8% (24/294)        
2023-04-10T02:36:45.6292102Z remote: Compressing objects:   9% (27/294)        
2023-04-10T02:36:45.6294660Z remote: Compressing objects:  10% (30/294)        
2023-04-10T02:36:45.6295192Z remote: Compressing objects:  11% (33/294)        
2023-04-10T02:36:45.6295719Z remote: Compressing objects:  12% (36/294)        
2023-04-10T02:36:45.6296174Z remote: Compressing objects:  13% (39/294)        
2023-04-10T02:36:45.6296659Z remote: Compressing objects:  14% (42/294)        
2023-04-10T02:36:45.6297119Z remote: Compressing objects:  15% (45/294)        
2023-04-10T02:36:45.6297611Z remote: Compressing objects:  16% (48/294)        
2023-04-10T02:36:45.6298079Z remote: Compressing objects:  17% (50/294)        
2023-04-10T02:36:45.6298641Z remote: Compressing objects:  18% (53/294)        
2023-04-10T02:36:45.6302067Z remote: Compressing objects:  19% (56/294)        
2023-04-10T02:36:45.6302665Z remote: Compressing objects:  20% (59/294)        
2023-04-10T02:36:45.6303348Z remote: Compressing objects:  21% (62/294)        
2023-04-10T02:36:45.6303843Z remote: Compressing objects:  22% (65/294)        
2023-04-10T02:36:45.6304309Z remote: Compressing objects:  23% (68/294)        
2023-04-10T02:36:45.6304963Z remote: Compressing objects:  24% (71/294)        
2023-04-10T02:36:45.6305413Z remote: Compressing objects:  25% (74/294)        
2023-04-10T02:36:45.6305855Z remote: Compressing objects:  26% (77/294)        
2023-04-10T02:36:45.6306309Z remote: Compressing objects:  27% (80/294)        
2023-04-10T02:36:45.6306813Z remote: Compressing objects:  28% (83/294)        
2023-04-10T02:36:45.6307258Z remote: Compressing objects:  29% (86/294)        
2023-04-10T02:36:45.6307712Z remote: Compressing objects:  30% (89/294)        
2023-04-10T02:36:45.6308153Z remote: Compressing objects:  31% (92/294)        
2023-04-10T02:36:45.6308652Z remote: Compressing objects:  32% (95/294)        
2023-04-10T02:36:45.6309105Z remote: Compressing objects:  33% (98/294)        
2023-04-10T02:36:45.6309560Z remote: Compressing objects:  34% (100/294)        
2023-04-10T02:36:45.6310010Z remote: Compressing objects:  35% (103/294)        
2023-04-10T02:36:45.6310525Z remote: Compressing objects:  36% (106/294)        
2023-04-10T02:36:45.6310973Z remote: Compressing objects:  37% (109/294)        
2023-04-10T02:36:45.6311431Z remote: Compressing objects:  38% (112/294)        
2023-04-10T02:36:45.6311873Z remote: Compressing objects:  39% (115/294)        
2023-04-10T02:36:45.6312352Z remote: Compressing objects:  40% (118/294)        
2023-04-10T02:36:45.6312800Z remote: Compressing objects:  41% (121/294)        
2023-04-10T02:36:45.6313207Z remote: Compressing objects:  42% (124/294)        
2023-04-10T02:36:45.6313706Z remote: Compressing objects:  43% (127/294)        
2023-04-10T02:36:45.6314213Z remote: Compressing objects:  44% (130/294)        
2023-04-10T02:36:45.6314656Z remote: Compressing objects:  45% (133/294)        
2023-04-10T02:36:45.6315113Z remote: Compressing objects:  46% (136/294)        
2023-04-10T02:36:45.6315556Z remote: Compressing objects:  47% (139/294)        
2023-04-10T02:36:45.6316059Z remote: Compressing objects:  48% (142/294)        
2023-04-10T02:36:45.6316503Z remote: Compressing objects:  49% (145/294)        
2023-04-10T02:36:45.6316955Z remote: Compressing objects:  50% (147/294)        
2023-04-10T02:36:45.6317394Z remote: Compressing objects:  51% (150/294)        
2023-04-10T02:36:45.6317865Z remote: Compressing objects:  52% (153/294)        
2023-04-10T02:36:45.6318349Z remote: Compressing objects:  53% (156/294)        
2023-04-10T02:36:45.6318958Z remote: Compressing objects:  54% (159/294)        
2023-04-10T02:36:45.6319413Z remote: Compressing objects:  55% (162/294)        
2023-04-10T02:36:45.6319912Z remote: Compressing objects:  56% (165/294)        
2023-04-10T02:36:45.6320352Z remote: Compressing objects:  57% (168/294)        
2023-04-10T02:36:45.6320799Z remote: Compressing objects:  58% (171/294)        
2023-04-10T02:36:45.6321245Z remote: Compressing objects:  59% (174/294)        
2023-04-10T02:36:45.6321733Z remote: Compressing objects:  60% (177/294)        
2023-04-10T02:36:45.6322171Z remote: Compressing objects:  61% (180/294)        
2023-04-10T02:36:45.6322567Z remote: Compressing objects:  62% (183/294)        
2023-04-10T02:36:45.6323011Z remote: Compressing objects:  63% (186/294)        
2023-04-10T02:36:45.6323506Z remote: Compressing objects:  64% (189/294)        
2023-04-10T02:36:45.6323951Z remote: Compressing objects:  65% (192/294)        
2023-04-10T02:36:45.6326999Z remote: Compressing objects:  66% (195/294)        
2023-04-10T02:36:45.6327914Z remote: Compressing objects:  67% (197/294)        
2023-04-10T02:36:45.6328395Z remote: Compressing objects:  68% (200/294)        
2023-04-10T02:36:45.6328820Z remote: Compressing objects:  69% (203/294)        
2023-04-10T02:36:45.6329188Z remote: Compressing objects:  70% (206/294)        
2023-04-10T02:36:45.6329775Z remote: Compressing objects:  71% (209/294)        
2023-04-10T02:36:45.6330199Z remote: Compressing objects:  72% (212/294)        
2023-04-10T02:36:45.6330563Z remote: Compressing objects:  73% (215/294)        
2023-04-10T02:36:45.6331659Z remote: Compressing objects:  74% (218/294)        
2023-04-10T02:36:45.6331993Z remote: Compressing objects:  75% (221/294)        
2023-04-10T02:36:45.6332411Z remote: Compressing objects:  76% (224/294)        
2023-04-10T02:36:45.6332779Z remote: Compressing objects:  77% (227/294)        
2023-04-10T02:36:45.6333144Z remote: Compressing objects:  78% (230/294)        
2023-04-10T02:36:45.6334058Z remote: Compressing objects:  79% (233/294)        
2023-04-10T02:36:45.6334539Z remote: Compressing objects:  80% (236/294)        
2023-04-10T02:36:45.6334902Z remote: Compressing objects:  81% (239/294)        
2023-04-10T02:36:45.6335262Z remote: Compressing objects:  82% (242/294)        
2023-04-10T02:36:45.6335634Z remote: Compressing objects:  83% (245/294)        
2023-04-10T02:36:45.6336602Z remote: Compressing objects:  84% (247/294)        
2023-04-10T02:36:45.6336957Z remote: Compressing objects:  85% (250/294)        
2023-04-10T02:36:45.6337324Z remote: Compressing objects:  86% (253/294)        
2023-04-10T02:36:45.6337703Z remote: Compressing objects:  87% (256/294)        
2023-04-10T02:36:45.6338068Z remote: Compressing objects:  88% (259/294)        
2023-04-10T02:36:45.6338483Z remote: Compressing objects:  89% (262/294)        
2023-04-10T02:36:45.6339504Z remote: Compressing objects:  90% (265/294)        
2023-04-10T02:36:45.6339914Z remote: Compressing objects:  91% (268/294)        
2023-04-10T02:36:45.6340283Z remote: Compressing objects:  92% (271/294)        
2023-04-10T02:36:45.6340692Z remote: Compressing objects:  93% (274/294)        
2023-04-10T02:36:45.6341118Z remote: Compressing objects:  94% (277/294)        
2023-04-10T02:36:45.6342163Z remote: Compressing objects:  95% (280/294)        
2023-04-10T02:36:45.6342527Z remote: Compressing objects:  96% (283/294)        
2023-04-10T02:36:45.6343003Z remote: Compressing objects:  97% (286/294)        
2023-04-10T02:36:45.6343376Z remote: Compressing objects:  98% (289/294)        
2023-04-10T02:36:45.6343737Z remote: Compressing objects:  99% (292/294)        
2023-04-10T02:36:45.6344096Z remote: Compressing objects: 100% (294/294)        
2023-04-10T02:36:45.6344452Z remote: Compressing objects: 100% (294/294), done.        
2023-04-10T02:36:45.6475295Z Receiving objects:   0% (1/1571)
2023-04-10T02:36:45.6475798Z Receiving objects:   1% (16/1571)
2023-04-10T02:36:45.6476137Z Receiving objects:   2% (32/1571)
2023-04-10T02:36:45.6476695Z Receiving objects:   3% (48/1571)
2023-04-10T02:36:45.6477042Z Receiving objects:   4% (63/1571)
2023-04-10T02:36:45.6477410Z Receiving objects:   5% (79/1571)
2023-04-10T02:36:45.6477749Z Receiving objects:   6% (95/1571)
2023-04-10T02:36:45.6478074Z Receiving objects:   7% (110/1571)
2023-04-10T02:36:45.6478360Z Receiving objects:   8% (126/1571)
2023-04-10T02:36:45.6478726Z Receiving objects:   9% (142/1571)
2023-04-10T02:36:45.6479050Z Receiving objects:  10% (158/1571)
2023-04-10T02:36:45.6479388Z Receiving objects:  11% (173/1571)
2023-04-10T02:36:45.6479709Z Receiving objects:  12% (189/1571)
2023-04-10T02:36:45.6480060Z Receiving objects:  13% (205/1571)
2023-04-10T02:36:45.6480388Z Receiving objects:  14% (220/1571)
2023-04-10T02:36:45.6480704Z Receiving objects:  15% (236/1571)
2023-04-10T02:36:45.6481023Z Receiving objects:  16% (252/1571)
2023-04-10T02:36:45.6481312Z Receiving objects:  17% (268/1571)
2023-04-10T02:36:45.6481670Z Receiving objects:  18% (283/1571)
2023-04-10T02:36:45.6482008Z Receiving objects:  19% (299/1571)
2023-04-10T02:36:45.6482328Z Receiving objects:  20% (315/1571)
2023-04-10T02:36:45.6482643Z Receiving objects:  21% (330/1571)
2023-04-10T02:36:45.6482999Z Receiving objects:  22% (346/1571)
2023-04-10T02:36:45.6483316Z Receiving objects:  23% (362/1571)
2023-04-10T02:36:45.6483631Z Receiving objects:  24% (378/1571)
2023-04-10T02:36:45.6484105Z Receiving objects:  25% (393/1571)
2023-04-10T02:36:45.6484422Z Receiving objects:  26% (409/1571)
2023-04-10T02:36:45.6484748Z Receiving objects:  27% (425/1571)
2023-04-10T02:36:45.6485071Z Receiving objects:  28% (440/1571)
2023-04-10T02:36:45.6499015Z Receiving objects:  29% (456/1571)
2023-04-10T02:36:45.6499911Z Receiving objects:  30% (472/1571)
2023-04-10T02:36:45.7508527Z Receiving objects:  31% (488/1571)
2023-04-10T02:36:45.7509048Z Receiving objects:  32% (503/1571)
2023-04-10T02:36:45.7509876Z Receiving objects:  33% (519/1571)
2023-04-10T02:36:45.7552234Z Receiving objects:  34% (535/1571)
2023-04-10T02:36:45.7557643Z Receiving objects:  35% (550/1571)
2023-04-10T02:36:45.7559012Z Receiving objects:  36% (566/1571)
2023-04-10T02:36:45.7559405Z Receiving objects:  37% (582/1571)
2023-04-10T02:36:45.7560872Z Receiving objects:  38% (597/1571)
2023-04-10T02:36:45.7562350Z Receiving objects:  39% (613/1571)
2023-04-10T02:36:45.7562687Z Receiving objects:  40% (629/1571)
2023-04-10T02:36:45.7563038Z Receiving objects:  41% (645/1571)
2023-04-10T02:36:45.7563385Z Receiving objects:  42% (660/1571)
2023-04-10T02:36:45.7563902Z Receiving objects:  43% (676/1571)
2023-04-10T02:36:45.7601143Z Receiving objects:  44% (692/1571)
2023-04-10T02:36:45.7603410Z Receiving objects:  45% (707/1571)
2023-04-10T02:36:45.7604388Z Receiving objects:  46% (723/1571)
2023-04-10T02:36:45.7605834Z Receiving objects:  47% (739/1571)
2023-04-10T02:36:45.7606186Z Receiving objects:  48% (755/1571)
2023-04-10T02:36:45.7606526Z Receiving objects:  49% (770/1571)
2023-04-10T02:36:45.7606874Z Receiving objects:  50% (786/1571)
2023-04-10T02:36:45.7607258Z Receiving objects:  51% (802/1571)
2023-04-10T02:36:45.7680219Z Receiving objects:  52% (817/1571)
2023-04-10T02:36:45.7680658Z Receiving objects:  53% (833/1571)
2023-04-10T02:36:45.7682191Z Receiving objects:  54% (849/1571)
2023-04-10T02:36:45.7682689Z Receiving objects:  55% (865/1571)
2023-04-10T02:36:45.7683031Z Receiving objects:  56% (880/1571)
2023-04-10T02:36:45.7730036Z Receiving objects:  57% (896/1571)
2023-04-10T02:36:45.7730436Z Receiving objects:  58% (912/1571)
2023-04-10T02:36:45.7730704Z Receiving objects:  59% (927/1571)
2023-04-10T02:36:45.7730961Z Receiving objects:  60% (943/1571)
2023-04-10T02:36:45.7731925Z Receiving objects:  61% (959/1571)
2023-04-10T02:36:45.7831169Z Receiving objects:  62% (975/1571)
2023-04-10T02:36:45.7839131Z Receiving objects:  63% (990/1571)
2023-04-10T02:36:45.7937558Z Receiving objects:  64% (1006/1571)
2023-04-10T02:36:45.7964271Z Receiving objects:  65% (1022/1571)
2023-04-10T02:36:45.7965466Z Receiving objects:  66% (1037/1571)
2023-04-10T02:36:45.7967279Z Receiving objects:  67% (1053/1571)
2023-04-10T02:36:45.7968482Z Receiving objects:  68% (1069/1571)
2023-04-10T02:36:45.7969904Z Receiving objects:  69% (1084/1571)
2023-04-10T02:36:45.7970952Z Receiving objects:  70% (1100/1571)
2023-04-10T02:36:45.7972727Z Receiving objects:  71% (1116/1571)
2023-04-10T02:36:45.7973803Z Receiving objects:  72% (1132/1571)
2023-04-10T02:36:45.7974261Z Receiving objects:  73% (1147/1571)
2023-04-10T02:36:45.7974652Z Receiving objects:  74% (1163/1571)
2023-04-10T02:36:45.7992723Z Receiving objects:  75% (1179/1571)
2023-04-10T02:36:45.7993106Z Receiving objects:  76% (1194/1571)
2023-04-10T02:36:45.7993673Z Receiving objects:  77% (1210/1571)
2023-04-10T02:36:45.7994334Z Receiving objects:  78% (1226/1571)
2023-04-10T02:36:45.7994892Z Receiving objects:  79% (1242/1571)
2023-04-10T02:36:45.7995149Z Receiving objects:  80% (1257/1571)
2023-04-10T02:36:45.7995398Z Receiving objects:  81% (1273/1571)
2023-04-10T02:36:45.7995751Z Receiving objects:  82% (1289/1571)
2023-04-10T02:36:45.7996385Z Receiving objects:  83% (1304/1571)
2023-04-10T02:36:45.7996955Z Receiving objects:  84% (1320/1571)
2023-04-10T02:36:45.7997501Z Receiving objects:  85% (1336/1571)
2023-04-10T02:36:45.7999803Z Receiving objects:  86% (1352/1571)
2023-04-10T02:36:45.8000211Z Receiving objects:  87% (1367/1571)
2023-04-10T02:36:45.8000755Z Receiving objects:  88% (1383/1571)
2023-04-10T02:36:45.8001372Z Receiving objects:  89% (1399/1571)
2023-04-10T02:36:45.8001969Z Receiving objects:  90% (1414/1571)
2023-04-10T02:36:45.8005814Z Receiving objects:  91% (1430/1571)
2023-04-10T02:36:45.8008189Z Receiving objects:  92% (1446/1571)
2023-04-10T02:36:45.8010235Z Receiving objects:  93% (1462/1571)
2023-04-10T02:36:45.8012886Z Receiving objects:  94% (1477/1571)
2023-04-10T02:36:45.8015859Z Receiving objects:  95% (1493/1571)
2023-04-10T02:36:45.8017567Z Receiving objects:  96% (1509/1571)
2023-04-10T02:36:45.8019842Z Receiving objects:  97% (1524/1571)
2023-04-10T02:36:45.8023295Z Receiving objects:  98% (1540/1571)
2023-04-10T02:36:45.8072058Z Receiving objects:  99% (1556/1571)
2023-04-10T02:36:45.8072881Z remote: Total 1571 (delta 255), reused 412 (delta 211), pack-reused 1061        
2023-04-10T02:36:45.8077040Z Receiving objects: 100% (1571/1571)
2023-04-10T02:36:45.8077728Z Receiving objects: 100% (1571/1571), 1.67 MiB | 9.91 MiB/s, done.
2023-04-10T02:36:45.8082602Z Resolving deltas:   0% (0/786)
2023-04-10T02:36:45.8082960Z Resolving deltas:   1% (8/786)
2023-04-10T02:36:45.8086266Z Resolving deltas:   2% (16/786)
2023-04-10T02:36:45.8086663Z Resolving deltas:   3% (24/786)
2023-04-10T02:36:45.8087240Z Resolving deltas:   4% (32/786)
2023-04-10T02:36:45.8089143Z Resolving deltas:   5% (40/786)
2023-04-10T02:36:45.8089819Z Resolving deltas:   6% (48/786)
2023-04-10T02:36:45.8091772Z Resolving deltas:   7% (56/786)
2023-04-10T02:36:45.8093403Z Resolving deltas:   8% (63/786)
2023-04-10T02:36:45.8095045Z Resolving deltas:   9% (71/786)
2023-04-10T02:36:45.8096742Z Resolving deltas:  10% (79/786)
2023-04-10T02:36:45.8098488Z Resolving deltas:  11% (87/786)
2023-04-10T02:36:45.8100084Z Resolving deltas:  12% (95/786)
2023-04-10T02:36:45.8101889Z Resolving deltas:  13% (103/786)
2023-04-10T02:36:45.8103558Z Resolving deltas:  14% (111/786)
2023-04-10T02:36:45.8105410Z Resolving deltas:  15% (118/786)
2023-04-10T02:36:45.8108783Z Resolving deltas:  16% (126/786)
2023-04-10T02:36:45.8109112Z Resolving deltas:  17% (134/786)
2023-04-10T02:36:45.8109449Z Resolving deltas:  18% (142/786)
2023-04-10T02:36:45.8109703Z Resolving deltas:  19% (150/786)
2023-04-10T02:36:45.8112894Z Resolving deltas:  20% (158/786)
2023-04-10T02:36:45.8113186Z Resolving deltas:  21% (166/786)
2023-04-10T02:36:45.8113533Z Resolving deltas:  22% (173/786)
2023-04-10T02:36:45.8115967Z Resolving deltas:  23% (181/786)
2023-04-10T02:36:45.8118141Z Resolving deltas:  24% (189/786)
2023-04-10T02:36:45.8120515Z Resolving deltas:  25% (197/786)
2023-04-10T02:36:45.8123902Z Resolving deltas:  26% (205/786)
2023-04-10T02:36:45.8126178Z Resolving deltas:  27% (213/786)
2023-04-10T02:36:45.8129103Z Resolving deltas:  28% (221/786)
2023-04-10T02:36:45.8132072Z Resolving deltas:  29% (228/786)
2023-04-10T02:36:45.8134695Z Resolving deltas:  30% (236/786)
2023-04-10T02:36:45.8136937Z Resolving deltas:  31% (245/786)
2023-04-10T02:36:45.8140017Z Resolving deltas:  32% (252/786)
2023-04-10T02:36:45.8142889Z Resolving deltas:  33% (260/786)
2023-04-10T02:36:45.8143255Z Resolving deltas:  34% (268/786)
2023-04-10T02:36:45.8146170Z Resolving deltas:  35% (276/786)
2023-04-10T02:36:45.8152211Z Resolving deltas:  36% (283/786)
2023-04-10T02:36:45.8152574Z Resolving deltas:  37% (291/786)
2023-04-10T02:36:45.8154003Z Resolving deltas:  38% (299/786)
2023-04-10T02:36:45.8156800Z Resolving deltas:  39% (307/786)
2023-04-10T02:36:45.8158466Z Resolving deltas:  40% (315/786)
2023-04-10T02:36:45.8160745Z Resolving deltas:  41% (323/786)
2023-04-10T02:36:45.8162789Z Resolving deltas:  42% (332/786)
2023-04-10T02:36:45.8165037Z Resolving deltas:  43% (338/786)
2023-04-10T02:36:45.8167560Z Resolving deltas:  44% (346/786)
2023-04-10T02:36:45.8169742Z Resolving deltas:  45% (354/786)
2023-04-10T02:36:45.8172918Z Resolving deltas:  46% (362/786)
2023-04-10T02:36:45.8176608Z Resolving deltas:  47% (370/786)
2023-04-10T02:36:45.8178704Z Resolving deltas:  48% (378/786)
2023-04-10T02:36:45.8181204Z Resolving deltas:  49% (386/786)
2023-04-10T02:36:45.8183949Z Resolving deltas:  50% (393/786)
2023-04-10T02:36:45.8186603Z Resolving deltas:  51% (401/786)
2023-04-10T02:36:45.8189637Z Resolving deltas:  52% (409/786)
2023-04-10T02:36:45.8189999Z Resolving deltas:  53% (418/786)
2023-04-10T02:36:45.8191793Z Resolving deltas:  54% (425/786)
2023-04-10T02:36:45.8194061Z Resolving deltas:  55% (433/786)
2023-04-10T02:36:45.8196756Z Resolving deltas:  56% (441/786)
2023-04-10T02:36:45.8197528Z Resolving deltas:  57% (449/786)
2023-04-10T02:36:45.8200734Z Resolving deltas:  58% (456/786)
2023-04-10T02:36:45.8202959Z Resolving deltas:  59% (464/786)
2023-04-10T02:36:45.8204964Z Resolving deltas:  60% (472/786)
2023-04-10T02:36:45.8212138Z Resolving deltas:  61% (480/786)
2023-04-10T02:36:45.8280529Z Resolving deltas:  62% (488/786)
2023-04-10T02:36:45.8305166Z Resolving deltas:  63% (496/786)
2023-04-10T02:36:45.8320252Z Resolving deltas:  64% (504/786)
2023-04-10T02:36:45.8337581Z Resolving deltas:  65% (511/786)
2023-04-10T02:36:45.8358421Z Resolving deltas:  66% (519/786)
2023-04-10T02:36:45.8362316Z Resolving deltas:  67% (527/786)
2023-04-10T02:36:45.8364689Z Resolving deltas:  68% (535/786)
2023-04-10T02:36:45.8367930Z Resolving deltas:  69% (543/786)
2023-04-10T02:36:45.8368338Z Resolving deltas:  70% (551/786)
2023-04-10T02:36:45.8368605Z Resolving deltas:  71% (559/786)
2023-04-10T02:36:45.8369394Z Resolving deltas:  72% (566/786)
2023-04-10T02:36:45.8371336Z Resolving deltas:  73% (574/786)
2023-04-10T02:36:45.8373017Z Resolving deltas:  74% (582/786)
2023-04-10T02:36:45.8374801Z Resolving deltas:  75% (590/786)
2023-04-10T02:36:45.8376370Z Resolving deltas:  76% (598/786)
2023-04-10T02:36:45.8378247Z Resolving deltas:  77% (606/786)
2023-04-10T02:36:45.8379848Z Resolving deltas:  78% (614/786)
2023-04-10T02:36:45.8381640Z Resolving deltas:  79% (621/786)
2023-04-10T02:36:45.8383309Z Resolving deltas:  80% (629/786)
2023-04-10T02:36:45.8385052Z Resolving deltas:  81% (637/786)
2023-04-10T02:36:45.8386708Z Resolving deltas:  82% (645/786)
2023-04-10T02:36:45.8388390Z Resolving deltas:  83% (653/786)
2023-04-10T02:36:45.8390076Z Resolving deltas:  84% (661/786)
2023-04-10T02:36:45.8391824Z Resolving deltas:  85% (669/786)
2023-04-10T02:36:45.8393668Z Resolving deltas:  86% (676/786)
2023-04-10T02:36:45.8395530Z Resolving deltas:  87% (684/786)
2023-04-10T02:36:45.8397658Z Resolving deltas:  88% (692/786)
2023-04-10T02:36:45.8400016Z Resolving deltas:  89% (700/786)
2023-04-10T02:36:45.8400839Z Resolving deltas:  90% (708/786)
2023-04-10T02:36:45.8403569Z Resolving deltas:  91% (716/786)
2023-04-10T02:36:45.8406140Z Resolving deltas:  92% (724/786)
2023-04-10T02:36:45.8410007Z Resolving deltas:  93% (731/786)
2023-04-10T02:36:45.8413187Z Resolving deltas:  94% (739/786)
2023-04-10T02:36:45.8415990Z Resolving deltas:  95% (747/786)
2023-04-10T02:36:45.8419090Z Resolving deltas:  96% (755/786)
2023-04-10T02:36:45.8421570Z Resolving deltas:  97% (763/786)
2023-04-10T02:36:45.8425761Z Resolving deltas:  98% (771/786)
2023-04-10T02:36:45.8482992Z Resolving deltas:  99% (779/786)
2023-04-10T02:36:45.8483524Z Resolving deltas: 100% (786/786)
2023-04-10T02:36:45.8484204Z Resolving deltas: 100% (786/786), done.
2023-04-10T02:36:45.8700455Z From https://github.com/CasperDash/useWallet
2023-04-10T02:36:45.8701334Z  * [new branch]      build-core                  -> origin/build-core
2023-04-10T02:36:45.8702201Z  * [new branch]      build-react                 -> origin/build-react
2023-04-10T02:36:45.8702842Z  * [new branch]      build-react-2               -> origin/build-react-2
2023-04-10T02:36:45.8703700Z  * [new branch]      build-react-core-2          -> origin/build-react-core-2
2023-04-10T02:36:45.8704337Z  * [new branch]      build/core                  -> origin/build/core
2023-04-10T02:36:45.8705371Z  * [new branch]      build/react                 -> origin/build/react
2023-04-10T02:36:45.8706000Z  * [new branch]      chore/remove-space          -> origin/chore/remove-space
2023-04-10T02:36:45.8706812Z  * [new branch]      develop                     -> origin/develop
2023-04-10T02:36:45.8707674Z  * [new branch]      doc                         -> origin/doc
2023-04-10T02:36:45.8708529Z  * [new branch]      docs/import-wallet-on-readme -> origin/docs/import-wallet-on-readme
2023-04-10T02:36:45.8709215Z  * [new branch]      docs/update-hooks           -> origin/docs/update-hooks
2023-04-10T02:36:45.8710088Z  * [new branch]      docs/update-readme-features -> origin/docs/update-readme-features
2023-04-10T02:36:45.8710798Z  * [new branch]      feat/#36-integrate-with-ledger -> origin/feat/#36-integrate-with-ledger
2023-04-10T02:36:45.8711652Z  * [new branch]      feat/actions                -> origin/feat/actions
2023-04-10T02:36:45.8712318Z  * [new branch]      feat/casper-wallet-connector -> origin/feat/casper-wallet-connector
2023-04-10T02:36:45.8713170Z  * [new branch]      feat/connectors             -> origin/feat/connectors
2023-04-10T02:36:45.8713828Z  * [new branch]      feat/window-events-account  -> origin/feat/window-events-account
2023-04-10T02:36:45.8715225Z  * [new branch]      feature/documentation       -> origin/feature/documentation
2023-04-10T02:36:45.8715780Z  * [new branch]      fix/auto-connect            -> origin/fix/auto-connect
2023-04-10T02:36:45.8716420Z  * [new branch]      fix/onconnect-event-with-use-account -> origin/fix/onconnect-event-with-use-account
2023-04-10T02:36:45.8717073Z  * [new branch]      improvement-add-comments    -> origin/improvement-add-comments
2023-04-10T02:36:45.8717600Z  * [new branch]      main                        -> origin/main
2023-04-10T02:36:45.8718196Z  * [new branch]      refactor/rename-casper-dash-global -> origin/refactor/rename-casper-dash-global
2023-04-10T02:36:45.8718777Z  * [new branch]      release/0.0.1               -> origin/release/0.0.1
2023-04-10T02:36:45.8719274Z  * [new branch]      release/0.0.2               -> origin/release/0.0.2
2023-04-10T02:36:45.8719767Z  * [new branch]      release/0.0.3               -> origin/release/0.0.3
2023-04-10T02:36:45.8720249Z  * [new branch]      release/0.0.4               -> origin/release/0.0.4
2023-04-10T02:36:45.8720813Z  * [new branch]      test/casper-wallet-connector -> origin/test/casper-wallet-connector
2023-04-10T02:36:45.8721375Z  * [new branch]      test/use-account            -> origin/test/use-account
2023-04-10T02:36:45.8721878Z  * [new branch]      update-doc                  -> origin/update-doc
2023-04-10T02:36:45.8722428Z  * [new tag]         @casperdash/usewallet-core@0.0.1 -> @casperdash/usewallet-core@0.0.1
2023-04-10T02:36:45.8723010Z  * [new tag]         @casperdash/usewallet-core@0.0.2 -> @casperdash/usewallet-core@0.0.2
2023-04-10T02:36:45.8723769Z  * [new tag]         @casperdash/usewallet-core@0.0.3 -> @casperdash/usewallet-core@0.0.3
2023-04-10T02:36:45.8724336Z  * [new tag]         @casperdash/usewallet@0.0.1 -> @casperdash/usewallet@0.0.1
2023-04-10T02:36:45.8724877Z  * [new tag]         @casperdash/usewallet@0.0.2 -> @casperdash/usewallet@0.0.2
2023-04-10T02:36:45.8725405Z  * [new tag]         @casperdash/usewallet@0.0.3 -> @casperdash/usewallet@0.0.3
2023-04-10T02:36:45.8725895Z  * [new tag]         docs-0.0.2                  -> docs-0.0.2
2023-04-10T02:36:45.8726346Z  * [new tag]         docs-0.0.3                  -> docs-0.0.3
2023-04-10T02:36:45.8726789Z  * [new tag]         docs-0.0.4                  -> docs-0.0.4
2023-04-10T02:36:45.8727270Z  * [new tag]         docs-0.0.5                  -> docs-0.0.5
2023-04-10T02:36:45.8727710Z  * [new tag]         docs-0.0.6                  -> docs-0.0.6
2023-04-10T02:36:45.8743750Z [command]/usr/bin/git branch --list --remote origin/main
2023-04-10T02:36:45.8777525Z   origin/main
2023-04-10T02:36:45.8793552Z [command]/usr/bin/git rev-parse refs/remotes/origin/main
2023-04-10T02:36:45.8817060Z 25f8ac7a84341a7485ddf7707522bda42d38972c
2023-04-10T02:36:45.8822577Z ##[endgroup]
2023-04-10T02:36:45.8823199Z ##[group]Determining the checkout info
2023-04-10T02:36:45.8824538Z ##[endgroup]
2023-04-10T02:36:45.8826522Z ##[group]Checking out the ref
2023-04-10T02:36:45.8830302Z [command]/usr/bin/git checkout --progress --force -B main refs/remotes/origin/main
2023-04-10T02:36:45.9010514Z Switched to a new branch 'main'
2023-04-10T02:36:45.9011190Z branch 'main' set up to track 'origin/main'.
2023-04-10T02:36:45.9018196Z ##[endgroup]
2023-04-10T02:36:45.9058845Z [command]/usr/bin/git log -1 --format='%H'
2023-04-10T02:36:45.9087198Z '25f8ac7a84341a7485ddf7707522bda42d38972c'
2023-04-10T02:36:45.9378375Z ##[group]Run pnpm/action-setup@v2.2.4
2023-04-10T02:36:45.9378656Z with:
2023-04-10T02:36:45.9378863Z   version: 7.26.3
2023-04-10T02:36:45.9379092Z   dest: ~/setup-pnpm
2023-04-10T02:36:45.9379317Z   run_install: null
2023-04-10T02:36:45.9379535Z ##[endgroup]
2023-04-10T02:36:46.0568711Z ##[group]Running self-installer...
2023-04-10T02:36:46.5505309Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:36:46.5603032Z Packages: +1
2023-04-10T02:36:46.5603697Z +
2023-04-10T02:36:47.1428367Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:36:47.1428972Z   Content-addressable store is at: /home/runner/.pnpm-store/v3
2023-04-10T02:36:47.1429316Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:36:47.1702570Z 
2023-04-10T02:36:47.1702974Z dependencies:
2023-04-10T02:36:47.1703287Z + pnpm 7.26.3 (8.2.0 is available)
2023-04-10T02:36:47.1703456Z 
2023-04-10T02:36:47.5527492Z Progress: resolved 1, reused 0, downloaded 1, added 1, done
2023-04-10T02:36:47.5666137Z ##[endgroup]
2023-04-10T02:36:47.5670530Z Installation Completed!
2023-04-10T02:36:47.5811270Z ##[group]Run actions/setup-node@v3
2023-04-10T02:36:47.5811528Z with:
2023-04-10T02:36:47.5811720Z   cache: pnpm
2023-04-10T02:36:47.5811941Z   node-version: 18
2023-04-10T02:36:47.5812174Z   always-auth: false
2023-04-10T02:36:47.5812409Z   check-latest: false
2023-04-10T02:36:47.5812841Z   token: ***
2023-04-10T02:36:47.5813056Z env:
2023-04-10T02:36:47.5813339Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:47.5813613Z ##[endgroup]
2023-04-10T02:36:47.7846580Z Found in cache @ /opt/hostedtoolcache/node/18.15.0/x64
2023-04-10T02:36:47.7857511Z ##[group]Environment details
2023-04-10T02:36:48.6491342Z node: v18.15.0
2023-04-10T02:36:48.6492112Z npm: 9.5.0
2023-04-10T02:36:48.6493235Z yarn: 1.22.19
2023-04-10T02:36:48.6494395Z ##[endgroup]
2023-04-10T02:36:48.6505124Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm store path --silent
2023-04-10T02:36:49.1594928Z /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:36:49.2911475Z pnpm cache is not found
2023-04-10T02:36:49.3052541Z ##[group]Run pnpm i
2023-04-10T02:36:49.3052830Z [36;1mpnpm i[0m
2023-04-10T02:36:49.3110086Z shell: /usr/bin/bash -e {0}
2023-04-10T02:36:49.3110341Z env:
2023-04-10T02:36:49.3110634Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:36:49.3110915Z ##[endgroup]
2023-04-10T02:36:49.8712251Z Scope: all 5 workspace projects
2023-04-10T02:36:49.9534656Z Lockfile is up to date, resolution step is skipped
2023-04-10T02:36:50.0361273Z Progress: resolved 1, reused 0, downloaded 0, added 0
2023-04-10T02:36:50.2735280Z Packages: +1012
2023-04-10T02:36:50.2736101Z ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2023-04-10T02:36:50.8593708Z Packages are hard linked from the content-addressable store to the virtual store.
2023-04-10T02:36:50.8594993Z   Content-addressable store is at: /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:36:50.8595754Z   Virtual store is at:             node_modules/.pnpm
2023-04-10T02:36:51.0355685Z Progress: resolved 1012, reused 0, downloaded 14, added 11
2023-04-10T02:36:52.0419745Z Progress: resolved 1012, reused 0, downloaded 101, added 95
2023-04-10T02:36:53.0533895Z Progress: resolved 1012, reused 0, downloaded 173, added 172
2023-04-10T02:36:54.0529393Z Progress: resolved 1012, reused 0, downloaded 242, added 240
2023-04-10T02:36:55.0585603Z Progress: resolved 1012, reused 0, downloaded 322, added 319
2023-04-10T02:36:56.0655208Z Progress: resolved 1012, reused 0, downloaded 400, added 399
2023-04-10T02:36:57.0656739Z Progress: resolved 1012, reused 0, downloaded 480, added 483
2023-04-10T02:36:58.0663221Z Progress: resolved 1012, reused 0, downloaded 568, added 571
2023-04-10T02:36:59.0693348Z Progress: resolved 1012, reused 0, downloaded 674, added 676
2023-04-10T02:37:00.0832093Z Progress: resolved 1012, reused 0, downloaded 721, added 723
2023-04-10T02:37:01.1019922Z Progress: resolved 1012, reused 0, downloaded 772, added 773
2023-04-10T02:37:02.1035122Z Progress: resolved 1012, reused 0, downloaded 866, added 866
2023-04-10T02:37:03.1088435Z Progress: resolved 1012, reused 0, downloaded 949, added 949
2023-04-10T02:37:04.1090449Z Progress: resolved 1012, reused 0, downloaded 1001, added 1004
2023-04-10T02:37:05.1145759Z Progress: resolved 1012, reused 0, downloaded 1003, added 1007
2023-04-10T02:37:06.1140311Z Progress: resolved 1012, reused 0, downloaded 1006, added 1010
2023-04-10T02:37:07.1148149Z Progress: resolved 1012, reused 0, downloaded 1008, added 1010
2023-04-10T02:37:08.1352496Z Progress: resolved 1012, reused 0, downloaded 1008, added 1012, done
2023-04-10T02:37:08.3378110Z .../@napi-rs/simple-git-linux-x64-gnu postinstall$ node install.js
2023-04-10T02:37:08.3382521Z .../@napi-rs/simple-git-linux-x64-musl postinstall$ node install.js
2023-04-10T02:37:08.3760873Z .../node_modules/secp256k1 install$ npm run rebuild || echo "Secp256k1 bindings compilation fail. Pure JS implementation will be used."
2023-04-10T02:37:08.4007537Z .../keccak@3.0.3/node_modules/keccak install$ node-gyp-build || exit 0
2023-04-10T02:37:08.4013044Z .../node_modules/secp256k1 install$ node-gyp-build || exit 0
2023-04-10T02:37:08.4482089Z .../@napi-rs/simple-git-linux-x64-gnu postinstall: Done
2023-04-10T02:37:08.4858936Z .../@napi-rs/simple-git-linux-x64-musl postinstall: Failed
2023-04-10T02:37:08.6254035Z .../keccak@3.0.3/node_modules/keccak install: Done
2023-04-10T02:37:08.6622804Z .../node_modules/secp256k1 install: Done
2023-04-10T02:37:08.9189705Z .../node_modules/secp256k1 install: > secp256k1@3.7.1 rebuild
2023-04-10T02:37:08.9191072Z .../node_modules/secp256k1 install: > node-gyp rebuild
2023-04-10T02:37:09.0185143Z .../node_modules/secp256k1 install: gyp info it worked if it ends with ok
2023-04-10T02:37:09.0202556Z .../node_modules/secp256k1 install: gyp info using node-gyp@9.3.1
2023-04-10T02:37:09.0203189Z .../node_modules/secp256k1 install: gyp info using node@18.15.0 | linux | x64
2023-04-10T02:37:09.1132055Z .../node_modules/secp256k1 install: gyp info find Python using Python version 3.10.6 found at "/usr/bin/python3"
2023-04-10T02:37:09.2497429Z .../node_modules/secp256k1 install: gyp http GET https://nodejs.org/download/release/v18.15.0/node-v18.15.0-headers.tar.gz
2023-04-10T02:37:09.3411487Z .../node_modules/secp256k1 install: gyp http 200 https://nodejs.org/download/release/v18.15.0/node-v18.15.0-headers.tar.gz
2023-04-10T02:37:10.8923054Z .../node_modules/secp256k1 install: gyp http GET https://nodejs.org/download/release/v18.15.0/SHASUMS256.txt
2023-04-10T02:37:10.9161927Z .../node_modules/secp256k1 install: gyp http 200 https://nodejs.org/download/release/v18.15.0/SHASUMS256.txt
2023-04-10T02:37:10.9289739Z .../node_modules/secp256k1 install: gyp info spawn /usr/bin/python3
2023-04-10T02:37:10.9290750Z .../node_modules/secp256k1 install: gyp info spawn args [
2023-04-10T02:37:10.9292480Z .../node_modules/secp256k1 install: gyp info spawn args   '/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py',
2023-04-10T02:37:10.9293188Z .../node_modules/secp256k1 install: gyp info spawn args   'binding.gyp',
2023-04-10T02:37:10.9293743Z .../node_modules/secp256k1 install: gyp info spawn args   '-f',
2023-04-10T02:37:10.9294245Z .../node_modules/secp256k1 install: gyp info spawn args   'make',
2023-04-10T02:37:10.9294746Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:10.9295593Z .../node_modules/secp256k1 install: gyp info spawn args   '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build/config.gypi',
2023-04-10T02:37:10.9296565Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:10.9297338Z .../node_modules/secp256k1 install: gyp info spawn args   '/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/addon.gypi',
2023-04-10T02:37:10.9297934Z .../node_modules/secp256k1 install: gyp info spawn args   '-I',
2023-04-10T02:37:10.9298615Z .../node_modules/secp256k1 install: gyp info spawn args   '/home/runner/.cache/node-gyp/18.15.0/include/node/common.gypi',
2023-04-10T02:37:10.9299250Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dlibrary=shared_library',
2023-04-10T02:37:10.9299836Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dvisibility=default',
2023-04-10T02:37:10.9300516Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_root_dir=/home/runner/.cache/node-gyp/18.15.0',
2023-04-10T02:37:10.9301359Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_gyp_dir=/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp',
2023-04-10T02:37:10.9302207Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_lib_file=/home/runner/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
2023-04-10T02:37:10.9303354Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dmodule_root_dir=/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1',
2023-04-10T02:37:10.9304028Z .../node_modules/secp256k1 install: gyp info spawn args   '-Dnode_engine=v8',
2023-04-10T02:37:10.9304661Z .../node_modules/secp256k1 install: gyp info spawn args   '--depth=.',
2023-04-10T02:37:10.9305455Z .../node_modules/secp256k1 install: gyp info spawn args   '--no-parallel',
2023-04-10T02:37:10.9306102Z .../node_modules/secp256k1 install: gyp info spawn args   '--generator-output',
2023-04-10T02:37:10.9306700Z .../node_modules/secp256k1 install: gyp info spawn args   'build',
2023-04-10T02:37:10.9307310Z .../node_modules/secp256k1 install: gyp info spawn args   '-Goutput_dir=.'
2023-04-10T02:37:10.9307800Z .../node_modules/secp256k1 install: gyp info spawn args ]
2023-04-10T02:37:11.3885261Z .../node_modules/secp256k1 install: gyp info spawn make
2023-04-10T02:37:11.3886228Z .../node_modules/secp256k1 install: gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
2023-04-10T02:37:11.3906864Z .../node_modules/secp256k1 install: make: Entering directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build'
2023-04-10T02:37:11.3950577Z .../node_modules/secp256k1 install:   CXX(target) Release/obj.target/secp256k1/src/addon.o
2023-04-10T02:37:12.2742575Z .../node_modules/secp256k1 install: In file included from ../src/addon.cc:2:
2023-04-10T02:37:12.2744962Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2023-04-10T02:37:12.2746694Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2298:7: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2023-04-10T02:37:12.2748174Z .../node_modules/secp256k1 install:  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2023-04-10T02:37:12.2748898Z .../node_modules/secp256k1 install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:12.2787215Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::SetAccessor(v8::Local<v8::ObjectTemplate>, v8::Local<v8::String>, Nan::GetterCallback, Nan::SetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, Nan::imp::Sig)’:
2023-04-10T02:37:12.2789766Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2536:19: warning: ‘void v8::ObjectTemplate::SetAccessor(v8::Local<v8::Name>, v8::AccessorNameGetterCallback, v8::AccessorNameSetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, v8::Local<v8::AccessorSignature>, v8::SideEffectType, v8::SideEffectType)’ is deprecated: Do signature check in accessor [-Wdeprecated-declarations]
2023-04-10T02:37:12.2791410Z .../node_modules/secp256k1 install:  2536 |   tpl->SetAccessor(
2023-04-10T02:37:12.2791978Z .../node_modules/secp256k1 install:       |   ~~~~~~~~~~~~~~~~^
2023-04-10T02:37:12.2792515Z .../node_modules/secp256k1 install:  2537 |       name
2023-04-10T02:37:12.2793058Z .../node_modules/secp256k1 install:       |       ~~~~         
2023-04-10T02:37:12.2793587Z .../node_modules/secp256k1 install:  2538 |     , getter_
2023-04-10T02:37:12.2794118Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~      
2023-04-10T02:37:12.2794644Z .../node_modules/secp256k1 install:  2539 |     , setter_
2023-04-10T02:37:12.2795184Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~      
2023-04-10T02:37:12.2795708Z .../node_modules/secp256k1 install:  2540 |     , obj
2023-04-10T02:37:12.2796244Z .../node_modules/secp256k1 install:       |     ~~~~~          
2023-04-10T02:37:12.2796781Z .../node_modules/secp256k1 install:  2541 |     , settings
2023-04-10T02:37:12.2797314Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~     
2023-04-10T02:37:12.2797847Z .../node_modules/secp256k1 install:  2542 |     , attribute
2023-04-10T02:37:12.2798416Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~~    
2023-04-10T02:37:12.2798964Z .../node_modules/secp256k1 install:  2543 |     , signature);
2023-04-10T02:37:12.2799498Z .../node_modules/secp256k1 install:       |     ~~~~~~~~~~~~   
2023-04-10T02:37:12.2800382Z .../node_modules/secp256k1 install: In file included from /home/runner/.cache/node-gyp/18.15.0/include/node/v8-function.h:15,
2023-04-10T02:37:12.2801328Z .../node_modules/secp256k1 install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/v8.h:33,
2023-04-10T02:37:12.2816785Z .../node_modules/secp256k1 install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:73,
2023-04-10T02:37:12.2817393Z .../node_modules/secp256k1 install:                  from ../src/addon.cc:1:
2023-04-10T02:37:12.2818248Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/v8-template.h:838:8: note: declared here
2023-04-10T02:37:12.2818902Z .../node_modules/secp256k1 install:   838 |   void SetAccessor(
2023-04-10T02:37:12.2819584Z .../node_modules/secp256k1 install:       |        ^~~~~~~~~~~
2023-04-10T02:37:12.2887459Z .../node_modules/secp256k1 install: In file included from ../../../../nan@2.14.0/node_modules/nan/nan.h:2884,
2023-04-10T02:37:12.2888007Z .../node_modules/secp256k1 install:                  from ../src/addon.cc:2:
2023-04-10T02:37:12.2889156Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h: In constructor ‘Nan::TypedArrayContents<T>::TypedArrayContents(v8::Local<v8::Value>)’:
2023-04-10T02:37:12.2890274Z .../node_modules/secp256k1 install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h:34:43: error: ‘class v8::ArrayBuffer’ has no member named ‘GetContents’
2023-04-10T02:37:12.2891116Z .../node_modules/secp256k1 install:    34 |       data   = static_cast<char*>(buffer->GetContents().Data()) + byte_offset;
2023-04-10T02:37:12.2891641Z .../node_modules/secp256k1 install:       |                                           ^~~~~~~~~~~
2023-04-10T02:37:12.2910337Z .../node_modules/secp256k1 install: In file included from ../src/addon.cc:1:
2023-04-10T02:37:12.2910849Z .../node_modules/secp256k1 install: ../src/addon.cc: At global scope:
2023-04-10T02:37:12.2912551Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:978:7: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2023-04-10T02:37:12.2913740Z .../node_modules/secp256k1 install:   978 |       (node::addon_register_func) (regfunc),                          \
2023-04-10T02:37:12.2914231Z .../node_modules/secp256k1 install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:12.2915014Z .../node_modules/secp256k1 install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:1012:3: note: in expansion of macro ‘NODE_MODULE_X’
2023-04-10T02:37:12.2923321Z .../node_modules/secp256k1 install:  1012 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2023-04-10T02:37:12.2923830Z .../node_modules/secp256k1 install:       |   ^~~~~~~~~~~~~
2023-04-10T02:37:12.2924539Z .../node_modules/secp256k1 install: ../src/addon.cc:50:1: note: in expansion of macro ‘NODE_MODULE’
2023-04-10T02:37:12.2925036Z .../node_modules/secp256k1 install:    50 | NODE_MODULE(secp256k1, Init)
2023-04-10T02:37:12.2925460Z .../node_modules/secp256k1 install:       | ^~~~~~~~~~~
2023-04-10T02:37:12.3699986Z .../node_modules/secp256k1 install: make: *** [secp256k1.target.mk:168: Release/obj.target/secp256k1/src/addon.o] Error 1
2023-04-10T02:37:12.3706169Z .../node_modules/secp256k1 install: gyp ERR! build error 
2023-04-10T02:37:12.3706767Z .../node_modules/secp256k1 install: gyp ERR! stack Error: `make` failed with exit code: 2
2023-04-10T02:37:12.3708141Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess.onExit (/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/lib/build.js:203:23)
2023-04-10T02:37:12.3708914Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
2023-04-10T02:37:12.3709631Z .../node_modules/secp256k1 install: gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
2023-04-10T02:37:12.3710346Z .../node_modules/secp256k1 install: gyp ERR! System Linux 5.15.0-1035-azure
2023-04-10T02:37:12.3711481Z .../node_modules/secp256k1 install: gyp ERR! command "/opt/hostedtoolcache/node/18.15.0/x64/bin/node" "/opt/hostedtoolcache/node/18.15.0/x64/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
2023-04-10T02:37:12.3712379Z .../node_modules/secp256k1 install: gyp ERR! cwd /home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1
2023-04-10T02:37:12.3713051Z .../node_modules/secp256k1 install: gyp ERR! node -v v18.15.0
2023-04-10T02:37:12.3713925Z .../node_modules/secp256k1 install: gyp ERR! node-gyp -v v9.3.1
2023-04-10T02:37:12.3714401Z .../node_modules/secp256k1 install: gyp ERR! not ok 
2023-04-10T02:37:12.3715322Z .../node_modules/secp256k1 install: make: Leaving directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/secp256k1@3.7.1/node_modules/secp256k1/build'
2023-04-10T02:37:12.3839284Z .../node_modules/secp256k1 install: Secp256k1 bindings compilation fail. Pure JS implementation will be used.
2023-04-10T02:37:12.3846195Z .../node_modules/secp256k1 install: Done
2023-04-10T02:37:12.4543880Z .../node_modules/@swc/core postinstall$ node postinstall.js
2023-04-10T02:37:12.4714796Z .../eccrypto@1.1.6/node_modules/eccrypto install$ node-gyp rebuild || exit 0
2023-04-10T02:37:12.4913137Z .../esbuild@0.15.18/node_modules/esbuild postinstall$ node install.js
2023-04-10T02:37:12.4946837Z .../esbuild@0.17.12/node_modules/esbuild postinstall$ node install.js
2023-04-10T02:37:12.5394969Z .../node_modules/@swc/core postinstall: Done
2023-04-10T02:37:12.6102473Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info it worked if it ends with ok
2023-04-10T02:37:12.6121197Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info using node-gyp@9.3.1
2023-04-10T02:37:12.6121772Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info using node@18.15.0 | linux | x64
2023-04-10T02:37:12.6346487Z .../esbuild@0.15.18/node_modules/esbuild postinstall: Done
2023-04-10T02:37:12.6408113Z .../esbuild@0.17.12/node_modules/esbuild postinstall: Done
2023-04-10T02:37:12.7277429Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info find Python using Python version 3.10.6 found at "/usr/bin/python3"
2023-04-10T02:37:12.8418654Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn /usr/bin/python3
2023-04-10T02:37:12.8426614Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args [
2023-04-10T02:37:12.8431319Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/gyp/gyp_main.py',
2023-04-10T02:37:12.8433988Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'binding.gyp',
2023-04-10T02:37:12.8439066Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-f',
2023-04-10T02:37:12.8442379Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'make',
2023-04-10T02:37:12.8445324Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:12.8448773Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build/config.gypi',
2023-04-10T02:37:12.8451406Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:12.8454752Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/addon.gypi',
2023-04-10T02:37:12.8457471Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-I',
2023-04-10T02:37:12.8460433Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '/home/runner/.cache/node-gyp/18.15.0/include/node/common.gypi',
2023-04-10T02:37:12.8463321Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dlibrary=shared_library',
2023-04-10T02:37:12.8466440Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dvisibility=default',
2023-04-10T02:37:12.8469465Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_root_dir=/home/runner/.cache/node-gyp/18.15.0',
2023-04-10T02:37:12.8472655Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_gyp_dir=/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp',
2023-04-10T02:37:12.8475900Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_lib_file=/home/runner/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
2023-04-10T02:37:12.8478704Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dmodule_root_dir=/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto',
2023-04-10T02:37:12.8481365Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Dnode_engine=v8',
2023-04-10T02:37:12.8484275Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--depth=.',
2023-04-10T02:37:12.8487206Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--no-parallel',
2023-04-10T02:37:12.8490085Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '--generator-output',
2023-04-10T02:37:12.8493640Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   'build',
2023-04-10T02:37:12.8494481Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args   '-Goutput_dir=.'
2023-04-10T02:37:12.8495400Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args ]
2023-04-10T02:37:13.0071168Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn make
2023-04-10T02:37:13.0075920Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp info spawn args [ 'BUILDTYPE=Release', '-C', 'build' ]
2023-04-10T02:37:13.0083802Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: Entering directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build'
2023-04-10T02:37:13.0092729Z .../eccrypto@1.1.6/node_modules/eccrypto install:   CXX(target) Release/obj.target/ecdh/ecdh.o
2023-04-10T02:37:13.6987559Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:2:
2023-04-10T02:37:13.6992599Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::AsyncQueueWorker(Nan::AsyncWorker*)’:
2023-04-10T02:37:13.6994526Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2298:7: warning: cast between incompatible function types from ‘void (*)(uv_work_t*)’ {aka ‘void (*)(uv_work_s*)’} to ‘uv_after_work_cb’ {aka ‘void (*)(uv_work_s*, int)’} [-Wcast-function-type]
2023-04-10T02:37:13.6995621Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2298 |     , reinterpret_cast<uv_after_work_cb>(AsyncExecuteComplete)
2023-04-10T02:37:13.6996392Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7027081Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h: In function ‘void Nan::SetAccessor(v8::Local<v8::ObjectTemplate>, v8::Local<v8::String>, Nan::GetterCallback, Nan::SetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, Nan::imp::Sig)’:
2023-04-10T02:37:13.7029397Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan.h:2536:19: warning: ‘void v8::ObjectTemplate::SetAccessor(v8::Local<v8::Name>, v8::AccessorNameGetterCallback, v8::AccessorNameSetterCallback, v8::Local<v8::Value>, v8::AccessControl, v8::PropertyAttribute, v8::Local<v8::AccessorSignature>, v8::SideEffectType, v8::SideEffectType)’ is deprecated: Do signature check in accessor [-Wdeprecated-declarations]
2023-04-10T02:37:13.7030551Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2536 |   tpl->SetAccessor(
2023-04-10T02:37:13.7031104Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~~~~~~^
2023-04-10T02:37:13.7031706Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2537 |       name
2023-04-10T02:37:13.7032310Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ~~~~         
2023-04-10T02:37:13.7032815Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2538 |     , getter_
2023-04-10T02:37:13.7033336Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~      
2023-04-10T02:37:13.7034175Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2539 |     , setter_
2023-04-10T02:37:13.7034724Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~      
2023-04-10T02:37:13.7035334Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2540 |     , obj
2023-04-10T02:37:13.7049761Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~          
2023-04-10T02:37:13.7050523Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2541 |     , settings
2023-04-10T02:37:13.7051245Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~     
2023-04-10T02:37:13.7051988Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2542 |     , attribute
2023-04-10T02:37:13.7052698Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~~    
2023-04-10T02:37:13.7053416Z .../eccrypto@1.1.6/node_modules/eccrypto install:  2543 |     , signature);
2023-04-10T02:37:13.7054127Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ~~~~~~~~~~~~   
2023-04-10T02:37:13.7055261Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from /home/runner/.cache/node-gyp/18.15.0/include/node/v8-function.h:15,
2023-04-10T02:37:13.7056324Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/v8.h:33,
2023-04-10T02:37:13.7057353Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:73,
2023-04-10T02:37:13.7058139Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from ../ecdh.cc:1:
2023-04-10T02:37:13.7059495Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/v8-template.h:838:8: note: declared here
2023-04-10T02:37:13.7060296Z .../eccrypto@1.1.6/node_modules/eccrypto install:   838 |   void SetAccessor(
2023-04-10T02:37:13.7060948Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |        ^~~~~~~~~~~
2023-04-10T02:37:13.7118819Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../../../../nan@2.14.0/node_modules/nan/nan.h:2884,
2023-04-10T02:37:13.7121368Z .../eccrypto@1.1.6/node_modules/eccrypto install:                  from ../ecdh.cc:2:
2023-04-10T02:37:13.7130198Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h: In constructor ‘Nan::TypedArrayContents<T>::TypedArrayContents(v8::Local<v8::Value>)’:
2023-04-10T02:37:13.7134728Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../../../../nan@2.14.0/node_modules/nan/nan_typedarray_contents.h:34:43: error: ‘class v8::ArrayBuffer’ has no member named ‘GetContents’
2023-04-10T02:37:13.7148248Z .../eccrypto@1.1.6/node_modules/eccrypto install:    34 |       data   = static_cast<char*>(buffer->GetContents().Data()) + byte_offset;
2023-04-10T02:37:13.7151165Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                           ^~~~~~~~~~~
2023-04-10T02:37:13.7358460Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc: In function ‘int derive(const uint8_t*, const uint8_t*, uint8_t*)’:
2023-04-10T02:37:13.7362501Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:37:41: warning: ‘EC_KEY* EC_KEY_new_by_curve_name(int)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7365780Z .../eccrypto@1.1.6/node_modules/eccrypto install:    37 |   CHECK((pkey = EC_KEY_new_by_curve_name(NID_secp256k1)) != NULL);
2023-04-10T02:37:13.7368722Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                 ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:13.7371840Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:13.7374741Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:13.7377383Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:13.7380685Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7383907Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:998:31: note: declared here
2023-04-10T02:37:13.7387254Z .../eccrypto@1.1.6/node_modules/eccrypto install:   998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
2023-04-10T02:37:13.7390090Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                               ^~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7395099Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:38:31: warning: ‘int EC_KEY_set_private_key(EC_KEY*, const BIGNUM*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7398082Z .../eccrypto@1.1.6/node_modules/eccrypto install:    38 |   CHECK(EC_KEY_set_private_key(pkey, pkey_bn) == 1);
2023-04-10T02:37:13.7400825Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:13.7403865Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:13.7406760Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:13.7409474Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:13.7412029Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7415603Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1056:27: note: declared here
2023-04-10T02:37:13.7418578Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1056 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_private_key(EC_KEY *key, const BIGNUM *prv);
2023-04-10T02:37:13.7421418Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7424358Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:40:29: warning: ‘int EVP_PKEY_set1_EC_KEY(EVP_PKEY*, ec_key_st*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7427161Z .../eccrypto@1.1.6/node_modules/eccrypto install:    40 |   CHECK(EVP_PKEY_set1_EC_KEY(evp_pkey, pkey) == 1);
2023-04-10T02:37:13.7429567Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7432185Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:13.7434734Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:13.7437050Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:13.7439383Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:3:
2023-04-10T02:37:13.7441999Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/evp.h:1370:5: note: declared here
2023-04-10T02:37:13.7444657Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1370 | int EVP_PKEY_set1_EC_KEY(EVP_PKEY *pkey, struct ec_key_st *key);
2023-04-10T02:37:13.7447178Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7450197Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:43:44: warning: ‘EC_KEY* EC_KEY_new_by_curve_name(int)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7452801Z .../eccrypto@1.1.6/node_modules/eccrypto install:    43 |   CHECK((peerkey = EC_KEY_new_by_curve_name(NID_secp256k1)) != NULL);
2023-04-10T02:37:13.7455269Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                    ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:13.7458161Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:13.7460798Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:13.7463128Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:13.7465648Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7468471Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:998:31: note: declared here
2023-04-10T02:37:13.7471032Z .../eccrypto@1.1.6/node_modules/eccrypto install:   998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
2023-04-10T02:37:13.7473409Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                               ^~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7476557Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:51:50: warning: ‘int EC_POINT_set_compressed_coordinates_GFp(const EC_GROUP*, EC_POINT*, const BIGNUM*, int, BN_CTX*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7479307Z .../eccrypto@1.1.6/node_modules/eccrypto install:    51 |     res = EC_POINT_set_compressed_coordinates_GFp(peerkey_group,
2023-04-10T02:37:13.7481715Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~
2023-04-10T02:37:13.7484118Z .../eccrypto@1.1.6/node_modules/eccrypto install:    52 |                                                  peerkey_p,
2023-04-10T02:37:13.7486852Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~
2023-04-10T02:37:13.7489204Z .../eccrypto@1.1.6/node_modules/eccrypto install:    53 |                                                  peerkey_bn,
2023-04-10T02:37:13.7491606Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~
2023-04-10T02:37:13.7494012Z .../eccrypto@1.1.6/node_modules/eccrypto install:    54 |                                                  compressed_y_bit,
2023-04-10T02:37:13.7496408Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7498705Z .../eccrypto@1.1.6/node_modules/eccrypto install:    55 |                                                  NULL);
2023-04-10T02:37:13.7501036Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~
2023-04-10T02:37:13.7503383Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7506281Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:686:27: note: declared here
2023-04-10T02:37:13.7508772Z .../eccrypto@1.1.6/node_modules/eccrypto install:   686 | OSSL_DEPRECATEDIN_3_0 int EC_POINT_set_compressed_coordinates_GFp
2023-04-10T02:37:13.7511175Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7514144Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:57:32: warning: ‘int EC_KEY_set_public_key(EC_KEY*, const EC_POINT*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7516734Z .../eccrypto@1.1.6/node_modules/eccrypto install:    57 |     res = EC_KEY_set_public_key(peerkey, peerkey_p);
2023-04-10T02:37:13.7519160Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7521501Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7524161Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1070:27: note: declared here
2023-04-10T02:37:13.7526955Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1070 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_public_key(EC_KEY *key, const EC_POINT *pub);
2023-04-10T02:37:13.7529486Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7532622Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:62:51: warning: ‘int EC_KEY_set_public_key_affine_coordinates(EC_KEY*, BIGNUM*, BIGNUM*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7535430Z .../eccrypto@1.1.6/node_modules/eccrypto install:    62 |     res = EC_KEY_set_public_key_affine_coordinates(peerkey,
2023-04-10T02:37:13.7537845Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~
2023-04-10T02:37:13.7540286Z .../eccrypto@1.1.6/node_modules/eccrypto install:    63 |                                                  peerkey_bn_x,
2023-04-10T02:37:13.7542699Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~
2023-04-10T02:37:13.7545221Z .../eccrypto@1.1.6/node_modules/eccrypto install:    64 |                                                  peerkey_bn_y);
2023-04-10T02:37:13.7547649Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                                  ~~~~~~~~~~~~~
2023-04-10T02:37:13.7549986Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7552626Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1122:27: note: declared here
2023-04-10T02:37:13.7555653Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1122 | OSSL_DEPRECATEDIN_3_0 int EC_KEY_set_public_key_affine_coordinates(EC_KEY *key,
2023-04-10T02:37:13.7558096Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7561029Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:69:29: warning: ‘int EVP_PKEY_set1_EC_KEY(EVP_PKEY*, ec_key_st*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7563663Z .../eccrypto@1.1.6/node_modules/eccrypto install:    69 |   CHECK(EVP_PKEY_set1_EC_KEY(evp_peerkey, peerkey) == 1);
2023-04-10T02:37:13.7566181Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |         ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7568782Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:14:32: note: in definition of macro ‘CHECK’
2023-04-10T02:37:13.7571307Z .../eccrypto@1.1.6/node_modules/eccrypto install:    14 | #define CHECK(cond) do { if (!(cond)) goto error; } while (0)
2023-04-10T02:37:13.7573847Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                                ^~~~
2023-04-10T02:37:13.7576123Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:3:
2023-04-10T02:37:13.7578820Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/evp.h:1370:5: note: declared here
2023-04-10T02:37:13.7581422Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1370 | int EVP_PKEY_set1_EC_KEY(EVP_PKEY *pkey, struct ec_key_st *key);
2023-04-10T02:37:13.7583767Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |     ^~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7586729Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:82:14: warning: ‘void EC_KEY_free(EC_KEY*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7589445Z .../eccrypto@1.1.6/node_modules/eccrypto install:    82 |   EC_KEY_free(peerkey);
2023-04-10T02:37:13.7591698Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~^~~~~~~~~
2023-04-10T02:37:13.7594178Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7597576Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1003:28: note: declared here
2023-04-10T02:37:13.7600264Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1003 | OSSL_DEPRECATEDIN_3_0 void EC_KEY_free(EC_KEY *key);
2023-04-10T02:37:13.7602757Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                            ^~~~~~~~~~~
2023-04-10T02:37:13.7605617Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:90:14: warning: ‘void EC_KEY_free(EC_KEY*)’ is deprecated: Since OpenSSL 3.0 [-Wdeprecated-declarations]
2023-04-10T02:37:13.7608148Z .../eccrypto@1.1.6/node_modules/eccrypto install:    90 |   EC_KEY_free(pkey);
2023-04-10T02:37:13.7610382Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ~~~~~~~~~~~^~~~~~
2023-04-10T02:37:13.7612795Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:4:
2023-04-10T02:37:13.7615456Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/openssl/ec.h:1003:28: note: declared here
2023-04-10T02:37:13.7618086Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1003 | OSSL_DEPRECATEDIN_3_0 void EC_KEY_free(EC_KEY *key);
2023-04-10T02:37:13.7620414Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |                            ^~~~~~~~~~~
2023-04-10T02:37:13.7622853Z .../eccrypto@1.1.6/node_modules/eccrypto install: In file included from ../ecdh.cc:1:
2023-04-10T02:37:13.7625194Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc: At global scope:
2023-04-10T02:37:13.7628965Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:978:7: warning: cast between incompatible function types from ‘void (*)(Nan::ADDON_REGISTER_FUNCTION_ARGS_TYPE)’ {aka ‘void (*)(v8::Local<v8::Object>)’} to ‘node::addon_register_func’ {aka ‘void (*)(v8::Local<v8::Object>, v8::Local<v8::Value>, void*)’} [-Wcast-function-type]
2023-04-10T02:37:13.7632225Z .../eccrypto@1.1.6/node_modules/eccrypto install:   978 |       (node::addon_register_func) (regfunc),                          \
2023-04-10T02:37:13.7634768Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
2023-04-10T02:37:13.7637565Z .../eccrypto@1.1.6/node_modules/eccrypto install: /home/runner/.cache/node-gyp/18.15.0/include/node/node.h:1012:3: note: in expansion of macro ‘NODE_MODULE_X’
2023-04-10T02:37:13.7640233Z .../eccrypto@1.1.6/node_modules/eccrypto install:  1012 |   NODE_MODULE_X(modname, regfunc, NULL, 0)  // NOLINT (readability/null_usage)
2023-04-10T02:37:13.7642626Z .../eccrypto@1.1.6/node_modules/eccrypto install:       |   ^~~~~~~~~~~~~
2023-04-10T02:37:13.7645213Z .../eccrypto@1.1.6/node_modules/eccrypto install: ../ecdh.cc:131:1: note: in expansion of macro ‘NODE_MODULE’
2023-04-10T02:37:13.7647759Z .../eccrypto@1.1.6/node_modules/eccrypto install:   131 | NODE_MODULE(ecdh, InitAll)
2023-04-10T02:37:13.7650015Z .../eccrypto@1.1.6/node_modules/eccrypto install:       | ^~~~~~~~~~~
2023-04-10T02:37:13.8277180Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: *** [ecdh.target.mk:119: Release/obj.target/ecdh/ecdh.o] Error 1
2023-04-10T02:37:13.8278920Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! build error 
2023-04-10T02:37:13.8279510Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack Error: `make` failed with exit code: 2
2023-04-10T02:37:13.8280815Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess.onExit (/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/lib/build.js:203:23)
2023-04-10T02:37:13.8281585Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
2023-04-10T02:37:13.8282257Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
2023-04-10T02:37:13.8282933Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! System Linux 5.15.0-1035-azure
2023-04-10T02:37:13.8284536Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! command "/opt/hostedtoolcache/node/18.15.0/x64/bin/node" "/home/runner/setup-pnpm/node_modules/.pnpm/pnpm@7.26.3/node_modules/pnpm/dist/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
2023-04-10T02:37:13.8285589Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! cwd /home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto
2023-04-10T02:37:13.8286243Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! node -v v18.15.0
2023-04-10T02:37:13.8286826Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! node-gyp -v v9.3.1
2023-04-10T02:37:13.8287283Z .../eccrypto@1.1.6/node_modules/eccrypto install: gyp ERR! not ok 
2023-04-10T02:37:13.8288146Z .../eccrypto@1.1.6/node_modules/eccrypto install: make: Leaving directory '/home/runner/work/useWallet/useWallet/node_modules/.pnpm/eccrypto@1.1.6/node_modules/eccrypto/build'
2023-04-10T02:37:13.8327400Z .../eccrypto@1.1.6/node_modules/eccrypto install: Done
2023-04-10T02:37:14.0348733Z 
2023-04-10T02:37:14.0350088Z devDependencies:
2023-04-10T02:37:14.0350628Z + @babel/core 7.20.12
2023-04-10T02:37:14.0351504Z + @changesets/changelog-github 0.4.8
2023-04-10T02:37:14.0352036Z + @changesets/cli 2.26.0
2023-04-10T02:37:14.0352804Z + @typescript-eslint/eslint-plugin 5.48.0
2023-04-10T02:37:14.0353386Z + @typescript-eslint/parser 5.48.0
2023-04-10T02:37:14.0406664Z + @vitest/coverage-c8 0.28.3
2023-04-10T02:37:14.0406960Z + @vitest/ui 0.28.4
2023-04-10T02:37:14.0407192Z + eslint 8.31.0
2023-04-10T02:37:14.0407955Z + eslint-config-airbnb-typescript 17.0.0
2023-04-10T02:37:14.0408364Z + eslint-config-prettier 8.6.0
2023-04-10T02:37:14.0408705Z + eslint-plugin-import 2.26.0
2023-04-10T02:37:14.0409082Z + eslint-plugin-prettier 4.2.1
2023-04-10T02:37:14.0409422Z + eslint-plugin-sonar 0.9.2
2023-04-10T02:37:14.0409673Z + husky 8.0.3
2023-04-10T02:37:14.0409892Z + jsdom 20.0.3
2023-04-10T02:37:14.0410170Z + lint-staged 13.1.0
2023-04-10T02:37:14.0410407Z + prettier 2.8.1
2023-04-10T02:37:14.0410644Z + semver 7.3.8
2023-04-10T02:37:14.0410861Z + tsup 6.5.0
2023-04-10T02:37:14.0411099Z + typescript 4.9.4
2023-04-10T02:37:14.0411411Z + vite-tsconfig-paths 4.0.5
2023-04-10T02:37:14.0411667Z + vitest 0.26.3
2023-04-10T02:37:14.0411859Z 
2023-04-10T02:37:14.0412024Z . prepare$ husky install
2023-04-10T02:37:14.1033409Z . prepare: husky - Git hooks installed
2023-04-10T02:37:14.1080927Z . prepare: Done
2023-04-10T02:37:14.1101229Z Done in 24.7s
2023-04-10T02:37:14.1771885Z ##[group]Run aws-actions/configure-aws-credentials@v1
2023-04-10T02:37:14.1772189Z with:
2023-04-10T02:37:14.1772867Z   aws-access-key-id: ***
2023-04-10T02:37:14.1773270Z   aws-secret-access-key: ***
2023-04-10T02:37:14.1773538Z   aws-region: ap-southeast-1
2023-04-10T02:37:14.1773790Z   audience: sts.amazonaws.com
2023-04-10T02:37:14.1774014Z env:
2023-04-10T02:37:14.1774282Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:14.1774550Z ##[endgroup]
2023-04-10T02:37:15.6643340Z 
2023-04-10T02:37:15.6660204Z ##[warning]The `set-output` command is deprecated and will be disabled soon. Please upgrade to using Environment Files. For more information see: https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/
2023-04-10T02:37:15.6799227Z ##[group]Run pnpm docs:export
2023-04-10T02:37:15.6799533Z [36;1mpnpm docs:export[0m
2023-04-10T02:37:15.6853258Z shell: /usr/bin/bash -e {0}
2023-04-10T02:37:15.6853512Z env:
2023-04-10T02:37:15.6853810Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:15.6854158Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:15.6854444Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:15.6854906Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:15.6855262Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:15.6855509Z ##[endgroup]
2023-04-10T02:37:16.2003013Z 
2023-04-10T02:37:16.2003991Z > root@0.0.3 docs:export /home/runner/work/useWallet/useWallet
2023-04-10T02:37:16.2004920Z > pnpm -r --filter './docs' export
2023-04-10T02:37:16.2005303Z 
2023-04-10T02:37:16.7666126Z 
2023-04-10T02:37:16.7667503Z > usewallet-docs@0.0.1 export /home/runner/work/useWallet/useWallet/docs
2023-04-10T02:37:16.7668014Z > next build && next export
2023-04-10T02:37:16.7668497Z 
2023-04-10T02:37:17.2196849Z warn  - No build cache found. Please configure build caching for faster rebuilds. Read more: https://nextjs.org/docs/messages/no-cache
2023-04-10T02:37:17.2354306Z Attention: Next.js now collects completely anonymous telemetry regarding usage.
2023-04-10T02:37:17.2355342Z This information is used to shape Next.js' roadmap and prioritize features.
2023-04-10T02:37:17.2356218Z You can learn more, including how to opt-out if you'd not like to participate in this anonymous program, by visiting the following URL:
2023-04-10T02:37:17.2356741Z https://nextjs.org/telemetry
2023-04-10T02:37:17.2356993Z 
2023-04-10T02:37:17.3711105Z info  - Linting and checking validity of types...
2023-04-10T02:37:18.8880089Z warn  - The Next.js plugin was not detected in your ESLint configuration. See https://nextjs.org/docs/basic-features/eslint#migrating-existing-config
2023-04-10T02:37:22.1113748Z info  - Creating an optimized production build...
2023-04-10T02:37:33.8445734Z info  - Compiled successfully
2023-04-10T02:37:33.8446469Z info  - Collecting page data...
2023-04-10T02:37:34.3098549Z info  - Generating static pages (0/9)
2023-04-10T02:37:34.4517496Z info  - Generating static pages (2/9)
2023-04-10T02:37:34.5070133Z info  - Generating static pages (4/9)
2023-04-10T02:37:34.5724099Z info  - Generating static pages (6/9)
2023-04-10T02:37:34.6011809Z info  - Generating static pages (9/9)
2023-04-10T02:37:34.6108031Z info  - Finalizing page optimization...
2023-04-10T02:37:34.6151887Z 
2023-04-10T02:37:34.6250891Z Route (pages)                              Size     First Load JS
2023-04-10T02:37:34.6251935Z ┌ ○ /                                      2.8 kB          166 kB
2023-04-10T02:37:34.6253220Z ├ ○ /404                                   182 B          76.9 kB
2023-04-10T02:37:34.6254687Z ├ ○ /react/getting-started                 2.57 kB         166 kB
2023-04-10T02:37:34.6255338Z ├ ○ /react/hooks/useAccount                2.01 kB         165 kB
2023-04-10T02:37:34.6255956Z ├ ○ /react/hooks/useConnect                2.58 kB         166 kB
2023-04-10T02:37:34.6256540Z ├ ○ /react/hooks/useDisconnect             2.35 kB         165 kB
2023-04-10T02:37:34.6257106Z ├ ○ /react/hooks/useSign                   2.54 kB         166 kB
2023-04-10T02:37:34.6257672Z └ ○ /react/hooks/useSignMessage            2.54 kB         166 kB
2023-04-10T02:37:34.6258183Z + First Load JS shared by all              76.8 kB
2023-04-10T02:37:34.6258703Z   ├ chunks/framework-ea81dd6b0e8bf8e4.js   45.2 kB
2023-04-10T02:37:34.6259213Z   ├ chunks/main-f7b8bbffe96256d0.js        30.5 kB
2023-04-10T02:37:34.6259707Z   ├ chunks/pages/_app-1185fb668a685920.js  195 B
2023-04-10T02:37:34.6260202Z   └ chunks/webpack-38cee4c0e358b1a3.js     862 B
2023-04-10T02:37:34.6260461Z 
2023-04-10T02:37:34.6260923Z ○  (Static)  automatically rendered as static HTML (uses no initial props)
2023-04-10T02:37:34.6261165Z 
2023-04-10T02:37:35.2894933Z info  - using build directory: /home/runner/work/useWallet/useWallet/docs/.next
2023-04-10T02:37:35.2902721Z warn  - rewrites, redirects, and headers are not applied when exporting your application, detected (rewrites). See more info here: https://nextjs.org/docs/messages/export-no-custom-routes
2023-04-10T02:37:35.2970255Z info  - Copying "static build" directory
2023-04-10T02:37:35.3005928Z info  - No "exportPathMap" found in "/home/runner/work/useWallet/useWallet/docs/next.config.js". Generating map from "./pages"
2023-04-10T02:37:35.3016522Z info  - Launching 1 workers
2023-04-10T02:37:35.3040362Z info  - Exporting (0/9)
2023-04-10T02:37:35.4612598Z info  - Exporting (2/9)
2023-04-10T02:37:35.4641731Z info  - Exporting (4/9)
2023-04-10T02:37:35.4686007Z info  - Exporting (6/9)
2023-04-10T02:37:35.4724234Z info  - Exporting (9/9)
2023-04-10T02:37:35.4787650Z Export successful. Files written to /home/runner/work/useWallet/useWallet/docs/out
2023-04-10T02:37:35.5153038Z ##[group]Run eisberg-labs/static-website-to-s3@main
2023-04-10T02:37:35.5153325Z with:
2023-04-10T02:37:35.5153544Z   target: docs/out
2023-04-10T02:37:35.5153774Z   dest: deploy
2023-04-10T02:37:35.5154033Z   exclusions: docs\/out\/(index|404).html$
2023-04-10T02:37:35.5154332Z   bucket: usewallet.casperdash.io
2023-04-10T02:37:35.5154577Z env:
2023-04-10T02:37:35.5154859Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:35.5155195Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:35.5155477Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:35.5155837Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:35.5156185Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:35.5156423Z ##[endgroup]
2023-04-10T02:37:35.5421141Z ##[group]Run unfor19/install-aws-cli-action@v1
2023-04-10T02:37:35.5421430Z with:
2023-04-10T02:37:35.5421634Z   version: 2
2023-04-10T02:37:35.5421855Z   verbose: false
2023-04-10T02:37:35.5422086Z   lightsailctl: false
2023-04-10T02:37:35.5422374Z   arch: amd64
2023-04-10T02:37:35.5422580Z env:
2023-04-10T02:37:35.5422862Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:35.5423187Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:35.5423465Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:35.5423896Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:35.5424246Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:35.5424486Z ##[endgroup]
2023-04-10T02:37:35.5442181Z ##[group]Run echo "AWS_CLI_VERSION=2" >> $GITHUB_ENV
2023-04-10T02:37:35.5442732Z [36;1mecho "AWS_CLI_VERSION=2" >> $GITHUB_ENV[0m
2023-04-10T02:37:35.5443049Z [36;1mecho "AWS_CLI_ARCH=amd64" >> $GITHUB_ENV        [0m
2023-04-10T02:37:35.5443364Z [36;1mecho "VERBOSE=false" >> $GITHUB_ENV[0m
2023-04-10T02:37:35.5443670Z [36;1mecho "LIGHTSAILCTL=false" >> $GITHUB_ENV[0m
2023-04-10T02:37:35.5443967Z [36;1mecho "ROOTDIR=" >> $GITHUB_ENV[0m
2023-04-10T02:37:35.5444241Z [36;1mecho "WORKDIR=" >> $GITHUB_ENV[0m
2023-04-10T02:37:35.5500372Z shell: /usr/bin/bash --noprofile --norc -e -o pipefail {0}
2023-04-10T02:37:35.5500668Z env:
2023-04-10T02:37:35.5500956Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:35.5501287Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:35.5501568Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:35.5501916Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:35.5502270Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:35.5502512Z ##[endgroup]
2023-04-10T02:37:35.5622342Z ##[group]Run sudo --preserve-env /home/runner/work/_actions/unfor19/install-aws-cli-action/v1/entrypoint.sh
2023-04-10T02:37:35.5622890Z [36;1msudo --preserve-env /home/runner/work/_actions/unfor19/install-aws-cli-action/v1/entrypoint.sh[0m
2023-04-10T02:37:35.5674461Z shell: /usr/bin/bash --noprofile --norc -e -o pipefail {0}
2023-04-10T02:37:35.5674748Z env:
2023-04-10T02:37:35.5675018Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:35.5675342Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:35.5675624Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:35.5676000Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:35.5676367Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:35.5676600Z   AWS_CLI_VERSION: 2
2023-04-10T02:37:35.5676836Z   AWS_CLI_ARCH: amd64
2023-04-10T02:37:35.5677069Z   VERBOSE: false
2023-04-10T02:37:35.5677302Z   LIGHTSAILCTL: false
2023-04-10T02:37:35.5677522Z   ROOTDIR: 
2023-04-10T02:37:35.5677727Z   WORKDIR: 
2023-04-10T02:37:35.5677938Z ##[endgroup]
2023-04-10T02:37:35.5864718Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Provided ROOTDIR: 
2023-04-10T02:37:35.5878464Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Provided WORKDIR: 
2023-04-10T02:37:35.5894160Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Final WORKDIR path: /home/runner/work/useWallet/useWallet/unfor19-awscli
2023-04-10T02:37:35.5917876Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Validating semantic version - 2
2023-04-10T02:37:35.5933102Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Valid version input
2023-04-10T02:37:35.6700905Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Provided version exists - https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip
2023-04-10T02:37:35.6716525Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Downloading with wget ...
2023-04-10T02:37:35.9430620Z [LOG] Mon Apr 10 02:37:35 UTC 2023 :: Unzipping unfor19-awscli.zip
2023-04-10T02:37:37.6137250Z [LOG] Mon Apr 10 02:37:37 UTC 2023 :: Installing AWS CLI - 2
2023-04-10T02:37:37.6167642Z [LOG] Mon Apr 10 02:37:37 UTC 2023 :: aws_path = /usr/local/bin/aws
2023-04-10T02:37:38.6245524Z You can now run: /usr/local/bin/aws --version
2023-04-10T02:37:38.6273668Z [LOG] Mon Apr 10 02:37:38 UTC 2023 :: Installation completed
2023-04-10T02:37:38.6299882Z [LOG] Mon Apr 10 02:37:38 UTC 2023 :: Printing AWS CLI installed version
2023-04-10T02:37:39.2400557Z aws-cli/2.11.11 Python/3.11.2 Linux/5.15.0-1035-azure exe/x86_64.ubuntu.22 prompt/off
2023-04-10T02:37:39.3961094Z ##[group]Run echo "version=$(aws --version)" >> $GITHUB_OUTPUT
2023-04-10T02:37:39.3961484Z [36;1mecho "version=$(aws --version)" >> $GITHUB_OUTPUT[0m
2023-04-10T02:37:39.4018376Z shell: /usr/bin/bash --noprofile --norc -e -o pipefail {0}
2023-04-10T02:37:39.4018666Z env:
2023-04-10T02:37:39.4018960Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:39.4019280Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:39.4019549Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:39.4019932Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:39.4020289Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:39.4020535Z   AWS_CLI_VERSION: 2
2023-04-10T02:37:39.4020980Z   AWS_CLI_ARCH: amd64
2023-04-10T02:37:39.4021213Z   VERBOSE: false
2023-04-10T02:37:39.4021450Z   LIGHTSAILCTL: false
2023-04-10T02:37:39.4021680Z   ROOTDIR: 
2023-04-10T02:37:39.4021889Z   WORKDIR: 
2023-04-10T02:37:39.4022104Z ##[endgroup]
2023-04-10T02:37:40.0479786Z ##[group]Run /home/runner/work/_actions/eisberg-labs/static-website-to-s3/main/deploy-doc-to-s3.sh "docs/out" "docs\/out\/(index|404).html$" "usewallet.casperdash.io" "deploy"
2023-04-10T02:37:40.0480507Z [36;1m/home/runner/work/_actions/eisberg-labs/static-website-to-s3/main/deploy-doc-to-s3.sh "docs/out" "docs\/out\/(index|404).html$" "usewallet.casperdash.io" "deploy"[0m
2023-04-10T02:37:40.0534694Z shell: /usr/bin/bash --noprofile --norc -e -o pipefail {0}
2023-04-10T02:37:40.0534991Z env:
2023-04-10T02:37:40.0535284Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:40.0535619Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:40.0535908Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:40.0536290Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:40.0536681Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:40.0536934Z   AWS_CLI_VERSION: 2
2023-04-10T02:37:40.0537175Z   AWS_CLI_ARCH: amd64
2023-04-10T02:37:40.0537411Z   VERBOSE: false
2023-04-10T02:37:40.0537650Z   LIGHTSAILCTL: false
2023-04-10T02:37:40.0537878Z   ROOTDIR: 
2023-04-10T02:37:40.0538091Z   WORKDIR: 
2023-04-10T02:37:40.0538305Z ##[endgroup]
2023-04-10T02:37:40.0662195Z skipping $filename
2023-04-10T02:37:40.0663096Z skipping $filename
2023-04-10T02:37:40.0686929Z mv docs/out/react/hooks/useConnect.html docs/out/react/hooks/useConnect
2023-04-10T02:37:40.0734966Z mv docs/out/react/hooks/useSignMessage.html docs/out/react/hooks/useSignMessage
2023-04-10T02:37:40.0774311Z mv docs/out/react/hooks/useDisconnect.html docs/out/react/hooks/useDisconnect
2023-04-10T02:37:40.0812034Z mv docs/out/react/hooks/useAccount.html docs/out/react/hooks/useAccount
2023-04-10T02:37:40.0848666Z mv docs/out/react/hooks/useSign.html docs/out/react/hooks/useSign
2023-04-10T02:37:40.0885111Z mv docs/out/react/getting-started.html docs/out/react/getting-started
2023-04-10T02:37:42.2068500Z Completed 2.3 KiB/1.7 MiB (4.6 KiB/s) with 38 file(s) remaining
2023-04-10T02:37:42.2070515Z upload: docs/out/404.html to s3://usewallet.casperdash.io/deploy/404.html
2023-04-10T02:37:42.6971218Z Completed 2.3 KiB/1.7 MiB (4.6 KiB/s) with 37 file(s) remaining
2023-04-10T02:37:42.6972385Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/614-52d30210f4e4acdc.js
2023-04-10T02:37:42.9219950Z Completed 2.3 KiB/1.7 MiB (4.6 KiB/s) with 36 file(s) remaining
2023-04-10T02:37:42.9221072Z Completed 27.8 KiB/1.7 MiB (22.9 KiB/s) with 36 file(s) remaining
2023-04-10T02:37:42.9222594Z upload: docs/out/_next/static/chunks/pages/index-b2d8fbed33fa49a8.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/index-b2d8fbed33fa49a8.js
2023-04-10T02:37:42.9258177Z Completed 27.8 KiB/1.7 MiB (22.9 KiB/s) with 35 file(s) remaining
2023-04-10T02:37:42.9270972Z Completed 28.1 KiB/1.7 MiB (23.1 KiB/s) with 35 file(s) remaining
2023-04-10T02:37:42.9271922Z upload: docs/out/_next/static/chunks/pages/_app-1185fb668a685920.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/_app-1185fb668a685920.js
2023-04-10T02:37:42.9347717Z Completed 28.1 KiB/1.7 MiB (23.1 KiB/s) with 34 file(s) remaining
2023-04-10T02:37:42.9348222Z Completed 28.1 KiB/1.7 MiB (23.0 KiB/s) with 34 file(s) remaining
2023-04-10T02:37:42.9348991Z upload: docs/out/_next/static/8XYDkZCebbhb8Zme7qPgH/_ssgManifest.js to s3://usewallet.casperdash.io/deploy/_next/static/8XYDkZCebbhb8Zme7qPgH/_ssgManifest.js
2023-04-10T02:37:42.9396115Z Completed 28.1 KiB/1.7 MiB (23.0 KiB/s) with 33 file(s) remaining
2023-04-10T02:37:42.9397285Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/index-df59db2bce784310.js
2023-04-10T02:37:42.9604815Z Completed 28.1 KiB/1.7 MiB (23.0 KiB/s) with 32 file(s) remaining
2023-04-10T02:37:42.9605288Z Completed 29.3 KiB/1.7 MiB (23.4 KiB/s) with 32 file(s) remaining
2023-04-10T02:37:42.9607427Z upload: docs/out/_next/static/8XYDkZCebbhb8Zme7qPgH/_buildManifest.js to s3://usewallet.casperdash.io/deploy/_next/static/8XYDkZCebbhb8Zme7qPgH/_buildManifest.js
2023-04-10T02:37:42.9610377Z Completed 29.3 KiB/1.7 MiB (23.4 KiB/s) with 31 file(s) remaining
2023-04-10T02:37:42.9614208Z Completed 29.5 KiB/1.7 MiB (23.6 KiB/s) with 31 file(s) remaining
2023-04-10T02:37:42.9635686Z Completed 43.0 KiB/1.7 MiB (34.3 KiB/s) with 31 file(s) remaining
2023-04-10T02:37:42.9636810Z upload: docs/out/_next/static/chunks/pages/_error-dd1d181c16cd5e35.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/_error-dd1d181c16cd5e35.js
2023-04-10T02:37:42.9637398Z Completed 43.0 KiB/1.7 MiB (34.3 KiB/s) with 30 file(s) remaining
2023-04-10T02:37:42.9638199Z upload: docs/out/_next/static/chunks/nextra-data-en-US.json to s3://usewallet.casperdash.io/deploy/_next/static/chunks/nextra-data-en-US.json
2023-04-10T02:37:43.0923822Z Completed 43.0 KiB/1.7 MiB (34.3 KiB/s) with 29 file(s) remaining
2023-04-10T02:37:43.1690729Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 29 file(s) remaining
2023-04-10T02:37:43.1691773Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/getting-started-91ac4feb606efad5.js
2023-04-10T02:37:43.1867890Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 28 file(s) remaining
2023-04-10T02:37:43.1868913Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useAccount-f7dc03701748c6f1.js
2023-04-10T02:37:43.2092557Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 27 file(s) remaining
2023-04-10T02:37:43.2093731Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useConnect-19381b2d5ea724b4.js
2023-04-10T02:37:43.2209742Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 26 file(s) remaining
2023-04-10T02:37:43.2210860Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useDisconnect-54802e394ff5e717.js
2023-04-10T02:37:43.4327732Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 25 file(s) remaining
2023-04-10T02:37:43.4328915Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useSign-5168ed86f2ff43ff.js
2023-04-10T02:37:43.4555107Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 24 file(s) remaining
2023-04-10T02:37:43.4556212Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/webpack-2e3d8389f89f79f1.js
2023-04-10T02:37:43.5979282Z Completed 299.0 KiB/1.7 MiB (216.0 KiB/s) with 23 file(s) remaining
2023-04-10T02:37:43.6040079Z Completed 397.1 KiB/1.7 MiB (210.4 KiB/s) with 23 file(s) remaining
2023-04-10T02:37:43.6041541Z upload: docs/out/_next/static/chunks/main-f7b8bbffe96256d0.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/main-f7b8bbffe96256d0.js
2023-04-10T02:37:43.6271411Z Completed 397.1 KiB/1.7 MiB (210.4 KiB/s) with 22 file(s) remaining
2023-04-10T02:37:43.6283555Z Completed 425.0 KiB/1.7 MiB (221.6 KiB/s) with 22 file(s) remaining
2023-04-10T02:37:43.6285033Z upload: docs/out/_next/static/chunks/pages/react/getting-started-1cbb5f40f96dfe81.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/getting-started-1cbb5f40f96dfe81.js
2023-04-10T02:37:43.6388655Z Completed 425.0 KiB/1.7 MiB (221.6 KiB/s) with 21 file(s) remaining
2023-04-10T02:37:43.6403615Z Completed 439.8 KiB/1.7 MiB (227.8 KiB/s) with 21 file(s) remaining
2023-04-10T02:37:43.6404837Z upload: docs/out/_next/static/chunks/pages/react/hooks/useAccount-7ee5a9f36105301d.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useAccount-7ee5a9f36105301d.js
2023-04-10T02:37:43.6771058Z Completed 439.8 KiB/1.7 MiB (227.8 KiB/s) with 20 file(s) remaining
2023-04-10T02:37:43.6772101Z delete: s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useSignMessage-4919115f6ab15833.js
2023-04-10T02:37:43.7022358Z Completed 439.8 KiB/1.7 MiB (227.8 KiB/s) with 19 file(s) remaining
2023-04-10T02:37:43.7022996Z Completed 466.4 KiB/1.7 MiB (234.0 KiB/s) with 19 file(s) remaining
2023-04-10T02:37:43.7024997Z upload: docs/out/_next/static/chunks/pages/react/hooks/useConnect-955381b0305a7968.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useConnect-955381b0305a7968.js
2023-04-10T02:37:43.7208752Z Completed 466.4 KiB/1.7 MiB (234.0 KiB/s) with 18 file(s) remaining
2023-04-10T02:37:43.7220992Z Completed 604.1 KiB/1.7 MiB (300.2 KiB/s) with 18 file(s) remaining
2023-04-10T02:37:43.7222488Z upload: docs/out/_next/static/chunks/framework-ea81dd6b0e8bf8e4.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/framework-ea81dd6b0e8bf8e4.js
2023-04-10T02:37:43.7604129Z Completed 604.1 KiB/1.7 MiB (300.2 KiB/s) with 17 file(s) remaining
2023-04-10T02:37:43.7604736Z Completed 617.8 KiB/1.7 MiB (301.3 KiB/s) with 17 file(s) remaining
2023-04-10T02:37:43.7605972Z upload: docs/out/_next/static/chunks/496-e81d33ddf55b6b60.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/496-e81d33ddf55b6b60.js
2023-04-10T02:37:43.8647141Z Completed 617.8 KiB/1.7 MiB (301.3 KiB/s) with 16 file(s) remaining
2023-04-10T02:37:43.8647738Z Completed 640.8 KiB/1.7 MiB (297.3 KiB/s) with 16 file(s) remaining
2023-04-10T02:37:43.8649147Z upload: docs/out/_next/static/chunks/pages/react/hooks/useDisconnect-ef69979eb51eb1ef.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useDisconnect-ef69979eb51eb1ef.js
2023-04-10T02:37:43.9226901Z Completed 640.8 KiB/1.7 MiB (297.3 KiB/s) with 15 file(s) remaining
2023-04-10T02:37:43.9227541Z delete: s3://usewallet.casperdash.io/deploy/_next/static/css/93ad2b9badc7a8f8.css
2023-04-10T02:37:43.9447384Z Completed 640.8 KiB/1.7 MiB (297.3 KiB/s) with 14 file(s) remaining
2023-04-10T02:37:43.9448213Z delete: s3://usewallet.casperdash.io/deploy/_next/static/rMGhkEx5TlWEkkwDe1y5b/_buildManifest.js
2023-04-10T02:37:43.9719168Z Completed 640.8 KiB/1.7 MiB (297.3 KiB/s) with 13 file(s) remaining
2023-04-10T02:37:43.9719964Z delete: s3://usewallet.casperdash.io/deploy/_next/static/rMGhkEx5TlWEkkwDe1y5b/_ssgManifest.js
2023-04-10T02:37:43.9903585Z Completed 640.8 KiB/1.7 MiB (297.3 KiB/s) with 12 file(s) remaining
2023-04-10T02:37:43.9909304Z Completed 668.8 KiB/1.7 MiB (293.1 KiB/s) with 12 file(s) remaining
2023-04-10T02:37:43.9910762Z upload: docs/out/_next/static/chunks/pages/react/hooks/useSignMessage-3695531d47b3fdd8.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useSignMessage-3695531d47b3fdd8.js
2023-04-10T02:37:44.0667757Z Completed 668.8 KiB/1.7 MiB (293.1 KiB/s) with 11 file(s) remaining
2023-04-10T02:37:44.0668736Z Completed 670.4 KiB/1.7 MiB (284.5 KiB/s) with 11 file(s) remaining
2023-04-10T02:37:44.0669959Z upload: docs/out/_next/static/chunks/webpack-38cee4c0e358b1a3.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/webpack-38cee4c0e358b1a3.js
2023-04-10T02:37:44.1208562Z Completed 670.4 KiB/1.7 MiB (284.5 KiB/s) with 10 file(s) remaining
2023-04-10T02:37:44.1209152Z Completed 699.2 KiB/1.7 MiB (289.9 KiB/s) with 10 file(s) remaining
2023-04-10T02:37:44.1210426Z upload: docs/out/_next/static/chunks/pages/react/hooks/useSign-5b9ef954b186c743.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/pages/react/hooks/useSign-5b9ef954b186c743.js
2023-04-10T02:37:44.2217786Z Completed 699.2 KiB/1.7 MiB (289.9 KiB/s) with 9 file(s) remaining
2023-04-10T02:37:44.2218357Z Completed 739.8 KiB/1.7 MiB (294.4 KiB/s) with 9 file(s) remaining
2023-04-10T02:37:44.2219149Z upload: docs/out/index.html to s3://usewallet.casperdash.io/deploy/index.html
2023-04-10T02:37:44.3727455Z Completed 739.8 KiB/1.7 MiB (294.4 KiB/s) with 8 file(s) remaining
2023-04-10T02:37:44.3728065Z Completed 799.8 KiB/1.7 MiB (300.2 KiB/s) with 8 file(s) remaining
2023-04-10T02:37:44.3728776Z upload: docs/out/_next/static/css/0dadcc82f3eb59d9.css to s3://usewallet.casperdash.io/deploy/_next/static/css/0dadcc82f3eb59d9.css
2023-04-10T02:37:44.3999727Z Completed 799.8 KiB/1.7 MiB (300.2 KiB/s) with 7 file(s) remaining
2023-04-10T02:37:44.4000401Z Completed 889.1 KiB/1.7 MiB (330.3 KiB/s) with 7 file(s) remaining
2023-04-10T02:37:44.4002272Z upload: docs/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js to s3://usewallet.casperdash.io/deploy/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
2023-04-10T02:37:44.5014328Z Completed 889.1 KiB/1.7 MiB (330.3 KiB/s) with 6 file(s) remaining
2023-04-10T02:37:44.5015005Z Completed 945.9 KiB/1.7 MiB (338.7 KiB/s) with 6 file(s) remaining
2023-04-10T02:37:44.5015779Z upload: docs/out/react/hooks/useDisconnect to s3://usewallet.casperdash.io/deploy/react/hooks/useDisconnect
2023-04-10T02:37:44.5601813Z Completed 945.9 KiB/1.7 MiB (338.7 KiB/s) with 5 file(s) remaining
2023-04-10T02:37:44.5603466Z Completed 1005.8 KiB/1.7 MiB (352.7 KiB/s) with 5 file(s) remaining
2023-04-10T02:37:44.5604296Z upload: docs/out/react/hooks/useSignMessage to s3://usewallet.casperdash.io/deploy/react/hooks/useSignMessage
2023-04-10T02:37:44.5807329Z Completed 1005.8 KiB/1.7 MiB (352.7 KiB/s) with 4 file(s) remaining
2023-04-10T02:37:44.5807822Z Completed 1.0 MiB/1.7 MiB (369.4 KiB/s) with 4 file(s) remaining   
2023-04-10T02:37:44.5808757Z upload: docs/out/react/getting-started to s3://usewallet.casperdash.io/deploy/react/getting-started
2023-04-10T02:37:44.6816288Z Completed 1.0 MiB/1.7 MiB (369.4 KiB/s) with 3 file(s) remaining
2023-04-10T02:37:44.6816903Z Completed 1.1 MiB/1.7 MiB (377.4 KiB/s) with 3 file(s) remaining
2023-04-10T02:37:44.6817545Z upload: docs/out/react/hooks/useConnect to s3://usewallet.casperdash.io/deploy/react/hooks/useConnect
2023-04-10T02:37:44.7045966Z Completed 1.1 MiB/1.7 MiB (377.4 KiB/s) with 2 file(s) remaining
2023-04-10T02:37:44.7046682Z Completed 1.2 MiB/1.7 MiB (394.9 KiB/s) with 2 file(s) remaining
2023-04-10T02:37:44.7047391Z upload: docs/out/react/hooks/useSign to s3://usewallet.casperdash.io/deploy/react/hooks/useSign
2023-04-10T02:37:44.8866381Z Completed 1.2 MiB/1.7 MiB (394.9 KiB/s) with 1 file(s) remaining
2023-04-10T02:37:44.8866956Z Completed 1.2 MiB/1.7 MiB (387.1 KiB/s) with 1 file(s) remaining
2023-04-10T02:37:44.8867601Z upload: docs/out/react/hooks/useAccount to s3://usewallet.casperdash.io/deploy/react/hooks/useAccount
2023-04-10T02:37:45.0066408Z Uploading to  s3://usewallet.casperdash.io/deploy
2023-04-10T02:37:47.5996243Z Completed 47.2 KiB/341.3 KiB (47.3 KiB/s) with 6 file(s) remaining
2023-04-10T02:37:47.5997418Z copy: s3://usewallet.casperdash.io/deploy/react/hooks/useAccount to s3://usewallet.casperdash.io/deploy/react/hooks/useAccount
2023-04-10T02:37:47.6206670Z Completed 47.2 KiB/341.3 KiB (47.3 KiB/s) with 5 file(s) remaining
2023-04-10T02:37:47.6207756Z Completed 102.3 KiB/341.3 KiB (100.5 KiB/s) with 5 file(s) remaining
2023-04-10T02:37:47.6208916Z copy: s3://usewallet.casperdash.io/deploy/react/getting-started to s3://usewallet.casperdash.io/deploy/react/getting-started
2023-04-10T02:37:47.6432761Z Completed 102.3 KiB/341.3 KiB (100.5 KiB/s) with 4 file(s) remaining
2023-04-10T02:37:47.6433310Z Completed 162.2 KiB/341.3 KiB (155.9 KiB/s) with 4 file(s) remaining
2023-04-10T02:37:47.6434073Z copy: s3://usewallet.casperdash.io/deploy/react/hooks/useSignMessage to s3://usewallet.casperdash.io/deploy/react/hooks/useSignMessage
2023-04-10T02:37:47.6678240Z Completed 162.2 KiB/341.3 KiB (155.9 KiB/s) with 3 file(s) remaining
2023-04-10T02:37:47.6679155Z Completed 219.1 KiB/341.3 KiB (205.6 KiB/s) with 3 file(s) remaining
2023-04-10T02:37:47.6680428Z copy: s3://usewallet.casperdash.io/deploy/react/hooks/useDisconnect to s3://usewallet.casperdash.io/deploy/react/hooks/useDisconnect
2023-04-10T02:37:47.6720527Z Completed 219.1 KiB/341.3 KiB (205.6 KiB/s) with 2 file(s) remaining
2023-04-10T02:37:47.6721104Z Completed 280.0 KiB/341.3 KiB (261.8 KiB/s) with 2 file(s) remaining
2023-04-10T02:37:47.6721844Z copy: s3://usewallet.casperdash.io/deploy/react/hooks/useSign to s3://usewallet.casperdash.io/deploy/react/hooks/useSign
2023-04-10T02:37:47.7029227Z Completed 280.0 KiB/341.3 KiB (261.8 KiB/s) with 1 file(s) remaining
2023-04-10T02:37:47.7032552Z Completed 341.3 KiB/341.3 KiB (310.1 KiB/s) with 1 file(s) remaining
2023-04-10T02:37:47.7033530Z copy: s3://usewallet.casperdash.io/deploy/react/hooks/useConnect to s3://usewallet.casperdash.io/deploy/react/hooks/useConnect
2023-04-10T02:37:47.8233929Z ##[group]Run aws cloudfront create-invalidation --distribution-id *** --paths "/*" --no-cli-pager
2023-04-10T02:37:47.8234490Z [36;1maws cloudfront create-invalidation --distribution-id *** --paths "/*" --no-cli-pager[0m
2023-04-10T02:37:47.8288823Z shell: /usr/bin/bash -e {0}
2023-04-10T02:37:47.8289076Z env:
2023-04-10T02:37:47.8289375Z   PNPM_HOME: /home/runner/setup-pnpm/node_modules/.bin
2023-04-10T02:37:47.8289714Z   AWS_DEFAULT_REGION: ap-southeast-1
2023-04-10T02:37:47.8290004Z   AWS_REGION: ap-southeast-1
2023-04-10T02:37:47.8290354Z   AWS_ACCESS_KEY_ID: ***
2023-04-10T02:37:47.8290706Z   AWS_SECRET_ACCESS_KEY: ***
2023-04-10T02:37:47.8290954Z   AWS_CLI_VERSION: 2
2023-04-10T02:37:47.8291194Z   AWS_CLI_ARCH: amd64
2023-04-10T02:37:47.8291427Z   VERBOSE: false
2023-04-10T02:37:47.8291652Z   LIGHTSAILCTL: false
2023-04-10T02:37:47.8291886Z   ROOTDIR: 
2023-04-10T02:37:47.8292159Z   WORKDIR: 
2023-04-10T02:37:47.8292373Z ##[endgroup]
2023-04-10T02:37:48.6506288Z {
2023-04-10T02:37:48.6507883Z     "Location": "https://cloudfront.amazonaws.com/2020-05-31/distribution/***/invalidation/I7A2XAXPAZV03L0U1USBH0VQ10",
2023-04-10T02:37:48.6508377Z     "Invalidation": {
2023-04-10T02:37:48.6508752Z         "Id": "I7A2XAXPAZV03L0U1USBH0VQ10",
2023-04-10T02:37:48.6509111Z         "Status": "InProgress",
2023-04-10T02:37:48.6509588Z         "CreateTime": "2023-04-10T02:37:48.597000+00:00",
2023-04-10T02:37:48.6509947Z         "InvalidationBatch": {
2023-04-10T02:37:48.6510244Z             "Paths": {
2023-04-10T02:37:48.6510552Z                 "Quantity": 1,
2023-04-10T02:37:48.6510809Z                 "Items": [
2023-04-10T02:37:48.6511068Z                     "/*"
2023-04-10T02:37:48.6511325Z                 ]
2023-04-10T02:37:48.6511566Z             },
2023-04-10T02:37:48.6511991Z             "CallerReference": "cli-1681094268-788900"
2023-04-10T02:37:48.6512285Z         }
2023-04-10T02:37:48.6512535Z     }
2023-04-10T02:37:48.6512764Z }
2023-04-10T02:37:48.7635467Z Post job cleanup.
2023-04-10T02:37:48.8176165Z Post job cleanup.
2023-04-10T02:37:48.9815183Z [command]/home/runner/setup-pnpm/node_modules/.bin/pnpm store path --silent
2023-04-10T02:37:49.4863179Z /home/runner/setup-pnpm/node_modules/.bin/store/v3
2023-04-10T02:37:49.5119118Z [command]/usr/bin/tar --posix -z -cf cache.tgz --exclude cache.tgz -P -C /home/runner/work/useWallet/useWallet --files-from manifest.txt
2023-04-10T02:38:18.1181058Z Failed to save: Unable to reserve cache with key node-cache-Linux-pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8, another job may be creating this cache. More details: Cache already exists. Scope: refs/heads/main, Key: node-cache-Linux-pnpm-e8a7a1e163cefe28462115280424f67a6415596718e293bb30846ac21c4d13c8, Version: 5e34942b09d60f26936dbe01f6e5a1104cb7cc62c7c0c778bb12993b02ca0328
2023-04-10T02:38:18.1562162Z Post job cleanup.
2023-04-10T02:38:18.2722442Z Pruning is unnecessary.
2023-04-10T02:38:18.2810307Z Post job cleanup.
2023-04-10T02:38:18.4236089Z [command]/usr/bin/git version
2023-04-10T02:38:18.4286353Z git version 2.40.0
2023-04-10T02:38:18.4331202Z Copying '/home/runner/.gitconfig' to '/home/runner/work/_temp/3c492034-9b9f-4a3a-bd8d-583749cc8c44/.gitconfig'
2023-04-10T02:38:18.4342562Z Temporarily overriding HOME='/home/runner/work/_temp/3c492034-9b9f-4a3a-bd8d-583749cc8c44' before making global git config changes
2023-04-10T02:38:18.4343473Z Adding repository directory to the temporary git global config as a safe directory
2023-04-10T02:38:18.4348668Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/useWallet/useWallet
2023-04-10T02:38:18.4391651Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2023-04-10T02:38:18.4428189Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2023-04-10T02:38:18.4657502Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2023-04-10T02:38:18.4685155Z http.https://github.com/.extraheader
2023-04-10T02:38:18.4697264Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2023-04-10T02:38:18.4735040Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2023-04-10T02:38:18.5213303Z Cleaning up orphan processes
```