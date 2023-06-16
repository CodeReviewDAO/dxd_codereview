```
[0KRunning with gitlab-runner 15.10.1 (dcfb4b66)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY, system ID: r_dW1UqOXgbibd[0;m
section_start:1682102675:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.9 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...[0;m
[0KUsing docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...[0;m
[0KWaiting for services to be up and running (timeout 30 seconds)...[0;m
[0KPulling docker image python:3.9 ...[0;m
[0KUsing docker image sha256:2202efa5d0ba3a90c3217c1499b2cd42b22cdc6cd7b447947f874939ae4d11bc for python:3.9 with digest python@sha256:2d8875d28ca023a9056a828518adcdd634ba03740e1e3b197c06eb4527c6152c ...[0;m
section_end:1682102678:prepare_executor
[0Ksection_start:1682102678:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-705-concurrent-0 via eb1c4665fc9b...
section_end:1682102679:prepare_script
[0Ksection_start:1682102679:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 20...[0;m
Initialized empty Git repository in /builds/memri/plugins/google-photos/.git/
[32;1mCreated fresh repository.[0;m
[32;1mChecking out 0b16a3ed as detached HEAD (ref is v0.2)...[0;m

[32;1mSkipping Git submodules setup[0;m
section_end:1682102680:get_sources
[0Ksection_start:1682102680:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:2202efa5d0ba3a90c3217c1499b2cd42b22cdc6cd7b447947f874939ae4d11bc for python:3.9 with digest python@sha256:2d8875d28ca023a9056a828518adcdd634ba03740e1e3b197c06eb4527c6152c ...[0;m
[32;1m$ apt-get update && apt-get install -y libsqlcipher-dev && apt-get install -y libgl1-mesa-glx[0;m
Get:1 http://deb.debian.org/debian bullseye InRelease [116 kB]
Get:2 http://deb.debian.org/debian-security bullseye-security InRelease [48.4 kB]
Get:3 http://deb.debian.org/debian bullseye-updates InRelease [44.1 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 Packages [8183 kB]
Get:5 http://deb.debian.org/debian-security bullseye-security/main amd64 Packages [237 kB]
Get:6 http://deb.debian.org/debian bullseye-updates/main amd64 Packages [14.6 kB]
Fetched 8643 kB in 1s (6891 kB/s)
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
0 upgraded, 2 newly installed, 0 to remove and 2 not upgraded.
Need to get 998 kB of archives.
After this operation, 2809 kB of additional disk space will be used.
Get:1 http://deb.debian.org/debian bullseye/main amd64 libsqlcipher0 amd64 3.4.1-2 [433 kB]
Get:2 http://deb.debian.org/debian bullseye/main amd64 libsqlcipher-dev amd64 3.4.1-2 [565 kB]
debconf: delaying package configuration, since apt-utils is not installed
Fetched 998 kB in 0s (42.7 MB/s)
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
(Reading database ... 23426 files and directories currently installed.)
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
0 upgraded, 33 newly installed, 0 to remove and 2 not upgraded.
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
Fetched 40.6 MB in 0s (144 MB/s)
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
(Reading database ... 23444 files and directories currently installed.)
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
Obtaining file:///builds/memri/plugins/google-photos
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri@ git+https://gitlab.memri.io/memri/pymemri@dev
  Cloning https://gitlab.memri.io/memri/pymemri (to revision dev) to /tmp/pip-install-aqj36wzw/pymemri_988ff829ebbb4b3bbd97800011c7a232
  Running command git clone --filter=blob:none --quiet https://gitlab.memri.io/memri/pymemri /tmp/pip-install-aqj36wzw/pymemri_988ff829ebbb4b3bbd97800011c7a232
  warning: redirecting to https://gitlab.memri.io/memri/pymemri.git/
  Resolved https://gitlab.memri.io/memri/pymemri to commit eebc605bd25efa2f753482e333de8d0d1078a7c9
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pytest>=6.2.4
  Downloading pytest-7.3.1-py3-none-any.whl (320 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 320.5/320.5 KB 41.3 MB/s eta 0:00:00
Collecting loguru>=0.6.0
  Downloading loguru-0.7.0-py3-none-any.whl (59 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.0/60.0 KB 14.6 MB/s eta 0:00:00
Collecting requests
  Downloading requests-2.28.2-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 14.4 MB/s eta 0:00:00
Collecting google-auth-oauthlib
  Downloading google_auth_oauthlib-1.0.0-py2.py3-none-any.whl (18 kB)
Collecting google-api-python-client
  Downloading google_api_python_client-2.86.0-py2.py3-none-any.whl (11.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.3/11.3 MB 98.0 MB/s eta 0:00:00
Collecting iniconfig
  Downloading iniconfig-2.0.0-py3-none-any.whl (5.9 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting packaging
  Downloading packaging-23.1-py3-none-any.whl (48 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 48.9/48.9 KB 10.0 MB/s eta 0:00:00
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.1.1-py3-none-any.whl (14 kB)
Collecting uritemplate<5,>=3.0.1
  Downloading uritemplate-4.1.1-py2.py3-none-any.whl (10 kB)
Collecting google-auth<3.0.0dev,>=1.19.0
  Downloading google_auth-2.17.3-py2.py3-none-any.whl (178 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 178.2/178.2 KB 29.5 MB/s eta 0:00:00
Collecting httplib2<1dev,>=0.15.0
  Downloading httplib2-0.22.0-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.9/96.9 KB 24.5 MB/s eta 0:00:00
Collecting google-auth-httplib2>=0.1.0
  Downloading google_auth_httplib2-0.1.0-py2.py3-none-any.whl (9.3 kB)
Collecting google-api-core!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0,<3.0.0dev,>=1.31.5
  Downloading google_api_core-2.11.0-py3-none-any.whl (120 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.3/120.3 KB 21.5 MB/s eta 0:00:00
Collecting requests-oauthlib>=0.7.0
  Downloading requests_oauthlib-1.3.1-py2.py3-none-any.whl (23 kB)
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 13.8 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 14.9 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 90.2 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 42.3 MB/s eta 0:00:00
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 25.4 MB/s eta 0:00:00
Collecting loguru>=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 11.8 MB/s eta 0:00:00
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 13.2/13.2 MB 84.1 MB/s eta 0:00:00
Collecting numpy
  Downloading numpy-1.24.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 17.3/17.3 MB 83.5 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 13.7 MB/s eta 0:00:00
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.10-cp39-cp39-manylinux_2_28_x86_64.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.5/140.5 KB 32.8 MB/s eta 0:00:00
Collecting pyyaml<7.0.0,>=5.3.1
  Downloading PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (661 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 661.8/661.8 KB 57.9 MB/s eta 0:00:00
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 12.8 MB/s eta 0:00:00
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (52 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 52.8/52.8 KB 3.3 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.1-py2.py3-none-any.whl (22 kB)
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Requirement already satisfied: pip in /usr/local/lib/python3.9/site-packages (from fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri@dev->google-photos==0.1.4) (22.0.4)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.10-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.7/62.7 KB 14.5 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting typing-extensions>=4.1.0
  Downloading typing_extensions-4.5.0-py3-none-any.whl (27 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 18.0 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.15-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.9/140.9 KB 34.1 MB/s eta 0:00:00
Collecting charset-normalizer<4,>=2
  Downloading charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (199 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 199.2/199.2 KB 42.0 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 14.2 MB/s eta 0:00:00
Collecting certifi>=2017.4.17
  Downloading certifi-2022.12.7-py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 KB 32.0 MB/s eta 0:00:00
Collecting protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
  Downloading protobuf-4.22.3-cp37-abi3-manylinux2014_x86_64.whl (302 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 302.4/302.4 KB 49.1 MB/s eta 0:00:00
Collecting googleapis-common-protos<2.0dev,>=1.56.2
  Downloading googleapis_common_protos-1.59.0-py2.py3-none-any.whl (223 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 223.6/223.6 KB 47.7 MB/s eta 0:00:00
Collecting six>=1.9.0
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting cachetools<6.0,>=2.0.0
  Downloading cachetools-5.3.0-py3-none-any.whl (9.3 kB)
Collecting pyasn1-modules>=0.2.1
  Downloading pyasn1_modules-0.3.0-py2.py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.3/181.3 KB 13.1 MB/s eta 0:00:00
Collecting rsa<5,>=3.1.4
  Downloading rsa-4.9-py3-none-any.whl (34 kB)
Collecting pyparsing!=3.0.0,!=3.0.1,!=3.0.2,!=3.0.3,<4,>=2.4.2
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 25.6 MB/s eta 0:00:00
Collecting oauthlib>=3.0.0
  Downloading oauthlib-3.2.2-py3-none-any.whl (151 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 151.7/151.7 KB 26.0 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.3.0-py3-none-any.whl (283 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 283.7/283.7 KB 40.7 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting pyasn1<0.6.0,>=0.4.6
  Downloading pyasn1-0.5.0-py2.py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.9/83.9 KB 19.7 MB/s eta 0:00:00
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 14.5 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.6.0-py3-none-any.whl (23 kB)
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 25.5 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (417 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 417.9/417.9 KB 33.8 MB/s eta 0:00:00
Collecting websockets>=10.0
  Downloading websockets-11.0.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (129 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 129.7/129.7 KB 23.7 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-1.0.0-py3-none-any.whl (19 kB)
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 71.1 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Building wheels for collected packages: pymemri, python-multipart
  Building wheel for pymemri (setup.py): started
  Building wheel for pymemri (setup.py): finished with status 'done'
  Created wheel for pymemri: filename=pymemri-0.0.46-py3-none-any.whl size=70351 sha256=333420d4ffb608d5f105cf73354602a58ef53fd288dbb0dbedbe7dd2712c2bf0
  Stored in directory: /tmp/pip-ephem-wheel-cache-z1e_gbtd/wheels/4e/0c/ff/a548eed7b13bc328af0f49dc28bd1e35ce4a72092ba4ef42f2
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31677 sha256=872b23e8830f177f50efd2eb3e127dfe6ec97964084e6dcb532545d20afb3a17
  Stored in directory: /root/.cache/pip/wheels/fe/04/d1/a10661cc45f03c3cecda50deb2d2c22f57b4e84a75b2a5987e
Successfully built pymemri python-multipart
Installing collected packages: websockets, uvloop, urllib3, uritemplate, ujson, typing-extensions, tomli, sniffio, smmap, six, pyyaml, python-dotenv, pyparsing, pyasn1, protobuf, pluggy, pillow, packaging, orjson, oauthlib, numpy, MarkupSafe, loguru, itsdangerous, iniconfig, idna, httptools, h11, giturlparse, fastprogress, exceptiongroup, dnspython, click, charset-normalizer, certifi, cachetools, asgiref, uvicorn, rsa, requests, python-multipart, pytest, pydantic, pyasn1-modules, jinja2, httplib2, googleapis-common-protos, gitdb, fastscript, fastcore, email_validator, anyio, watchgod, starlette, requests-oauthlib, google-auth, GitPython, google-auth-oauthlib, google-auth-httplib2, google-api-core, fastapi, google-api-python-client, pymemri, google-photos
  Running setup.py develop for google-photos
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.2 anyio-3.6.2 asgiref-3.6.0 cachetools-5.3.0 certifi-2022.12.7 charset-normalizer-3.1.0 click-8.1.3 dnspython-2.3.0 email_validator-1.3.1 exceptiongroup-1.1.1 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 gitdb-4.0.10 giturlparse-0.10.0 google-api-core-2.11.0 google-api-python-client-2.86.0 google-auth-2.17.3 google-auth-httplib2-0.1.0 google-auth-oauthlib-1.0.0 google-photos-0.1.4 googleapis-common-protos-1.59.0 h11-0.14.0 httplib2-0.22.0 httptools-0.5.0 idna-3.4 iniconfig-2.0.0 itsdangerous-2.1.2 jinja2-3.0.0 loguru-0.6.0 numpy-1.24.2 oauthlib-3.2.2 orjson-3.8.10 packaging-23.1 pillow-8.4.0 pluggy-1.0.0 protobuf-4.22.3 pyasn1-0.5.0 pyasn1-modules-0.3.0 pydantic-1.10.2 pymemri-0.0.46 pyparsing-3.0.9 pytest-7.3.1 python-dotenv-1.0.0 python-multipart-0.0.5 pyyaml-6.0 requests-2.28.2 requests-oauthlib-1.3.1 rsa-4.9 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tomli-2.0.1 typing-extensions-4.5.0 ujson-5.7.0 uritemplate-4.1.1 urllib3-1.26.15 uvicorn-0.17.6 uvloop-0.17.0 watchgod-0.8.2 websockets-11.0.2
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 23.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0{"build_profile":null,"cargo":"0.4.4","git_describe":null}
100    58  100    58    0     0  58000      0 --:--:-- --:--:-- --:--:-- 58000
[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pytest[0;m
============================= test session starts ==============================
platform linux -- Python 3.9.16, pytest-7.3.1, pluggy-1.0.0
rootdir: /builds/memri/plugins/google-photos
plugins: anyio-3.6.2
collected 3 items

tests/test_plugin.py ...                                                 [100%]

=============================== warnings summary ===============================
tests/test_plugin.py::TestPlugin::test_user_info
  /usr/local/lib/python3.9/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    warnings.warn(

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
========================= 3 passed, 1 warning in 3.30s =========================
section_end:1682102715:step_script
[0Ksection_start:1682102715:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1682102715:cleanup_file_variables
[0K[32;1mJob succeeded[0;m
```