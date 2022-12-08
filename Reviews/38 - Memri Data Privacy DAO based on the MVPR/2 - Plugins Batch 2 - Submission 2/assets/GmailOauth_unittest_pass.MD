```Running with gitlab-runner 14.9.1 (bd40e3da)
  on gitlab memri public docker-runner Ryesm3zY
Preparing the "docker" executor
00:03
Using Docker executor with image python:3.7 ...
Starting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...
Authenticating with credentials from job payload (GitLab Registry)
Pulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...
Using docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...
Waiting for services to be up and running...
Pulling docker image python:3.7 ...
Using docker image sha256:3e36461b4ff4bafb4a3bf307fce984e1eec3abb1fb0cd55a651b807ce5569297 for python:3.7 with digest python@sha256:458fde344b3049edc578e709f25b22754e2d7fef0f730bdae46eaffba10733a8 ...
Preparing environment
00:01
Running on runner-ryesm3zy-project-481-concurrent-0 via 8e6b65718045...
Getting source from Git repository
00:01
Fetching changes with git depth set to 50...
Reinitialized existing Git repository in /builds/memri/plugins/gmail_oauth/.git/
Checking out e720cc4b as dev...
Removing .mypy_cache/
Removing .pytest_cache/
Removing gmail_oauth.egg-info/
Removing gmail_oauth/__pycache__/
Removing tests/__pycache__/
Skipping Git submodules setup
Executing "step_script" stage of the job script
02:13
Using docker image sha256:3e36461b4ff4bafb4a3bf307fce984e1eec3abb1fb0cd55a651b807ce5569297 for python:3.7 with digest python@sha256:458fde344b3049edc578e709f25b22754e2d7fef0f730bdae46eaffba10733a8 ...
$ pip install -e .
Obtaining file:///builds/memri/plugins/gmail_oauth
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting simplegmail~=4.0.4
  Downloading simplegmail-4.0.4-py3-none-any.whl (18 kB)
Collecting pytest~=7.0
  Downloading pytest-7.2.0-py3-none-any.whl (316 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 316.8/316.8 KB 5.2 MB/s eta 0:00:00
Collecting pymemri==0.0.34
  Downloading pymemri-0.0.34-py3-none-any.whl (68 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 68.9/68.9 KB 10.7 MB/s eta 0:00:00
Collecting loguru~=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 6.9 MB/s eta 0:00:00
Collecting pre-commit~=2.20
  Downloading pre_commit-2.20.0-py2.py3-none-any.whl (199 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 199.5/199.5 KB 23.7 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 3.0 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 20.7 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 37.7 MB/s eta 0:00:00
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 10.6 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting pandas
  Downloading pandas-1.3.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.3/11.3 MB 54.2 MB/s eta 0:00:00
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 6.8 MB/s eta 0:00:00
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (11.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.8/11.8 MB 53.3 MB/s eta 0:00:00
Collecting requests
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 286.1 kB/s eta 0:00:00
Collecting tqdm
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 KB 5.5 MB/s eta 0:00:00
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 7.6 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.5.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (45 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 45.9/45.9 KB 6.1 MB/s eta 0:00:00
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pyyaml<7.0.0,>=5.3.1
  Downloading PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (596 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 596.3/596.3 KB 32.8 MB/s eta 0:00:00
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.2-cp37-cp37m-manylinux_2_28_x86_64.whl (144 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 144.7/144.7 KB 17.7 MB/s eta 0:00:00
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 6.5 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.0-py2.py3-none-any.whl (22 kB)
Requirement already satisfied: pip in /usr/local/lib/python3.7/site-packages (from fastcore==1.3.21->pymemri==0.0.34->gmail-oauth==0.0.1) (22.0.4)
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 KB 5.5 MB/s eta 0:00:00
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 KB 7.6 MB/s eta 0:00:00
Collecting typing-extensions>=3.7.4.3
  Downloading typing_extensions-4.4.0-py3-none-any.whl (26 kB)
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 11.9 MB/s eta 0:00:00
Collecting toml
  Downloading toml-0.10.2-py2.py3-none-any.whl (16 kB)
Collecting virtualenv>=20.0.8
  Downloading virtualenv-20.16.7-py3-none-any.whl (8.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.8/8.8 MB 51.6 MB/s eta 0:00:00
Collecting identify>=1.0.0
  Downloading identify-2.5.9-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.8/98.8 KB 12.8 MB/s eta 0:00:00
Collecting importlib-metadata
  Downloading importlib_metadata-5.0.0-py3-none-any.whl (21 kB)
Collecting nodeenv>=0.11.1
  Downloading nodeenv-1.7.0-py2.py3-none-any.whl (21 kB)
Collecting cfgv>=2.0.0
  Downloading cfgv-3.3.1-py2.py3-none-any.whl (7.3 kB)
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.0.4-py3-none-any.whl (14 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 KB 8.4 MB/s eta 0:00:00
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting oauth2client>=4.1.3
  Downloading oauth2client-4.1.3-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.2/98.2 KB 11.3 MB/s eta 0:00:00
Collecting google-api-python-client>=1.7.3
  Downloading google_api_python_client-2.66.0-py2.py3-none-any.whl (10.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 10.5/10.5 MB 58.2 MB/s eta 0:00:00
Collecting bs4>=0.0.1
  Downloading bs4-0.0.1.tar.gz (1.1 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting python-dateutil>=2.8.1
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 KB 22.0 MB/s eta 0:00:00
Collecting lxml>=4.4.2
  Downloading lxml-4.9.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl (6.4 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 6.4/6.4 MB 60.2 MB/s eta 0:00:00
Collecting beautifulsoup4
  Downloading beautifulsoup4-4.11.1-py3-none-any.whl (128 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 128.2/128.2 KB 17.6 MB/s eta 0:00:00
Collecting google-auth<3.0.0dev,>=1.19.0
  Downloading google_auth-2.14.1-py2.py3-none-any.whl (175 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 175.4/175.4 KB 17.8 MB/s eta 0:00:00
Collecting google-api-core!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0,<3.0.0dev,>=1.31.5
  Downloading google_api_core-2.10.2-py3-none-any.whl (115 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 115.6/115.6 KB 14.6 MB/s eta 0:00:00
Collecting httplib2<1dev,>=0.15.0
  Downloading httplib2-0.21.0-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.8/96.8 KB 12.5 MB/s eta 0:00:00
Collecting google-auth-httplib2>=0.1.0
  Downloading google_auth_httplib2-0.1.0-py2.py3-none-any.whl (9.3 kB)
Collecting uritemplate<5,>=3.0.1
  Downloading uritemplate-4.1.1-py2.py3-none-any.whl (10 kB)
Collecting zipp>=0.5
  Downloading zipp-3.10.0-py3-none-any.whl (6.2 kB)
Requirement already satisfied: setuptools in /usr/local/lib/python3.7/site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->gmail-oauth==0.0.1) (57.5.0)
Collecting rsa>=3.1.4
  Downloading rsa-4.9-py3-none-any.whl (34 kB)
Collecting six>=1.6.1
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting pyasn1-modules>=0.0.5
  Downloading pyasn1_modules-0.2.8-py2.py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 KB 16.7 MB/s eta 0:00:00
Collecting pyasn1>=0.1.7
  Downloading pyasn1-0.4.8-py2.py3-none-any.whl (77 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 77.1/77.1 KB 8.7 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 KB 18.0 MB/s eta 0:00:00
Collecting certifi>=2017.4.17
  Downloading certifi-2022.9.24-py3-none-any.whl (161 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 161.1/161.1 KB 17.1 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 6.9 MB/s eta 0:00:00
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting platformdirs<3,>=2.4
  Downloading platformdirs-2.5.4-py3-none-any.whl (14 kB)
Collecting filelock<4,>=3.4.1
  Downloading filelock-3.8.0-py3-none-any.whl (10 kB)
Collecting distlib<1,>=0.3.6
  Downloading distlib-0.3.6-py2.py3-none-any.whl (468 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 468.5/468.5 KB 28.7 MB/s eta 0:00:00
Collecting pyparsing!=3.0.5,>=2.0.2
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 11.3 MB/s eta 0:00:00
Collecting pytz>=2017.3
  Downloading pytz-2022.6-py2.py3-none-any.whl (498 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 498.1/498.1 KB 32.5 MB/s eta 0:00:00
Collecting numpy>=1.17.3
  Downloading numpy-1.21.6-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (15.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 15.7/15.7 MB 51.0 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 KB 22.9 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting googleapis-common-protos<2.0dev,>=1.56.2
  Downloading googleapis_common_protos-1.57.0-py2.py3-none-any.whl (217 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 218.0/218.0 KB 25.3 MB/s eta 0:00:00
Collecting protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
  Downloading protobuf-4.21.9-cp37-abi3-manylinux2014_x86_64.whl (408 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 408.4/408.4 KB 34.5 MB/s eta 0:00:00
Collecting cachetools<6.0,>=2.0.0
  Downloading cachetools-5.2.0-py3-none-any.whl (9.3 kB)
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 13.0 MB/s eta 0:00:00
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 8.4 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting websockets>=10.0
  Downloading websockets-10.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.7/106.7 KB 13.7 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 63.9 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (404 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 404.7/404.7 KB 32.6 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting soupsieve>1.2
  Downloading soupsieve-2.3.2.post1-py3-none-any.whl (37 kB)
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Building wheels for collected packages: bs4, python-multipart
  Building wheel for bs4 (setup.py): started
  Building wheel for bs4 (setup.py): finished with status 'done'
  Created wheel for bs4: filename=bs4-0.0.1-py3-none-any.whl size=1271 sha256=c4fdcc47a12779c452b41995ad5770fc2d6937f9a8381be0a75c36e3ababc18c
  Stored in directory: /root/.cache/pip/wheels/0a/9e/ba/20e5bbc1afef3a491f0b3bb74d508f99403aabe76eda2167ca
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=f5473158a542f142cd98f737ea7ab31194801313ad679d1da1a69b11b7d7cd2e
  Stored in directory: /root/.cache/pip/wheels/2c/41/7c/bfd1c180534ffdcc0972f78c5758f89881602175d48a8bcd2c
Successfully built bs4 python-multipart
Installing collected packages: pytz, pyasn1, iniconfig, distlib, zipp, websockets, uvloop, urllib3, uritemplate, ujson, typing-extensions, tqdm, tomli, toml, soupsieve, sniffio, smmap, six, rsa, pyyaml, python-dotenv, pyparsing, pyasn1-modules, protobuf, platformdirs, pillow, orjson, numpy, nodeenv, MarkupSafe, lxml, loguru, itsdangerous, idna, identify, httptools, giturlparse, filelock, fastprogress, exceptiongroup, dnspython, charset-normalizer, cfgv, certifi, cachetools, attrs, requests, python-multipart, python-dateutil, pydantic, packaging, jinja2, importlib-metadata, httplib2, h11, googleapis-common-protos, google-auth, gitdb, email_validator, beautifulsoup4, asgiref, anyio, watchgod, virtualenv, starlette, pluggy, pandas, oauth2client, google-auth-httplib2, google-api-core, GitPython, fastscript, fastcore, click, bs4, uvicorn, pytest, pre-commit, google-api-python-client, fastapi, simplegmail, pymemri, gmail-oauth
  Running setup.py develop for gmail-oauth
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.1 anyio-3.6.2 asgiref-3.5.2 attrs-22.1.0 beautifulsoup4-4.11.1 bs4-0.0.1 cachetools-5.2.0 certifi-2022.9.24 cfgv-3.3.1 charset-normalizer-2.1.1 click-8.1.3 distlib-0.3.6 dnspython-2.2.1 email_validator-1.3.0 exceptiongroup-1.0.4 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 filelock-3.8.0 gitdb-4.0.9 giturlparse-0.10.0 gmail-oauth-0.0.1 google-api-core-2.10.2 google-api-python-client-2.66.0 google-auth-2.14.1 google-auth-httplib2-0.1.0 googleapis-common-protos-1.57.0 h11-0.14.0 httplib2-0.21.0 httptools-0.5.0 identify-2.5.9 idna-3.4 importlib-metadata-5.0.0 iniconfig-1.1.1 itsdangerous-2.1.2 jinja2-3.0.0 loguru-0.6.0 lxml-4.9.1 nodeenv-1.7.0 numpy-1.21.6 oauth2client-4.1.3 orjson-3.8.2 packaging-21.3 pandas-1.3.5 pillow-8.4.0 platformdirs-2.5.4 pluggy-1.0.0 pre-commit-2.20.0 protobuf-4.21.9 pyasn1-0.4.8 pyasn1-modules-0.2.8 pydantic-1.10.2 pymemri-0.0.34 pyparsing-3.0.9 pytest-7.2.0 python-dateutil-2.8.2 python-dotenv-0.21.0 python-multipart-0.0.5 pytz-2022.6 pyyaml-6.0 requests-2.28.1 rsa-4.9 simplegmail-4.0.4 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 soupsieve-2.3.2.post1 starlette-0.19.1 toml-0.10.2 tomli-2.0.1 tqdm-4.64.1 typing-extensions-4.4.0 ujson-5.5.0 uritemplate-4.1.1 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.17.0 virtualenv-20.16.7 watchgod-0.8.2 websockets-10.4 zipp-3.10.0
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
$ curl http://pod:3030/version
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    58  100    58    0     0  58000      0 --:--:-- --:--:-- --:--:-- 58000
{"build_profile":null,"cargo":"0.4.4","git_describe":null}$ export POD_ADDRESS='http://pod:3030'
$ pre-commit run --all-files
[INFO] Initializing environment for https://github.com/psf/black.
[INFO] Initializing environment for https://github.com/pycqa/isort.
[INFO] Initializing environment for https://github.com/pycqa/flake8.
[INFO] Initializing environment for https://github.com/pre-commit/mirrors-mypy.
[INFO] Initializing environment for https://github.com/pre-commit/mirrors-mypy:types-all.
[INFO] Installing environment for https://github.com/psf/black.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pycqa/isort.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pycqa/flake8.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
[INFO] Installing environment for https://github.com/pre-commit/mirrors-mypy.
[INFO] Once installed this environment will be reused.
[INFO] This may take a few minutes...
black....................................................................Passed
isort (python)...........................................................Passed
flake8...................................................................Passed
mypy.....................................................................Passed
$ pytest
============================= test session starts ==============================
platform linux -- Python 3.7.15, pytest-7.2.0, pluggy-1.0.0
rootdir: /builds/memri/plugins/gmail_oauth
plugins: anyio-3.6.2
collected 6 items
tests/test_gmail_api.py ......                                           [100%]
=============================== warnings summary ===============================
tests/test_gmail_api.py::test_import_emails
  /usr/local/lib/python3.7/site-packages/pymemri/plugin/pluginbase.py:31: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    RuntimeWarning,
-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
========================= 6 passed, 1 warning in 6.35s =========================
Cleaning up project directory and file based variables
00:00
Job succeeded```