# GitHub Workflow

## Set up job `(1s)`

```sh
Current runner version: '2.311.0'
Operating System
  Ubuntu
  22.04.3
  LTS
Runner Image
  Image: ubuntu-22.04
  Version: 20231025.1.0
  Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20231025.1/images/linux/Ubuntu2204-Readme.md
  Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20231025.1
Runner Image Provisioner
  2.0.312.1
GITHUB_TOKEN Permissions
  Actions: write
  Checks: write
  Contents: write
  Deployments: write
  Discussions: write
  Issues: write
  Metadata: read
  Packages: write
  Pages: write
  PullRequests: write
  RepositoryProjects: write
  SecurityEvents: write
  Statuses: write
Secret source: Actions
Prepare workflow directory
Prepare all required actions
Getting action download info
Download action repository 'actions/checkout@v2' (SHA:ee0669bd1cc54295c223e0bb666b733df41de1c5)
Download action repository 'actions-rs/toolchain@v1' (SHA:16499b5e05bf2e26879000db0c1d13f7e13fa3af)
Complete job name: build
```

## Run actions/checkout@v2 `(1s)`

```sh
Run actions/checkout@v2
  with:
    repository: ggurbet/casper_staking
    token: ***
    ssh-strict: true
    persist-credentials: true
    clean: true
    fetch-depth: 1
    lfs: false
    submodules: false
    set-safe-directory: true
  env:
    CARGO_TERM_COLOR: always
Syncing repository: ggurbet/casper_staking
Getting Git version info
  Working directory is '/home/runner/work/casper_staking/casper_staking'
  /usr/bin/git version
  git version 2.42.0
Temporarily overriding HOME='/home/runner/work/_temp/8db5b38d-fe5a-43e9-90cd-8bf2b7cb3fdb' before making global git config changes
Adding repository directory to the temporary git global config as a safe directory
/usr/bin/git config --global --add safe.directory /home/runner/work/casper_staking/casper_staking
Deleting the contents of '/home/runner/work/casper_staking/casper_staking'
Initializing the repository
  /usr/bin/git init /home/runner/work/casper_staking/casper_staking
  hint: Using 'master' as the name for the initial branch. This default branch name
  hint: is subject to change. To configure the initial branch name to use in all
  hint: of your new repositories, which will suppress this warning, call:
  hint: 
  hint: 	git config --global init.defaultBranch <name>
  hint: 
  hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
  hint: 'development'. The just-created branch can be renamed via this command:
  hint: 
  hint: 	git branch -m <name>
  Initialized empty Git repository in /home/runner/work/casper_staking/casper_staking/.git/
  /usr/bin/git remote add origin https://github.com/ggurbet/casper_staking
Disabling automatic garbage collection
  /usr/bin/git config --local gc.auto 0
Setting up auth
  /usr/bin/git config --local --name-only --get-regexp core\.sshCommand
  /usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
  /usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
  /usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
  /usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
Fetching the repository
  /usr/bin/git -c protocol.version=2 fetch --no-tags --prune --progress --no-recurse-submodules --depth=1 origin +626ef8a9a48ca9245574812c6fcf05f203f73c62:refs/remotes/origin/main
  remote: Enumerating objects: 110, done.        
  remote: Counting objects:   0% (1/110)        
  remote: Counting objects:   1% (2/110)        
  remote: Counting objects:   2% (3/110)        
  remote: Counting objects:   3% (4/110)        
  remote: Counting objects:   4% (5/110)        
  remote: Counting objects:   5% (6/110)        
  remote: Counting objects:   6% (7/110)        
  remote: Counting objects:   7% (8/110)        
  remote: Counting objects:   8% (9/110)        
  remote: Counting objects:   9% (10/110)        
  remote: Counting objects:  10% (11/110)        
  remote: Counting objects:  11% (13/110)        
  remote: Counting objects:  12% (14/110)        
  remote: Counting objects:  13% (15/110)        
  remote: Counting objects:  14% (16/110)        
  remote: Counting objects:  15% (17/110)        
  remote: Counting objects:  16% (18/110)        
  remote: Counting objects:  17% (19/110)        
  remote: Counting objects:  18% (20/110)        
  remote: Counting objects:  19% (21/110)        
  remote: Counting objects:  20% (22/110)        
  remote: Counting objects:  21% (24/110)        
  remote: Counting objects:  22% (25/110)        
  remote: Counting objects:  23% (26/110)        
  remote: Counting objects:  24% (27/110)        
  remote: Counting objects:  25% (28/110)        
  remote: Counting objects:  26% (29/110)        
  remote: Counting objects:  27% (30/110)        
  remote: Counting objects:  28% (31/110)        
  remote: Counting objects:  29% (32/110)        
  remote: Counting objects:  30% (33/110)        
  remote: Counting objects:  31% (35/110)        
  remote: Counting objects:  32% (36/110)        
  remote: Counting objects:  33% (37/110)        
  remote: Counting objects:  34% (38/110)        
  remote: Counting objects:  35% (39/110)        
  remote: Counting objects:  36% (40/110)        
  remote: Counting objects:  37% (41/110)        
  remote: Counting objects:  38% (42/110)        
  remote: Counting objects:  39% (43/110)        
  remote: Counting objects:  40% (44/110)        
  remote: Counting objects:  41% (46/110)        
  remote: Counting objects:  42% (47/110)        
  remote: Counting objects:  43% (48/110)        
  remote: Counting objects:  44% (49/110)        
  remote: Counting objects:  45% (50/110)        
  remote: Counting objects:  46% (51/110)        
  remote: Counting objects:  47% (52/110)        
  remote: Counting objects:  48% (53/110)        
  remote: Counting objects:  49% (54/110)        
  remote: Counting objects:  50% (55/110)        
  remote: Counting objects:  51% (57/110)        
  remote: Counting objects:  52% (58/110)        
  remote: Counting objects:  53% (59/110)        
  remote: Counting objects:  54% (60/110)        
  remote: Counting objects:  55% (61/110)        
  remote: Counting objects:  56% (62/110)        
  remote: Counting objects:  57% (63/110)        
  remote: Counting objects:  58% (64/110)        
  remote: Counting objects:  59% (65/110)        
  remote: Counting objects:  60% (66/110)        
  remote: Counting objects:  61% (68/110)        
  remote: Counting objects:  62% (69/110)        
  remote: Counting objects:  63% (70/110)        
  remote: Counting objects:  64% (71/110)        
  remote: Counting objects:  65% (72/110)        
  remote: Counting objects:  66% (73/110)        
  remote: Counting objects:  67% (74/110)        
  remote: Counting objects:  68% (75/110)        
  remote: Counting objects:  69% (76/110)        
  remote: Counting objects:  70% (77/110)        
  remote: Counting objects:  71% (79/110)        
  remote: Counting objects:  72% (80/110)        
  remote: Counting objects:  73% (81/110)        
  remote: Counting objects:  74% (82/110)        
  remote: Counting objects:  75% (83/110)        
  remote: Counting objects:  76% (84/110)        
  remote: Counting objects:  77% (85/110)        
  remote: Counting objects:  78% (86/110)        
  remote: Counting objects:  79% (87/110)        
  remote: Counting objects:  80% (88/110)        
  remote: Counting objects:  81% (90/110)        
  remote: Counting objects:  82% (91/110)        
  remote: Counting objects:  83% (92/110)        
  remote: Counting objects:  84% (93/110)        
  remote: Counting objects:  85% (94/110)        
  remote: Counting objects:  86% (95/110)        
  remote: Counting objects:  87% (96/110)        
  remote: Counting objects:  88% (97/110)        
  remote: Counting objects:  89% (98/110)        
  remote: Counting objects:  90% (99/110)        
  remote: Counting objects:  91% (101/110)        
  remote: Counting objects:  92% (102/110)        
  remote: Counting objects:  93% (103/110)        
  remote: Counting objects:  94% (104/110)        
  remote: Counting objects:  95% (105/110)        
  remote: Counting objects:  96% (106/110)        
  remote: Counting objects:  97% (107/110)        
  remote: Counting objects:  98% (108/110)        
  remote: Counting objects:  99% (109/110)        
  remote: Counting objects: 100% (110/110)        
  remote: Counting objects: 100% (110/110), done.        
  remote: Compressing objects:   1% (1/94)        
  remote: Compressing objects:   2% (2/94)        
  remote: Compressing objects:   3% (3/94)        
  remote: Compressing objects:   4% (4/94)        
  remote: Compressing objects:   5% (5/94)        
  remote: Compressing objects:   6% (6/94)        
  remote: Compressing objects:   7% (7/94)        
  remote: Compressing objects:   8% (8/94)        
  remote: Compressing objects:   9% (9/94)        
  remote: Compressing objects:  10% (10/94)        
  remote: Compressing objects:  11% (11/94)        
  remote: Compressing objects:  12% (12/94)        
  remote: Compressing objects:  13% (13/94)        
  remote: Compressing objects:  14% (14/94)        
  remote: Compressing objects:  15% (15/94)        
  remote: Compressing objects:  17% (16/94)        
  remote: Compressing objects:  18% (17/94)        
  remote: Compressing objects:  19% (18/94)        
  remote: Compressing objects:  20% (19/94)        
  remote: Compressing objects:  21% (20/94)        
  remote: Compressing objects:  22% (21/94)        
  remote: Compressing objects:  23% (22/94)        
  remote: Compressing objects:  24% (23/94)        
  remote: Compressing objects:  25% (24/94)        
  remote: Compressing objects:  26% (25/94)        
  remote: Compressing objects:  27% (26/94)        
  remote: Compressing objects:  28% (27/94)        
  remote: Compressing objects:  29% (28/94)        
  remote: Compressing objects:  30% (29/94)        
  remote: Compressing objects:  31% (30/94)        
  remote: Compressing objects:  32% (31/94)        
  remote: Compressing objects:  34% (32/94)        
  remote: Compressing objects:  35% (33/94)        
  remote: Compressing objects:  36% (34/94)        
  remote: Compressing objects:  37% (35/94)        
  remote: Compressing objects:  38% (36/94)        
  remote: Compressing objects:  39% (37/94)        
  remote: Compressing objects:  40% (38/94)        
  remote: Compressing objects:  41% (39/94)        
  remote: Compressing objects:  42% (40/94)        
  remote: Compressing objects:  43% (41/94)        
  remote: Compressing objects:  44% (42/94)        
  remote: Compressing objects:  45% (43/94)        
  remote: Compressing objects:  46% (44/94)        
  remote: Compressing objects:  47% (45/94)        
  remote: Compressing objects:  48% (46/94)        
  remote: Compressing objects:  50% (47/94)        
  remote: Compressing objects:  51% (48/94)        
  remote: Compressing objects:  52% (49/94)        
  remote: Compressing objects:  53% (50/94)        
  remote: Compressing objects:  54% (51/94)        
  remote: Compressing objects:  55% (52/94)        
  remote: Compressing objects:  56% (53/94)        
  remote: Compressing objects:  57% (54/94)        
  remote: Compressing objects:  58% (55/94)        
  remote: Compressing objects:  59% (56/94)        
  remote: Compressing objects:  60% (57/94)        
  remote: Compressing objects:  61% (58/94)        
  remote: Compressing objects:  62% (59/94)        
  remote: Compressing objects:  63% (60/94)        
  remote: Compressing objects:  64% (61/94)        
  remote: Compressing objects:  65% (62/94)        
  remote: Compressing objects:  67% (63/94)        
  remote: Compressing objects:  68% (64/94)        
  remote: Compressing objects:  69% (65/94)        
  remote: Compressing objects:  70% (66/94)        
  remote: Compressing objects:  71% (67/94)        
  remote: Compressing objects:  72% (68/94)        
  remote: Compressing objects:  73% (69/94)        
  remote: Compressing objects:  74% (70/94)        
  remote: Compressing objects:  75% (71/94)        
  remote: Compressing objects:  76% (72/94)        
  remote: Compressing objects:  77% (73/94)        
  remote: Compressing objects:  78% (74/94)        
  remote: Compressing objects:  79% (75/94)        
  remote: Compressing objects:  80% (76/94)        
  remote: Compressing objects:  81% (77/94)        
  remote: Compressing objects:  82% (78/94)        
  remote: Compressing objects:  84% (79/94)        
  remote: Compressing objects:  85% (80/94)        
  remote: Compressing objects:  86% (81/94)        
  remote: Compressing objects:  87% (82/94)        
  remote: Compressing objects:  88% (83/94)        
  remote: Compressing objects:  89% (84/94)        
  remote: Compressing objects:  90% (85/94)        
  remote: Compressing objects:  91% (86/94)        
  remote: Compressing objects:  92% (87/94)        
  remote: Compressing objects:  93% (88/94)        
  remote: Compressing objects:  94% (89/94)        
  remote: Compressing objects:  95% (90/94)        
  remote: Compressing objects:  96% (91/94)        
  remote: Compressing objects:  97% (92/94)        
  remote: Compressing objects:  98% (93/94)        
  remote: Compressing objects: 100% (94/94)        
  remote: Compressing objects: 100% (94/94), done.        
  Receiving objects:   0% (1/110)
  Receiving objects:   1% (2/110)
  Receiving objects:   2% (3/110)
  Receiving objects:   3% (4/110)
  Receiving objects:   4% (5/110)
  Receiving objects:   5% (6/110)
  Receiving objects:   6% (7/110)
  Receiving objects:   7% (8/110)
  Receiving objects:   8% (9/110)
  Receiving objects:   9% (10/110)
  Receiving objects:  10% (11/110)
  Receiving objects:  11% (13/110)
  Receiving objects:  12% (14/110)
  Receiving objects:  13% (15/110)
  Receiving objects:  14% (16/110)
  Receiving objects:  15% (17/110)
  Receiving objects:  16% (18/110)
  Receiving objects:  17% (19/110)
  Receiving objects:  18% (20/110)
  Receiving objects:  19% (21/110)
  Receiving objects:  20% (22/110)
  Receiving objects:  21% (24/110)
  Receiving objects:  22% (25/110)
  Receiving objects:  23% (26/110)
  Receiving objects:  24% (27/110)
  Receiving objects:  25% (28/110)
  Receiving objects:  26% (29/110)
  Receiving objects:  27% (30/110)
  Receiving objects:  28% (31/110)
  Receiving objects:  29% (32/110)
  Receiving objects:  30% (33/110)
  Receiving objects:  31% (35/110)
  Receiving objects:  32% (36/110)
  Receiving objects:  33% (37/110)
  Receiving objects:  34% (38/110)
  Receiving objects:  35% (39/110)
  Receiving objects:  36% (40/110)
  Receiving objects:  37% (41/110)
  Receiving objects:  38% (42/110)
  Receiving objects:  39% (43/110)
  Receiving objects:  40% (44/110)
  Receiving objects:  41% (46/110)
  Receiving objects:  42% (47/110)
  Receiving objects:  43% (48/110)
  Receiving objects:  44% (49/110)
  Receiving objects:  45% (50/110)
  Receiving objects:  46% (51/110)
  Receiving objects:  47% (52/110)
  Receiving objects:  48% (53/110)
  Receiving objects:  49% (54/110)
  Receiving objects:  50% (55/110)
  Receiving objects:  51% (57/110)
  Receiving objects:  52% (58/110)
  Receiving objects:  53% (59/110)
  Receiving objects:  54% (60/110)
  Receiving objects:  55% (61/110)
  Receiving objects:  56% (62/110)
  Receiving objects:  57% (63/110)
  Receiving objects:  58% (64/110)
  Receiving objects:  59% (65/110)
  Receiving objects:  60% (66/110)
  Receiving objects:  61% (68/110)
  Receiving objects:  62% (69/110)
  Receiving objects:  63% (70/110)
  Receiving objects:  64% (71/110)
  Receiving objects:  65% (72/110)
  Receiving objects:  66% (73/110)
  Receiving objects:  67% (74/110)
  Receiving objects:  68% (75/110)
  Receiving objects:  69% (76/110)
  Receiving objects:  70% (77/110)
  Receiving objects:  71% (79/110)
  Receiving objects:  72% (80/110)
  Receiving objects:  73% (81/110)
  Receiving objects:  74% (82/110)
  Receiving objects:  75% (83/110)
  Receiving objects:  76% (84/110)
  Receiving objects:  77% (85/110)
  remote: Total 110 (delta 15), reused 64 (delta 7), pack-reused 0        
  Receiving objects:  78% (86/110)
  Receiving objects:  79% (87/110)
  Receiving objects:  80% (88/110)
  Receiving objects:  81% (90/110)
  Receiving objects:  82% (91/110)
  Receiving objects:  83% (92/110)
  Receiving objects:  84% (93/110)
  Receiving objects:  85% (94/110)
  Receiving objects:  86% (95/110)
  Receiving objects:  87% (96/110)
  Receiving objects:  88% (97/110)
  Receiving objects:  89% (98/110)
  Receiving objects:  90% (99/110)
  Receiving objects:  91% (101/110)
  Receiving objects:  92% (102/110)
  Receiving objects:  93% (103/110)
  Receiving objects:  94% (104/110)
  Receiving objects:  95% (105/110)
  Receiving objects:  96% (106/110)
  Receiving objects:  97% (107/110)
  Receiving objects:  98% (108/110)
  Receiving objects:  99% (109/110)
  Receiving objects: 100% (110/110)
  Receiving objects: 100% (110/110), 212.54 KiB | 11.19 MiB/s, done.
  Resolving deltas:   0% (0/15)
  Resolving deltas:   6% (1/15)
  Resolving deltas:  13% (2/15)
  Resolving deltas:  20% (3/15)
  Resolving deltas:  26% (4/15)
  Resolving deltas:  33% (5/15)
  Resolving deltas:  40% (6/15)
  Resolving deltas:  46% (7/15)
  Resolving deltas:  53% (8/15)
  Resolving deltas:  60% (9/15)
  Resolving deltas:  66% (10/15)
  Resolving deltas:  73% (11/15)
  Resolving deltas:  80% (12/15)
  Resolving deltas:  86% (13/15)
  Resolving deltas:  93% (14/15)
  Resolving deltas: 100% (15/15)
  Resolving deltas: 100% (15/15), done.
  From https://github.com/ggurbet/casper_staking
   * [new ref]         626ef8a9a48ca9245574812c6fcf05f203f73c62 -> origin/main
Determining the checkout info
Checking out the ref
  /usr/bin/git checkout --progress --force -B main refs/remotes/origin/main
  Switched to a new branch 'main'
  branch 'main' set up to track 'origin/main'.
/usr/bin/git log -1 --format='%H'
'626ef8a9a48ca9245574812c6fcf05f203f73c62'
```

