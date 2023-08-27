```
[0KRunning with gitlab-runner 15.7.1 (6d480948)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1679328881:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.9 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...[0;m
[0KUsing docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...[0;m
[0KWaiting for services to be up and running (timeout 30 seconds)...[0;m
[0KPulling docker image python:3.9 ...[0;m
[0KUsing docker image sha256:5407c5455ab9da6157328d0e6c7bdd114b84cdb13f811bf1fee4c34142802be0 for python:3.9 with digest python@sha256:940ea29f268668b00305e22a93e3cbd0f3b05a221716a134f55a3ad8f88bc09f ...[0;m
section_end:1679328886:prepare_executor
[0Ksection_start:1679328886:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-709-concurrent-1 via cab6f0e97d50...
section_end:1679328888:prepare_script
[0Ksection_start:1679328888:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 20...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/summarization-plugin/.git/
[32;1mChecking out 2a59397b as dev...[0;m
Removing summarization_plugin.egg-info/

[32;1mSkipping Git submodules setup[0;m
section_end:1679328890:get_sources
[0Ksection_start:1679328890:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:5407c5455ab9da6157328d0e6c7bdd114b84cdb13f811bf1fee4c34142802be0 for python:3.9 with digest python@sha256:940ea29f268668b00305e22a93e3cbd0f3b05a221716a134f55a3ad8f88bc09f ...[0;m
[32;1m$ apt-get update && apt-get install -y libsqlcipher-dev && apt-get install -y libgl1-mesa-glx[0;m
Get:1 http://deb.debian.org/debian bullseye InRelease [116 kB]
Get:2 http://deb.debian.org/debian-security bullseye-security InRelease [48.4 kB]
Get:3 http://deb.debian.org/debian bullseye-updates InRelease [44.1 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 Packages [8183 kB]
Get:5 http://deb.debian.org/debian-security bullseye-security/main amd64 Packages [236 kB]
Get:6 http://deb.debian.org/debian bullseye-updates/main amd64 Packages [14.6 kB]
Fetched 8642 kB in 2s (3708 kB/s)
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
0 upgraded, 2 newly installed, 0 to remove and 1 not upgraded.
Need to get 998 kB of archives.
After this operation, 2809 kB of additional disk space will be used.
Get:1 http://deb.debian.org/debian bullseye/main amd64 libsqlcipher0 amd64 3.4.1-2 [433 kB]
Get:2 http://deb.debian.org/debian bullseye/main amd64 libsqlcipher-dev amd64 3.4.1-2 [565 kB]
debconf: delaying package configuration, since apt-utils is not installed
Fetched 998 kB in 0s (23.9 MB/s)
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
(Reading database ... 23423 files and directories currently installed.)
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
0 upgraded, 33 newly installed, 0 to remove and 1 not upgraded.
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
Fetched 40.6 MB in 0s (102 MB/s)
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
(Reading database ... 23441 files and directories currently installed.)
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
[32;1m$ pip install -e .[dev][0;m
Obtaining file:///builds/memri/plugins/summarization-plugin
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Checking if build backend supports build_editable: started
  Checking if build backend supports build_editable: finished with status 'done'
  Getting requirements to build editable: started
  Getting requirements to build editable: finished with status 'done'
  Installing backend dependencies: started
  Installing backend dependencies: finished with status 'done'
  Preparing editable metadata (pyproject.toml): started
  Preparing editable metadata (pyproject.toml): finished with status 'done'
Collecting transformers
  Downloading transformers-4.27.1-py3-none-any.whl (6.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 6.7/6.7 MB 48.8 MB/s eta 0:00:00
Collecting pymemri
  Downloading pymemri-0.0.45-py3-none-any.whl (69 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 69.9/69.9 KB 10.1 MB/s eta 0:00:00
Collecting torch>=2.0.0
  Downloading torch-2.0.0-cp39-cp39-manylinux1_x86_64.whl (619.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 619.9/619.9 MB 2.8 MB/s eta 0:00:00
Collecting summa
  Downloading summa-1.2.0.tar.gz (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.9/54.9 KB 6.0 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pytest
  Downloading pytest-7.2.2-py3-none-any.whl (317 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 317.2/317.2 KB 12.6 MB/s eta 0:00:00
Collecting pre-commit
  Downloading pre_commit-3.2.0-py2.py3-none-any.whl (202 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 202.7/202.7 KB 21.2 MB/s eta 0:00:00
Collecting networkx
  Downloading networkx-3.0-py3-none-any.whl (2.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.0/2.0 MB 50.5 MB/s eta 0:00:00
Collecting typing-extensions
  Downloading typing_extensions-4.5.0-py3-none-any.whl (27 kB)
Collecting nvidia-cublas-cu11==11.10.3.66
  Downloading nvidia_cublas_cu11-11.10.3.66-py3-none-manylinux1_x86_64.whl (317.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 317.1/317.1 MB 4.2 MB/s eta 0:00:00
Collecting nvidia-cuda-nvrtc-cu11==11.7.99
  Downloading nvidia_cuda_nvrtc_cu11-11.7.99-2-py3-none-manylinux1_x86_64.whl (21.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 21.0/21.0 MB 32.0 MB/s eta 0:00:00
Collecting nvidia-cuda-runtime-cu11==11.7.99
  Downloading nvidia_cuda_runtime_cu11-11.7.99-py3-none-manylinux1_x86_64.whl (849 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 849.3/849.3 KB 40.4 MB/s eta 0:00:00
Collecting nvidia-cusparse-cu11==11.7.4.91
  Downloading nvidia_cusparse_cu11-11.7.4.91-py3-none-manylinux1_x86_64.whl (173.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 173.2/173.2 MB 9.4 MB/s eta 0:00:00
Collecting nvidia-nccl-cu11==2.14.3
  Downloading nvidia_nccl_cu11-2.14.3-py3-none-manylinux1_x86_64.whl (177.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 177.1/177.1 MB 9.2 MB/s eta 0:00:00
Collecting triton==2.0.0
  Downloading triton-2.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (63.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 MB 21.5 MB/s eta 0:00:00
Collecting nvidia-cudnn-cu11==8.5.0.96
  Downloading nvidia_cudnn_cu11-8.5.0.96-2-py3-none-manylinux1_x86_64.whl (557.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 557.1/557.1 MB 2.2 MB/s eta 0:00:00
Collecting nvidia-curand-cu11==10.2.10.91
  Downloading nvidia_curand_cu11-10.2.10.91-py3-none-manylinux1_x86_64.whl (54.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 MB 25.1 MB/s eta 0:00:00
Collecting sympy
  Downloading sympy-1.11.1-py3-none-any.whl (6.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 6.5/6.5 MB 34.8 MB/s eta 0:00:00
Collecting jinja2
  Downloading Jinja2-3.1.2-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.1/133.1 KB 19.5 MB/s eta 0:00:00
Collecting nvidia-nvtx-cu11==11.7.91
  Downloading nvidia_nvtx_cu11-11.7.91-py3-none-manylinux1_x86_64.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.6/98.6 KB 14.1 MB/s eta 0:00:00
Collecting nvidia-cufft-cu11==10.9.0.58
  Downloading nvidia_cufft_cu11-10.9.0.58-py3-none-manylinux1_x86_64.whl (168.4 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 168.4/168.4 MB 10.4 MB/s eta 0:00:00
Collecting nvidia-cuda-cupti-cu11==11.7.101
  Downloading nvidia_cuda_cupti_cu11-11.7.101-py3-none-manylinux1_x86_64.whl (11.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.8/11.8 MB 57.7 MB/s eta 0:00:00
Collecting filelock
  Downloading filelock-3.10.0-py3-none-any.whl (9.9 kB)
Collecting nvidia-cusolver-cu11==11.4.0.1
  Downloading nvidia_cusolver_cu11-11.4.0.1-2-py3-none-manylinux1_x86_64.whl (102.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 102.6/102.6 MB 16.2 MB/s eta 0:00:00
Requirement already satisfied: wheel in /usr/local/lib/python3.9/site-packages (from nvidia-cublas-cu11==11.10.3.66->torch>=2.0.0->summarization-plugin==0.0.1) (0.38.4)
Requirement already satisfied: setuptools in /usr/local/lib/python3.9/site-packages (from nvidia-cublas-cu11==11.10.3.66->torch>=2.0.0->summarization-plugin==0.0.1) (58.1.0)
Collecting cmake
  Downloading cmake-3.26.0-py2.py3-none-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (24.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 24.0/24.0 MB 41.2 MB/s eta 0:00:00
Collecting lit
  Downloading lit-16.0.0.tar.gz (144 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 145.0/145.0 KB 14.8 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pyyaml>=5.1
  Downloading PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (661 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 661.8/661.8 KB 34.0 MB/s eta 0:00:00
Collecting cfgv>=2.0.0
  Downloading cfgv-3.3.1-py2.py3-none-any.whl (7.3 kB)
Collecting virtualenv>=20.10.0
  Downloading virtualenv-20.21.0-py3-none-any.whl (8.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.7/8.7 MB 66.4 MB/s eta 0:00:00
Collecting nodeenv>=0.11.1
  Downloading nodeenv-1.7.0-py2.py3-none-any.whl (21 kB)
Collecting identify>=1.0.0
  Downloading identify-2.5.21-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.8/98.8 KB 8.8 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 6.1 MB/s eta 0:00:00
Collecting requests
  Downloading requests-2.28.2-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 7.7 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting numpy
  Downloading numpy-1.24.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 17.3/17.3 MB 51.5 MB/s eta 0:00:00
Collecting loguru~=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 2.7 MB/s eta 0:00:00
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 4.8 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 60.2 MB/s eta 0:00:00
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 13.2/13.2 MB 60.9 MB/s eta 0:00:00
Collecting jinja2
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 18.1 MB/s eta 0:00:00
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 21.2 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 5.9 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.1-py2.py3-none-any.whl (22 kB)
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.7-cp39-cp39-manylinux_2_28_x86_64.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.9/140.9 KB 16.2 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (52 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 52.8/52.8 KB 6.3 MB/s eta 0:00:00
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 6.7 MB/s eta 0:00:00
Collecting packaging
  Downloading packaging-23.0-py3-none-any.whl (42 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 42.7/42.7 KB 4.2 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.9/site-packages (from fastcore==1.3.21->pymemri->summarization-plugin==0.0.1) (22.0.4)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.10-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.7/62.7 KB 7.1 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 9.7 MB/s eta 0:00:00
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting iniconfig
  Downloading iniconfig-2.0.0-py3-none-any.whl (5.9 kB)
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.1.1-py3-none-any.whl (14 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.2.0-py3-none-any.whl (60 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.0/60.0 KB 1.1 MB/s eta 0:00:00
Collecting scipy>=0.19
  Downloading scipy-1.10.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (34.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 34.5/34.5 MB 34.9 MB/s eta 0:00:00
Collecting huggingface-hub<1.0,>=0.11.0
  Downloading huggingface_hub-0.13.3-py3-none-any.whl (199 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 199.8/199.8 KB 24.2 MB/s eta 0:00:00
Collecting regex!=2019.12.17
  Downloading regex-2022.10.31-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (769 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 770.0/770.0 KB 18.5 MB/s eta 0:00:00
Collecting tokenizers!=0.11.3,<0.14,>=0.11.1
  Downloading tokenizers-0.13.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (7.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 7.6/7.6 MB 66.6 MB/s eta 0:00:00
Collecting tqdm>=4.27
  Downloading tqdm-4.65.0-py3-none-any.whl (77 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 77.1/77.1 KB 9.3 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 8.4 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.15-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.9/140.9 KB 16.0 MB/s eta 0:00:00
Collecting charset-normalizer<4,>=2
  Downloading charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (199 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 199.2/199.2 KB 22.6 MB/s eta 0:00:00
Collecting certifi>=2017.4.17
  Downloading certifi-2022.12.7-py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 KB 20.6 MB/s eta 0:00:00
Collecting platformdirs<4,>=2.4
  Downloading platformdirs-3.1.1-py3-none-any.whl (14 kB)
Collecting distlib<1,>=0.3.6
  Downloading distlib-0.3.6-py2.py3-none-any.whl (468 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 468.5/468.5 KB 21.6 MB/s eta 0:00:00
Collecting mpmath>=0.19
  Downloading mpmath-1.3.0-py3-none-any.whl (536 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 536.2/536.2 KB 36.7 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.3.0-py3-none-any.whl (283 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 283.7/283.7 KB 18.3 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting six>=1.4.0
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 8.8 MB/s eta 0:00:00
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 11.6 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.6.0-py3-none-any.whl (23 kB)
Collecting python-dotenv>=0.13
  Downloading python_dotenv-1.0.0-py3-none-any.whl (19 kB)
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 66.0 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting websockets>=10.0
  Downloading websockets-10.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.5/106.5 KB 15.3 MB/s eta 0:00:00
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (417 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 417.9/417.9 KB 30.4 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Building wheels for collected packages: summa, summarization-plugin, python-multipart, lit
  Building wheel for summa (setup.py): started
  Building wheel for summa (setup.py): finished with status 'done'
  Created wheel for summa: filename=summa-1.2.0-py3-none-any.whl size=54410 sha256=2cb0fcd2d31b41d8384c8c7d898d0e1733830eee2f21bf24351b4388c156c531
  Stored in directory: /root/.cache/pip/wheels/ed/2c/5f/a0ccc5955d44d2cea78729f4425e73f818d2629517f7af0f8b
  Building editable for summarization-plugin (pyproject.toml): started
  Building editable for summarization-plugin (pyproject.toml): finished with status 'done'
  Created wheel for summarization-plugin: filename=summarization_plugin-0.0.1-0.editable-py3-none-any.whl size=10893 sha256=b647dc909740b16ef512e525c24bf1c4871c4529f0aafe58b11b1a8d9439d829
  Stored in directory: /tmp/pip-ephem-wheel-cache-4uyp_212/wheels/5c/3e/e2/81f8308b6e0d59d2a9ca3025d608d7de7bf32868e8e9f55bed
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=7c1688d2c792725cef11391f4c8e4e976a20743bc5396bb88f067a321cf1a7ed
  Stored in directory: /root/.cache/pip/wheels/fe/04/d1/a10661cc45f03c3cecda50deb2d2c22f57b4e84a75b2a5987e
  Building wheel for lit (setup.py): started
  Building wheel for lit (setup.py): finished with status 'done'
  Created wheel for lit: filename=lit-16.0.0-py3-none-any.whl size=93602 sha256=8f583a91b37f98df6bc76ba9016c22c5b4e4963165faf7d9a16833156acb65e0
  Stored in directory: /root/.cache/pip/wheels/c7/ee/80/1520ca86c3557f70e5504b802072f7fc3b0e2147f376b133ed
Successfully built summa summarization-plugin python-multipart lit
Installing collected packages: tokenizers, mpmath, lit, distlib, cmake, websockets, uvloop, urllib3, ujson, typing-extensions, tqdm, tomli, sympy, sniffio, smmap, six, regex, pyyaml, python-dotenv, pluggy, platformdirs, pillow, packaging, orjson, nvidia-nvtx-cu11, nvidia-nccl-cu11, nvidia-cusparse-cu11, nvidia-curand-cu11, nvidia-cufft-cu11, nvidia-cuda-runtime-cu11, nvidia-cuda-nvrtc-cu11, nvidia-cuda-cupti-cu11, nvidia-cublas-cu11, numpy, nodeenv, networkx, MarkupSafe, loguru, itsdangerous, iniconfig, idna, identify, httptools, h11, giturlparse, filelock, fastprogress, exceptiongroup, dnspython, click, charset-normalizer, cfgv, certifi, attrs, asgiref, virtualenv, uvicorn, scipy, requests, python-multipart, pytest, pydantic, nvidia-cusolver-cu11, nvidia-cudnn-cu11, jinja2, gitdb, fastscript, fastcore, email_validator, anyio, watchgod, summa, starlette, pre-commit, huggingface-hub, GitPython, transformers, fastapi, pymemri, triton, torch, summarization-plugin
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.2 anyio-3.6.2 asgiref-3.6.0 attrs-22.2.0 certifi-2022.12.7 cfgv-3.3.1 charset-normalizer-3.1.0 click-8.1.3 cmake-3.26.0 distlib-0.3.6 dnspython-2.3.0 email_validator-1.3.1 exceptiongroup-1.1.1 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 filelock-3.10.0 gitdb-4.0.10 giturlparse-0.10.0 h11-0.14.0 httptools-0.5.0 huggingface-hub-0.13.3 identify-2.5.21 idna-3.4 iniconfig-2.0.0 itsdangerous-2.1.2 jinja2-3.0.0 lit-16.0.0 loguru-0.6.0 mpmath-1.3.0 networkx-3.0 nodeenv-1.7.0 numpy-1.24.2 nvidia-cublas-cu11-11.10.3.66 nvidia-cuda-cupti-cu11-11.7.101 nvidia-cuda-nvrtc-cu11-11.7.99 nvidia-cuda-runtime-cu11-11.7.99 nvidia-cudnn-cu11-8.5.0.96 nvidia-cufft-cu11-10.9.0.58 nvidia-curand-cu11-10.2.10.91 nvidia-cusolver-cu11-11.4.0.1 nvidia-cusparse-cu11-11.7.4.91 nvidia-nccl-cu11-2.14.3 nvidia-nvtx-cu11-11.7.91 orjson-3.8.7 packaging-23.0 pillow-8.4.0 platformdirs-3.1.1 pluggy-1.0.0 pre-commit-3.2.0 pydantic-1.10.2 pymemri-0.0.45 pytest-7.2.2 python-dotenv-1.0.0 python-multipart-0.0.5 pyyaml-6.0 regex-2022.10.31 requests-2.28.2 scipy-1.10.1 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 summa-1.2.0 summarization-plugin-0.0.1 sympy-1.11.1 tokenizers-0.13.2 tomli-2.0.1 torch-2.0.0 tqdm-4.65.0 transformers-4.27.1 triton-2.0.0 typing-extensions-4.5.0 ujson-5.7.0 urllib3-1.26.15 uvicorn-0.17.6 uvloop-0.17.0 virtualenv-20.21.0 watchgod-0.8.2 websockets-10.4
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 23.0.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100    58  100    58    0     0   2000      0 --:--:-- --:--:-- --:-{"build_profile":null,"cargo":"0.4.4","git_describe":null}-:--  2000
[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pre-commit run --all-files --show-diff-on-failure[0;m
[INFO] Initializing environment for https://github.com/charliermarsh/ruff-pre-commit.
[INFO] Initializing environment for https://github.com/psf/black.
[INFO] Installing environment for https://github.com/charliermarsh/ruff-pre-commit.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/psf/black.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
ruff.....................................................................Passed
black....................................................................Passed
[32;1m$ pytest -s .[0;m
============================= test session starts ==============================
platform linux -- Python 3.9.16, pytest-7.2.2, pluggy-1.0.0
rootdir: /builds/memri/plugins/summarization-plugin, configfile: pyproject.toml
plugins: anyio-3.6.2
collected 2 items

tests/test_plugin.py 2023-03-20 16:19:06.562 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
2023-03-20 16:19:06.676 | INFO     | summarization_plugin.plugin:__init__:17 - Loading model...
2023-03-20 16:19:06.676 | DEBUG    | summarization_plugin.model:__init__:30 - Using device: cpu

Downloading (…)okenizer_config.json:   0%|          | 0.00/300 [00:00<?, ?B/s]
Downloading (…)okenizer_config.json: 100%|██████████| 300/300 [00:00<00:00, 27.0kB/s]

Downloading (…)lve/main/config.json:   0%|          | 0.00/1.63k [00:00<?, ?B/s]
Downloading (…)lve/main/config.json: 100%|██████████| 1.63k/1.63k [00:00<00:00, 159kB/s]

Downloading (…)olve/main/vocab.json:   0%|          | 0.00/798k [00:00<?, ?B/s]
Downloading (…)olve/main/vocab.json: 100%|██████████| 798k/798k [00:00<00:00, 1.74MB/s]
Downloading (…)olve/main/vocab.json: 100%|██████████| 798k/798k [00:00<00:00, 1.73MB/s]

Downloading (…)olve/main/merges.txt:   0%|          | 0.00/456k [00:00<?, ?B/s]
Downloading (…)olve/main/merges.txt: 100%|██████████| 456k/456k [00:00<00:00, 1.29MB/s]
Downloading (…)olve/main/merges.txt: 100%|██████████| 456k/456k [00:00<00:00, 1.29MB/s]

Downloading (…)cial_tokens_map.json:   0%|          | 0.00/239 [00:00<?, ?B/s]
Downloading (…)cial_tokens_map.json: 100%|██████████| 239/239 [00:00<00:00, 62.2kB/s]

Downloading pytorch_model.bin:   0%|          | 0.00/1.63G [00:00<?, ?B/s]
Downloading pytorch_model.bin:   2%|▏         | 31.5M/1.63G [00:00<00:08, 193MB/s]
Downloading pytorch_model.bin:   4%|▍         | 62.9M/1.63G [00:00<00:06, 248MB/s]
Downloading pytorch_model.bin:   6%|▋         | 105M/1.63G [00:00<00:05, 284MB/s] 
Downloading pytorch_model.bin:   9%|▉         | 147M/1.63G [00:00<00:04, 303MB/s]
Downloading pytorch_model.bin:  12%|█▏        | 189M/1.63G [00:00<00:04, 318MB/s]
Downloading pytorch_model.bin:  14%|█▍        | 231M/1.63G [00:00<00:04, 327MB/s]
Downloading pytorch_model.bin:  17%|█▋        | 273M/1.63G [00:00<00:04, 336MB/s]
Downloading pytorch_model.bin:  19%|█▉        | 315M/1.63G [00:01<00:03, 333MB/s]
Downloading pytorch_model.bin:  22%|██▏       | 357M/1.63G [00:01<00:03, 330MB/s]
Downloading pytorch_model.bin:  25%|██▍       | 398M/1.63G [00:01<00:03, 332MB/s]
Downloading pytorch_model.bin:  27%|██▋       | 440M/1.63G [00:01<00:03, 331MB/s]
Downloading pytorch_model.bin:  30%|██▉       | 482M/1.63G [00:01<00:03, 337MB/s]
Downloading pytorch_model.bin:  32%|███▏      | 524M/1.63G [00:01<00:03, 342MB/s]
Downloading pytorch_model.bin:  35%|███▍      | 566M/1.63G [00:01<00:03, 345MB/s]
Downloading pytorch_model.bin:  37%|███▋      | 608M/1.63G [00:01<00:02, 350MB/s]
Downloading pytorch_model.bin:  40%|███▉      | 650M/1.63G [00:01<00:02, 347MB/s]
Downloading pytorch_model.bin:  43%|████▎     | 692M/1.63G [00:02<00:02, 337MB/s]
Downloading pytorch_model.bin:  45%|████▌     | 734M/1.63G [00:02<00:02, 340MB/s]
Downloading pytorch_model.bin:  48%|████▊     | 776M/1.63G [00:02<00:02, 337MB/s]
Downloading pytorch_model.bin:  50%|█████     | 818M/1.63G [00:02<00:02, 336MB/s]
Downloading pytorch_model.bin:  53%|█████▎    | 860M/1.63G [00:02<00:02, 337MB/s]
Downloading pytorch_model.bin:  55%|█████▌    | 902M/1.63G [00:02<00:02, 325MB/s]
Downloading pytorch_model.bin:  58%|█████▊    | 944M/1.63G [00:02<00:02, 314MB/s]
Downloading pytorch_model.bin:  61%|██████    | 986M/1.63G [00:03<00:01, 325MB/s]
Downloading pytorch_model.bin:  63%|██████▎   | 1.03G/1.63G [00:03<00:01, 334MB/s]
Downloading pytorch_model.bin:  66%|██████▌   | 1.07G/1.63G [00:03<00:01, 335MB/s]
Downloading pytorch_model.bin:  68%|██████▊   | 1.11G/1.63G [00:03<00:01, 335MB/s]
Downloading pytorch_model.bin:  71%|███████   | 1.15G/1.63G [00:03<00:01, 337MB/s]
Downloading pytorch_model.bin:  74%|███████▎  | 1.20G/1.63G [00:03<00:01, 339MB/s]
Downloading pytorch_model.bin:  76%|███████▌  | 1.24G/1.63G [00:03<00:01, 332MB/s]
Downloading pytorch_model.bin:  79%|███████▊  | 1.28G/1.63G [00:03<00:01, 328MB/s]
Downloading pytorch_model.bin:  81%|████████▏ | 1.32G/1.63G [00:04<00:00, 332MB/s]
Downloading pytorch_model.bin:  84%|████████▍ | 1.36G/1.63G [00:04<00:00, 337MB/s]
Downloading pytorch_model.bin:  86%|████████▋ | 1.41G/1.63G [00:04<00:00, 309MB/s]
Downloading pytorch_model.bin:  89%|████████▉ | 1.45G/1.63G [00:04<00:00, 314MB/s]
Downloading pytorch_model.bin:  92%|█████████▏| 1.49G/1.63G [00:04<00:00, 322MB/s]
Downloading pytorch_model.bin:  94%|█████████▍| 1.53G/1.63G [00:04<00:00, 326MB/s]
Downloading pytorch_model.bin:  97%|█████████▋| 1.57G/1.63G [00:04<00:00, 329MB/s]
Downloading pytorch_model.bin:  99%|█████████▉| 1.61G/1.63G [00:04<00:00, 302MB/s]
Downloading pytorch_model.bin: 100%|██████████| 1.63G/1.63G [00:05<00:00, 324MB/s]
2023-03-20 16:19:52.451 | DEBUG    | summarization_plugin.model:summarize:69 - Summarized 3 documents in 20.03603196144104 seconds
2023-03-20 16:20:46.719 | DEBUG    | summarization_plugin.model:summarize:69 - Summarized 3 documents in 54.26732921600342 seconds
.2023-03-20 16:20:46.724 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 3/3 items/edges
2023-03-20 16:20:46.739 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 3 items/edges
2023-03-20 16:20:46.753 | INFO     | summarization_plugin.plugin:summarize_rss_entries_endpoint:108 - Summarizing 3 RSSEntries...
2023-03-20 16:20:46.753 | DEBUG    | summarization_plugin.plugin:summarize_rss_entries:66 - Filtered 0 entries
2023-03-20 16:21:07.865 | DEBUG    | summarization_plugin.model:summarize:69 - Summarized 3 documents in 21.111137628555298 seconds
2023-03-20 16:21:07.866 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 3/3 items/edges
2023-03-20 16:21:07.877 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 3 items/edges
.

======================== 2 passed in 126.51s (0:02:06) =========================
section_end:1679329269:step_script
[0Ksection_start:1679329269:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1679329269:cleanup_file_variables
[0K[32;1mJob succeeded[0;m
```