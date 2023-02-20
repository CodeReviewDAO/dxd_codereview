```
[0KRunning with gitlab-runner 15.7.1 (6d480948)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1674647187:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.9 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...[0;m
[0KUsing docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...[0;m
[0KWaiting for services to be up and running (timeout 30 seconds)...[0;m
[0KPulling docker image python:3.9 ...[0;m
[0KUsing docker image sha256:0a3ee4bd701a644ae954f16b37a4bced05fb59fb54013d1037e8b22bbbf66813 for python:3.9 with digest python@sha256:7af616b934168e213d469bff23bd8e4f07d09ccbe87e82c464cacd8e2fb244bf ...[0;m
section_end:1674647191:prepare_executor
[0Ksection_start:1674647191:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-685-concurrent-0 via cab6f0e97d50...
section_end:1674647192:prepare_script
[0Ksection_start:1674647192:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 50...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/ocr/.git/
[32;1mChecking out e098ad2b as main...[0;m
Removing .mypy_cache/
Removing .pytest_cache/
Removing ocr.egg-info/
Removing ocr/__pycache__/
Removing tests/__pycache__/

[32;1mSkipping Git submodules setup[0;m
section_end:1674647193:get_sources
[0Ksection_start:1674647193:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:0a3ee4bd701a644ae954f16b37a4bced05fb59fb54013d1037e8b22bbbf66813 for python:3.9 with digest python@sha256:7af616b934168e213d469bff23bd8e4f07d09ccbe87e82c464cacd8e2fb244bf ...[0;m
[32;1m$ pip install -e .[0;m
Obtaining file:///builds/memri/plugins/ocr
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pytest~=7.0
  Downloading pytest-7.2.1-py3-none-any.whl (317 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 317.1/317.1 KB 5.3 MB/s eta 0:00:00
Collecting pymemri~=0.0.41
  Downloading pymemri-0.0.41-py3-none-any.whl (69 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 69.6/69.6 KB 723.9 kB/s eta 0:00:00
Collecting loguru~=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 6.2 MB/s eta 0:00:00
Collecting pre-commit~=2.20
  Downloading pre_commit-2.21.0-py2.py3-none-any.whl (201 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 201.9/201.9 KB 18.1 MB/s eta 0:00:00
Collecting easyocr~=1.6.2
  Downloading easyocr-1.6.2-py3-none-any.whl (2.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.9/2.9 MB 23.9 MB/s eta 0:00:00
Collecting ninja
  Downloading ninja-1.11.1-py2.py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.whl (145 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 146.0/146.0 KB 14.9 MB/s eta 0:00:00
Collecting PyYAML
  Downloading PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (661 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 661.8/661.8 KB 30.9 MB/s eta 0:00:00
Collecting opencv-python-headless<=4.5.4.60
  Downloading opencv_python_headless-4.5.4.60-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (47.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 47.6/47.6 MB 23.3 MB/s eta 0:00:00
Collecting torch
  Downloading torch-1.13.1-cp39-cp39-manylinux1_x86_64.whl (887.4 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 887.4/887.4 MB 1.3 MB/s eta 0:00:00
Collecting pyclipper
  Downloading pyclipper-1.3.0.post4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl (608 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 608.2/608.2 KB 33.0 MB/s eta 0:00:00
Collecting numpy
  Downloading numpy-1.24.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 17.3/17.3 MB 41.6 MB/s eta 0:00:00
Collecting Shapely
  Downloading shapely-2.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (2.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.3/2.3 MB 65.9 MB/s eta 0:00:00
Collecting Pillow
  Downloading Pillow-9.4.0-cp39-cp39-manylinux_2_28_x86_64.whl (3.4 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.4/3.4 MB 60.3 MB/s eta 0:00:00
Collecting python-bidi
  Downloading python_bidi-0.4.2-py2.py3-none-any.whl (30 kB)
Collecting scipy
  Downloading scipy-1.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (34.4 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 34.4/34.4 MB 35.6 MB/s eta 0:00:00
Collecting scikit-image
  Downloading scikit_image-0.19.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (14.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 14.0/14.0 MB 50.3 MB/s eta 0:00:00
Collecting torchvision>=0.5
  Downloading torchvision-0.14.1-cp39-cp39-manylinux1_x86_64.whl (24.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 24.2/24.2 MB 35.4 MB/s eta 0:00:00
Collecting cfgv>=2.0.0
  Downloading cfgv-3.3.1-py2.py3-none-any.whl (7.3 kB)
Collecting nodeenv>=0.11.1
  Downloading nodeenv-1.7.0-py2.py3-none-any.whl (21 kB)
Collecting identify>=1.0.0
  Downloading identify-2.5.15-py2.py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.7/98.7 KB 7.9 MB/s eta 0:00:00
Collecting virtualenv>=20.10.0
  Downloading virtualenv-20.17.1-py3-none-any.whl (8.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.8/8.8 MB 60.1 MB/s eta 0:00:00
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 13.2/13.2 MB 59.5 MB/s eta 0:00:00
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting requests
  Downloading requests-2.28.2-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 9.2 MB/s eta 0:00:00
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 16.9 MB/s eta 0:00:00
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 8.0 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 14.6 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 4.9 MB/s eta 0:00:00
Collecting Pillow
  Downloading Pillow-8.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 59.2 MB/s eta 0:00:00
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 8.1 MB/s eta 0:00:00
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (52 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 52.8/52.8 KB 2.5 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 7.0 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.1-py2.py3-none-any.whl (22 kB)
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.5-cp39-cp39-manylinux_2_28_x86_64.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.7/140.7 KB 11.7 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.9/site-packages (from fastcore==1.3.21->pymemri~=0.0.41->ocr==0.0.1) (22.0.4)
Collecting packaging
  Downloading packaging-23.0-py3-none-any.whl (42 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 42.7/42.7 KB 3.3 MB/s eta 0:00:00
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.10-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.7/62.7 KB 8.7 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting typing-extensions>=4.1.0
  Downloading typing_extensions-4.4.0-py3-none-any.whl (26 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 10.1 MB/s eta 0:00:00
Collecting attrs>=19.2.0
  Downloading attrs-22.2.0-py3-none-any.whl (60 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.0/60.0 KB 2.1 MB/s eta 0:00:00
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.1.0-py3-none-any.whl (14 kB)
Collecting iniconfig
  Downloading iniconfig-2.0.0-py3-none-any.whl (5.9 kB)
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Requirement already satisfied: setuptools in /usr/local/lib/python3.9/site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->ocr==0.0.1) (58.1.0)
Collecting certifi>=2017.4.17
  Downloading certifi-2022.12.7-py3-none-any.whl (155 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 155.3/155.3 KB 7.3 MB/s eta 0:00:00
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 7.4 MB/s eta 0:00:00
Collecting charset-normalizer<4,>=2
  Downloading charset_normalizer-3.0.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (198 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 198.8/198.8 KB 15.1 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.14-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.6/140.6 KB 10.8 MB/s eta 0:00:00
Collecting nvidia-cuda-runtime-cu11==11.7.99
  Downloading nvidia_cuda_runtime_cu11-11.7.99-py3-none-manylinux1_x86_64.whl (849 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 849.3/849.3 KB 41.8 MB/s eta 0:00:00
Collecting nvidia-cublas-cu11==11.10.3.66
  Downloading nvidia_cublas_cu11-11.10.3.66-py3-none-manylinux1_x86_64.whl (317.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 317.1/317.1 MB 6.1 MB/s eta 0:00:00
Collecting nvidia-cudnn-cu11==8.5.0.96
  Downloading nvidia_cudnn_cu11-8.5.0.96-2-py3-none-manylinux1_x86_64.whl (557.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 557.1/557.1 MB 2.7 MB/s eta 0:00:00
Collecting nvidia-cuda-nvrtc-cu11==11.7.99
  Downloading nvidia_cuda_nvrtc_cu11-11.7.99-2-py3-none-manylinux1_x86_64.whl (21.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 21.0/21.0 MB 48.5 MB/s eta 0:00:00
Requirement already satisfied: wheel in /usr/local/lib/python3.9/site-packages (from nvidia-cublas-cu11==11.10.3.66->torch->easyocr~=1.6.2->ocr==0.0.1) (0.38.4)
Collecting platformdirs<3,>=2.4
  Downloading platformdirs-2.6.2-py3-none-any.whl (14 kB)
Collecting filelock<4,>=3.4.1
  Downloading filelock-3.9.0-py3-none-any.whl (9.7 kB)
Collecting distlib<1,>=0.3.6
  Downloading distlib-0.3.6-py2.py3-none-any.whl (468 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 468.5/468.5 KB 42.9 MB/s eta 0:00:00
Collecting six
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting networkx>=2.2
  Downloading networkx-3.0-py3-none-any.whl (2.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.0/2.0 MB 66.3 MB/s eta 0:00:00
Collecting imageio>=2.4.1
  Downloading imageio-2.25.0-py3-none-any.whl (3.4 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.4/3.4 MB 71.3 MB/s eta 0:00:00
Collecting PyWavelets>=1.1.1
  Downloading PyWavelets-1.4.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (6.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 6.9/6.9 MB 67.9 MB/s eta 0:00:00
Collecting tifffile>=2019.7.26
  Downloading tifffile-2023.1.23.1-py3-none-any.whl (214 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 214.8/214.8 KB 27.3 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.3.0-py3-none-any.whl (283 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 283.7/283.7 KB 420.4 kB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 8.8 MB/s eta 0:00:00
Collecting click>=7.0
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 9.1 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.6.0-py3-none-any.whl (23 kB)
Collecting websockets>=10.0
  Downloading websockets-10.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.5/106.5 KB 13.6 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 63.9 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.1-py3-none-any.whl (19 kB)
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (417 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 417.9/417.9 KB 41.8 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Building wheels for collected packages: python-multipart
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=f58bd01970815c209cfe1c502e9534e459d2d91057232e9d8331ffd957511fe7
  Stored in directory: /root/.cache/pip/wheels/fe/04/d1/a10661cc45f03c3cecda50deb2d2c22f57b4e84a75b2a5987e
Successfully built python-multipart
Installing collected packages: pyclipper, ninja, distlib, charset-normalizer, websockets, uvloop, urllib3, ujson, typing-extensions, tomli, sniffio, smmap, six, PyYAML, python-dotenv, pluggy, platformdirs, Pillow, packaging, orjson, nvidia-cuda-runtime-cu11, nvidia-cuda-nvrtc-cu11, nvidia-cublas-cu11, numpy, nodeenv, networkx, MarkupSafe, loguru, itsdangerous, iniconfig, idna, identify, httptools, h11, giturlparse, filelock, fastprogress, exceptiongroup, dnspython, click, cfgv, certifi, attrs, asgiref, virtualenv, uvicorn, tifffile, Shapely, scipy, requests, PyWavelets, python-multipart, python-bidi, pytest, pydantic, opencv-python-headless, nvidia-cudnn-cu11, jinja2, imageio, gitdb, fastscript, fastcore, email_validator, anyio, watchgod, torch, starlette, scikit-image, pre-commit, GitPython, torchvision, fastapi, easyocr, pymemri, ocr
  Running setup.py develop for ocr
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.2 Pillow-8.4.0 PyWavelets-1.4.1 PyYAML-6.0 Shapely-2.0.0 anyio-3.6.2 asgiref-3.6.0 attrs-22.2.0 certifi-2022.12.7 cfgv-3.3.1 charset-normalizer-3.0.1 click-8.1.3 distlib-0.3.6 dnspython-2.3.0 easyocr-1.6.2 email_validator-1.3.1 exceptiongroup-1.1.0 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 filelock-3.9.0 gitdb-4.0.10 giturlparse-0.10.0 h11-0.14.0 httptools-0.5.0 identify-2.5.15 idna-3.4 imageio-2.25.0 iniconfig-2.0.0 itsdangerous-2.1.2 jinja2-3.0.0 loguru-0.6.0 networkx-3.0 ninja-1.11.1 nodeenv-1.7.0 numpy-1.24.1 nvidia-cublas-cu11-11.10.3.66 nvidia-cuda-nvrtc-cu11-11.7.99 nvidia-cuda-runtime-cu11-11.7.99 nvidia-cudnn-cu11-8.5.0.96 ocr-0.0.1 opencv-python-headless-4.5.4.60 orjson-3.8.5 packaging-23.0 platformdirs-2.6.2 pluggy-1.0.0 pre-commit-2.21.0 pyclipper-1.3.0.post4 pydantic-1.10.2 pymemri-0.0.41 pytest-7.2.1 python-bidi-0.4.2 python-dotenv-0.21.1 python-multipart-0.0.5 requests-2.28.2 scikit-image-0.19.3 scipy-1.10.0 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tifffile-2023.1.23.1 tomli-2.0.1 torch-1.13.1 torchvision-0.14.1 typing-extensions-4.4.0 ujson-5.7.0 urllib3-1.26.14 uvicorn-0.17.6 uvloop-0.17.0 virtualenv-20.17.1 watchgod-0.8.2 websockets-10.4
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100    58  100    58    0     0  58000      0 --:--:-- --:--:-- --:--:-- 58000
{"build_profile":null,"cargo":"0.4.4","git_describe":null}[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pre-commit run --all-files[0;m
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
[32;1m$ pytest[0;m
============================= test session starts ==============================
platform linux -- Python 3.9.16, pytest-7.2.1, pluggy-1.0.0
rootdir: /builds/memri/plugins/ocr
plugins: anyio-3.6.2
collected 4 items

tests/test_ocr.py ...                                                    [ 75%]
tests/test_photo_item.py .                                               [100%]

=============================== warnings summary ===============================
../../../../usr/local/lib/python3.9/site-packages/skimage/util/dtype.py:27
  /usr/local/lib/python3.9/site-packages/skimage/util/dtype.py:27: DeprecationWarning: `np.bool8` is a deprecated alias for `np.bool_`.  (Deprecated NumPy 1.24)
    np.bool8: (False, True),

tests/test_photo_item.py::test_photo_item
  /usr/local/lib/python3.9/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    warnings.warn(

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
======================== 4 passed, 2 warnings in 45.01s ========================
section_end:1674647444:step_script
[0Ksection_start:1674647444:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1674647445:cleanup_file_variables
[0K[32;1mJob succeeded[0;m
```