## Run actions-rs/toolchain@v1 `(37s)`

```sh
Run actions-rs/toolchain@v1
  with:
    toolchain: nightly-2023-01-16
    override: true
    default: false
  env:
    CARGO_TERM_COLOR: always
/home/runner/.cargo/bin/rustup show
Default host: x86_64-unknown-linux-gnu
rustup home:  /home/runner/.rustup

info: syncing channel updates for 'nightly-2022-01-03-x86_64-unknown-linux-gnu'
info: latest update on 2022-01-03, rust version 1.59.0-nightly (8f3238f89 2022-01-02)
info: downloading component 'cargo'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: installing component 'cargo'
info: installing component 'rust-std'
info: installing component 'rustc'
nightly-2022-01-03-x86_64-unknown-linux-gnu (overridden by '/home/runner/work/casper_staking/casper_staking/rust-toolchain')
rustc 1.59.0-nightly (8f3238f89 2022-01-02)
/home/runner/.cargo/bin/rustup toolchain install nightly-2023-01-16
info: syncing channel updates for 'nightly-2023-01-16-x86_64-unknown-linux-gnu'
info: latest update on 2023-01-16, rust version 1.68.0-nightly (9e75dddf6 2023-01-15)
info: downloading component 'cargo'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: installing component 'cargo'
info: installing component 'rust-std'
info: installing component 'rustc'

  nightly-2023-01-16-x86_64-unknown-linux-gnu installed - rustc 1.68.0-nightly (9e75dddf6 2023-01-15)

info: checking for self-update
warning: tool `rust-analyzer` is already installed, remove it from `/home/runner/.cargo/bin`, then run `rustup update` to have rustup manage this tool.
warning: tool `rustfmt` is already installed, remove it from `/home/runner/.cargo/bin`, then run `rustup update` to have rustup manage this tool.
warning: tool `cargo-fmt` is already installed, remove it from `/home/runner/.cargo/bin`, then run `rustup update` to have rustup manage this tool.
/home/runner/.cargo/bin/rustup override set nightly-2023-01-16
info: using existing install for 'nightly-2023-01-16-x86_64-unknown-linux-gnu'
info: override toolchain for '/home/runner/work/casper_staking/casper_staking' set to 'nightly-2023-01-16-x86_64-unknown-linux-gnu'

  nightly-2023-01-16-x86_64-unknown-linux-gnu unchanged - rustc 1.68.0-nightly (9e75dddf6 2023-01-15)

Gathering installed versions
  /home/runner/.cargo/bin/rustc -V
  rustc 1.68.0-nightly (9e75dddf6 2023-01-15)
  Warning: The `set-output` command is deprecated and will be disabled soon. Please upgrade to using Environment Files. For more information see: https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/
  Warning: The `set-output` command is deprecated and will be disabled soon. Please upgrade to using Environment Files. For more information see: https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/
  /home/runner/.cargo/bin/cargo -V
  cargo 1.68.0-nightly (1cd6d3803 2023-01-12)
  Warning: The `set-output` command is deprecated and will be disabled soon. Please upgrade to using Environment Files. For more information see: https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/
  /home/runner/.cargo/bin/rustup -V
  rustup 1.26.0 (5af9b9484 2023-04-05)
  info: This is the version for the rustup toolchain manager, not the rustc compiler.
  info: The currently active `rustc` version is `rustc 1.68.0-nightly (9e75dddf6 2023-01-15)`
  Warning: The `set-output` command is deprecated and will be disabled soon. Please upgrade to using Environment Files. For more information see: https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/
```

