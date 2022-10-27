Running with gitlab-runner 14.9.1 (bd40e3da)
  on gitlab memri public docker-runner Ryesm3zY
Preparing the "docker" executor
Using Docker executor with image python:3.7 ...
Starting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...
Authenticating with credentials from job payload (GitLab Registry)
Pulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...
Using docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...
Waiting for services to be up and running...
Pulling docker image python:3.7 ...
Using docker image sha256:d74a76afa4e0a85ede9045050f871b53e99e2d86e0290468b0dfa86ddce03e00 for python:3.7 with digest python@sha256:233f03ae08cc3fe8e9d31803b683123d3dc0dc7e1b74ef396e1389799d8da2fc ...
Preparing environment
Running on runner-ryesm3zy-project-174-concurrent-0 via 8e6b65718045...
Getting source from Git repository
Fetching changes with git depth set to 50...
Reinitialized existing Git repository in /builds/memri/plugins/whatsapp-multi-device/.git/
Checking out 084b8a44 as dev...
Skipping Git submodules setup
Executing "step_script" stage of the job script
Using docker image sha256:d74a76afa4e0a85ede9045050f871b53e99e2d86e0290468b0dfa86ddce03e00 for python:3.7 with digest python@sha256:233f03ae08cc3fe8e9d31803b683123d3dc0dc7e1b74ef396e1389799d8da2fc ...

