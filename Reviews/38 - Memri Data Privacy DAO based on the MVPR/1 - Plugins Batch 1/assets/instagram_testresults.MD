[0KRunning with gitlab-runner 14.9.1 (bd40e3da)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1663321401:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.7 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...[0;m
[0KUsing docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...[0;m
[0KWaiting for services to be up and running...[0;m
[0KPulling docker image python:3.7 ...[0;m
[0KUsing docker image sha256:7d2ecbd72983ae5e5926ef92c94284c4a1391d7744badc6a8e9d5245b04030b7 for python:3.7 with digest python@sha256:2341ac5eedd71f1e6481afe854af572f5ec1b78fa3aea2293dba65942108e663 ...[0;m
section_end:1663321405:prepare_executor
[0Ksection_start:1663321405:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-134-concurrent-0 via 8e6b65718045...
section_end:1663321405:prepare_script
[0Ksection_start:1663321405:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 50...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/instagram/.git/
[32;1mChecking out 76578372 as dev...[0;m

[32;1mSkipping Git submodules setup[0;m
section_end:1663321406:get_sources
[0Ksection_start:1663321406:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:7d2ecbd72983ae5e5926ef92c94284c4a1391d7744badc6a8e9d5245b04030b7 for python:3.7 with digest python@sha256:2341ac5eedd71f1e6481afe854af572f5ec1b78fa3aea2293dba65942108e663 ...[0;m
[32;1m$ apt-get update && apt-get install -y libsqlcipher-dev && apt-get install -y libgl1-mesa-glx[0;m
Get:1 http://deb.debian.org/debian bullseye InRelease [116 kB]
Get:2 http://deb.debian.org/debian-security bullseye-security InRelease [48.4 kB]
Get:3 http://deb.debian.org/debian bullseye-updates InRelease [44.1 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 Packages [8184 kB]
Get:5 http://deb.debian.org/debian-security bullseye-security/main amd64 Packages [183 kB]
Get:6 http://deb.debian.org/debian bullseye-updates/main amd64 Packages [2596 B]
Fetched 8578 kB in 1s (6096 kB/s)
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
Fetched 998 kB in 0s (40.1 MB/s)
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
Processing triggers for libc-bin (2.31-13+deb11u4) ...
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
Fetched 40.6 MB in 0s (147 MB/s)
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
Processing triggers for libc-bin (2.31-13+deb11u4) ...
[32;1m$ pip install -e .[0;m
Obtaining file:///builds/memri/plugins/instagram
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.25
  Cloning https://gitlab.memri.io/memri/pymemri.git (to revision v0.0.25) to /tmp/pip-install-0oif7e41/pymemri_94768eff611440c694451e27420c03b0
  Running command git clone --filter=blob:none --quiet https://gitlab.memri.io/memri/pymemri.git /tmp/pip-install-0oif7e41/pymemri_94768eff611440c694451e27420c03b0
  Running command git checkout -q 8697a4f00de76180df2128315e62cc2c72e2405b
  Resolved https://gitlab.memri.io/memri/pymemri.git to commit 8697a4f00de76180df2128315e62cc2c72e2405b
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting instaloader==4.9.2
  Downloading instaloader-4.9.2.tar.gz (60 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.2/60.2 KB 12.8 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pytest
  Downloading pytest-7.1.3-py3-none-any.whl (298 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 298.2/298.2 KB 46.4 MB/s eta 0:00:00
Collecting requests>=2.4
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 14.3 MB/s eta 0:00:00
Collecting tqdm
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 KB 14.8 MB/s eta 0:00:00
Collecting ipdb
  Downloading ipdb-0.13.9.tar.gz (16 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 10.9 MB/s eta 0:00:00
Collecting nbdev==1.1.21
  Downloading nbdev-1.1.21-py3-none-any.whl (46 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 46.9/46.9 KB 10.6 MB/s eta 0:00:00
Collecting matplotlib
  Downloading matplotlib-3.5.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (11.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.2/11.2 MB 82.5 MB/s eta 0:00:00
Collecting jupyter-client==6.1.12
  Downloading jupyter_client-6.1.12-py3-none-any.whl (112 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 112.7/112.7 KB 23.3 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 12.7 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting pandas
  Downloading pandas-1.3.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.3/11.3 MB 82.4 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 82.5 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 33.9 MB/s eta 0:00:00
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 32.7 MB/s eta 0:00:00
Collecting pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
  Downloading pydantic-1.10.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.8/11.8 MB 78.2 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 13.7 MB/s eta 0:00:00
Collecting pyyaml<7.0.0,>=5.3.1
  Downloading PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (596 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 596.3/596.3 KB 62.3 MB/s eta 0:00:00
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.0-cp37-cp37m-manylinux_2_28_x86_64.whl (145 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 145.9/145.9 KB 30.4 MB/s eta 0:00:00
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.5.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (45 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 45.9/45.9 KB 11.4 MB/s eta 0:00:00
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 13.8 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.2.1-py2.py3-none-any.whl (22 kB)
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Requirement already satisfied: pip in /usr/local/lib/python3.7/site-packages (from fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.25->instagram==0.0.7) (22.0.4)
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 KB 10.3 MB/s eta 0:00:00
Collecting typing-extensions>=3.7.4.3
  Downloading typing_extensions-4.3.0-py3-none-any.whl (25 kB)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 KB 16.2 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting pyzmq>=13
  Downloading pyzmq-24.0.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 77.4 MB/s eta 0:00:00
Collecting tornado>=4.1
  Downloading tornado-6.2-cp37-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (423 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 424.0/424.0 KB 57.3 MB/s eta 0:00:00
Collecting traitlets
  Downloading traitlets-5.4.0-py3-none-any.whl (107 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 107.1/107.1 KB 25.5 MB/s eta 0:00:00
Collecting python-dateutil>=2.1
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 KB 43.2 MB/s eta 0:00:00
Collecting jupyter-core>=4.6.0
  Downloading jupyter_core-4.11.1-py3-none-any.whl (88 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 88.4/88.4 KB 21.8 MB/s eta 0:00:00
Collecting nbconvert<6
  Downloading nbconvert-5.6.1-py2.py3-none-any.whl (455 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 455.1/455.1 KB 56.8 MB/s eta 0:00:00
Collecting nbformat>=4.4.0
  Downloading nbformat-5.5.0-py3-none-any.whl (75 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 75.3/75.3 KB 18.5 MB/s eta 0:00:00
Collecting ipykernel
  Downloading ipykernel-6.15.3-py3-none-any.whl (138 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 138.3/138.3 KB 36.1 MB/s eta 0:00:00
Collecting fastrelease
  Downloading fastrelease-0.1.17-py3-none-any.whl (13 kB)
Collecting ghapi
  Downloading ghapi-1.0.3-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.1/58.1 KB 10.6 MB/s eta 0:00:00
Collecting jupyter
  Downloading jupyter-1.0.0-py2.py3-none-any.whl (2.7 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.1-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 23.8 MB/s eta 0:00:00
Collecting importlib-metadata>=0.12
  Downloading importlib_metadata-4.12.0-py3-none-any.whl (21 kB)
Collecting py>=1.8.2
  Downloading py-1.11.0-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.7/98.7 KB 27.1 MB/s eta 0:00:00
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 KB 13.9 MB/s eta 0:00:00
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting zipp>=0.5
  Downloading zipp-3.8.1-py3-none-any.whl (5.6 kB)
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 KB 32.6 MB/s eta 0:00:00
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting certifi>=2017.4.17
  Downloading certifi-2022.9.14-py3-none-any.whl (162 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 162.5/162.5 KB 36.6 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 15.0 MB/s eta 0:00:00
Requirement already satisfied: setuptools in /usr/local/lib/python3.7/site-packages (from ipdb->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.25->instagram==0.0.7) (57.5.0)
Collecting ipython>=7.17.0
  Downloading ipython-7.34.0-py3-none-any.whl (793 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 793.8/793.8 KB 65.9 MB/s eta 0:00:00
Collecting toml>=0.10.2
  Downloading toml-0.10.2-py2.py3-none-any.whl (16 kB)
Collecting decorator
  Downloading decorator-5.1.1-py3-none-any.whl (9.1 kB)
Collecting kiwisolver>=1.0.1
  Downloading kiwisolver-1.4.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 78.2 MB/s eta 0:00:00
Collecting cycler>=0.10
  Downloading cycler-0.11.0-py3-none-any.whl (6.4 kB)
Collecting pyparsing>=2.2.1
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 19.6 MB/s eta 0:00:00
Collecting fonttools>=4.22.0
  Downloading fonttools-4.37.2-py3-none-any.whl (959 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 959.8/959.8 KB 61.9 MB/s eta 0:00:00
Collecting numpy>=1.17
  Downloading numpy-1.21.6-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (15.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 15.7/15.7 MB 69.9 MB/s eta 0:00:00
Collecting pytz>=2017.3
  Downloading pytz-2022.2.1-py2.py3-none-any.whl (500 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 500.6/500.6 KB 61.1 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 KB 44.0 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting matplotlib-inline
  Downloading matplotlib_inline-0.1.6-py3-none-any.whl (9.4 kB)
Collecting pygments
  Downloading Pygments-2.13.0-py3-none-any.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 70.1 MB/s eta 0:00:00
Collecting backcall
  Downloading backcall-0.2.0-py2.py3-none-any.whl (11 kB)
Collecting pexpect>4.3
  Downloading pexpect-4.8.0-py2.py3-none-any.whl (59 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 59.0/59.0 KB 13.6 MB/s eta 0:00:00
Collecting jedi>=0.16
  Downloading jedi-0.18.1-py2.py3-none-any.whl (1.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.6/1.6 MB 80.0 MB/s eta 0:00:00
Collecting prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0
  Downloading prompt_toolkit-3.0.31-py3-none-any.whl (382 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 382.3/382.3 KB 49.1 MB/s eta 0:00:00
Collecting pickleshare
  Downloading pickleshare-0.7.5-py2.py3-none-any.whl (6.9 kB)
Collecting defusedxml
  Downloading defusedxml-0.7.1-py2.py3-none-any.whl (25 kB)
Collecting pandocfilters>=1.4.1
  Downloading pandocfilters-1.5.0-py2.py3-none-any.whl (8.7 kB)
Collecting entrypoints>=0.2.2
  Downloading entrypoints-0.4-py3-none-any.whl (5.3 kB)
Collecting testpath
  Downloading testpath-0.6.0-py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.9/83.9 KB 18.9 MB/s eta 0:00:00
Collecting mistune<2,>=0.8.1
  Downloading mistune-0.8.4-py2.py3-none-any.whl (16 kB)
Collecting bleach
  Downloading bleach-5.0.1-py3-none-any.whl (160 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 160.9/160.9 KB 32.0 MB/s eta 0:00:00
Collecting fastjsonschema
  Downloading fastjsonschema-2.16.1-py3-none-any.whl (22 kB)
Collecting jsonschema>=2.6
  Downloading jsonschema-4.16.0-py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.1/83.1 KB 20.4 MB/s eta 0:00:00
Collecting six>=1.5
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting h11>=0.8
  Downloading h11-0.13.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.2/58.2 KB 17.1 MB/s eta 0:00:00
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 25.4 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting websockets>=10.0
  Downloading websockets-10.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (112 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 112.1/112.1 KB 28.8 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (404 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 404.7/404.7 KB 55.0 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 88.8 MB/s eta 0:00:00
Collecting ghapi
  Downloading ghapi-1.0.2-py3-none-any.whl (57 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 57.7/57.7 KB 13.9 MB/s eta 0:00:00
  Downloading ghapi-1.0.1-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.5/58.5 KB 16.9 MB/s eta 0:00:00
  Downloading ghapi-1.0.0-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 13.6 MB/s eta 0:00:00
  Downloading ghapi-0.1.23-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 15.1 MB/s eta 0:00:00
  Downloading ghapi-0.1.22-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 12.5 MB/s eta 0:00:00
Collecting nest-asyncio
  Downloading nest_asyncio-1.5.5-py3-none-any.whl (5.2 kB)
Collecting debugpy>=1.0
  Downloading debugpy-1.6.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (1.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.8/1.8 MB 46.3 MB/s eta 0:00:00
Collecting psutil
  Downloading psutil-5.9.2-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (281 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 281.3/281.3 KB 51.1 MB/s eta 0:00:00
Collecting qtconsole
  Downloading qtconsole-5.3.2-py3-none-any.whl (120 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.8/120.8 KB 31.6 MB/s eta 0:00:00
Collecting ipywidgets
  Downloading ipywidgets-8.0.2-py3-none-any.whl (134 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 134.4/134.4 KB 30.0 MB/s eta 0:00:00
Collecting jupyter-console
  Downloading jupyter_console-6.4.4-py3-none-any.whl (22 kB)
Collecting notebook
  Downloading notebook-6.4.12-py3-none-any.whl (9.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.9/9.9 MB 86.7 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Collecting parso<0.9.0,>=0.8.0
  Downloading parso-0.8.3-py2.py3-none-any.whl (100 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.8/100.8 KB 28.2 MB/s eta 0:00:00
Collecting pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0
  Downloading pyrsistent-0.18.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (117 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 117.1/117.1 KB 27.3 MB/s eta 0:00:00
Collecting importlib-resources>=1.4.0
  Downloading importlib_resources-5.9.0-py3-none-any.whl (33 kB)
Collecting pkgutil-resolve-name>=1.3.10
  Downloading pkgutil_resolve_name-1.3.10-py3-none-any.whl (4.7 kB)
Collecting ptyprocess>=0.5
  Downloading ptyprocess-0.7.0-py2.py3-none-any.whl (13 kB)
Collecting wcwidth
  Downloading wcwidth-0.2.5-py2.py3-none-any.whl (30 kB)
Collecting webencodings
  Downloading webencodings-0.5.1-py2.py3-none-any.whl (11 kB)
Collecting widgetsnbextension~=4.0
  Downloading widgetsnbextension-4.0.3-py3-none-any.whl (2.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.0/2.0 MB 83.2 MB/s eta 0:00:00
Collecting jupyterlab-widgets~=3.0
  Downloading jupyterlab_widgets-3.0.3-py3-none-any.whl (384 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 384.1/384.1 KB 39.8 MB/s eta 0:00:00
Collecting jupyter-console
  Downloading jupyter_console-6.4.3-py3-none-any.whl (22 kB)
  Downloading jupyter_console-6.4.2-py3-none-any.whl (23 kB)
Collecting terminado>=0.8.3
  Downloading terminado-0.15.0-py3-none-any.whl (16 kB)
Collecting argon2-cffi
  Downloading argon2_cffi-21.3.0-py3-none-any.whl (14 kB)
Collecting prometheus-client
  Downloading prometheus_client-0.14.1-py3-none-any.whl (59 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 59.5/59.5 KB 14.4 MB/s eta 0:00:00
Collecting ipython-genutils
  Downloading ipython_genutils-0.2.0-py2.py3-none-any.whl (26 kB)
Collecting Send2Trash>=1.8.0
  Downloading Send2Trash-1.8.0-py3-none-any.whl (18 kB)
Collecting qtpy>=2.0.1
  Downloading QtPy-2.2.0-py3-none-any.whl (82 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 82.3/82.3 KB 21.8 MB/s eta 0:00:00
Collecting argon2-cffi-bindings
  Downloading argon2_cffi_bindings-21.2.0-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (86 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 86.2/86.2 KB 21.3 MB/s eta 0:00:00
Collecting cffi>=1.0.1
  Downloading cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (427 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 427.9/427.9 KB 48.5 MB/s eta 0:00:00
Collecting pycparser
  Downloading pycparser-2.21-py2.py3-none-any.whl (118 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 118.7/118.7 KB 27.7 MB/s eta 0:00:00
Building wheels for collected packages: instaloader, pymemri, ipdb, python-multipart
  Building wheel for instaloader (setup.py): started
  Building wheel for instaloader (setup.py): finished with status 'done'
  Created wheel for instaloader: filename=instaloader-4.9.2-py3-none-any.whl size=62014 sha256=4de3ded2c0a7ef4edff4f07be59409252706917fbd407e9fcc043d9b735072a8
  Stored in directory: /root/.cache/pip/wheels/45/60/8f/9fc4a34847bae5413c4c37ed84e7ff49328e85e24edd17a62c
  Building wheel for pymemri (setup.py): started
  Building wheel for pymemri (setup.py): finished with status 'done'
  Created wheel for pymemri: filename=pymemri-0.0.24-py3-none-any.whl size=75607 sha256=a9552a991074964045ae9613443e0bcc4d8d990711a1d98c420b12311ba40690
  Stored in directory: /tmp/pip-ephem-wheel-cache-gvsxarld/wheels/47/d0/7c/4f7eab4f00388073f15d02761f51bce8274d28380e6134f1ae
  Building wheel for ipdb (setup.py): started
  Building wheel for ipdb (setup.py): finished with status 'done'
  Created wheel for ipdb: filename=ipdb-0.13.9-py3-none-any.whl size=11648 sha256=dba337ab8a9b4d8b8749829cf2b3bb1fca3a645890401de4a40844283f8f586f
  Stored in directory: /root/.cache/pip/wheels/65/cd/cc/aaf92acae337a28fdd2aa4d632196a59745c8c39f76eaeed01
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=b7652babb1e9e1b21ee42c9ab8f37f107fedd3c8b0fe744a2ab6ba853f51de9b
  Stored in directory: /root/.cache/pip/wheels/2c/41/7c/bfd1c180534ffdcc0972f78c5758f89881602175d48a8bcd2c
Successfully built instaloader pymemri ipdb python-multipart
Installing collected packages: webencodings, wcwidth, Send2Trash, pytz, ptyprocess, pickleshare, mistune, ipython-genutils, iniconfig, fastjsonschema, backcall, zipp, widgetsnbextension, websockets, uvloop, urllib3, ujson, typing-extensions, traitlets, tqdm, tornado, tomli, toml, testpath, sniffio, smmap, six, pyzmq, pyyaml, python-dotenv, pyrsistent, pyparsing, pygments, pycparser, py, psutil, prompt-toolkit, prometheus-client, pkgutil-resolve-name, pillow, pexpect, parso, pandocfilters, orjson, numpy, nest-asyncio, MarkupSafe, jupyterlab-widgets, itsdangerous, idna, httptools, giturlparse, fonttools, fastprogress, entrypoints, dnspython, defusedxml, decorator, debugpy, cycler, charset-normalizer, certifi, attrs, terminado, requests, python-multipart, python-dateutil, pydantic, packaging, matplotlib-inline, kiwisolver, jupyter-core, jinja2, jedi, importlib-resources, importlib-metadata, h11, gitdb, email_validator, cffi, bleach, asgiref, anyio, watchgod, starlette, qtpy, pluggy, pandas, matplotlib, jupyter-client, jsonschema, ipython, instaloader, GitPython, fastscript, fastcore, click, argon2-cffi-bindings, uvicorn, pytest, nbformat, ipykernel, ipdb, ghapi, fastapi, argon2-cffi, qtconsole, nbconvert, jupyter-console, ipywidgets, fastrelease, notebook, jupyter, nbdev, pymemri, instagram
  Running setup.py develop for instagram
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.1 Send2Trash-1.8.0 anyio-3.6.1 argon2-cffi-21.3.0 argon2-cffi-bindings-21.2.0 asgiref-3.5.2 attrs-22.1.0 backcall-0.2.0 bleach-5.0.1 certifi-2022.9.14 cffi-1.15.1 charset-normalizer-2.1.1 click-8.1.3 cycler-0.11.0 debugpy-1.6.3 decorator-5.1.1 defusedxml-0.7.1 dnspython-2.2.1 email_validator-1.2.1 entrypoints-0.4 fastapi-0.78.0 fastcore-1.3.21 fastjsonschema-2.16.1 fastprogress-1.0.3 fastrelease-0.1.17 fastscript-1.0.0 fonttools-4.37.2 ghapi-0.1.22 gitdb-4.0.9 giturlparse-0.10.0 h11-0.13.0 httptools-0.5.0 idna-3.4 importlib-metadata-4.12.0 importlib-resources-5.9.0 iniconfig-1.1.1 instagram-0.0.7 instaloader-4.9.2 ipdb-0.13.9 ipykernel-6.15.3 ipython-7.34.0 ipython-genutils-0.2.0 ipywidgets-8.0.2 itsdangerous-2.1.2 jedi-0.18.1 jinja2-3.0.0 jsonschema-4.16.0 jupyter-1.0.0 jupyter-client-6.1.12 jupyter-console-6.4.2 jupyter-core-4.11.1 jupyterlab-widgets-3.0.3 kiwisolver-1.4.4 matplotlib-3.5.3 matplotlib-inline-0.1.6 mistune-0.8.4 nbconvert-5.6.1 nbdev-1.1.21 nbformat-5.5.0 nest-asyncio-1.5.5 notebook-6.4.12 numpy-1.21.6 orjson-3.8.0 packaging-21.3 pandas-1.3.5 pandocfilters-1.5.0 parso-0.8.3 pexpect-4.8.0 pickleshare-0.7.5 pillow-8.4.0 pkgutil-resolve-name-1.3.10 pluggy-1.0.0 prometheus-client-0.14.1 prompt-toolkit-3.0.31 psutil-5.9.2 ptyprocess-0.7.0 py-1.11.0 pycparser-2.21 pydantic-1.10.2 pygments-2.13.0 pymemri-0.0.24 pyparsing-3.0.9 pyrsistent-0.18.1 pytest-7.1.3 python-dateutil-2.8.2 python-dotenv-0.21.0 python-multipart-0.0.5 pytz-2022.2.1 pyyaml-6.0 pyzmq-24.0.0 qtconsole-5.3.2 qtpy-2.2.0 requests-2.28.1 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 terminado-0.15.0 testpath-0.6.0 toml-0.10.2 tomli-2.0.1 tornado-6.2 tqdm-4.64.1 traitlets-5.4.0 typing-extensions-4.3.0 ujson-5.5.0 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.17.0 watchgod-0.8.2 wcwidth-0.2.5 webencodings-0.5.1 websockets-10.3 widgetsnbextension-4.0.3 zipp-3.8.1
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.2.2 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100    58  100    58    0     0  58000      0 --:--:-- --:--:-- --:--:-- 58000
{"build_profile":null,"cargo":"0.4.4","git_describe":null}[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pytest[0;m
============================= test session starts ==============================
platform linux -- Python 3.7.14, pytest-7.1.3, pluggy-1.0.0
rootdir: /builds/memri/plugins/instagram
plugins: anyio-3.6.1
collected 1 item

tests/test_login.py .                                                    [100%]

=============================== warnings summary ===============================
tests/test_login.py::test_login
  /usr/local/lib/python3.7/site-packages/pymemri/plugin/pluginbase.py:55: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    RuntimeWarning)

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
========================= 1 passed, 1 warning in 2.21s =========================
section_end:1663321467:step_script
[0Ksection_start:1663321467:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1663321467:cleanup_file_variables
[0K[32;1mJob succeeded[0;m