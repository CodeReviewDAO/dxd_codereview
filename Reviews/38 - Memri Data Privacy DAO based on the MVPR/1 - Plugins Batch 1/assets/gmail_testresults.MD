'''[0KRunning with gitlab-runner 14.9.1 (bd40e3da)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1666829017:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.7 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...[0;m
[0KUsing docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...[0;m
[0KWaiting for services to be up and running...[0;m
[0KPulling docker image python:3.7 ...[0;m
[0KUsing docker image sha256:c643d609e9657d8adb9d684950718a8b4e67a312758a0d476c19d54de7bb23b2 for python:3.7 with digest python@sha256:53e59319730a41a52e8b3c43bd114131c91ebc8689dcece363b796cb4e623cc1 ...[0;m
section_end:1666829021:prepare_executor
[0Ksection_start:1666829021:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-90-concurrent-3 via 8e6b65718045...
section_end:1666829022:prepare_script
[0Ksection_start:1666829022:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 50...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/gmail/.git/
[32;1mChecking out 795a5072 as dev...[0;m
Removing .pytest_cache/
Removing gmail_importer.egg-info/
Removing gmail_importer/__pycache__/
Removing tests/__pycache__/

[32;1mSkipping Git submodules setup[0;m
section_end:1666829024:get_sources
[0Ksection_start:1666829024:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:c643d609e9657d8adb9d684950718a8b4e67a312758a0d476c19d54de7bb23b2 for python:3.7 with digest python@sha256:53e59319730a41a52e8b3c43bd114131c91ebc8689dcece363b796cb4e623cc1 ...[0;m
[32;1m$ apt-get update && apt-get install -y libsqlcipher-dev && apt-get install -y libgl1-mesa-glx[0;m
Get:1 http://deb.debian.org/debian bullseye InRelease [116 kB]
Get:2 http://deb.debian.org/debian-security bullseye-security InRelease [48.4 kB]
Get:3 http://deb.debian.org/debian bullseye-updates InRelease [44.1 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 Packages [8184 kB]
Get:5 http://deb.debian.org/debian-security bullseye-security/main amd64 Packages [193 kB]
Get:6 http://deb.debian.org/debian bullseye-updates/main amd64 Packages [14.6 kB]
Fetched 8599 kB in 2s (4827 kB/s)
Reading package lists...
Reading package lists...
Building dependency tree...
Reading state information...
The following additional packages will be installed:
  libsqlcipher0
Suggested packages:
  sqlite3-doc
The following NEW packages will be installed:
  libsqlcipher-dev libsqlcipher0
0 upgraded, 2 newly installed, 0 to remove and 0 not upgraded.
Need to get 998 kB of archives.
After this operation, 2809 kB of additional disk space will be used.
Get:1 http://deb.debian.org/debian bullseye/main amd64 libsqlcipher0 amd64 3.4.1-2 [433 kB]
Get:2 http://deb.debian.org/debian bullseye/main amd64 libsqlcipher-dev amd64 3.4.1-2 [565 kB]
debconf: delaying package configuration, since apt-utils is not installed
Fetched 998 kB in 0s (30.2 MB/s)
Selecting previously unselected package libsqlcipher0:amd64.
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
(Reading database ... 23422 files and directories currently installed.)
Preparing to unpack .../libsqlcipher0_3.4.1-2_amd64.deb ...
Unpacking libsqlcipher0:amd64 (3.4.1-2) ...
Selecting previously unselected package libsqlcipher-dev.
Preparing to unpack .../libsqlcipher-dev_3.4.1-2_amd64.deb ...
Unpacking libsqlcipher-dev (3.4.1-2) ...
Setting up libsqlcipher0:amd64 (3.4.1-2) ...
Setting up libsqlcipher-dev (3.4.1-2) ...
Processing triggers for libc-bin (2.31-13+deb11u5) ...
Reading package lists...
Building dependency tree...
Reading state information...
The following additional packages will be installed:
  libdrm-amdgpu1 libdrm-common libdrm-intel1 libdrm-nouveau2 libdrm-radeon1
  libdrm2 libgl1 libgl1-mesa-dri libglapi-mesa libglvnd0 libglx-mesa0 libglx0
  libllvm11 libpciaccess0 libsensors-config libsensors5 libvulkan1
  libwayland-client0 libx11-xcb1 libxcb-dri2-0 libxcb-dri3-0 libxcb-glx0
  libxcb-present0 libxcb-randr0 libxcb-sync1 libxcb-xfixes0 libxdamage1
  libxfixes3 libxshmfence1 libxxf86vm1 libz3-4 mesa-vulkan-drivers
Suggested packages:
  pciutils lm-sensors
The following NEW packages will be installed:
  libdrm-amdgpu1 libdrm-common libdrm-intel1 libdrm-nouveau2 libdrm-radeon1
  libdrm2 libgl1 libgl1-mesa-dri libgl1-mesa-glx libglapi-mesa libglvnd0
  libglx-mesa0 libglx0 libllvm11 libpciaccess0 libsensors-config libsensors5
  libvulkan1 libwayland-client0 libx11-xcb1 libxcb-dri2-0 libxcb-dri3-0
  libxcb-glx0 libxcb-present0 libxcb-randr0 libxcb-sync1 libxcb-xfixes0
  libxdamage1 libxfixes3 libxshmfence1 libxxf86vm1 libz3-4 mesa-vulkan-drivers
0 upgraded, 33 newly installed, 0 to remove and 0 not upgraded.
Need to get 40.6 MB of archives.
After this operation, 168 MB of additional disk space will be used.
Get:1 http://deb.debian.org/debian bullseye/main amd64 libdrm-common all 2.4.104-1 [14.9 kB]
Get:2 http://deb.debian.org/debian bullseye/main amd64 libdrm2 amd64 2.4.104-1 [41.5 kB]
Get:3 http://deb.debian.org/debian bullseye/main amd64 libdrm-amdgpu1 amd64 2.4.104-1 [28.5 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 libpciaccess0 amd64 0.16-1 [53.6 kB]
Get:5 http://deb.debian.org/debian bullseye/main amd64 libdrm-intel1 amd64 2.4.104-1 [71.8 kB]
Get:6 http://deb.debian.org/debian bullseye/main amd64 libdrm-nouveau2 amd64 2.4.104-1 [26.8 kB]
Get:7 http://deb.debian.org/debian bullseye/main amd64 libdrm-radeon1 amd64 2.4.104-1 [30.2 kB]
Get:8 http://deb.debian.org/debian bullseye/main amd64 libglapi-mesa amd64 20.3.5-1 [71.7 kB]
Get:9 http://deb.debian.org/debian bullseye/main amd64 libz3-4 amd64 4.8.10-1 [6949 kB]
Get:10 http://deb.debian.org/debian bullseye/main amd64 libllvm11 amd64 1:11.0.1-2 [17.9 MB]
Get:11 http://deb.debian.org/debian bullseye/main amd64 libsensors-config all 1:3.6.0-7 [32.3 kB]
Get:12 http://deb.debian.org/debian bullseye/main amd64 libsensors5 amd64 1:3.6.0-7 [52.3 kB]
Get:13 http://deb.debian.org/debian bullseye/main amd64 libvulkan1 amd64 1.2.162.0-1 [103 kB]
Get:14 http://deb.debian.org/debian bullseye/main amd64 libgl1-mesa-dri amd64 20.3.5-1 [9633 kB]
Get:15 http://deb.debian.org/debian bullseye/main amd64 libglvnd0 amd64 1.3.2-1 [53.6 kB]
Get:16 http://deb.debian.org/debian bullseye/main amd64 libx11-xcb1 amd64 2:1.7.2-1 [203 kB]
Get:17 http://deb.debian.org/debian bullseye/main amd64 libxcb-dri2-0 amd64 1.14-3 [103 kB]
Get:18 http://deb.debian.org/debian bullseye/main amd64 libxcb-dri3-0 amd64 1.14-3 [102 kB]
Get:19 http://deb.debian.org/debian bullseye/main amd64 libxcb-glx0 amd64 1.14-3 [118 kB]
Get:20 http://deb.debian.org/debian bullseye/main amd64 libxcb-present0 amd64 1.14-3 [101 kB]
Get:21 http://deb.debian.org/debian bullseye/main amd64 libxcb-sync1 amd64 1.14-3 [105 kB]
Get:22 http://deb.debian.org/debian bullseye/main amd64 libxcb-xfixes0 amd64 1.14-3 [105 kB]
Get:23 http://deb.debian.org/debian bullseye/main amd64 libxdamage1 amd64 1:1.1.5-2 [15.7 kB]
Get:24 http://deb.debian.org/debian bullseye/main amd64 libxfixes3 amd64 1:5.0.3-2 [22.1 kB]
Get:25 http://deb.debian.org/debian bullseye/main amd64 libxshmfence1 amd64 1.3-1 [8820 B]
Get:26 http://deb.debian.org/debian bullseye/main amd64 libxxf86vm1 amd64 1:1.1.4-1+b2 [20.8 kB]
Get:27 http://deb.debian.org/debian bullseye/main amd64 libglx-mesa0 amd64 20.3.5-1 [186 kB]
Get:28 http://deb.debian.org/debian bullseye/main amd64 libglx0 amd64 1.3.2-1 [35.7 kB]
Get:29 http://deb.debian.org/debian bullseye/main amd64 libgl1 amd64 1.3.2-1 [89.5 kB]
Get:30 http://deb.debian.org/debian bullseye/main amd64 libgl1-mesa-glx amd64 20.3.5-1 [51.1 kB]
Get:31 http://deb.debian.org/debian bullseye/main amd64 libwayland-client0 amd64 1.18.0-2~exp1.1 [26.9 kB]
Get:32 http://deb.debian.org/debian bullseye/main amd64 libxcb-randr0 amd64 1.14-3 [113 kB]
Get:33 http://deb.debian.org/debian bullseye/main amd64 mesa-vulkan-drivers amd64 20.3.5-1 [4086 kB]
debconf: delaying package configuration, since apt-utils is not installed
Fetched 40.6 MB in 0s (94.4 MB/s)
Selecting previously unselected package libdrm-common.
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
(Reading database ... 23440 files and directories currently installed.)
Preparing to unpack .../00-libdrm-common_2.4.104-1_all.deb ...
Unpacking libdrm-common (2.4.104-1) ...
Selecting previously unselected package libdrm2:amd64.
Preparing to unpack .../01-libdrm2_2.4.104-1_amd64.deb ...
Unpacking libdrm2:amd64 (2.4.104-1) ...
Selecting previously unselected package libdrm-amdgpu1:amd64.
Preparing to unpack .../02-libdrm-amdgpu1_2.4.104-1_amd64.deb ...
Unpacking libdrm-amdgpu1:amd64 (2.4.104-1) ...
Selecting previously unselected package libpciaccess0:amd64.
Preparing to unpack .../03-libpciaccess0_0.16-1_amd64.deb ...
Unpacking libpciaccess0:amd64 (0.16-1) ...
Selecting previously unselected package libdrm-intel1:amd64.
Preparing to unpack .../04-libdrm-intel1_2.4.104-1_amd64.deb ...
Unpacking libdrm-intel1:amd64 (2.4.104-1) ...
Selecting previously unselected package libdrm-nouveau2:amd64.
Preparing to unpack .../05-libdrm-nouveau2_2.4.104-1_amd64.deb ...
Unpacking libdrm-nouveau2:amd64 (2.4.104-1) ...
Selecting previously unselected package libdrm-radeon1:amd64.
Preparing to unpack .../06-libdrm-radeon1_2.4.104-1_amd64.deb ...
Unpacking libdrm-radeon1:amd64 (2.4.104-1) ...
Selecting previously unselected package libglapi-mesa:amd64.
Preparing to unpack .../07-libglapi-mesa_20.3.5-1_amd64.deb ...
Unpacking libglapi-mesa:amd64 (20.3.5-1) ...
Selecting previously unselected package libz3-4:amd64.
Preparing to unpack .../08-libz3-4_4.8.10-1_amd64.deb ...
Unpacking libz3-4:amd64 (4.8.10-1) ...
Selecting previously unselected package libllvm11:amd64.
Preparing to unpack .../09-libllvm11_1%3a11.0.1-2_amd64.deb ...
Unpacking libllvm11:amd64 (1:11.0.1-2) ...
Selecting previously unselected package libsensors-config.
Preparing to unpack .../10-libsensors-config_1%3a3.6.0-7_all.deb ...
Unpacking libsensors-config (1:3.6.0-7) ...
Selecting previously unselected package libsensors5:amd64.
Preparing to unpack .../11-libsensors5_1%3a3.6.0-7_amd64.deb ...
Unpacking libsensors5:amd64 (1:3.6.0-7) ...
Selecting previously unselected package libvulkan1:amd64.
Preparing to unpack .../12-libvulkan1_1.2.162.0-1_amd64.deb ...
Unpacking libvulkan1:amd64 (1.2.162.0-1) ...
Selecting previously unselected package libgl1-mesa-dri:amd64.
Preparing to unpack .../13-libgl1-mesa-dri_20.3.5-1_amd64.deb ...
Unpacking libgl1-mesa-dri:amd64 (20.3.5-1) ...
Selecting previously unselected package libglvnd0:amd64.
Preparing to unpack .../14-libglvnd0_1.3.2-1_amd64.deb ...
Unpacking libglvnd0:amd64 (1.3.2-1) ...
Selecting previously unselected package libx11-xcb1:amd64.
Preparing to unpack .../15-libx11-xcb1_2%3a1.7.2-1_amd64.deb ...
Unpacking libx11-xcb1:amd64 (2:1.7.2-1) ...
Selecting previously unselected package libxcb-dri2-0:amd64.
Preparing to unpack .../16-libxcb-dri2-0_1.14-3_amd64.deb ...
Unpacking libxcb-dri2-0:amd64 (1.14-3) ...
Selecting previously unselected package libxcb-dri3-0:amd64.
Preparing to unpack .../17-libxcb-dri3-0_1.14-3_amd64.deb ...
Unpacking libxcb-dri3-0:amd64 (1.14-3) ...
Selecting previously unselected package libxcb-glx0:amd64.
Preparing to unpack .../18-libxcb-glx0_1.14-3_amd64.deb ...
Unpacking libxcb-glx0:amd64 (1.14-3) ...
Selecting previously unselected package libxcb-present0:amd64.
Preparing to unpack .../19-libxcb-present0_1.14-3_amd64.deb ...
Unpacking libxcb-present0:amd64 (1.14-3) ...
Selecting previously unselected package libxcb-sync1:amd64.
Preparing to unpack .../20-libxcb-sync1_1.14-3_amd64.deb ...
Unpacking libxcb-sync1:amd64 (1.14-3) ...
Selecting previously unselected package libxcb-xfixes0:amd64.
Preparing to unpack .../21-libxcb-xfixes0_1.14-3_amd64.deb ...
Unpacking libxcb-xfixes0:amd64 (1.14-3) ...
Selecting previously unselected package libxdamage1:amd64.
Preparing to unpack .../22-libxdamage1_1%3a1.1.5-2_amd64.deb ...
Unpacking libxdamage1:amd64 (1:1.1.5-2) ...
Selecting previously unselected package libxfixes3:amd64.
Preparing to unpack .../23-libxfixes3_1%3a5.0.3-2_amd64.deb ...
Unpacking libxfixes3:amd64 (1:5.0.3-2) ...
Selecting previously unselected package libxshmfence1:amd64.
Preparing to unpack .../24-libxshmfence1_1.3-1_amd64.deb ...
Unpacking libxshmfence1:amd64 (1.3-1) ...
Selecting previously unselected package libxxf86vm1:amd64.
Preparing to unpack .../25-libxxf86vm1_1%3a1.1.4-1+b2_amd64.deb ...
Unpacking libxxf86vm1:amd64 (1:1.1.4-1+b2) ...
Selecting previously unselected package libglx-mesa0:amd64.
Preparing to unpack .../26-libglx-mesa0_20.3.5-1_amd64.deb ...
Unpacking libglx-mesa0:amd64 (20.3.5-1) ...
Selecting previously unselected package libglx0:amd64.
Preparing to unpack .../27-libglx0_1.3.2-1_amd64.deb ...
Unpacking libglx0:amd64 (1.3.2-1) ...
Selecting previously unselected package libgl1:amd64.
Preparing to unpack .../28-libgl1_1.3.2-1_amd64.deb ...
Unpacking libgl1:amd64 (1.3.2-1) ...
Selecting previously unselected package libgl1-mesa-glx:amd64.
Preparing to unpack .../29-libgl1-mesa-glx_20.3.5-1_amd64.deb ...
Unpacking libgl1-mesa-glx:amd64 (20.3.5-1) ...
Selecting previously unselected package libwayland-client0:amd64.
Preparing to unpack .../30-libwayland-client0_1.18.0-2~exp1.1_amd64.deb ...
Unpacking libwayland-client0:amd64 (1.18.0-2~exp1.1) ...
Selecting previously unselected package libxcb-randr0:amd64.
Preparing to unpack .../31-libxcb-randr0_1.14-3_amd64.deb ...
Unpacking libxcb-randr0:amd64 (1.14-3) ...
Selecting previously unselected package mesa-vulkan-drivers:amd64.
Preparing to unpack .../32-mesa-vulkan-drivers_20.3.5-1_amd64.deb ...
Unpacking mesa-vulkan-drivers:amd64 (20.3.5-1) ...
Setting up libxcb-dri3-0:amd64 (1.14-3) ...
Setting up libx11-xcb1:amd64 (2:1.7.2-1) ...
Setting up libpciaccess0:amd64 (0.16-1) ...
Setting up libxdamage1:amd64 (1:1.1.5-2) ...
Setting up libxcb-xfixes0:amd64 (1.14-3) ...
Setting up libglvnd0:amd64 (1.3.2-1) ...
Setting up libxcb-glx0:amd64 (1.14-3) ...
Setting up libsensors-config (1:3.6.0-7) ...
Setting up libxxf86vm1:amd64 (1:1.1.4-1+b2) ...
Setting up libxcb-present0:amd64 (1.14-3) ...
Setting up libz3-4:amd64 (4.8.10-1) ...
Setting up libllvm11:amd64 (1:11.0.1-2) ...
Setting up libxfixes3:amd64 (1:5.0.3-2) ...
Setting up libxcb-sync1:amd64 (1.14-3) ...
Setting up libsensors5:amd64 (1:3.6.0-7) ...
Setting up libglapi-mesa:amd64 (20.3.5-1) ...
Setting up libvulkan1:amd64 (1.2.162.0-1) ...
Setting up libxcb-dri2-0:amd64 (1.14-3) ...
Setting up libxshmfence1:amd64 (1.3-1) ...
Setting up libxcb-randr0:amd64 (1.14-3) ...
Setting up libdrm-common (2.4.104-1) ...
Setting up libwayland-client0:amd64 (1.18.0-2~exp1.1) ...
Setting up libdrm2:amd64 (2.4.104-1) ...
Setting up libdrm-amdgpu1:amd64 (2.4.104-1) ...
Setting up mesa-vulkan-drivers:amd64 (20.3.5-1) ...
Setting up libdrm-nouveau2:amd64 (2.4.104-1) ...
Setting up libdrm-radeon1:amd64 (2.4.104-1) ...
Setting up libdrm-intel1:amd64 (2.4.104-1) ...
Setting up libgl1-mesa-dri:amd64 (20.3.5-1) ...
Setting up libglx-mesa0:amd64 (20.3.5-1) ...
Setting up libglx0:amd64 (1.3.2-1) ...
Setting up libgl1:amd64 (1.3.2-1) ...
Setting up libgl1-mesa-glx:amd64 (20.3.5-1) ...
Processing triggers for libc-bin (2.31-13+deb11u5) ...
[32;1m$ pip install -e .[0;m
Obtaining file:///builds/memri/plugins/gmail
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.25
  Cloning https://gitlab.memri.io/memri/pymemri.git (to revision v0.0.25) to /tmp/pip-install-7e13dcru/pymemri_f9882e147bfd47f78e822b79d4e12edb
  Running command git clone --filter=blob:none --quiet https://gitlab.memri.io/memri/pymemri.git /tmp/pip-install-7e13dcru/pymemri_f9882e147bfd47f78e822b79d4e12edb
  Running command git checkout -q 8697a4f00de76180df2128315e62cc2c72e2405b
  Resolved https://gitlab.memri.io/memri/pymemri.git to commit 8697a4f00de76180df2128315e62cc2c72e2405b
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting requests
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 4.7 MB/s eta 0:00:00
Collecting tqdm
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 KB 9.0 MB/s eta 0:00:00
Collecting ipdb
  Downloading ipdb-0.13.9.tar.gz (16 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting opencv-python
  Downloading opencv_python-4.6.0.66-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (60.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.9/60.9 MB 5.5 MB/s eta 0:00:00
Collecting nbdev==1.1.21
  Downloading nbdev-1.1.21-py3-none-any.whl (46 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 46.9/46.9 KB 1.9 MB/s eta 0:00:00
Collecting matplotlib
  Downloading matplotlib-3.5.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (11.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.2/11.2 MB 53.1 MB/s eta 0:00:00
Collecting imaplib2
  Downloading imaplib2-3.6-py3-none-any.whl (25 kB)
Collecting pytest
  Downloading pytest-7.2.0-py3-none-any.whl (316 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 316.8/316.8 KB 20.7 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.7/site-packages (from nbdev==1.1.21->gmail-importer==0.0.5) (22.0.4)
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 KB 4.0 MB/s eta 0:00:00
Collecting ipykernel
  Downloading ipykernel-6.16.2-py3-none-any.whl (138 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 138.5/138.5 KB 13.4 MB/s eta 0:00:00
Collecting fastcore>=1.3.21
  Downloading fastcore-1.5.27-py3-none-any.whl (67 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 67.1/67.1 KB 4.5 MB/s eta 0:00:00
Collecting ghapi
  Downloading ghapi-1.0.3-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.1/58.1 KB 6.5 MB/s eta 0:00:00
Collecting nbformat>=4.4.0
  Downloading nbformat-5.7.0-py3-none-any.whl (77 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 77.1/77.1 KB 7.1 MB/s eta 0:00:00
Collecting fastrelease
  Downloading fastrelease-0.1.17-py3-none-any.whl (13 kB)
Collecting nbconvert<6
  Downloading nbconvert-5.6.1-py2.py3-none-any.whl (455 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 455.1/455.1 KB 19.7 MB/s eta 0:00:00
Collecting pyyaml
  Downloading PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (596 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 596.3/596.3 KB 33.9 MB/s eta 0:00:00
Collecting jupyter
  Downloading jupyter-1.0.0-py2.py3-none-any.whl (2.7 kB)
Requirement already satisfied: setuptools in /usr/local/lib/python3.7/site-packages (from ipdb->gmail-importer==0.0.5) (57.5.0)
Collecting ipython>=7.17.0
  Downloading ipython-7.34.0-py3-none-any.whl (793 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 793.8/793.8 KB 28.3 MB/s eta 0:00:00
Collecting toml>=0.10.2
  Downloading toml-0.10.2-py2.py3-none-any.whl (16 kB)
Collecting decorator
  Downloading decorator-5.1.1-py3-none-any.whl (9.1 kB)
Collecting numpy>=1.17
  Downloading numpy-1.21.6-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (15.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 15.7/15.7 MB 39.8 MB/s eta 0:00:00
Collecting fonttools>=4.22.0
  Downloading fonttools-4.38.0-py3-none-any.whl (965 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 965.4/965.4 KB 42.1 MB/s eta 0:00:00
Collecting pyparsing>=2.2.1
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 9.2 MB/s eta 0:00:00
Collecting pillow>=6.2.0
  Downloading Pillow-9.2.0-cp37-cp37m-manylinux_2_28_x86_64.whl (3.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.2/3.2 MB 46.7 MB/s eta 0:00:00
Collecting cycler>=0.10
  Downloading cycler-0.11.0-py3-none-any.whl (6.4 kB)
Collecting kiwisolver>=1.0.1
  Downloading kiwisolver-1.4.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 37.0 MB/s eta 0:00:00
Collecting python-dateutil>=2.7
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 KB 20.3 MB/s eta 0:00:00
Collecting fastcore>=1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 4.3 MB/s eta 0:00:00
Collecting jupyter-client==6.1.12
  Downloading jupyter_client-6.1.12-py3-none-any.whl (112 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 112.7/112.7 KB 132.3 kB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 2.8 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting pandas
  Downloading pandas-1.3.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.3/11.3 MB 52.7 MB/s eta 0:00:00
Collecting pillow>=6.2.0
  Downloading Pillow-8.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 49.6 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 4.0 MB/s eta 0:00:00
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 399.4 kB/s eta 0:00:00
Collecting pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
  Downloading pydantic-1.10.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.8/11.8 MB 53.5 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 4.6 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.0-py2.py3-none-any.whl (22 kB)
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.5.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (45 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 45.9/45.9 KB 5.1 MB/s eta 0:00:00
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.1-cp37-cp37m-manylinux_2_28_x86_64.whl (143 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 143.6/143.6 KB 13.6 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 4.5 MB/s eta 0:00:00
Collecting typing-extensions>=3.7.4.3
  Downloading typing_extensions-4.4.0-py3-none-any.whl (26 kB)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 KB 4.7 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting jupyter-core>=4.6.0
  Downloading jupyter_core-4.11.2-py3-none-any.whl (88 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 88.5/88.5 KB 7.2 MB/s eta 0:00:00
Collecting traitlets
  Downloading traitlets-5.5.0-py3-none-any.whl (107 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 107.4/107.4 KB 9.0 MB/s eta 0:00:00
Collecting pyzmq>=13
  Downloading pyzmq-24.0.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 7.1 MB/s eta 0:00:00
Collecting tornado>=4.1
  Downloading tornado-6.2-cp37-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (423 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 424.0/424.0 KB 24.4 MB/s eta 0:00:00
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 6.3 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 5.0 MB/s eta 0:00:00
Collecting certifi>=2017.4.17
  Downloading certifi-2022.9.24-py3-none-any.whl (161 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 161.1/161.1 KB 16.5 MB/s eta 0:00:00
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 KB 8.8 MB/s eta 0:00:00
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 KB 6.6 MB/s eta 0:00:00
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.0.0rc9-py3-none-any.whl (12 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting importlib-metadata>=0.12
  Downloading importlib_metadata-5.0.0-py3-none-any.whl (21 kB)
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting zipp>=0.5
  Downloading zipp-3.10.0-py3-none-any.whl (6.2 kB)
Collecting pygments
  Downloading Pygments-2.13.0-py3-none-any.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 32.3 MB/s eta 0:00:00
Collecting pickleshare
  Downloading pickleshare-0.7.5-py2.py3-none-any.whl (6.9 kB)
Collecting prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0
  Downloading prompt_toolkit-3.0.31-py3-none-any.whl (382 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 382.3/382.3 KB 16.6 MB/s eta 0:00:00
Collecting pexpect>4.3
  Downloading pexpect-4.8.0-py2.py3-none-any.whl (59 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 59.0/59.0 KB 4.7 MB/s eta 0:00:00
Collecting backcall
  Downloading backcall-0.2.0-py2.py3-none-any.whl (11 kB)
Collecting matplotlib-inline
  Downloading matplotlib_inline-0.1.6-py3-none-any.whl (9.4 kB)
Collecting jedi>=0.16
  Downloading jedi-0.18.1-py2.py3-none-any.whl (1.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.6/1.6 MB 38.2 MB/s eta 0:00:00
Collecting mistune<2,>=0.8.1
  Downloading mistune-0.8.4-py2.py3-none-any.whl (16 kB)
Collecting defusedxml
  Downloading defusedxml-0.7.1-py2.py3-none-any.whl (25 kB)
Collecting pandocfilters>=1.4.1
  Downloading pandocfilters-1.5.0-py2.py3-none-any.whl (8.7 kB)
Collecting bleach
  Downloading bleach-5.0.1-py3-none-any.whl (160 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 160.9/160.9 KB 9.1 MB/s eta 0:00:00
Collecting entrypoints>=0.2.2
  Downloading entrypoints-0.4-py3-none-any.whl (5.3 kB)
Collecting testpath
  Downloading testpath-0.6.0-py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.9/83.9 KB 6.5 MB/s eta 0:00:00
Collecting jsonschema>=2.6
  Downloading jsonschema-4.16.0-py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.1/83.1 KB 4.6 MB/s eta 0:00:00
Collecting fastjsonschema
  Downloading fastjsonschema-2.16.2-py3-none-any.whl (22 kB)
Collecting six>=1.5
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting ghapi
  Downloading ghapi-1.0.2-py3-none-any.whl (57 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 57.7/57.7 KB 3.9 MB/s eta 0:00:00
  Downloading ghapi-1.0.1-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.5/58.5 KB 3.1 MB/s eta 0:00:00
  Downloading ghapi-1.0.0-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 5.4 MB/s eta 0:00:00
  Downloading ghapi-0.1.23-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 2.8 MB/s eta 0:00:00
  Downloading ghapi-0.1.22-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 2.8 MB/s eta 0:00:00
Collecting psutil
  Downloading psutil-5.9.3-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (291 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 291.4/291.4 KB 3.6 MB/s eta 0:00:00
Collecting debugpy>=1.0
  Downloading debugpy-1.6.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (1.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.8/1.8 MB 30.5 MB/s eta 0:00:00
Collecting nest-asyncio
  Downloading nest_asyncio-1.5.6-py3-none-any.whl (5.2 kB)
Collecting qtconsole
  Downloading qtconsole-5.3.2-py3-none-any.whl (120 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.8/120.8 KB 7.3 MB/s eta 0:00:00
Collecting ipywidgets
  Downloading ipywidgets-8.0.2-py3-none-any.whl (134 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 134.4/134.4 KB 11.5 MB/s eta 0:00:00
Collecting notebook
  Downloading notebook-6.5.1-py3-none-any.whl (439 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 439.1/439.1 KB 13.7 MB/s eta 0:00:00
Collecting jupyter-console
  Downloading jupyter_console-6.4.4-py3-none-any.whl (22 kB)
Collecting pytz>=2017.3
  Downloading pytz-2022.5-py2.py3-none-any.whl (500 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 500.7/500.7 KB 17.4 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 KB 18.4 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting parso<0.9.0,>=0.8.0
  Downloading parso-0.8.3-py2.py3-none-any.whl (100 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.8/100.8 KB 5.6 MB/s eta 0:00:00
Collecting pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0
  Downloading pyrsistent-0.18.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (117 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 117.1/117.1 KB 7.9 MB/s eta 0:00:00
Collecting importlib-resources>=1.4.0
  Downloading importlib_resources-5.10.0-py3-none-any.whl (34 kB)
Collecting pkgutil-resolve-name>=1.3.10
  Downloading pkgutil_resolve_name-1.3.10-py3-none-any.whl (4.7 kB)
Collecting ptyprocess>=0.5
  Downloading ptyprocess-0.7.0-py2.py3-none-any.whl (13 kB)
Collecting wcwidth
  Downloading wcwidth-0.2.5-py2.py3-none-any.whl (30 kB)
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 3.3 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 8.5 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 51.9 MB/s eta 0:00:00
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (404 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 404.7/404.7 KB 19.9 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting websockets>=10.0
  Downloading websockets-10.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.7/106.7 KB 6.3 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting webencodings
  Downloading webencodings-0.5.1-py2.py3-none-any.whl (11 kB)
Collecting widgetsnbextension~=4.0
  Downloading widgetsnbextension-4.0.3-py3-none-any.whl (2.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.0/2.0 MB 49.8 MB/s eta 0:00:00
Collecting jupyterlab-widgets~=3.0
  Downloading jupyterlab_widgets-3.0.3-py3-none-any.whl (384 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 384.1/384.1 KB 17.5 MB/s eta 0:00:00
Collecting jupyter-console
  Downloading jupyter_console-6.4.3-py3-none-any.whl (22 kB)
  Downloading jupyter_console-6.4.2-py3-none-any.whl (23 kB)
Collecting ipython-genutils
  Downloading ipython_genutils-0.2.0-py2.py3-none-any.whl (26 kB)
Collecting argon2-cffi
  Downloading argon2_cffi-21.3.0-py3-none-any.whl (14 kB)
Collecting prometheus-client
  Downloading prometheus_client-0.15.0-py3-none-any.whl (60 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.1/60.1 KB 4.8 MB/s eta 0:00:00
Collecting Send2Trash>=1.8.0
  Downloading Send2Trash-1.8.0-py3-none-any.whl (18 kB)
Collecting nbclassic==0.4.5
  Downloading nbclassic-0.4.5-py3-none-any.whl (9.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.8/9.8 MB 53.6 MB/s eta 0:00:00
Collecting terminado>=0.8.3
  Downloading terminado-0.17.0-py3-none-any.whl (16 kB)
Collecting notebook-shim>=0.1.0
  Downloading notebook_shim-0.2.0-py3-none-any.whl (13 kB)
Collecting jupyter-server>=1.8
  Downloading jupyter_server-1.21.0-py3-none-any.whl (346 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 346.5/346.5 KB 17.3 MB/s eta 0:00:00
Collecting qtpy>=2.0.1
  Downloading QtPy-2.2.1-py3-none-any.whl (82 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 82.6/82.6 KB 5.7 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Collecting argon2-cffi-bindings
  Downloading argon2_cffi_bindings-21.2.0-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (86 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 86.2/86.2 KB 4.4 MB/s eta 0:00:00
Collecting jupyter-server>=1.8
  Downloading jupyter_server-1.19.1-py3-none-any.whl (346 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 346.4/346.4 KB 22.3 MB/s eta 0:00:00
  Downloading jupyter_server-1.19.0-py3-none-any.whl (346 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 346.3/346.3 KB 18.1 MB/s eta 0:00:00
  Downloading jupyter_server-1.18.1-py3-none-any.whl (344 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 344.9/344.9 KB 25.7 MB/s eta 0:00:00
  Downloading jupyter_server-1.18.0-py3-none-any.whl (344 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 344.6/344.6 KB 30.9 MB/s eta 0:00:00
  Downloading jupyter_server-1.17.1-py3-none-any.whl (344 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 344.5/344.5 KB 30.2 MB/s eta 0:00:00
  Downloading jupyter_server-1.17.0-py3-none-any.whl (342 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 342.8/342.8 KB 24.6 MB/s eta 0:00:00
  Downloading jupyter_server-1.16.0-py3-none-any.whl (343 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 343.1/343.1 KB 21.0 MB/s eta 0:00:00
  Downloading jupyter_server-1.15.6-py3-none-any.whl (341 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 341.5/341.5 KB 26.3 MB/s eta 0:00:00
Collecting websocket-client
  Downloading websocket_client-1.4.1-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.0/55.0 KB 268.5 kB/s eta 0:00:00
Collecting cffi>=1.0.1
  Downloading cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (427 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 427.9/427.9 KB 23.7 MB/s eta 0:00:00
Collecting pycparser
  Downloading pycparser-2.21-py2.py3-none-any.whl (118 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 118.7/118.7 KB 7.0 MB/s eta 0:00:00
Building wheels for collected packages: ipdb, pymemri, python-multipart
  Building wheel for ipdb (setup.py): started
  Building wheel for ipdb (setup.py): finished with status 'done'
  Created wheel for ipdb: filename=ipdb-0.13.9-py3-none-any.whl size=11648 sha256=b0806abb01fdb6dd95c115118ada3570a7251ce7a4ac1f0718e5cc4a8d7b462a
  Stored in directory: /root/.cache/pip/wheels/65/cd/cc/aaf92acae337a28fdd2aa4d632196a59745c8c39f76eaeed01
  Building wheel for pymemri (setup.py): started
  Building wheel for pymemri (setup.py): finished with status 'done'
  Created wheel for pymemri: filename=pymemri-0.0.24-py3-none-any.whl size=75607 sha256=393ff470a31b4cd7bf18539af34ed98c14c6c41ab088dd6475893e04ebeb98b2
  Stored in directory: /tmp/pip-ephem-wheel-cache-ysf9ldy7/wheels/47/d0/7c/4f7eab4f00388073f15d02761f51bce8274d28380e6134f1ae
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=0428a62032eca9a4708c53cb32d25691a90e3a6ff26794b4e4d6d9fa8242aa18
  Stored in directory: /root/.cache/pip/wheels/2c/41/7c/bfd1c180534ffdcc0972f78c5758f89881602175d48a8bcd2c
Successfully built ipdb pymemri python-multipart
Installing collected packages: webencodings, wcwidth, Send2Trash, pytz, ptyprocess, pickleshare, mistune, ipython-genutils, iniconfig, fastjsonschema, backcall, zipp, widgetsnbextension, websockets, websocket-client, uvloop, urllib3, ujson, typing-extensions, traitlets, tqdm, tornado, tomli, toml, testpath, sniffio, smmap, six, pyzmq, pyyaml, python-dotenv, pyrsistent, pyparsing, pygments, pycparser, psutil, prompt-toolkit, prometheus-client, pkgutil-resolve-name, pillow, pexpect, parso, pandocfilters, orjson, numpy, nest-asyncio, MarkupSafe, jupyterlab-widgets, itsdangerous, imaplib2, idna, httptools, giturlparse, fonttools, fastprogress, exceptiongroup, entrypoints, dnspython, defusedxml, decorator, debugpy, cycler, charset-normalizer, certifi, attrs, terminado, requests, python-multipart, python-dateutil, pydantic, packaging, opencv-python, matplotlib-inline, kiwisolver, jupyter-core, jinja2, jedi, importlib-resources, importlib-metadata, h11, gitdb, email_validator, cffi, bleach, asgiref, anyio, watchgod, starlette, qtpy, pluggy, pandas, matplotlib, jupyter-client, jsonschema, ipython, GitPython, fastscript, fastcore, click, argon2-cffi-bindings, uvicorn, pytest, nbformat, ipykernel, ipdb, ghapi, fastapi, argon2-cffi, qtconsole, nbconvert, jupyter-console, ipywidgets, fastrelease, jupyter-server, notebook-shim, nbclassic, notebook, jupyter, nbdev, pymemri, gmail-importer
  Running setup.py develop for gmail-importer
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.1 Send2Trash-1.8.0 anyio-3.6.2 argon2-cffi-21.3.0 argon2-cffi-bindings-21.2.0 asgiref-3.5.2 attrs-22.1.0 backcall-0.2.0 bleach-5.0.1 certifi-2022.9.24 cffi-1.15.1 charset-normalizer-2.1.1 click-8.1.3 cycler-0.11.0 debugpy-1.6.3 decorator-5.1.1 defusedxml-0.7.1 dnspython-2.2.1 email_validator-1.3.0 entrypoints-0.4 exceptiongroup-1.0.0rc9 fastapi-0.78.0 fastcore-1.3.21 fastjsonschema-2.16.2 fastprogress-1.0.3 fastrelease-0.1.17 fastscript-1.0.0 fonttools-4.38.0 ghapi-0.1.22 gitdb-4.0.9 giturlparse-0.10.0 gmail-importer-0.0.5 h11-0.14.0 httptools-0.5.0 idna-3.4 imaplib2-3.6 importlib-metadata-5.0.0 importlib-resources-5.10.0 iniconfig-1.1.1 ipdb-0.13.9 ipykernel-6.16.2 ipython-7.34.0 ipython-genutils-0.2.0 ipywidgets-8.0.2 itsdangerous-2.1.2 jedi-0.18.1 jinja2-3.0.0 jsonschema-4.16.0 jupyter-1.0.0 jupyter-client-6.1.12 jupyter-console-6.4.2 jupyter-core-4.11.2 jupyter-server-1.15.6 jupyterlab-widgets-3.0.3 kiwisolver-1.4.4 matplotlib-3.5.3 matplotlib-inline-0.1.6 mistune-0.8.4 nbclassic-0.4.5 nbconvert-5.6.1 nbdev-1.1.21 nbformat-5.7.0 nest-asyncio-1.5.6 notebook-6.5.1 notebook-shim-0.2.0 numpy-1.21.6 opencv-python-4.6.0.66 orjson-3.8.1 packaging-21.3 pandas-1.3.5 pandocfilters-1.5.0 parso-0.8.3 pexpect-4.8.0 pickleshare-0.7.5 pillow-8.4.0 pkgutil-resolve-name-1.3.10 pluggy-1.0.0 prometheus-client-0.15.0 prompt-toolkit-3.0.31 psutil-5.9.3 ptyprocess-0.7.0 pycparser-2.21 pydantic-1.10.2 pygments-2.13.0 pymemri-0.0.24 pyparsing-3.0.9 pyrsistent-0.18.1 pytest-7.2.0 python-dateutil-2.8.2 python-dotenv-0.21.0 python-multipart-0.0.5 pytz-2022.5 pyyaml-6.0 pyzmq-24.0.1 qtconsole-5.3.2 qtpy-2.2.1 requests-2.28.1 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 terminado-0.17.0 testpath-0.6.0 toml-0.10.2 tomli-2.0.1 tornado-6.2 tqdm-4.64.1 traitlets-5.5.0 typing-extensions-4.4.0 ujson-5.5.0 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.17.0 watchgod-0.8.2 wcwidth-0.2.5 webencodings-0.5.1 websocket-client-1.4.1 websockets-10.4 widgetsnbextension-4.0.3 zipp-3.10.0
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.3 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0{"build_profile":null,"cargo":"0.4.4","git_describe":null}
100    58  100    58    0     0  11600      0 --:--:-- --:--:-- --:--:-- 11600
[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pytest[0;m
============================= test session starts ==============================
platform linux -- Python 3.7.15, pytest-7.2.0, pluggy-1.0.0
rootdir: /builds/memri/plugins/gmail
plugins: anyio-3.6.2
collected 1 item

tests/test_gmail_importer.py .                                           [100%]

=============================== warnings summary ===============================
../../../../usr/local/lib/python3.7/site-packages/nbconvert/filters/strings.py:22
  /usr/local/lib/python3.7/site-packages/nbconvert/filters/strings.py:22: DeprecationWarning: defusedxml.cElementTree is deprecated, import from defusedxml.ElementTree instead.
    from defusedxml import cElementTree as ElementTree

../../../../usr/local/lib/python3.7/site-packages/nbconvert/exporters/html.py:76
  /usr/local/lib/python3.7/site-packages/nbconvert/exporters/html.py:76: DeprecationWarning: 'contextfilter' is renamed to 'pass_context', the old name will be removed in Jinja 3.1.
    @contextfilter

gmail_importer/imap_client.py:57
  /builds/memri/plugins/gmail/gmail_importer/imap_client.py:57: DeprecationWarning: invalid escape sequence \(
    attributes = re.search("\(([^)]+)\)", mailbox_str)[0][1:-1]

tests/test_gmail_importer.py::test_emails_imported
  /usr/local/lib/python3.7/site-packages/pymemri/plugin/pluginbase.py:55: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    RuntimeWarning)

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
======================== 1 passed, 4 warnings in 5.07s =========================
section_end:1666829154:step_script
[0Ksection_start:1666829154:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1666829155:cleanup_file_variables
[0K[32;1mJob succeeded[0;m'''