$ apt-get update && apt-get install -y libsqlcipher-dev && apt-get install -y libgl1-mesa-glx
'''
Get:1 http://deb.debian.org/debian bullseye InRelease [116 kB]
Get:2 http://deb.debian.org/debian-security bullseye-security InRelease [48.4 kB]
Get:3 http://deb.debian.org/debian bullseye-updates InRelease [44.1 kB]
Get:4 http://deb.debian.org/debian bullseye/main amd64 Packages [8184 kB]
Get:5 http://deb.debian.org/debian-security bullseye-security/main amd64 Packages [190 kB]
Get:6 http://deb.debian.org/debian bullseye-updates/main amd64 Packages [6340 B]
Fetched 8588 kB in 2s (3799 kB/s)
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
Fetched 998 kB in 0s (21.2 MB/s)
Selecting previously unselected package libsqlcipher0:amd64.
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
Fetched 40.6 MB in 1s (39.7 MB/s)
Selecting previously unselected package libdrm-common.
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
'''
$ pip install --upgrade pip
'''
Requirement already satisfied: pip in /usr/local/lib/python3.7/site-packages (22.0.4)
Collecting pip
  Downloading pip-22.3-py3-none-any.whl (2.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.1/2.1 MB 6.1 MB/s eta 0:00:00
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 22.0.4
    Uninstalling pip-22.0.4:
      Successfully uninstalled pip-22.0.4
Successfully installed pip-22.3
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
'''
$ pip install -e .
'''
Obtaining file:///builds/memri/plugins/whatsapp-multi-device
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31
  Cloning https://gitlab.memri.io/memri/pymemri.git (to revision v0.0.31) to /tmp/pip-install-idxssrad/pymemri_82fadf96c924483fa5165174bc20c4a3
  Running command git clone --filter=blob:none --quiet https://gitlab.memri.io/memri/pymemri.git /tmp/pip-install-idxssrad/pymemri_82fadf96c924483fa5165174bc20c4a3
  Running command git checkout -q a9cecb620c4b6dde75405a17801cade497c63995
  Resolved https://gitlab.memri.io/memri/pymemri.git to commit a9cecb620c4b6dde75405a17801cade497c63995
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting wamd@ git+https://github.com/alpdeniz/wamd.git@main
  Cloning https://github.com/alpdeniz/wamd.git (to revision main) to /tmp/pip-install-idxssrad/wamd_c5f9d70f447e4da799d588aa25b30075
  Running command git clone --filter=blob:none --quiet https://github.com/alpdeniz/wamd.git /tmp/pip-install-idxssrad/wamd_c5f9d70f447e4da799d588aa25b30075
  Resolved https://github.com/alpdeniz/wamd.git to commit 2d6b9662f03edbc83ea80d95053a7bb887a9e3a7
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting websocket-client
  Downloading websocket_client-1.4.1-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.0/55.0 kB 534.8 kB/s eta 0:00:00
Collecting curve25519-donna
  Downloading curve25519-donna-1.3.tar.gz (20 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pycrypto
  Downloading pycrypto-2.6.1.tar.gz (446 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 446.2/446.2 kB 34.6 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pyqrcode
  Downloading PyQRCode-1.2.1.zip (41 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 41.9/41.9 kB 3.1 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting protobuf==3.19.4
  Downloading protobuf-3.19.4-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 29.5 MB/s eta 0:00:00
Collecting pytest
  Downloading pytest-7.1.3-py3-none-any.whl (298 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 298.2/298.2 kB 17.3 MB/s eta 0:00:00
Collecting requests
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 kB 7.0 MB/s eta 0:00:00
Collecting tqdm
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 kB 7.7 MB/s eta 0:00:00
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 kB 6.1 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 kB 7.2 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting pandas
  Downloading pandas-1.3.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.3/11.3 MB 49.3 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 51.6 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 kB 19.5 MB/s eta 0:00:00
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 kB 10.3 MB/s eta 0:00:00
Collecting loguru~=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 kB 2.5 MB/s eta 0:00:00
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.8/11.8 MB 47.4 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 kB 2.5 MB/s eta 0:00:00
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.5.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (45 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 45.9/45.9 kB 6.6 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 kB 7.6 MB/s eta 0:00:00
Collecting pyyaml<7.0.0,>=5.3.1
  Downloading PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (596 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 596.3/596.3 kB 33.4 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.0-py2.py3-none-any.whl (22 kB)
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.0-cp37-cp37m-manylinux_2_28_x86_64.whl (145 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 145.9/145.9 kB 13.8 MB/s eta 0:00:00
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 kB 3.8 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.7/site-packages (from fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (22.3)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 kB 7.4 MB/s eta 0:00:00
Collecting typing-extensions>=3.7.4.3
  Downloading typing_extensions-4.4.0-py3-none-any.whl (26 kB)
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.1-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 kB 10.6 MB/s eta 0:00:00
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 kB 2.6 MB/s eta 0:00:00
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting py>=1.8.2
  Downloading py-1.11.0-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.7/98.7 kB 7.7 MB/s eta 0:00:00
Collecting importlib-metadata>=0.12
  Downloading importlib_metadata-5.0.0-py3-none-any.whl (21 kB)
Collecting twisted
  Downloading Twisted-22.8.0-py3-none-any.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 45.7 MB/s eta 0:00:00
Collecting PyOpenSSL
  Downloading pyOpenSSL-22.1.0-py3-none-any.whl (57 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 57.0/57.0 kB 3.4 MB/s eta 0:00:00
Collecting service_identity
  Downloading service_identity-21.1.0-py2.py3-none-any.whl (12 kB)
Collecting autobahn
  Downloading autobahn-22.7.1.tar.gz (476 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 476.8/476.8 kB 32.0 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting dissononce
  Downloading dissononce-0.34.3-py3-none-any.whl (51 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 51.8/51.8 kB 5.5 MB/s eta 0:00:00
Collecting consonance
  Downloading consonance-0.1.5-py3-none-any.whl (35 kB)
Collecting python-axolotl
  Downloading python_axolotl-0.2.3-py3-none-any.whl (76 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 76.1/76.1 kB 3.3 MB/s eta 0:00:00
Collecting python-magic
  Downloading python_magic-0.4.27-py2.py3-none-any.whl (13 kB)
Collecting setuptools-rust
  Downloading setuptools_rust-1.5.2-py3-none-any.whl (23 kB)
Collecting zipp>=0.5
  Downloading zipp-3.9.0-py3-none-any.whl (5.8 kB)
Collecting certifi>=2017.4.17
  Downloading certifi-2022.9.24-py3-none-any.whl (161 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 161.1/161.1 kB 11.2 MB/s eta 0:00:00
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 kB 9.4 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 kB 3.1 MB/s eta 0:00:00
Collecting txaio>=21.2.1
  Downloading txaio-22.2.1-py2.py3-none-any.whl (30 kB)
Collecting cryptography>=3.4.6
  Downloading cryptography-38.0.1-cp36-abi3-manylinux_2_28_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 22.6 MB/s eta 0:00:00
Collecting hyperlink>=21.0.0
  Downloading hyperlink-21.0.0-py2.py3-none-any.whl (74 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 74.6/74.6 kB 6.7 MB/s eta 0:00:00
Requirement already satisfied: setuptools in /usr/local/lib/python3.7/site-packages (from autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (57.5.0)
Collecting transitions
  Downloading transitions-0.9.0-py2.py3-none-any.whl (97 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 97.7/97.7 kB 2.6 MB/s eta 0:00:00
Collecting python-axolotl-curve25519
  Downloading python-axolotl-curve25519-0.4.1.post2.tar.gz (79 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 79.9/79.9 kB 4.9 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pyparsing!=3.0.5,>=2.0.2
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 kB 7.0 MB/s eta 0:00:00
Collecting numpy>=1.17.3
  Downloading numpy-1.21.6-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (15.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 15.7/15.7 MB 44.7 MB/s eta 0:00:00
Collecting python-dateutil>=2.7.3
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 kB 7.8 MB/s eta 0:00:00
Collecting pytz>=2017.3
  Downloading pytz-2022.4-py2.py3-none-any.whl (500 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 500.8/500.8 kB 27.8 MB/s eta 0:00:00
Collecting pyasn1-modules
  Downloading pyasn1_modules-0.2.8-py2.py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 kB 10.4 MB/s eta 0:00:00
Collecting pyasn1
  Downloading pyasn1-0.4.8-py2.py3-none-any.whl (77 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 77.1/77.1 kB 4.7 MB/s eta 0:00:00
Collecting six
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting semantic-version<3,>=2.8.2
  Downloading semantic_version-2.10.0-py2.py3-none-any.whl (15 kB)
Collecting setuptools
  Downloading setuptools-65.5.0-py3-none-any.whl (1.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 23.2 MB/s eta 0:00:00
Collecting Automat>=0.8.0
  Downloading Automat-20.2.0-py2.py3-none-any.whl (31 kB)
Collecting incremental>=21.3.0
  Downloading incremental-22.10.0-py2.py3-none-any.whl (16 kB)
Collecting constantly>=15.1
  Downloading constantly-15.1.0-py2.py3-none-any.whl (7.9 kB)
Collecting zope.interface>=4.4.2
  Downloading zope.interface-5.5.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (254 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 254.1/254.1 kB 9.3 MB/s eta 0:00:00
Collecting cffi>=1.12
  Downloading cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (427 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 427.9/427.9 kB 7.9 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 kB 5.7 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 kB 3.3 MB/s eta 0:00:00
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 kB 810.3 kB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting websockets>=10.0
  Downloading websockets-10.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (112 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 112.1/112.1 kB 263.7 kB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 37.8 MB/s eta 0:00:00
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (404 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 404.7/404.7 kB 26.2 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Collecting pycparser
  Downloading pycparser-2.21-py2.py3-none-any.whl (118 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 118.7/118.7 kB 11.0 MB/s eta 0:00:00
Building wheels for collected packages: curve25519-donna, pycrypto, pymemri, pyqrcode, wamd, autobahn, python-axolotl-curve25519, python-multipart
  Building wheel for curve25519-donna (setup.py): started
  Building wheel for curve25519-donna (setup.py): finished with status 'done'
  Created wheel for curve25519-donna: filename=curve25519_donna-1.3-cp37-cp37m-linux_x86_64.whl size=36783 sha256=a596d38c84e9a8ded000b10aa5ed566fb33879ae00c394ec91fc2b17d2eeacde
  Stored in directory: /root/.cache/pip/wheels/72/5a/97/a5d83272f5a1bee938fc483d0e9e6e0415839dfaf1297b6bd0
  Building wheel for pycrypto (setup.py): started
  Building wheel for pycrypto (setup.py): finished with status 'done'
  Created wheel for pycrypto: filename=pycrypto-2.6.1-cp37-cp37m-linux_x86_64.whl size=523005 sha256=78933f8abcb1e06797baa3075cd457684561a107d07f6ec5adbf29b1bf8cc53a
  Stored in directory: /root/.cache/pip/wheels/57/8b/74/7dc9b0ad863a980ff5940454215f3728c6126f10241df3af09
  Building wheel for pymemri (setup.py): started
  Building wheel for pymemri (setup.py): finished with status 'done'
  Created wheel for pymemri: filename=pymemri-0.0.31-py3-none-any.whl size=65242 sha256=6bef5fcfd60acae0fa41967159e7091d1fc91af2f808261a99412e254089acd2
  Stored in directory: /tmp/pip-ephem-wheel-cache-ad8axb0i/wheels/ed/5a/e6/147829c91a5bc592bf09c1d42ac4a806d95c859a8ae07eafad
  Building wheel for pyqrcode (setup.py): started
  Building wheel for pyqrcode (setup.py): finished with status 'done'
  Created wheel for pyqrcode: filename=PyQRCode-1.2.1-py3-none-any.whl size=36247 sha256=69873d63665c30a55bde42130e18b1ae79699e4e58da3fdc0eb2601971b23649
  Stored in directory: /root/.cache/pip/wheels/36/9d/cd/6b8e16779109d3b563ae4065ce74e0d0a038d5bc3ae66a9516
  Building wheel for wamd (setup.py): started
  Building wheel for wamd (setup.py): finished with status 'done'
  Created wheel for wamd: filename=wamd-0.0.0-py3-none-any.whl size=109913 sha256=796de767ebe3fd547c91bc287148b9d9422e26e61413274b0ac86ab02033e943
  Stored in directory: /tmp/pip-ephem-wheel-cache-ad8axb0i/wheels/88/d0/84/aa5b9b8caa3b327af924b55e84876ce8c7e66bc21cda7d7567
  Building wheel for autobahn (setup.py): started
  Building wheel for autobahn (setup.py): finished with status 'done'
  Created wheel for autobahn: filename=autobahn-22.7.1-py2.py3-none-any.whl size=664636 sha256=bb24537794669f9ff89ba28ada1511e93a97c7362234228509b1e8d2fee4ef12
  Stored in directory: /root/.cache/pip/wheels/a1/21/07/e2d54ea8fd824739960b201f8ff6891752a6d81dbe44da9927
  Building wheel for python-axolotl-curve25519 (setup.py): started
  Building wheel for python-axolotl-curve25519 (setup.py): finished with status 'done'
  Created wheel for python-axolotl-curve25519: filename=python_axolotl_curve25519-0.4.1.post2-cp37-cp37m-linux_x86_64.whl size=176960 sha256=63b531440e7b13aa62bc32879171bffe3b8968893c9fa39f3e6e8a35de94d719
  Stored in directory: /root/.cache/pip/wheels/a2/8b/29/55ca54bea2e4bf8357a93d2aa73e18d9ef7e3b50523908fc5b
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=065d6eed22807e47c471ce236a0b797963d76a0260f6cd7ce574e987bb5be30e
  Stored in directory: /root/.cache/pip/wheels/7b/24/20/55941b99a69639d6e3a3bce7d2d7b6a2d633f05125042a544a
Successfully built curve25519-donna pycrypto pymemri pyqrcode wamd autobahn python-axolotl-curve25519 python-multipart
Installing collected packages: pytz, python-axolotl-curve25519, pyqrcode, pycrypto, pyasn1, iniconfig, incremental, curve25519-donna, constantly, zipp, websockets, websocket-client, uvloop, urllib3, ujson, typing-extensions, txaio, tqdm, tomli, sniffio, smmap, six, setuptools, semantic-version, pyyaml, python-magic, python-dotenv, pyparsing, pycparser, pyasn1-modules, py, protobuf, pillow, orjson, numpy, MarkupSafe, loguru, itsdangerous, idna, httptools, giturlparse, fastprogress, dnspython, charset-normalizer, certifi, attrs, zope.interface, transitions, setuptools-rust, requests, python-multipart, python-dateutil, pydantic, packaging, jinja2, importlib-metadata, hyperlink, h11, gitdb, email_validator, cffi, Automat, asgiref, anyio, watchgod, twisted, starlette, pluggy, pandas, GitPython, fastscript, fastcore, cryptography, click, uvicorn, service_identity, python-axolotl, pytest, PyOpenSSL, fastapi, dissononce, autobahn, consonance, wamd, pymemri, whatsapp
  Attempting uninstall: setuptools
    Found existing installation: setuptools 57.5.0
    Uninstalling setuptools-57.5.0:
      Successfully uninstalled setuptools-57.5.0
  Running setup.py develop for whatsapp
Successfully installed Automat-20.2.0 GitPython-3.1.27 MarkupSafe-2.1.1 PyOpenSSL-22.1.0 anyio-3.6.1 asgiref-3.5.2 attrs-22.1.0 autobahn-22.7.1 certifi-2022.9.24 cffi-1.15.1 charset-normalizer-2.1.1 click-8.1.3 consonance-0.1.5 constantly-15.1.0 cryptography-38.0.1 curve25519-donna-1.3 dissononce-0.34.3 dnspython-2.2.1 email_validator-1.3.0 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 gitdb-4.0.9 giturlparse-0.10.0 h11-0.14.0 httptools-0.5.0 hyperlink-21.0.0 idna-3.4 importlib-metadata-5.0.0 incremental-22.10.0 iniconfig-1.1.1 itsdangerous-2.1.2 jinja2-3.0.0 loguru-0.6.0 numpy-1.21.6 orjson-3.8.0 packaging-21.3 pandas-1.3.5 pillow-8.4.0 pluggy-1.0.0 protobuf-3.19.4 py-1.11.0 pyasn1-0.4.8 pyasn1-modules-0.2.8 pycparser-2.21 pycrypto-2.6.1 pydantic-1.10.2 pymemri-0.0.31 pyparsing-3.0.9 pyqrcode-1.2.1 pytest-7.1.3 python-axolotl-0.2.3 python-axolotl-curve25519-0.4.1.post2 python-dateutil-2.8.2 python-dotenv-0.21.0 python-magic-0.4.27 python-multipart-0.0.5 pytz-2022.4 pyyaml-6.0 requests-2.28.1 semantic-version-2.10.0 service_identity-21.1.0 setuptools-65.5.0 setuptools-rust-1.5.2 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tomli-2.0.1 tqdm-4.64.1 transitions-0.9.0 twisted-22.8.0 txaio-22.2.1 typing-extensions-4.4.0 ujson-5.5.0 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.17.0 wamd-0.0.0 watchgod-0.8.2 websocket-client-1.4.1 websockets-10.3 whatsapp-1.0 zipp-3.9.0 zope.interface-5.5.0
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
'''
$ curl http://pod:3030/version
'''
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    58  100    58    0     0  19333      0 --:--:-- --:--:-- --:--:-- 19333
'''
$ export POD_ADDRESS='http://pod:3030'
$ pytest
'''
============================= test session starts ==============================
platform linux -- Python 3.7.15, pytest-7.1.3, pluggy-1.0.0
rootdir: /builds/memri/plugins/whatsapp-multi-device
plugins: anyio-3.6.1
collected 1 item
test/test_parse.py .                                                     [100%]
=============================== warnings summary ===============================
test/test_parse.py::test_answer
  /usr/local/lib/python3.7/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    RuntimeWarning,
-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
========================= 1 passed, 1 warning in 3.69s =========================
Cleaning up project directory and file based variables

Job succeeded
'''
