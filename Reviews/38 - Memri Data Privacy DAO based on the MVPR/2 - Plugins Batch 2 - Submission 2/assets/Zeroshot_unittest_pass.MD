```Running with gitlab-runner 14.9.1 (bd40e3da)
  on gitlab memri public docker-runner Ryesm3zY
Preparing the "docker" executor
00:07
Using Docker executor with image python:3.9 ...
Starting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...
Authenticating with credentials from job payload (GitLab Registry)
Pulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...
Using docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...
Waiting for services to be up and running...
Pulling docker image python:3.9 ...
Using docker image sha256:850f8694d221b7fba2358381b744c231cbe9096d3f3c888493f1889eccec25fb for python:3.9 with digest python@sha256:aa99b1963cc1e693bc06394de03fa541c4994a6fa69f746b0b97aa237a9ab0b5 ...
Preparing environment
00:01
Running on runner-ryesm3zy-project-630-concurrent-1 via 8e6b65718045...
Getting source from Git repository
00:01
Fetching changes with git depth set to 50...
Reinitialized existing Git repository in /builds/memri/plugins/zero-shot-plugin/.git/
Checking out c7b9796c as dev...
Removing .pytest_cache/
Removing tests/__pycache__/
Removing zero_shot_plugin.egg-info/
Removing zero_shot_plugin/__pycache__/
Skipping Git submodules setup
Executing "step_script" stage of the job script
04:14
Using docker image sha256:850f8694d221b7fba2358381b744c231cbe9096d3f3c888493f1889eccec25fb for python:3.9 with digest python@sha256:aa99b1963cc1e693bc06394de03fa541c4994a6fa69f746b0b97aa237a9ab0b5 ...
$ pip install -e .
Obtaining file:///builds/memri/plugins/zero-shot-plugin
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri==0.0.34
  Downloading pymemri-0.0.34-py3-none-any.whl (68 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 68.9/68.9 KB 3.3 MB/s eta 0:00:00
Collecting torch>=1.10
  Downloading torch-1.13.0-cp39-cp39-manylinux1_x86_64.whl (890.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 890.2/890.2 MB 1.7 MB/s eta 0:00:00
Collecting transformers>=4.20
  Downloading transformers-4.24.0-py3-none-any.whl (5.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 5.5/5.5 MB 60.1 MB/s eta 0:00:00
Collecting pytest
  Downloading pytest-7.2.0-py3-none-any.whl (316 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 316.8/316.8 KB 31.9 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 66.1 MB/s eta 0:00:00
Collecting loguru~=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 8.3 MB/s eta 0:00:00
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 13.2/13.2 MB 48.1 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 8.0 MB/s eta 0:00:00
Collecting requests
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 8.5 MB/s eta 0:00:00
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 15.8 MB/s eta 0:00:00
Collecting pandas
  Downloading pandas-1.5.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (12.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 12.2/12.2 MB 53.9 MB/s eta 0:00:00
Collecting tqdm
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 KB 10.9 MB/s eta 0:00:00
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 18.9 MB/s eta 0:00:00
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 6.8 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 8.8 MB/s eta 0:00:00
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (46 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 46.1/46.1 KB 6.5 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.0-py2.py3-none-any.whl (22 kB)
Collecting pyyaml<7.0.0,>=5.3.1
  Downloading PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (661 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 661.8/661.8 KB 37.5 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 8.5 MB/s eta 0:00:00
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.2-cp39-cp39-manylinux_2_28_x86_64.whl (144 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 144.8/144.8 KB 18.8 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.9/site-packages (from fastcore==1.3.21->pymemri==0.0.34->zero-shot-plugin==0.0.1) (22.0.4)
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 KB 5.9 MB/s eta 0:00:00
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 KB 8.0 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting typing-extensions>=4.1.0
  Downloading typing_extensions-4.4.0-py3-none-any.whl (26 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 12.8 MB/s eta 0:00:00
Collecting nvidia-cuda-nvrtc-cu11==11.7.99
  Downloading nvidia_cuda_nvrtc_cu11-11.7.99-2-py3-none-manylinux1_x86_64.whl (21.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 21.0/21.0 MB 50.1 MB/s eta 0:00:00
Collecting nvidia-cublas-cu11==11.10.3.66
  Downloading nvidia_cublas_cu11-11.10.3.66-py3-none-manylinux1_x86_64.whl (317.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 317.1/317.1 MB 5.2 MB/s eta 0:00:00
Collecting nvidia-cudnn-cu11==8.5.0.96
  Downloading nvidia_cudnn_cu11-8.5.0.96-2-py3-none-manylinux1_x86_64.whl (557.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 557.1/557.1 MB 3.0 MB/s eta 0:00:00
Collecting nvidia-cuda-runtime-cu11==11.7.99
  Downloading nvidia_cuda_runtime_cu11-11.7.99-py3-none-manylinux1_x86_64.whl (849 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 849.3/849.3 KB 45.3 MB/s eta 0:00:00
Requirement already satisfied: wheel in /usr/local/lib/python3.9/site-packages (from nvidia-cublas-cu11==11.10.3.66->torch>=1.10->zero-shot-plugin==0.0.1) (0.38.4)
Requirement already satisfied: setuptools in /usr/local/lib/python3.9/site-packages (from nvidia-cublas-cu11==11.10.3.66->torch>=1.10->zero-shot-plugin==0.0.1) (58.1.0)
Collecting regex!=2019.12.17
  Downloading regex-2022.10.31-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (769 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 770.0/770.0 KB 47.1 MB/s eta 0:00:00
Collecting tokenizers!=0.11.3,<0.14,>=0.11.1
  Downloading tokenizers-0.13.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (7.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 7.6/7.6 MB 62.4 MB/s eta 0:00:00
Collecting numpy>=1.17
  Downloading numpy-1.23.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 17.1/17.1 MB 55.7 MB/s eta 0:00:00
Collecting huggingface-hub<1.0,>=0.10.0
  Downloading huggingface_hub-0.11.0-py3-none-any.whl (182 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 182.1/182.1 KB 18.4 MB/s eta 0:00:00
Collecting filelock
  Downloading filelock-3.8.0-py3-none-any.whl (10 kB)
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 KB 3.0 MB/s eta 0:00:00
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.0.4-py3-none-any.whl (14 kB)
Collecting pyparsing!=3.0.5,>=2.0.2
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 10.1 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 KB 16.0 MB/s eta 0:00:00
Collecting certifi>=2017.4.17
  Downloading certifi-2022.9.24-py3-none-any.whl (161 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 161.1/161.1 KB 15.3 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 8.7 MB/s eta 0:00:00
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting pytz>=2020.1
  Downloading pytz-2022.6-py2.py3-none-any.whl (498 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 498.1/498.1 KB 32.5 MB/s eta 0:00:00
Collecting python-dateutil>=2.8.1
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 KB 25.2 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 KB 28.3 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting six>=1.5
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 7.9 MB/s eta 0:00:00
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 12.9 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting websockets>=10.0
  Downloading websockets-10.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.5/106.5 KB 11.7 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 60.0 MB/s eta 0:00:00
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (417 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 417.9/417.9 KB 31.0 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Building wheels for collected packages: python-multipart
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=c1314355f358cc1047877c9326464467967c5b44968c8322089d3de4a05412ab
  Stored in directory: /root/.cache/pip/wheels/fe/04/d1/a10661cc45f03c3cecda50deb2d2c22f57b4e84a75b2a5987e
Successfully built python-multipart
Installing collected packages: tokenizers, pytz, iniconfig, websockets, uvloop, urllib3, ujson, typing-extensions, tqdm, tomli, sniffio, smmap, six, regex, pyyaml, python-dotenv, pyparsing, pluggy, pillow, orjson, nvidia-cuda-runtime-cu11, nvidia-cuda-nvrtc-cu11, nvidia-cublas-cu11, numpy, MarkupSafe, loguru, itsdangerous, idna, httptools, h11, giturlparse, filelock, fastprogress, exceptiongroup, dnspython, click, charset-normalizer, certifi, attrs, asgiref, uvicorn, requests, python-multipart, python-dateutil, pydantic, packaging, nvidia-cudnn-cu11, jinja2, gitdb, email_validator, anyio, watchgod, torch, starlette, pytest, pandas, huggingface-hub, GitPython, fastscript, fastcore, transformers, fastapi, pymemri, zero-shot-plugin
  Running setup.py develop for zero-shot-plugin
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.1 anyio-3.6.2 asgiref-3.5.2 attrs-22.1.0 certifi-2022.9.24 charset-normalizer-2.1.1 click-8.1.3 dnspython-2.2.1 email_validator-1.3.0 exceptiongroup-1.0.4 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 filelock-3.8.0 gitdb-4.0.9 giturlparse-0.10.0 h11-0.14.0 httptools-0.5.0 huggingface-hub-0.11.0 idna-3.4 iniconfig-1.1.1 itsdangerous-2.1.2 jinja2-3.0.0 loguru-0.6.0 numpy-1.23.5 nvidia-cublas-cu11-11.10.3.66 nvidia-cuda-nvrtc-cu11-11.7.99 nvidia-cuda-runtime-cu11-11.7.99 nvidia-cudnn-cu11-8.5.0.96 orjson-3.8.2 packaging-21.3 pandas-1.5.2 pillow-8.4.0 pluggy-1.0.0 pydantic-1.10.2 pymemri-0.0.34 pyparsing-3.0.9 pytest-7.2.0 python-dateutil-2.8.2 python-dotenv-0.21.0 python-multipart-0.0.5 pytz-2022.6 pyyaml-6.0 regex-2022.10.31 requests-2.28.1 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tokenizers-0.13.2 tomli-2.0.1 torch-1.13.0 tqdm-4.64.1 transformers-4.24.0 typing-extensions-4.4.0 ujson-5.5.0 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.17.0 watchgod-0.8.2 websockets-10.4 zero-shot-plugin-0.0.1
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
$ curl http://pod:3030/version
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    58  100    58    0     0   1208      0 --:--:-- --:--:-- --:--:--  1208
{"build_profile":null,"cargo":"0.4.4","git_describe":null}$ export POD_ADDRESS='http://pod:3030'
$ pytest
============================= test session starts ==============================
platform linux -- Python 3.9.15, pytest-7.2.0, pluggy-1.0.0
rootdir: /builds/memri/plugins/zero-shot-plugin
plugins: anyio-3.6.2
collected 2 items
tests/test_plugin.py ..                                                  [100%]
=============================== warnings summary ===============================
tests/test_plugin.py::test_predict_sentences
tests/test_plugin.py::test_predict_items
  /usr/local/lib/python3.9/site-packages/pymemri/plugin/pluginbase.py:29: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    warnings.warn(
-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
=================== 2 passed, 2 warnings in 98.19s (0:01:38) ===================
Cleaning up project directory and file based variables
00:01
Job succeeded```