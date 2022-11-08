```[0KRunning with gitlab-runner 14.9.1 (bd40e3da)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1662735245:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.7 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-89f290c7 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-89f290c7 ...[0;m
[0KUsing docker image sha256:955f3d33e9a46f954ca86ea4016346586359981df75f968e8084f6340f2f19bf for gitlab.memri.io:5050/memri/pod:dev-89f290c7 with digest gitlab.memri.io:5050/memri/pod@sha256:992a24d9be08ab2afc2627ead974f00a790271dd28722e447e48faa26e0ccf93 ...[0;m
[0KWaiting for services to be up and running...[0;m
[0KPulling docker image python:3.7 ...[0;m
[0KUsing docker image sha256:c6373d2e1919b2229892190631b289e66032692885970c473035e25a1d7bdcd5 for python:3.7 with digest python@sha256:813b686c9bee9846a523cbeb14affb4996190b0b3473cd72d6e57f912c1fb3b8 ...[0;m
section_end:1662735250:prepare_executor
[0Ksection_start:1662735250:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-167-concurrent-0 via 8e6b65718045...
section_end:1662735250:prepare_script
[0Ksection_start:1662735250:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 50...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/sentiment_plugin/.git/
[32;1mChecking out 6f0e0ba6 as main...[0;m
Removing .pytest_cache/
Removing sentiment_plugin.egg-info/
Removing sentiment_plugin/__pycache__/
Removing tests/__pycache__/

[32;1mSkipping Git submodules setup[0;m
section_end:1662735252:get_sources
[0Ksection_start:1662735252:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:c6373d2e1919b2229892190631b289e66032692885970c473035e25a1d7bdcd5 for python:3.7 with digest python@sha256:813b686c9bee9846a523cbeb14affb4996190b0b3473cd72d6e57f912c1fb3b8 ...[0;m
[32;1m$ pip install -e .[0;m
Obtaining file:///builds/memri/plugins/sentiment_plugin
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.23
  Cloning https://gitlab.memri.io/memri/pymemri.git (to revision v0.0.23) to /tmp/pip-install-eud85yl9/pymemri_6bc3e0a24f5341a391585f9817c6215b
  Running command git clone --filter=blob:none --quiet https://gitlab.memri.io/memri/pymemri.git /tmp/pip-install-eud85yl9/pymemri_6bc3e0a24f5341a391585f9817c6215b
  Running command git checkout -q 55981e6f0978d97fa46b7c8952fb1aa3d7357ade
  Resolved https://gitlab.memri.io/memri/pymemri.git to commit 55981e6f0978d97fa46b7c8952fb1aa3d7357ade
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pytest
  Downloading pytest-7.1.3-py3-none-any.whl (298 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 298.2/298.2 KB 27.8 MB/s eta 0:00:00
Collecting torch==1.10.0
  Downloading torch-1.10.0-cp37-cp37m-manylinux1_x86_64.whl (881.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 881.9/881.9 MB 3.0 MB/s eta 0:00:00
Collecting transformers
  Downloading transformers-4.21.3-py3-none-any.whl (4.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.7/4.7 MB 68.1 MB/s eta 0:00:00
Collecting sentencepiece
  Downloading sentencepiece-0.1.97-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (1.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.3/1.3 MB 62.5 MB/s eta 0:00:00
Collecting protobuf==3.20.*
  Downloading protobuf-3.20.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.0/1.0 MB 74.5 MB/s eta 0:00:00
Collecting typing-extensions
  Downloading typing_extensions-4.3.0-py3-none-any.whl (25 kB)
Collecting requests
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 15.3 MB/s eta 0:00:00
Collecting tqdm
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 KB 13.9 MB/s eta 0:00:00
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
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 11.4 MB/s eta 0:00:00
Collecting nbdev==1.1.21
  Downloading nbdev-1.1.21-py3-none-any.whl (46 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 46.9/46.9 KB 7.4 MB/s eta 0:00:00
Collecting matplotlib
  Downloading matplotlib-3.5.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (11.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.2/11.2 MB 60.1 MB/s eta 0:00:00
Collecting jupyter-client==6.1.12
  Downloading jupyter_client-6.1.12-py3-none-any.whl (112 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 112.7/112.7 KB 15.2 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 9.0 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting pandas
  Downloading pandas-1.3.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.3/11.3 MB 81.4 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 85.0 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 31.0 MB/s eta 0:00:00
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 21.6 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 12.6 MB/s eta 0:00:00
Collecting pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
  Downloading pydantic-1.10.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.8/11.8 MB 75.5 MB/s eta 0:00:00
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (45 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 45.3/45.3 KB 5.8 MB/s eta 0:00:00
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.0-cp37-cp37m-manylinux_2_28_x86_64.whl (145 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 145.9/145.9 KB 22.5 MB/s eta 0:00:00
Collecting pyyaml<7.0.0,>=5.3.1
  Downloading PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (596 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 596.3/596.3 KB 42.7 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.2.1-py2.py3-none-any.whl (22 kB)
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 1.6 MB/s eta 0:00:00
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 KB 7.2 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.7/site-packages (from fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.23->sentiment-plugin==0.0.2) (22.0.4)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 KB 10.3 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting tornado>=4.1
  Downloading tornado-6.2-cp37-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (423 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 424.0/424.0 KB 42.8 MB/s eta 0:00:00
Collecting traitlets
  Downloading traitlets-5.3.0-py3-none-any.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.8/106.8 KB 21.3 MB/s eta 0:00:00
Collecting pyzmq>=13
  Downloading pyzmq-23.2.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 64.2 MB/s eta 0:00:00
Collecting python-dateutil>=2.1
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 KB 40.1 MB/s eta 0:00:00
Collecting jupyter-core>=4.6.0
  Downloading jupyter_core-4.11.1-py3-none-any.whl (88 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 88.4/88.4 KB 16.5 MB/s eta 0:00:00
Collecting nbconvert<6
  Downloading nbconvert-5.6.1-py2.py3-none-any.whl (455 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 455.1/455.1 KB 49.3 MB/s eta 0:00:00
Collecting ipykernel
  Downloading ipykernel-6.15.2-py3-none-any.whl (132 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 132.9/132.9 KB 31.0 MB/s eta 0:00:00
Collecting ghapi
  Downloading ghapi-1.0.2-py3-none-any.whl (57 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 57.7/57.7 KB 13.6 MB/s eta 0:00:00
Collecting nbformat>=4.4.0
  Downloading nbformat-5.4.0-py3-none-any.whl (73 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 73.3/73.3 KB 17.5 MB/s eta 0:00:00
Collecting jupyter
  Downloading jupyter-1.0.0-py2.py3-none-any.whl (2.7 kB)
Collecting fastrelease
  Downloading fastrelease-0.1.17-py3-none-any.whl (13 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.1-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 16.9 MB/s eta 0:00:00
Collecting importlib-metadata>=0.12
  Downloading importlib_metadata-4.12.0-py3-none-any.whl (21 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 KB 12.1 MB/s eta 0:00:00
Collecting py>=1.8.2
  Downloading py-1.11.0-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.7/98.7 KB 21.0 MB/s eta 0:00:00
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting filelock
  Downloading filelock-3.8.0-py3-none-any.whl (10 kB)
Collecting regex!=2019.12.17
  Downloading regex-2022.8.17-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (752 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 752.6/752.6 KB 66.8 MB/s eta 0:00:00
Collecting tokenizers!=0.11.3,<0.13,>=0.11.1
  Downloading tokenizers-0.12.1-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (6.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 6.6/6.6 MB 69.9 MB/s eta 0:00:00
Collecting numpy>=1.17
  Downloading numpy-1.21.6-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (15.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 15.7/15.7 MB 72.8 MB/s eta 0:00:00
Collecting huggingface-hub<1.0,>=0.1.0
  Downloading huggingface_hub-0.9.1-py3-none-any.whl (120 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.7/120.7 KB 20.7 MB/s eta 0:00:00
Collecting zipp>=0.5
  Downloading zipp-3.8.1-py3-none-any.whl (5.6 kB)
Collecting pyparsing!=3.0.5,>=2.0.2
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 19.6 MB/s eta 0:00:00
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting certifi>=2017.4.17
  Downloading certifi-2022.6.15.1-py3-none-any.whl (160 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 160.4/160.4 KB 25.2 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 KB 22.0 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.3-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.2/61.2 KB 9.6 MB/s eta 0:00:00
Requirement already satisfied: setuptools in /usr/local/lib/python3.7/site-packages (from ipdb->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.23->sentiment-plugin==0.0.2) (57.5.0)
Collecting ipython>=7.17.0
  Downloading ipython-7.34.0-py3-none-any.whl (793 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 793.8/793.8 KB 52.0 MB/s eta 0:00:00
Collecting toml>=0.10.2
  Downloading toml-0.10.2-py2.py3-none-any.whl (16 kB)
Collecting decorator
  Downloading decorator-5.1.1-py3-none-any.whl (9.1 kB)
Collecting fonttools>=4.22.0
  Downloading fonttools-4.37.1-py3-none-any.whl (957 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 957.2/957.2 KB 62.6 MB/s eta 0:00:00
Collecting kiwisolver>=1.0.1
  Downloading kiwisolver-1.4.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 61.4 MB/s eta 0:00:00
Collecting cycler>=0.10
  Downloading cycler-0.11.0-py3-none-any.whl (6.4 kB)
Collecting pytz>=2017.3
  Downloading pytz-2022.2.1-py2.py3-none-any.whl (500 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 500.6/500.6 KB 50.1 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 KB 42.9 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting backcall
  Downloading backcall-0.2.0-py2.py3-none-any.whl (11 kB)
Collecting matplotlib-inline
  Downloading matplotlib_inline-0.1.6-py3-none-any.whl (9.4 kB)
Collecting jedi>=0.16
  Downloading jedi-0.18.1-py2.py3-none-any.whl (1.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.6/1.6 MB 70.8 MB/s eta 0:00:00
Collecting pygments
  Downloading Pygments-2.13.0-py3-none-any.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 9.5 MB/s eta 0:00:00
Collecting pickleshare
  Downloading pickleshare-0.7.5-py2.py3-none-any.whl (6.9 kB)
Collecting prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0
  Downloading prompt_toolkit-3.0.31-py3-none-any.whl (382 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 382.3/382.3 KB 51.9 MB/s eta 0:00:00
Collecting pexpect>4.3
  Downloading pexpect-4.8.0-py2.py3-none-any.whl (59 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 59.0/59.0 KB 10.8 MB/s eta 0:00:00
Collecting testpath
  Downloading testpath-0.6.0-py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.9/83.9 KB 22.6 MB/s eta 0:00:00
Collecting bleach
  Downloading bleach-5.0.1-py3-none-any.whl (160 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 160.9/160.9 KB 32.3 MB/s eta 0:00:00
Collecting mistune<2,>=0.8.1
  Downloading mistune-0.8.4-py2.py3-none-any.whl (16 kB)
Collecting defusedxml
  Downloading defusedxml-0.7.1-py2.py3-none-any.whl (25 kB)
Collecting entrypoints>=0.2.2
  Downloading entrypoints-0.4-py3-none-any.whl (5.3 kB)
Collecting pandocfilters>=1.4.1
  Downloading pandocfilters-1.5.0-py2.py3-none-any.whl (8.7 kB)
Collecting fastjsonschema
  Downloading fastjsonschema-2.16.1-py3-none-any.whl (22 kB)
Collecting jsonschema>=2.6
  Downloading jsonschema-4.16.0-py3-none-any.whl (83 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 83.1/83.1 KB 19.0 MB/s eta 0:00:00
Collecting six>=1.5
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting h11>=0.8
  Downloading h11-0.13.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.2/58.2 KB 10.9 MB/s eta 0:00:00
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 17.2 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting httptools>=0.4.0
  Downloading httptools-0.4.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (406 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 406.7/406.7 KB 49.6 MB/s eta 0:00:00
Collecting websockets>=10.0
  Downloading websockets-10.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (112 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 112.1/112.1 KB 22.3 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.16.0-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (3.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.8/3.8 MB 68.3 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting ghapi
  Downloading ghapi-1.0.1-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.5/58.5 KB 14.4 MB/s eta 0:00:00
  Downloading ghapi-1.0.0-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 15.3 MB/s eta 0:00:00
  Downloading ghapi-0.1.23-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 15.3 MB/s eta 0:00:00
  Downloading ghapi-0.1.22-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.3/55.3 KB 13.3 MB/s eta 0:00:00
Collecting psutil
  Downloading psutil-5.9.2-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (281 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 281.3/281.3 KB 36.6 MB/s eta 0:00:00
Collecting debugpy>=1.0
  Downloading debugpy-1.6.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (1.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.8/1.8 MB 31.1 MB/s eta 0:00:00
Collecting nest-asyncio
  Downloading nest_asyncio-1.5.5-py3-none-any.whl (5.2 kB)
Collecting notebook
  Downloading notebook-6.4.12-py3-none-any.whl (9.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.9/9.9 MB 67.5 MB/s eta 0:00:00
Collecting qtconsole
  Downloading qtconsole-5.3.2-py3-none-any.whl (120 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.8/120.8 KB 26.5 MB/s eta 0:00:00
Collecting jupyter-console
  Downloading jupyter_console-6.4.4-py3-none-any.whl (22 kB)
Collecting ipywidgets
  Downloading ipywidgets-8.0.2-py3-none-any.whl (134 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 134.4/134.4 KB 32.0 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Collecting parso<0.9.0,>=0.8.0
  Downloading parso-0.8.3-py2.py3-none-any.whl (100 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100.8/100.8 KB 25.7 MB/s eta 0:00:00
Collecting pkgutil-resolve-name>=1.3.10
  Downloading pkgutil_resolve_name-1.3.10-py3-none-any.whl (4.7 kB)
Collecting importlib-resources>=1.4.0
  Downloading importlib_resources-5.9.0-py3-none-any.whl (33 kB)
Collecting pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0
  Downloading pyrsistent-0.18.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (117 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 117.1/117.1 KB 4.2 MB/s eta 0:00:00
Collecting ptyprocess>=0.5
  Downloading ptyprocess-0.7.0-py2.py3-none-any.whl (13 kB)
Collecting wcwidth
  Downloading wcwidth-0.2.5-py2.py3-none-any.whl (30 kB)
Collecting webencodings
  Downloading webencodings-0.5.1-py2.py3-none-any.whl (11 kB)
Collecting jupyterlab-widgets~=3.0
  Downloading jupyterlab_widgets-3.0.3-py3-none-any.whl (384 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 384.1/384.1 KB 4.8 MB/s eta 0:00:00
Collecting widgetsnbextension~=4.0
  Downloading widgetsnbextension-4.0.3-py3-none-any.whl (2.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.0/2.0 MB 79.4 MB/s eta 0:00:00
Collecting jupyter-console
  Downloading jupyter_console-6.4.3-py3-none-any.whl (22 kB)
  Downloading jupyter_console-6.4.2-py3-none-any.whl (23 kB)
Collecting prometheus-client
  Downloading prometheus_client-0.14.1-py3-none-any.whl (59 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 59.5/59.5 KB 13.7 MB/s eta 0:00:00
Collecting argon2-cffi
  Downloading argon2_cffi-21.3.0-py3-none-any.whl (14 kB)
Collecting ipython-genutils
  Downloading ipython_genutils-0.2.0-py2.py3-none-any.whl (26 kB)
Collecting Send2Trash>=1.8.0
  Downloading Send2Trash-1.8.0-py3-none-any.whl (18 kB)
Collecting terminado>=0.8.3
  Downloading terminado-0.15.0-py3-none-any.whl (16 kB)
Collecting qtpy>=2.0.1
  Downloading QtPy-2.2.0-py3-none-any.whl (82 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 82.3/82.3 KB 7.4 MB/s eta 0:00:00
Collecting argon2-cffi-bindings
  Downloading argon2_cffi_bindings-21.2.0-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (86 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 86.2/86.2 KB 21.2 MB/s eta 0:00:00
Collecting cffi>=1.0.1
  Downloading cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (427 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 427.9/427.9 KB 42.1 MB/s eta 0:00:00
Collecting pycparser
  Downloading pycparser-2.21-py2.py3-none-any.whl (118 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 118.7/118.7 KB 24.5 MB/s eta 0:00:00
Building wheels for collected packages: pymemri, ipdb, python-multipart
  Building wheel for pymemri (setup.py): started
  Building wheel for pymemri (setup.py): finished with status 'done'
  Created wheel for pymemri: filename=pymemri-0.0.17-py3-none-any.whl size=75224 sha256=29c90ff13c40d6f4f625a8c5e8c03784e1ddd85b7c709b21da85e7b9078e3a80
  Stored in directory: /tmp/pip-ephem-wheel-cache-r3m1emj5/wheels/b2/a7/d9/42223f3ae752969a703efc0541f5bcbf1434506552772e9474
  Building wheel for ipdb (setup.py): started
  Building wheel for ipdb (setup.py): finished with status 'done'
  Created wheel for ipdb: filename=ipdb-0.13.9-py3-none-any.whl size=11648 sha256=9e73f3eddfc7c7b81a438ffc0f2f9df7ac6d3f12019fc73206b6989d586f7d25
  Stored in directory: /root/.cache/pip/wheels/65/cd/cc/aaf92acae337a28fdd2aa4d632196a59745c8c39f76eaeed01
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=fe8458b1481c66ce36b1192f1a6ce6473274dc119a29fc41733b6303ae3e7396
  Stored in directory: /root/.cache/pip/wheels/2c/41/7c/bfd1c180534ffdcc0972f78c5758f89881602175d48a8bcd2c
Successfully built pymemri ipdb python-multipart
Installing collected packages: webencodings, wcwidth, tokenizers, sentencepiece, Send2Trash, pytz, ptyprocess, pickleshare, mistune, ipython-genutils, iniconfig, fastjsonschema, backcall, zipp, widgetsnbextension, websockets, uvloop, urllib3, ujson, typing-extensions, traitlets, tqdm, tornado, tomli, toml, testpath, sniffio, smmap, six, regex, pyzmq, pyyaml, python-dotenv, pyrsistent, pyparsing, pygments, pycparser, py, psutil, protobuf, prompt-toolkit, prometheus-client, pkgutil-resolve-name, pillow, pexpect, parso, pandocfilters, orjson, numpy, nest-asyncio, MarkupSafe, jupyterlab-widgets, itsdangerous, idna, httptools, giturlparse, fonttools, filelock, fastprogress, entrypoints, dnspython, defusedxml, decorator, debugpy, cycler, charset-normalizer, certifi, attrs, torch, terminado, requests, python-multipart, python-dateutil, pydantic, packaging, matplotlib-inline, kiwisolver, jupyter-core, jinja2, jedi, importlib-resources, importlib-metadata, h11, gitdb, email_validator, cffi, bleach, asgiref, anyio, watchgod, starlette, qtpy, pluggy, pandas, matplotlib, jupyter-client, jsonschema, ipython, huggingface-hub, GitPython, fastscript, fastcore, click, argon2-cffi-bindings, uvicorn, transformers, pytest, nbformat, ipykernel, ipdb, ghapi, fastapi, argon2-cffi, qtconsole, nbconvert, jupyter-console, ipywidgets, fastrelease, notebook, jupyter, nbdev, pymemri, sentiment-plugin
  Running setup.py develop for sentiment-plugin
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.1 Send2Trash-1.8.0 anyio-3.6.1 argon2-cffi-21.3.0 argon2-cffi-bindings-21.2.0 asgiref-3.5.2 attrs-22.1.0 backcall-0.2.0 bleach-5.0.1 certifi-2022.6.15.1 cffi-1.15.1 charset-normalizer-2.1.1 click-8.1.3 cycler-0.11.0 debugpy-1.6.3 decorator-5.1.1 defusedxml-0.7.1 dnspython-2.2.1 email_validator-1.2.1 entrypoints-0.4 fastapi-0.78.0 fastcore-1.3.21 fastjsonschema-2.16.1 fastprogress-1.0.3 fastrelease-0.1.17 fastscript-1.0.0 filelock-3.8.0 fonttools-4.37.1 ghapi-0.1.22 gitdb-4.0.9 giturlparse-0.10.0 h11-0.13.0 httptools-0.4.0 huggingface-hub-0.9.1 idna-3.3 importlib-metadata-4.12.0 importlib-resources-5.9.0 iniconfig-1.1.1 ipdb-0.13.9 ipykernel-6.15.2 ipython-7.34.0 ipython-genutils-0.2.0 ipywidgets-8.0.2 itsdangerous-2.1.2 jedi-0.18.1 jinja2-3.0.0 jsonschema-4.16.0 jupyter-1.0.0 jupyter-client-6.1.12 jupyter-console-6.4.2 jupyter-core-4.11.1 jupyterlab-widgets-3.0.3 kiwisolver-1.4.4 matplotlib-3.5.3 matplotlib-inline-0.1.6 mistune-0.8.4 nbconvert-5.6.1 nbdev-1.1.21 nbformat-5.4.0 nest-asyncio-1.5.5 notebook-6.4.12 numpy-1.21.6 orjson-3.8.0 packaging-21.3 pandas-1.3.5 pandocfilters-1.5.0 parso-0.8.3 pexpect-4.8.0 pickleshare-0.7.5 pillow-8.4.0 pkgutil-resolve-name-1.3.10 pluggy-1.0.0 prometheus-client-0.14.1 prompt-toolkit-3.0.31 protobuf-3.20.1 psutil-5.9.2 ptyprocess-0.7.0 py-1.11.0 pycparser-2.21 pydantic-1.10.2 pygments-2.13.0 pymemri-0.0.17 pyparsing-3.0.9 pyrsistent-0.18.1 pytest-7.1.3 python-dateutil-2.8.2 python-dotenv-0.21.0 python-multipart-0.0.5 pytz-2022.2.1 pyyaml-6.0 pyzmq-23.2.1 qtconsole-5.3.2 qtpy-2.2.0 regex-2022.8.17 requests-2.28.1 sentencepiece-0.1.97 sentiment-plugin-0.0.2 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 terminado-0.15.0 testpath-0.6.0 tokenizers-0.12.1 toml-0.10.2 tomli-2.0.1 torch-1.10.0 tornado-6.2 tqdm-4.64.1 traitlets-5.3.0 transformers-4.21.3 typing-extensions-4.3.0 ujson-5.4.0 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.16.0 watchgod-0.8.2 wcwidth-0.2.5 webencodings-0.5.1 websockets-10.3 widgetsnbextension-4.0.3 zipp-3.8.1
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.2.2 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100    58  100    58    0     0   5272      0 --:--:-- --:--:-- --:--:--  5272
{"build_profile":null,"cargo":"0.4.4","git_describe":null}[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pytest[0;m
============================= test session starts ==============================
platform linux -- Python 3.7.14, pytest-7.1.3, pluggy-1.0.0
rootdir: /builds/memri/plugins/sentiment_plugin
plugins: anyio-3.6.1
collected 1 item

tests/test_plugin.py .                                                   [100%]

=============================== warnings summary ===============================
tests/test_plugin.py::test_plugin
  /usr/local/lib/python3.7/site-packages/transformers/pipelines/text_classification.py:90: UserWarning: `return_all_scores` is now deprecated, use `top_k=1` if you want similar functionnality
    "`return_all_scores` is now deprecated, use `top_k=1` if you want similar functionnality", UserWarning

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
======================== 1 passed, 1 warning in 38.66s =========================
section_end:1662735382:step_script
[0Ksection_start:1662735382:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1662735382:cleanup_file_variables
[0K[32;1mJob succeeded[0;m```
