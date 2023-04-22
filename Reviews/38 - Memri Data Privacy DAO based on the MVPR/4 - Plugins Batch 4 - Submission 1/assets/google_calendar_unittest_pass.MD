```
[0KRunning with gitlab-runner 15.7.1 (6d480948)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1679986470:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.8 ...[0;m
[0KPulling docker image python:3.8 ...[0;m
[0KUsing docker image sha256:a865bc2909a48902fe4d5f3b64ed2ab2d0ba18ece4b0310808058ce9404aee39 for python:3.8 with digest python@sha256:79deacb15dd56e1a66d923f7c15a3ccadff232776b3329745d34fca98b52c5f8 ...[0;m
section_end:1679986472:prepare_executor
[0Ksection_start:1679986472:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-89-concurrent-0 via cab6f0e97d50...
section_end:1679986472:prepare_script
[0Ksection_start:1679986472:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 50...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/google-calendar/.git/
[32;1mChecking out b262a6ea as v0.1...[0;m
Removing google_calendar/__pycache__/
Removing google_calendar/data/__pycache__/
Removing google_calendar/google_api/__pycache__/
Removing tests/__pycache__/

[32;1mSkipping Git submodules setup[0;m
section_end:1679986474:get_sources
[0Ksection_start:1679986474:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:a865bc2909a48902fe4d5f3b64ed2ab2d0ba18ece4b0310808058ce9404aee39 for python:3.8 with digest python@sha256:79deacb15dd56e1a66d923f7c15a3ccadff232776b3329745d34fca98b52c5f8 ...[0;m
[32;1m$ apt update && apt-get install -y libgl1-mesa-glx[0;m

WARNING: apt does not have a stable CLI interface. Use with caution in scripts.

Get:1 http://deb.debian.org/debian bullseye InRelease [116 kB]
Get:2 http://deb.debian.org/debian-security bullseye-security InRelease [48.4 kB]
Get:3 http://deb.debian.org/debian bullseye-updates InRelease [44.1 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 Packages [8183 kB]
Get:5 http://deb.debian.org/debian-security bullseye-security/main amd64 Packages [236 kB]
Get:6 http://deb.debian.org/debian bullseye-updates/main amd64 Packages [14.6 kB]
Fetched 8642 kB in 2s (5541 kB/s)
Reading package lists...
Building dependency tree...
Reading state information...
1 package can be upgraded. Run 'apt list --upgradable' to see it.
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
Fetched 40.6 MB in 0s (110 MB/s)
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
(Reading database ... 23423 files and directories currently installed.)
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
[32;1m$ pip install --upgrade pip[0;m
Requirement already satisfied: pip in /usr/local/lib/python3.8/site-packages (22.0.4)
Collecting pip
  Downloading pip-23.0.1-py3-none-any.whl (2.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.1/2.1 MB 52.4 MB/s eta 0:00:00
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 22.0.4
    Uninstalling pip-22.0.4:
      Successfully uninstalled pip-22.0.4
Successfully installed pip-23.0.1
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
[32;1m$ pip install -r requirements.txt[0;m
Collecting amqp==5.1.1
  Downloading amqp-5.1.1-py3-none-any.whl (50 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 50.8/50.8 kB 5.7 MB/s eta 0:00:00
Collecting anyio==3.6.2
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 kB 10.9 MB/s eta 0:00:00
Collecting asgiref==3.4.1
  Downloading asgiref-3.4.1-py3-none-any.whl (25 kB)
Collecting async-timeout==4.0.2
  Downloading async_timeout-4.0.2-py3-none-any.whl (5.8 kB)
Collecting billiard==3.6.4.0
  Downloading billiard-3.6.4.0-py3-none-any.whl (89 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 89.5/89.5 kB 11.3 MB/s eta 0:00:00
Collecting cachetools==5.3.0
  Downloading cachetools-5.3.0-py3-none-any.whl (9.3 kB)
Collecting celery==5.2.7
  Downloading celery-5.2.7-py3-none-any.whl (405 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 405.6/405.6 kB 17.6 MB/s eta 0:00:00
Collecting certifi==2022.12.7
  Downloading certifi-2022.12.7-py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 kB 14.6 MB/s eta 0:00:00
Collecting charset-normalizer==3.0.1
  Downloading charset_normalizer-3.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (195 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 195.4/195.4 kB 20.9 MB/s eta 0:00:00
Collecting click==8.1.3
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 kB 13.0 MB/s eta 0:00:00
Collecting click-didyoumean==0.3.0
  Downloading click_didyoumean-0.3.0-py3-none-any.whl (2.7 kB)
Collecting click-plugins==1.1.1
  Downloading click_plugins-1.1.1-py2.py3-none-any.whl (7.5 kB)
Collecting click-repl==0.2.0
  Downloading click_repl-0.2.0-py3-none-any.whl (5.2 kB)
Collecting dnspython==2.3.0
  Downloading dnspython-2.3.0-py3-none-any.whl (283 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 283.7/283.7 kB 19.5 MB/s eta 0:00:00
Collecting email-validator==1.3.1
  Downloading email_validator-1.3.1-py2.py3-none-any.whl (22 kB)
Collecting fastapi==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 kB 6.7 MB/s eta 0:00:00
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 kB 6.2 MB/s eta 0:00:00
Collecting fastprogress==1.0.3
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting fastscript==1.0.0
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting gitdb==4.0.10
  Downloading gitdb-4.0.10-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.7/62.7 kB 8.1 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 kB 15.7 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting google-api-core==2.11.0
  Downloading google_api_core-2.11.0-py3-none-any.whl (120 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.3/120.3 kB 5.1 MB/s eta 0:00:00
Collecting google-api-python-client==2.79.0
  Downloading google_api_python_client-2.79.0-py2.py3-none-any.whl (11.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.0/11.0 MB 55.3 MB/s eta 0:00:00
Collecting google-auth==2.16.1
  Downloading google_auth-2.16.1-py2.py3-none-any.whl (177 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 177.2/177.2 kB 16.8 MB/s eta 0:00:00
Collecting google-auth-httplib2==0.1.0
  Downloading google_auth_httplib2-0.1.0-py2.py3-none-any.whl (9.3 kB)
Collecting google-auth-oauthlib==1.0.0
  Downloading google_auth_oauthlib-1.0.0-py2.py3-none-any.whl (18 kB)
Collecting googleapis-common-protos==1.58.0
  Downloading googleapis_common_protos-1.58.0-py2.py3-none-any.whl (223 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 223.0/223.0 kB 23.9 MB/s eta 0:00:00
Collecting h11==0.14.0
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 kB 7.0 MB/s eta 0:00:00
Collecting httplib2==0.21.0
  Downloading httplib2-0.21.0-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.8/96.8 kB 14.1 MB/s eta 0:00:00
Collecting httptools==0.5.0
  Downloading httptools-0.5.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (427 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 427.8/427.8 kB 33.3 MB/s eta 0:00:00
Collecting idna==3.4
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 kB 5.8 MB/s eta 0:00:00
Collecting itsdangerous==2.1.2
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting Jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 kB 15.3 MB/s eta 0:00:00
Collecting kombu==5.2.4
  Downloading kombu-5.2.4-py3-none-any.whl (189 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 189.2/189.2 kB 15.4 MB/s eta 0:00:00
Collecting loguru==0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 kB 6.9 MB/s eta 0:00:00
Collecting MarkupSafe==2.1.2
  Downloading MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting numpy==1.24.2
  Downloading numpy-1.24.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 17.3/17.3 MB 43.2 MB/s eta 0:00:00
Collecting oauthlib==3.2.2
  Downloading oauthlib-3.2.2-py3-none-any.whl (151 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 151.7/151.7 kB 15.3 MB/s eta 0:00:00
Collecting orjson==3.8.6
  Downloading orjson-3.8.6-cp38-cp38-manylinux_2_28_x86_64.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.7/140.7 kB 13.7 MB/s eta 0:00:00
Collecting packaging==23.0
  Downloading packaging-23.0-py3-none-any.whl (42 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 42.7/42.7 kB 3.0 MB/s eta 0:00:00
Collecting Pillow==8.4.0
  Downloading Pillow-8.4.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 10.0 MB/s eta 0:00:00
Collecting prompt-toolkit==3.0.37
  Downloading prompt_toolkit-3.0.37-py3-none-any.whl (385 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 385.2/385.2 kB 20.3 MB/s eta 0:00:00
Collecting protobuf==4.22.0
  Downloading protobuf-4.22.0-cp37-abi3-manylinux2014_x86_64.whl (302 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 302.4/302.4 kB 25.3 MB/s eta 0:00:00
Collecting pyasn1==0.4.8
  Downloading pyasn1-0.4.8-py2.py3-none-any.whl (77 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 77.1/77.1 kB 9.2 MB/s eta 0:00:00
Collecting pyasn1-modules==0.2.8
  Downloading pyasn1_modules-0.2.8-py2.py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 kB 13.4 MB/s eta 0:00:00
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 13.6/13.6 MB 57.3 MB/s eta 0:00:00
Collecting pymemri==0.0.45
  Downloading pymemri-0.0.45-py3-none-any.whl (69 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 69.9/69.9 kB 9.0 MB/s eta 0:00:00
Collecting pyparsing==3.0.9
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 kB 13.3 MB/s eta 0:00:00
Collecting python-dotenv==0.21.1
  Downloading python_dotenv-0.21.1-py3-none-any.whl (19 kB)
Collecting python-multipart==0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pytz==2022.7.1
  Downloading pytz-2022.7.1-py2.py3-none-any.whl (499 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 499.4/499.4 kB 38.0 MB/s eta 0:00:00
Collecting pytest==7.2.2
  Downloading pytest-7.2.2-py3-none-any.whl (317 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 317.2/317.2 kB 26.0 MB/s eta 0:00:00
Collecting PyYAML==6.0
  Downloading PyYAML-6.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (701 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 701.2/701.2 kB 38.2 MB/s eta 0:00:00
Collecting redis==4.5.1
  Downloading redis-4.5.1-py3-none-any.whl (238 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 238.5/238.5 kB 25.7 MB/s eta 0:00:00
Collecting requests==2.28.2
  Downloading requests-2.28.2-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 kB 7.4 MB/s eta 0:00:00
Collecting requests-oauthlib==1.3.1
  Downloading requests_oauthlib-1.3.1-py2.py3-none-any.whl (23 kB)
Collecting rsa==4.9
  Downloading rsa-4.9-py3-none-any.whl (34 kB)
Collecting six==1.16.0
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting smmap==5.0.0
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting sniffio==1.3.0
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 kB 7.2 MB/s eta 0:00:00
Collecting typing_extensions==4.5.0
  Downloading typing_extensions-4.5.0-py3-none-any.whl (27 kB)
Collecting ujson==5.7.0
  Downloading ujson-5.7.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (52 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 52.8/52.8 kB 6.6 MB/s eta 0:00:00
Collecting uritemplate==4.1.1
  Downloading uritemplate-4.1.1-py2.py3-none-any.whl (10 kB)
Collecting urllib3==1.26.14
  Downloading urllib3-1.26.14-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.6/140.6 kB 17.7 MB/s eta 0:00:00
Collecting uvicorn==0.17.6
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 kB 7.0 MB/s eta 0:00:00
Collecting uvloop==0.17.0
  Downloading uvloop-0.17.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.6/4.6 MB 68.1 MB/s eta 0:00:00
Collecting vine==5.0.0
  Downloading vine-5.0.0-py2.py3-none-any.whl (9.4 kB)
Collecting watchgod==0.8.2
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting wcwidth==0.2.6
  Downloading wcwidth-0.2.6-py2.py3-none-any.whl (29 kB)
Collecting websockets==10.4
  Downloading websockets-10.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 107.0/107.0 kB 14.9 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.8/site-packages (from fastcore==1.3.21->-r requirements.txt (line 17)) (23.0.1)
Collecting attrs>=19.2.0
  Downloading attrs-22.2.0-py3-none-any.whl (60 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.0/60.0 kB 7.6 MB/s eta 0:00:00
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.1.1-py3-none-any.whl (14 kB)
Collecting iniconfig
  Downloading iniconfig-2.0.0-py3-none-any.whl (5.9 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Building wheels for collected packages: python-multipart
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31677 sha256=77c3f43b69f3a1a68b026e62f63fd6f837370daad942ddc305cdf61eb705e019
  Stored in directory: /root/.cache/pip/wheels/9e/fc/1c/cf980e6413d3ee8e70cd8f39e2366b0f487e3e221aeb452eb0
Successfully built python-multipart
Installing collected packages: wcwidth, pytz, pyasn1, charset-normalizer, billiard, websockets, vine, uvloop, urllib3, uritemplate, ujson, typing_extensions, tomli, sniffio, smmap, six, rsa, PyYAML, python-dotenv, pyparsing, pyasn1-modules, protobuf, prompt-toolkit, pluggy, Pillow, packaging, orjson, oauthlib, numpy, MarkupSafe, loguru, itsdangerous, iniconfig, idna, httptools, h11, giturlparse, fastprogress, exceptiongroup, dnspython, click, certifi, cachetools, attrs, async-timeout, asgiref, uvicorn, requests, redis, python-multipart, pytest, pydantic, Jinja2, httplib2, googleapis-common-protos, google-auth, gitdb, fastscript, fastcore, email-validator, click-repl, click-plugins, click-didyoumean, anyio, amqp, watchgod, starlette, requests-oauthlib, kombu, google-auth-httplib2, google-api-core, GitPython, google-auth-oauthlib, google-api-python-client, fastapi, celery, pymemri
Successfully installed GitPython-3.1.27 Jinja2-3.0.0 MarkupSafe-2.1.2 Pillow-8.4.0 PyYAML-6.0 amqp-5.1.1 anyio-3.6.2 asgiref-3.4.1 async-timeout-4.0.2 attrs-22.2.0 billiard-3.6.4.0 cachetools-5.3.0 celery-5.2.7 certifi-2022.12.7 charset-normalizer-3.0.1 click-8.1.3 click-didyoumean-0.3.0 click-plugins-1.1.1 click-repl-0.2.0 dnspython-2.3.0 email-validator-1.3.1 exceptiongroup-1.1.1 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 gitdb-4.0.10 giturlparse-0.10.0 google-api-core-2.11.0 google-api-python-client-2.79.0 google-auth-2.16.1 google-auth-httplib2-0.1.0 google-auth-oauthlib-1.0.0 googleapis-common-protos-1.58.0 h11-0.14.0 httplib2-0.21.0 httptools-0.5.0 idna-3.4 iniconfig-2.0.0 itsdangerous-2.1.2 kombu-5.2.4 loguru-0.6.0 numpy-1.24.2 oauthlib-3.2.2 orjson-3.8.6 packaging-23.0 pluggy-1.0.0 prompt-toolkit-3.0.37 protobuf-4.22.0 pyasn1-0.4.8 pyasn1-modules-0.2.8 pydantic-1.10.2 pymemri-0.0.45 pyparsing-3.0.9 pytest-7.2.2 python-dotenv-0.21.1 python-multipart-0.0.5 pytz-2022.7.1 redis-4.5.1 requests-2.28.2 requests-oauthlib-1.3.1 rsa-4.9 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tomli-2.0.1 typing_extensions-4.5.0 ujson-5.7.0 uritemplate-4.1.1 urllib3-1.26.14 uvicorn-0.17.6 uvloop-0.17.0 vine-5.0.0 watchgod-0.8.2 wcwidth-0.2.6 websockets-10.4
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
[32;1m$ python -m unittest[0;m
2023-03-28 06:55:35.947 | WARNING  | pymemri.pod.client:create_account:81 - 400 "Failure: Error 400 Bad Request, Account for MYTESTINGKEY20Mar already exist"
/usr/local/lib/python3.8/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
  warnings.warn(
2023-03-28 06:55:37.753 | INFO     | google_calendar.plugin:write:322 - Creating 0 items, 0 edges, updating 3 and uploading 0 files
2023-03-28 06:55:37.755 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 3/3 items/edges
2023-03-28 06:55:38.157 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 3 items/edges
2023-03-28 06:55:38.158 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.40454983711242676
2023-03-28 06:55:38.258 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-03-28 06:55:38.359 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
.2023-03-28 06:55:38.930 | INFO     | google_calendar.plugin:write:322 - Creating 0 items, 0 edges, updating 4 and uploading 0 files
2023-03-28 06:55:38.932 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 4/4 items/edges
2023-03-28 06:55:39.333 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 4 items/edges
2023-03-28 06:55:39.333 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.40329766273498535
2023-03-28 06:55:39.434 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-03-28 06:55:39.535 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
...
----------------------------------------------------------------------
Ran 4 tests in 2.769s

OK
section_end:1679986540:step_script
[0Ksection_start:1679986540:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1679986541:cleanup_file_variables
[0K[32;1mJob succeeded[0;m
```