## Install dependencies `(18s)`

```sh
Run sudo apt update && sudo apt install -y build-essential wabt
  sudo apt update && sudo apt install -y build-essential wabt
  shell: /usr/bin/bash -e {0}
  env:
    CARGO_TERM_COLOR: always

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Get:1 file:/etc/apt/apt-mirrors.txt Mirrorlist [142 B]
Get:6 https://packages.microsoft.com/ubuntu/22.04/prod jammy InRelease [3611 B]
Hit:2 http://azure.archive.ubuntu.com/ubuntu jammy InRelease
Get:3 http://azure.archive.ubuntu.com/ubuntu jammy-updates InRelease [119 kB]
Get:4 http://azure.archive.ubuntu.com/ubuntu jammy-backports InRelease [109 kB]
Get:5 http://azure.archive.ubuntu.com/ubuntu jammy-security InRelease [110 kB]
Get:7 https://packages.microsoft.com/ubuntu/22.04/prod jammy/main amd64 Packages [110 kB]
Hit:8 https://ppa.launchpadcontent.net/ubuntu-toolchain-r/test/ubuntu jammy InRelease
Get:9 http://azure.archive.ubuntu.com/ubuntu jammy-updates/main amd64 Packages [1104 kB]
Get:10 http://azure.archive.ubuntu.com/ubuntu jammy-updates/main Translation-en [240 kB]
Get:11 http://azure.archive.ubuntu.com/ubuntu jammy-updates/main amd64 c-n-f Metadata [16.1 kB]
Get:12 http://azure.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 Packages [995 kB]
Get:13 http://azure.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 c-n-f Metadata [22.0 kB]
Get:14 http://azure.archive.ubuntu.com/ubuntu jammy-security/main amd64 Packages [896 kB]
Get:15 http://azure.archive.ubuntu.com/ubuntu jammy-security/main amd64 c-n-f Metadata [11.4 kB]
Get:16 http://azure.archive.ubuntu.com/ubuntu jammy-security/universe amd64 Packages [793 kB]
Get:17 http://azure.archive.ubuntu.com/ubuntu jammy-security/universe amd64 c-n-f Metadata [16.7 kB]
Fetched 4546 kB in 1s (3443 kB/s)
Reading package lists...
Building dependency tree...
Reading state information...
30 packages can be upgraded. Run 'apt list --upgradable' to see them.

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Reading package lists...
Building dependency tree...
Reading state information...
build-essential is already the newest version (12.9ubuntu3).
build-essential set to manually installed.
The following NEW packages will be installed:
  wabt
0 upgraded, 1 newly installed, 0 to remove and 30 not upgraded.
Need to get 1331 kB of archives.
After this operation, 12.0 MB of additional disk space will be used.
Get:1 file:/etc/apt/apt-mirrors.txt Mirrorlist [142 B]
Get:2 http://azure.archive.ubuntu.com/ubuntu jammy/universe amd64 wabt amd64 1.0.27-1 [1331 kB]
Fetched 1331 kB in 0s (7816 kB/s)
Selecting previously unselected package wabt.
(Reading database ... 
(Reading database ... 5%
(Reading database ... 10%
(Reading database ... 15%
(Reading database ... 20%
(Reading database ... 25%
(Reading database ... 30%
(Reading database ... 35%
(Reading database ... 40%
(Reading database ... 45%
(Reading database ... 50%
(Reading database ... 55%
(Reading database ... 60%
(Reading database ... 65%
(Reading database ... 70%
(Reading database ... 75%
(Reading database ... 80%
(Reading database ... 85%
(Reading database ... 90%
(Reading database ... 95%
(Reading database ... 100%
(Reading database ... 270283 files and directories currently installed.)
Preparing to unpack .../wabt_1.0.27-1_amd64.deb ...
Unpacking wabt (1.0.27-1) ...
Setting up wabt (1.0.27-1) ...
Processing triggers for man-db (2.10.2-1) ...
NEEDRESTART-VER: 3.5
NEEDRESTART-KCUR: 6.2.0-1015-azure
NEEDRESTART-KEXP: 6.2.0-1015-azure
NEEDRESTART-KSTA: 1
```

## Setup `(3s)`

```sh
Run cd staking_contract ; make prepare
  cd staking_contract ; make prepare
  shell: /usr/bin/bash -e {0}
  env:
    CARGO_TERM_COLOR: always
rustup target add wasm32-unknown-unknown
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
```

## Run clippy and fmt `(5m 32s)`

```sh
Run cd staking_contract ; rustup component add clippy --toolchain nightly-2023-01-16-x86_64-unknown-linux-gnu; rustup component add rustfmt --toolchain nightly-2023-01-16-x86_64-unknown-linux-gnu ; make check-lint
  cd staking_contract ; rustup component add clippy --toolchain nightly-2023-01-16-x86_64-unknown-linux-gnu; rustup component add rustfmt --toolchain nightly-2023-01-16-x86_64-unknown-linux-gnu ; make check-lint
  shell: /usr/bin/bash -e {0}
  env:
    CARGO_TERM_COLOR: always
info: downloading component 'clippy'
info: installing component 'clippy'
info: downloading component 'rustfmt'
info: installing component 'rustfmt'
cd staking_contract && cargo clippy --all-targets --all -- -D warnings
    Updating crates.io index
 Downloading crates ...
  Downloaded wasm-bindgen-backend v0.2.84
  Downloaded wasm-bindgen-macro-support v0.2.84
  Downloaded opaque-debug v0.3.0
  Downloaded syn v2.0.15
  Downloaded ed25519-dalek v1.0.1
  Downloaded wasm-bindgen v0.2.84
  Downloaded rand v0.8.5
  Downloaded cfg-if v1.0.0
  Downloaded rand v0.7.3
  Downloaded num-rational v0.4.1
  Downloaded num v0.4.0
  Downloaded subtle v2.4.1
  Downloaded hmac v0.10.1
  Downloaded js-sys v0.3.61
  Downloaded num-integer v0.1.45
  Downloaded bitflags v1.3.2
  Downloaded byteorder v1.4.3
  Downloaded hex_fmt v0.3.0
  Downloaded rand_chacha v0.2.2
  Downloaded crypto-mac v0.8.0
  Downloaded wasm-bindgen-shared v0.2.84
  Downloaded group v0.8.0
  Downloaded digest v0.9.0
  Downloaded radium v0.3.0
  Downloaded ed25519 v1.2.0
  Downloaded block-buffer v0.9.0
  Downloaded ppv-lite86 v0.2.17
  Downloaded cpufeatures v0.2.7
  Downloaded serde_bytes v0.11.9
  Downloaded version_check v0.9.4
  Downloaded signature v1.2.2
  Downloaded rand_core v0.6.4
  Downloaded wee_alloc v0.4.5
  Downloaded num-iter v0.1.43
  Downloaded ecdsa v0.10.2
  Downloaded itoa v1.0.6
  Downloaded sha2 v0.9.9
  Downloaded memory_units v0.4.0
  Downloaded static_assertions v1.1.0
  Downloaded generic-array v0.14.7
  Downloaded wyz v0.2.0
  Downloaded num-derive v0.3.3
  Downloaded crunchy v0.2.2
  Downloaded elliptic-curve v0.8.5
  Downloaded crypto-mac v0.10.1
  Downloaded base16 v0.2.1
  Downloaded cfg-if v0.1.10
  Downloaded rand_core v0.5.1
  Downloaded uint v0.9.5
  Downloaded zeroize v1.3.0
  Downloaded num-complex v0.4.3
  Downloaded log v0.4.17
  Downloaded blake2 v0.9.2
  Downloaded typenum v1.16.0
  Downloaded getrandom v0.2.9
  Downloaded funty v1.1.0
  Downloaded zeroize_derive v1.4.2
  Downloaded hex v0.4.3
  Downloaded wasm-bindgen-macro v0.2.84
  Downloaded num-traits v0.2.15
  Downloaded autocfg v1.1.0
  Downloaded ff v0.8.0
  Downloaded quote v1.0.26
  Downloaded base64 v0.13.1
  Downloaded ryu v1.0.13
  Downloaded once_cell v1.17.1
  Downloaded serde_derive v1.0.160
  Downloaded unicode-ident v1.0.8
  Downloaded bumpalo v3.12.1
  Downloaded proc-macro2 v1.0.56
  Downloaded k256 v0.7.3
  Downloaded num-bigint v0.4.3
  Downloaded serde v1.0.160
  Downloaded bitvec v0.18.5
  Downloaded serde_json v1.0.96
  Downloaded casper-types v1.5.0
  Downloaded syn v1.0.109
  Downloaded libc v0.2.142
  Downloaded curve25519-dalek v3.2.1
  Downloaded casper-contract v1.4.4
   Compiling proc-macro2 v1.0.56
   Compiling unicode-ident v1.0.8
   Compiling quote v1.0.26
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling typenum v1.16.0
   Compiling generic-array v0.14.7
   Compiling syn v2.0.15
    Checking rand_core v0.5.1
    Checking subtle v2.4.1
    Checking digest v0.9.0
   Compiling syn v1.0.109
   Compiling num-traits v0.2.15
   Compiling zeroize_derive v1.4.2
   Compiling num-integer v0.1.45
    Checking radium v0.3.0
    Checking funty v1.1.0
    Checking cfg-if v1.0.0
    Checking wyz v0.2.0
    Checking zeroize v1.3.0
   Compiling wasm-bindgen-shared v0.2.84
    Checking bitvec v0.18.5
   Compiling log v0.4.17
   Compiling serde_derive v1.0.160
    Checking signature v1.2.2
    Checking ff v0.8.0
   Compiling num-bigint v0.4.3
   Compiling serde v1.0.160
    Checking group v0.8.0
    Checking crypto-mac v0.10.1
   Compiling num-rational v0.4.1
   Compiling num-iter v0.1.43
   Compiling once_cell v1.17.1
   Compiling crunchy v0.2.2
    Checking ppv-lite86 v0.2.17
    Checking opaque-debug v0.3.0
    Checking byteorder v1.4.3
   Compiling bumpalo v3.12.1
   Compiling wasm-bindgen-backend v0.2.84
    Checking rand_chacha v0.2.2
    Checking hmac v0.10.1
    Checking elliptic-curve v0.8.5
    Checking block-buffer v0.9.0
   Compiling serde_json v1.0.96
    Checking sha2 v0.9.9
    Checking ecdsa v0.10.2
    Checking rand v0.7.3
   Compiling wasm-bindgen-macro-support v0.2.84
    Checking curve25519-dalek v3.2.1
    Checking ed25519 v1.2.0
    Checking num-complex v0.4.3
    Checking crypto-mac v0.8.0
    Checking hex v0.4.3
    Checking itoa v1.0.6
    Checking ryu v1.0.13
   Compiling wee_alloc v0.4.5
   Compiling wasm-bindgen v0.2.84
    Checking static_assertions v1.1.0
    Checking rand_core v0.6.4
    Checking uint v0.9.5
    Checking rand v0.8.5
   Compiling wasm-bindgen-macro v0.2.84
    Checking blake2 v0.9.2
    Checking num v0.4.0
    Checking ed25519-dalek v1.0.1
    Checking serde_bytes v0.11.9
    Checking k256 v0.7.3
   Compiling num-derive v0.3.3
    Checking bitflags v1.3.2
    Checking hex_fmt v0.3.0
    Checking base64 v0.13.1
    Checking base16 v0.2.1
    Checking memory_units v0.4.0
    Checking cfg-if v0.1.10
    Checking js-sys v0.3.61
    Checking casper-types v1.5.0
    Checking getrandom v0.2.9
    Checking casper-contract v1.4.4
    Checking contract-utils v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/utils/contract-utils)
    Checking staking_contract v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/staking_contract)
    Finished dev [unoptimized + debuginfo] target(s) in 5m 28s
cd staking_contract && cargo fmt --all -- --check
```

## Build `(1m 52s)`

```sh
Run cd staking_contract ; rustup target add wasm32-unknown-unknown ; make build-contract
  cd staking_contract ; rustup target add wasm32-unknown-unknown ; make build-contract
  shell: /usr/bin/bash -e {0}
  env:
    CARGO_TERM_COLOR: always
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
cd staking_contract && cargo build --release --target wasm32-unknown-unknown
   Compiling proc-macro2 v1.0.56
   Compiling unicode-ident v1.0.8
   Compiling quote v1.0.26
   Compiling version_check v0.9.4
   Compiling typenum v1.16.0
   Compiling autocfg v1.1.0
   Compiling generic-array v0.14.7
   Compiling syn v2.0.15
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling digest v0.9.0
   Compiling syn v1.0.109
   Compiling num-traits v0.2.15
   Compiling zeroize_derive v1.4.2
   Compiling num-integer v0.1.45
   Compiling radium v0.3.0
   Compiling cfg-if v1.0.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling zeroize v1.3.0
   Compiling serde_derive v1.0.160
   Compiling bitvec v0.18.5
   Compiling log v0.4.17
   Compiling wasm-bindgen-shared v0.2.84
   Compiling ff v0.8.0
   Compiling signature v1.2.2
   Compiling num-bigint v0.4.3
   Compiling serde v1.0.160
   Compiling group v0.8.0
   Compiling crypto-mac v0.10.1
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling bumpalo v3.12.1
   Compiling opaque-debug v0.3.0
   Compiling once_cell v1.17.1
   Compiling crunchy v0.2.2
   Compiling byteorder v1.4.3
   Compiling ppv-lite86 v0.2.17
   Compiling rand_chacha v0.2.2
   Compiling wasm-bindgen-backend v0.2.84
   Compiling hmac v0.10.1
   Compiling elliptic-curve v0.8.5
   Compiling block-buffer v0.9.0
   Compiling serde_json v1.0.96
   Compiling sha2 v0.9.9
   Compiling ecdsa v0.10.2
   Compiling wasm-bindgen-macro-support v0.2.84
   Compiling rand v0.7.3
   Compiling curve25519-dalek v3.2.1
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.3
   Compiling crypto-mac v0.8.0
   Compiling rand_core v0.6.4
   Compiling wee_alloc v0.4.5
   Compiling itoa v1.0.6
   Compiling hex v0.4.3
   Compiling ryu v1.0.13
   Compiling static_assertions v1.1.0
   Compiling wasm-bindgen v0.2.84
   Compiling uint v0.9.5
   Compiling rand v0.8.5
   Compiling blake2 v0.9.2
   Compiling num v0.4.0
   Compiling ed25519-dalek v1.0.1
   Compiling wasm-bindgen-macro v0.2.84
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.9
   Compiling num-derive v0.3.3
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling base64 v0.13.1
   Compiling cfg-if v0.1.10
   Compiling bitflags v1.3.2
   Compiling memory_units v0.4.0
   Compiling casper-types v1.5.0
   Compiling js-sys v0.3.61
   Compiling casper-contract v1.4.4
   Compiling contract-utils v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/utils/contract-utils)
   Compiling getrandom v0.2.9
   Compiling staking_contract v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/staking_contract)
    Finished release [optimized] target(s) in 1m 11s
wasm-strip staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cd ../erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
 Downloading crates ...
  Downloaded serde_derive v1.0.143
  Downloaded unicode-xid v0.2.3
  Downloaded itoa v1.0.3
  Downloaded zeroize_derive v1.3.2
  Downloaded uint v0.9.3
  Downloaded rand_core v0.6.3
  Downloaded ppv-lite86 v0.2.16
  Downloaded quote v1.0.21
  Downloaded typenum v1.15.0
  Downloaded serde_bytes v0.11.7
  Downloaded generic-array v0.14.6
  Downloaded once_cell v1.13.0
  Downloaded unicode-ident v1.0.3
  Downloaded num-complex v0.4.2
  Downloaded cpufeatures v0.2.2
  Downloaded proc-macro2 v1.0.43
  Downloaded serde v1.0.143
  Downloaded ryu v1.0.11
  Downloaded base64 v0.13.0
  Downloaded synstructure v0.12.6
  Downloaded syn v1.0.99
  Downloaded serde_json v1.0.83
  Downloaded libc v0.2.131
   Compiling autocfg v1.1.0
   Compiling typenum v1.15.0
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.43
   Compiling generic-array v0.14.6
   Compiling quote v1.0.21
   Compiling unicode-ident v1.0.3
   Compiling syn v1.0.99
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling digest v0.9.0
   Compiling num-traits v0.2.15
   Compiling unicode-xid v0.2.3
   Compiling num-integer v0.1.45
   Compiling synstructure v0.12.6
   Compiling radium v0.3.0
   Compiling wyz v0.2.0
   Compiling funty v1.1.0
   Compiling zeroize_derive v1.3.2
   Compiling bitvec v0.18.5
   Compiling zeroize v1.3.0
   Compiling serde_derive v1.0.143
   Compiling signature v1.2.2
   Compiling num-bigint v0.4.3
   Compiling ff v0.8.0
   Compiling serde v1.0.143
   Compiling group v0.8.0
   Compiling crypto-mac v0.10.1
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling byteorder v1.4.3
   Compiling crunchy v0.2.2
   Compiling ppv-lite86 v0.2.16
   Compiling opaque-debug v0.3.0
   Compiling cfg-if v1.0.0
   Compiling rand_chacha v0.2.2
   Compiling hmac v0.10.1
   Compiling elliptic-curve v0.8.5
   Compiling block-buffer v0.9.0
   Compiling serde_json v1.0.83
   Compiling sha2 v0.9.9
   Compiling ecdsa v0.10.2
   Compiling rand v0.7.3
   Compiling curve25519-dalek v3.2.1
   Compiling ed25519 v1.2.0
   Compiling num-complex v0.4.2
   Compiling crypto-mac v0.8.0
   Compiling static_assertions v1.1.0
   Compiling rand_core v0.6.3
   Compiling itoa v1.0.3
   Compiling wee_alloc v0.4.5
   Compiling ryu v1.0.11
   Compiling hex v0.4.3
   Compiling uint v0.9.3
   Compiling rand v0.8.5
   Compiling blake2 v0.9.2
   Compiling num v0.4.0
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.7
   Compiling num-derive v0.3.3
   Compiling hex_fmt v0.3.0
   Compiling base16 v0.2.1
   Compiling cfg-if v0.1.10
   Compiling bitflags v1.3.2
   Compiling memory_units v0.4.0
   Compiling base64 v0.13.0
   Compiling once_cell v1.13.0
   Compiling casper-types v1.5.0
   Compiling casper-contract v1.4.4
   Compiling casper-erc20 v0.2.1 (/home/runner/work/casper_staking/casper_staking/erc20/erc20)
warning: unused import: `alloc::string::String`
 --> erc20/src/error.rs:2:5
  |
2 | use alloc::string::String;
  |     ^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: missing documentation for a function
   --> erc20/src/entry_points.rs:145:1
    |
145 | pub fn mint() -> EntryPoint {
    | ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    |
note: the lint level is defined here
   --> erc20/src/lib.rs:13:9
    |
13  | #![warn(missing_docs)]
    |         ^^^^^^^^^^^^

warning: missing documentation for a variant
  --> erc20/src/error.rs:28:5
   |
28 |     UserAllowance(u16),
   |     ^^^^^^^^^^^^^

warning: `casper-erc20` (lib) generated 3 warnings (run `cargo fix --lib -p casper-erc20` to apply 1 suggestion)
   Compiling erc20-token v0.1.0 (/home/runner/work/casper_staking/casper_staking/erc20/erc20-token)
warning: unused import: `core::panic::PanicInfo`
  --> erc20-token/src/main.rs:10:5
   |
10 | use core::panic::PanicInfo;
   |     ^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `erc20-token` (bin "erc20_token") generated 1 warning (run `cargo fix --bin "erc20_token"` to apply 1 suggestion)
    Finished release [optimized] target(s) in 40.86s
wasm-strip ../erc20/erc20-token/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
```

## Test `(1m 49s)`

```sh
Run cd staking_contract ; rustup target add wasm32-unknown-unknown ; make build-contract ; make test
  cd staking_contract ; rustup target add wasm32-unknown-unknown ; make build-contract ; make test
  shell: /usr/bin/bash -e {0}
  env:
    CARGO_TERM_COLOR: always
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
cd staking_contract && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.07s
wasm-strip staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cd ../erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
wasm-strip ../erc20/erc20-token/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
warning: unused import: `alloc::string::String`
cd staking_contract && cargo build --release --target wasm32-unknown-unknown
 --> erc20/src/error.rs:2:5
  |
2 | use alloc::string::String;
  |     ^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: missing documentation for a function
   --> erc20/src/entry_points.rs:145:1
    |
145 | pub fn mint() -> EntryPoint {
    | ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    |
note: the lint level is defined here
   --> erc20/src/lib.rs:13:9
    |
13  | #![warn(missing_docs)]
    |         ^^^^^^^^^^^^

warning: missing documentation for a variant
  --> erc20/src/error.rs:28:5
   |
28 |     UserAllowance(u16),
   |     ^^^^^^^^^^^^^

warning: `casper-erc20` (lib) generated 3 warnings (run `cargo fix --lib -p casper-erc20` to apply 1 suggestion)
warning: unused import: `core::panic::PanicInfo`
  --> erc20-token/src/main.rs:10:5
   |
10 | use core::panic::PanicInfo;
   |     ^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `erc20-token` (bin "erc20_token") generated 1 warning (run `cargo fix --bin "erc20_token"` to apply 1 suggestion)
    Finished release [optimized] target(s) in 0.06s
    Finished release [optimized] target(s) in 0.07s
wasm-strip staking_contract/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cd ../erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
warning: unused import: `alloc::string::String`
 --> erc20/src/error.rs:2:5
  |
2 | use alloc::string::String;
  |     ^^^^^^^^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: missing documentation for a function
   --> erc20/src/entry_points.rs:145:1
    |
145 | pub fn mint() -> EntryPoint {
    | ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    |
note: the lint level is defined here
   --> erc20/src/lib.rs:13:9
    |
13  | #![warn(missing_docs)]
    |         ^^^^^^^^^^^^

warning: missing documentation for a variant
  --> erc20/src/error.rs:28:5
   |
28 |     UserAllowance(u16),
   |     ^^^^^^^^^^^^^

warning: `casper-erc20` (lib) generated 3 warnings (run `cargo fix --lib -p casper-erc20` to apply 1 suggestion)
warning: unused import: `core::panic::PanicInfo`
  --> erc20-token/src/main.rs:10:5
   |
10 | use core::panic::PanicInfo;
   |     ^^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: `erc20-token` (bin "erc20_token") generated 1 warning (run `cargo fix --bin "erc20_token"` to apply 1 suggestion)
    Finished release [optimized] target(s) in 0.06s
wasm-strip ../erc20/erc20-token/target/wasm32-unknown-unknown/release/staking_contract.wasm 2>/dev/null | true
cp staking_contract/target/wasm32-unknown-unknown/release/*.wasm staking_contract_tests/wasm
cp ../erc20/target/wasm32-unknown-unknown/release/erc20_token.wasm staking_contract_tests/wasm/erc20.wasm
cd staking_contract_tests && cargo test
 Downloading crates ...
  Downloaded downcast-rs v1.2.0
  Downloaded chrono v0.4.19
  Downloaded hex-buffer-serde v0.2.2
  Downloaded generic-array v0.14.5
  Downloaded uuid v0.8.2
  Downloaded tempfile v3.3.0
  Downloaded getrandom v0.2.7
  Downloaded either v1.7.0
  Downloaded serde_bytes v0.11.6
  Downloaded serde_derive_internals v0.25.0
  Downloaded tracing-attributes v0.1.22
  Downloaded once_cell v1.17.2
  Downloaded anyhow v1.0.58
  Downloaded proc-macro2 v1.0.40
  Downloaded bit-vec v0.6.3
  Downloaded bit-set v0.5.2
  Downloaded num-bigint v0.2.6
  Downloaded serde_json v1.0.82
  Downloaded time v0.1.44
  Downloaded itoa v1.0.2
  Downloaded thiserror v1.0.31
  Downloaded pin-project-lite v0.2.9
  Downloaded rusty-fork v0.3.0
  Downloaded indexmap v1.9.1
  Downloaded match_cfg v0.1.0
  Downloaded ryu v1.0.10
  Downloaded cc v1.0.73
  Downloaded fnv v1.0.7
  Downloaded fastrand v1.7.0
  Downloaded itertools v0.10.3
  Downloaded value-bag v1.0.0-alpha.9
  Downloaded rand_xorshift v0.3.0
  Downloaded num-rational v0.2.4
  Downloaded quick-error v2.0.1
  Downloaded schemars_derive v0.8.5
  Downloaded num_cpus v1.13.1
  Downloaded ctor v0.1.22
  Downloaded lazy_static v1.4.0
  Downloaded filesize v0.2.0
  Downloaded remove_dir_all v0.5.3
  Downloaded memory_units v0.3.0
  Downloaded unicode-ident v1.0.1
  Downloaded serde_derive v1.0.138
  Downloaded hashbrown v0.12.1
  Downloaded wasmi-validation v0.3.0
  Downloaded hex-buffer-serde v0.3.0
  Downloaded rand_chacha v0.3.1
  Downloaded bincode v1.3.3
  Downloaded wait-timeout v0.2.0
  Downloaded thiserror-impl v1.0.31
  Downloaded pkg-config v0.3.25
  Downloaded linked-hash-map v0.5.6
  Downloaded hostname v0.3.1
  Downloaded quick-error v1.2.3
  Downloaded dyn-clone v1.0.6
  Downloaded lmdb v0.8.0
  Downloaded serde v1.0.138
  Downloaded parity-wasm v0.41.0
  Downloaded quote v1.0.20
  Downloaded tracing v0.1.35
  Downloaded schemars v0.8.5
  Downloaded tracing-core v0.1.28
  Downloaded lmdb-sys v0.8.0
  Downloaded proptest v1.0.0
  Downloaded syn v1.0.98
  Downloaded regex-syntax v0.6.27
  Downloaded libc v0.2.126
  Downloaded datasize_derive v0.2.10
  Downloaded casper-hashing v1.4.3
  Downloaded datasize v0.2.10
  Downloaded casper-engine-test-support v2.2.0
  Downloaded pwasm-utils v0.16.0
  Downloaded wasmi v0.8.0
  Downloaded casper-execution-engine v2.0.0
   Compiling proc-macro2 v1.0.40
   Compiling unicode-ident v1.0.1
   Compiling quote v1.0.20
   Compiling syn v1.0.98
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling libc v0.2.126
   Compiling serde_derive v1.0.138
   Compiling typenum v1.15.0
   Compiling generic-array v0.14.5
   Compiling serde v1.0.138
   Compiling cfg-if v1.0.0
   Compiling num-traits v0.2.15
   Compiling rand_core v0.5.1
   Compiling subtle v2.4.1
   Compiling digest v0.9.0
   Compiling num-integer v0.1.45
   Compiling unicode-xid v0.2.3
   Compiling synstructure v0.12.6
   Compiling zeroize_derive v1.3.2
   Compiling getrandom v0.2.7
   Compiling radium v0.3.0
   Compiling funty v1.1.0
   Compiling wyz v0.2.0
   Compiling ppv-lite86 v0.2.16
   Compiling bitvec v0.18.5
   Compiling zeroize v1.3.0
   Compiling byteorder v1.4.3
   Compiling ff v0.8.0
   Compiling rand_core v0.6.3
   Compiling signature v1.2.2
   Compiling num-bigint v0.4.3
   Compiling group v0.8.0
   Compiling crypto-mac v0.10.1
   Compiling num-iter v0.1.43
   Compiling num-rational v0.4.1
   Compiling indexmap v1.9.1
   Compiling remove_dir_all v0.5.3
   Compiling serde_json v1.0.82
   Compiling hex v0.4.3
   Compiling opaque-debug v0.3.0
   Compiling crunchy v0.2.2
   Compiling fastrand v1.7.0
   Compiling tempfile v3.3.0
   Compiling hmac v0.10.1
   Compiling elliptic-curve v0.8.5
   Compiling rand_chacha v0.3.1
   Compiling rand_chacha v0.2.2
   Compiling block-buffer v0.9.0
   Compiling serde_derive_internals v0.25.0
   Compiling wait-timeout v0.2.0
   Compiling itoa v1.0.2
   Compiling quick-error v1.2.3
   Compiling once_cell v1.17.2
   Compiling cpufeatures v0.2.2
   Compiling ryu v1.0.10
   Compiling bit-vec v0.6.3
   Compiling fnv v1.0.7
   Compiling hashbrown v0.12.1
   Compiling bitflags v1.3.2
   Compiling schemars v0.8.5
   Compiling bit-set v0.5.2
   Compiling rusty-fork v0.3.0
   Compiling schemars_derive v0.8.5
   Compiling sha2 v0.9.9
   Compiling rand v0.7.3
   Compiling rand v0.8.5
   Compiling ecdsa v0.10.2
   Compiling ed25519 v1.2.0
   Compiling rand_xorshift v0.3.0
   Compiling curve25519-dalek v3.2.1
   Compiling datasize_derive v0.2.10
   Compiling crypto-mac v0.8.0
   Compiling num-complex v0.4.2
   Compiling regex-syntax v0.6.27
   Compiling quick-error v2.0.1
   Compiling dyn-clone v1.0.6
   Compiling static_assertions v1.1.0
   Compiling lazy_static v1.4.0
   Compiling uint v0.9.3
   Compiling proptest v1.0.0
   Compiling num v0.4.0
   Compiling datasize v0.2.10
   Compiling blake2 v0.9.2
   Compiling ed25519-dalek v1.0.1
   Compiling k256 v0.7.3
   Compiling serde_bytes v0.11.6
   Compiling num-derive v0.3.3
   Compiling value-bag v1.0.0-alpha.9
   Compiling num-bigint v0.2.6
   Compiling pkg-config v0.3.25
   Compiling base16 v0.2.1
   Compiling hex_fmt v0.3.0
   Compiling cc v1.0.73
   Compiling base64 v0.13.0
   Compiling casper-types v1.5.0
   Compiling lmdb-sys v0.8.0
   Compiling ctor v0.1.22
   Compiling num-rational v0.2.4
   Compiling log v0.4.17
   Compiling parity-wasm v0.41.0
   Compiling thiserror-impl v1.0.31
   Compiling either v1.7.0
   Compiling wee_alloc v0.4.5
   Compiling anyhow v1.0.58
   Compiling itertools v0.10.3
   Compiling thiserror v1.0.31
   Compiling wasmi-validation v0.3.0
   Compiling tracing-core v0.1.28
   Compiling hex-buffer-serde v0.3.0
   Compiling tracing-attributes v0.1.22
   Compiling time v0.1.44
   Compiling downcast-rs v1.2.0
   Compiling memory_units v0.4.0
   Compiling match_cfg v0.1.0
   Compiling memory_units v0.3.0
   Compiling cfg-if v0.1.10
   Compiling pin-project-lite v0.2.9
   Compiling wasmi v0.8.0
   Compiling tracing v0.1.35
   Compiling hostname v0.3.1
   Compiling chrono v0.4.19
   Compiling casper-hashing v1.4.3
   Compiling pwasm-utils v0.16.0
   Compiling lmdb v0.8.0
   Compiling hex-buffer-serde v0.2.2
   Compiling bincode v1.3.3
   Compiling uuid v0.8.2
   Compiling num_cpus v1.13.1
   Compiling linked-hash-map v0.5.6
   Compiling casper-execution-engine v2.0.0
   Compiling casper-contract v1.4.4
   Compiling filesize v0.2.0
   Compiling contract-utils v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/utils/contract-utils)
   Compiling casper-engine-test-support v2.2.0
   Compiling test-env v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/utils/test-env)
   Compiling staking_contract_tests v0.1.0 (/home/runner/work/casper_staking/casper_staking/staking_contract/staking_contract_tests)
warning: unused import: `std::convert::TryInto`
  --> src/staking_contract_tests.rs:15:5
   |
15 | use std::convert::TryInto;
   |     ^^^^^^^^^^^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `std::time::SystemTime`
  --> src/staking_contract_tests.rs:16:5
   |
16 | use std::time::SystemTime;
   |     ^^^^^^^^^^^^^^^^^^^^^

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:316:9
    |
316 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`
    |
    = note: `#[warn(unused_variables)]` on by default

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:452:9
    |
452 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:590:9
    |
590 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:745:9
    |
745 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
   --> src/staking_contract_tests.rs:901:9
    |
901 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
    |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1050:9
     |
1050 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1184:9
     |
1184 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1316:9
     |
1316 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: unused variable: `staking_contract_package_hash`
    --> src/staking_contract_tests.rs:1450:9
     |
1450 |     let staking_contract_package_hash = get_stacking_contract_package_hash(&builder);
     |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_staking_contract_package_hash`

warning: constant `ADDRESS` is never used
  --> src/staking_contract_tests.rs:18:7
   |
18 | const ADDRESS: &str = "9e7283533626d0c7d43fa9ca745af20d8dac7fc3bfe03cdfe50d523a2a0f498d";
   |       ^^^^^^^
   |
   = note: `#[warn(dead_code)]` on by default

warning: `staking_contract_tests` (lib test) generated 12 warnings (run `cargo fix --lib -p staking_contract_tests --tests` to apply 11 suggestions)
    Finished test [unoptimized + debuginfo] target(s) in 1m 41s
     Running unittests src/lib.rs (target/debug/deps/staking_contract_tests-15d14d7a818e324f)

running 11 tests
test staking_contract_tests::test_approve_and_stake ... ok
test staking_contract_tests::test_approve_and_stake_and_add_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_add_reward_withdrawable_amount_too_big - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_amount_staked ... ok
test staking_contract_tests::test_approve_and_stake_and_amount_staked_wrong_address - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_get_current_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_staker_reward ... ok
test staking_contract_tests::test_approve_and_stake_and_staker_reward_wrong_address - should panic ... ok
test staking_contract_tests::test_approve_and_stake_and_withdraw ... ok
test staking_contract_tests::test_approve_and_stake_and_withdraw_too_big_amount - should panic ... ok
test staking_contract_tests::test_stake_but_not_approve - should panic ... ok

test result: ok. 11 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 7.01s

   Doc-tests staking_contract_tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```

## Post Run actions/checkout@v2 `(0s)`

```sh
Post job cleanup.
/usr/bin/git version
git version 2.42.0
Temporarily overriding HOME='/home/runner/work/_temp/d32e7e18-ef3a-4079-8f05-9c8267b347c8' before making global git config changes
Adding repository directory to the temporary git global config as a safe directory
/usr/bin/git config --global --add safe.directory /home/runner/work/casper_staking/casper_staking
/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
http.https://github.com/.extraheader
/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
```

## Complete job `(0s)`

```sh
Cleaning up orphan processes
```