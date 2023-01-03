```Running with gitlab-runner 14.9.1 (bd40e3da)
  on gitlab memri public docker-runner Ryesm3zY
Preparing the "docker" executor
00:06
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
Running on runner-ryesm3zy-project-636-concurrent-1 via 8e6b65718045...
Getting source from Git repository
00:02
Fetching changes with git depth set to 50...
Reinitialized existing Git repository in /builds/memri/twitter-topic-model/.git/
Checking out 011d1303 as main...
Skipping Git submodules setup
Executing "step_script" stage of the job script
09:32
Using docker image sha256:850f8694d221b7fba2358381b744c231cbe9096d3f3c888493f1889eccec25fb for python:3.9 with digest python@sha256:aa99b1963cc1e693bc06394de03fa541c4994a6fa69f746b0b97aa237a9ab0b5 ...
$ pip install -e .
Obtaining file:///builds/memri/twitter-topic-model
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri==0.0.34
  Downloading pymemri-0.0.34-py3-none-any.whl (68 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 68.9/68.9 KB 2.7 MB/s eta 0:00:00
Collecting torch==1.12.0
  Downloading torch-1.12.0-cp39-cp39-manylinux1_x86_64.whl (776.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 776.3/776.3 MB 2.5 MB/s eta 0:00:00
Collecting BERTopic==0.12.0
  Downloading bertopic-0.12.0-py2.py3-none-any.whl (90 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 90.7/90.7 KB 8.4 MB/s eta 0:00:00
Collecting scikit-learn==1.1.3
  Downloading scikit_learn-1.1.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (30.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 30.8/30.8 MB 30.3 MB/s eta 0:00:00
Collecting nltk>=3.6.5
  Downloading nltk-3.7-py3-none-any.whl (1.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.5/1.5 MB 35.5 MB/s eta 0:00:00
Collecting pytest
  Downloading pytest-7.2.0-py3-none-any.whl (316 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 316.8/316.8 KB 24.9 MB/s eta 0:00:00
Collecting rich
  Downloading rich-12.6.0-py3-none-any.whl (237 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 237.5/237.5 KB 20.3 MB/s eta 0:00:00
Collecting numpy>=1.20.0
  Downloading numpy-1.23.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 17.1/17.1 MB 49.2 MB/s eta 0:00:00
Collecting hdbscan>=0.8.28
  Downloading hdbscan-0.8.29.tar.gz (5.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 5.2/5.2 MB 56.4 MB/s eta 0:00:00
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Collecting tqdm>=4.41.1
  Downloading tqdm-4.64.1-py2.py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.5/78.5 KB 10.0 MB/s eta 0:00:00
Collecting plotly>=4.7.0
  Downloading plotly-5.11.0-py2.py3-none-any.whl (15.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 15.3/15.3 MB 51.8 MB/s eta 0:00:00
Collecting sentence-transformers>=0.4.1
  Downloading sentence-transformers-2.2.2.tar.gz (85 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 86.0/86.0 KB 13.0 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pandas>=1.1.5
  Downloading pandas-1.5.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (12.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 12.2/12.2 MB 55.4 MB/s eta 0:00:00
Collecting umap-learn>=0.5.0
  Downloading umap-learn-0.5.3.tar.gz (88 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 88.2/88.2 KB 10.8 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pyyaml<6.0
  Downloading PyYAML-5.4.1-cp39-cp39-manylinux1_x86_64.whl (630 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 630.1/630.1 KB 35.6 MB/s eta 0:00:00
Collecting requests
  Downloading requests-2.28.1-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.8/62.8 KB 7.8 MB/s eta 0:00:00
Collecting giturlparse==0.10.0
  Downloading giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting jinja2==3.0.0
  Downloading Jinja2-3.0.0-py3-none-any.whl (133 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 133.4/133.4 KB 18.0 MB/s eta 0:00:00
Collecting loguru~=0.6.0
  Downloading loguru-0.6.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 8.5 MB/s eta 0:00:00
Collecting fastprogress
  Downloading fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting pydantic==1.10.2
  Downloading pydantic-1.10.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 13.2/13.2 MB 56.1 MB/s eta 0:00:00
Collecting fastcore==1.3.21
  Downloading fastcore-1.3.21-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.8/53.8 KB 7.6 MB/s eta 0:00:00
Collecting fastapi[all]==0.78.0
  Downloading fastapi-0.78.0-py3-none-any.whl (54 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 54.6/54.6 KB 5.5 MB/s eta 0:00:00
Collecting pillow==8.4.0
  Downloading Pillow-8.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.1/3.1 MB 58.5 MB/s eta 0:00:00
Collecting fastscript
  Downloading fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting GitPython==3.1.27
  Downloading GitPython-3.1.27-py3-none-any.whl (181 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 181.2/181.2 KB 21.9 MB/s eta 0:00:00
Collecting threadpoolctl>=2.0.0
  Downloading threadpoolctl-3.1.0-py3-none-any.whl (14 kB)
Collecting scipy>=1.3.2
  Downloading scipy-1.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (33.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 33.8/33.8 MB 34.5 MB/s eta 0:00:00
Collecting joblib>=1.0.0
  Downloading joblib-1.2.0-py3-none-any.whl (297 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 298.0/298.0 KB 32.6 MB/s eta 0:00:00
Collecting typing-extensions
  Downloading typing_extensions-4.4.0-py3-none-any.whl (26 kB)
Collecting starlette==0.19.1
  Downloading starlette-0.19.1-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.3/63.3 KB 9.5 MB/s eta 0:00:00
Collecting python-multipart<0.0.6,>=0.0.5
  Downloading python-multipart-0.0.5.tar.gz (32 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Downloading ujson-5.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (46 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 46.1/46.1 KB 5.4 MB/s eta 0:00:00
Collecting itsdangerous<3.0.0,>=1.1.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting orjson<4.0.0,>=3.2.1
  Downloading orjson-3.8.2-cp39-cp39-manylinux_2_28_x86_64.whl (144 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 144.8/144.8 KB 18.6 MB/s eta 0:00:00
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Downloading uvicorn-0.17.6-py3-none-any.whl (53 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53.6/53.6 KB 7.5 MB/s eta 0:00:00
Collecting email_validator<2.0.0,>=1.1.1
  Downloading email_validator-1.3.0-py2.py3-none-any.whl (22 kB)
Collecting packaging
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.8/40.8 KB 3.8 MB/s eta 0:00:00
Requirement already satisfied: pip in /usr/local/lib/python3.9/site-packages (from fastcore==1.3.21->pymemri==0.0.34->twitter-topic-model==0.0.1) (22.0.4)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.9-py3-none-any.whl (63 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 63.1/63.1 KB 9.3 MB/s eta 0:00:00
Collecting MarkupSafe>=2.0.0rc2
  Downloading MarkupSafe-2.1.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting anyio<5,>=3.4.0
  Downloading anyio-3.6.2-py3-none-any.whl (80 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 80.6/80.6 KB 10.2 MB/s eta 0:00:00
Collecting regex>=2021.8.3
  Downloading regex-2022.10.31-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (769 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 770.0/770.0 KB 46.0 MB/s eta 0:00:00
Collecting click
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 96.6/96.6 KB 13.5 MB/s eta 0:00:00
Collecting iniconfig
  Downloading iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting tomli>=1.0.0
  Downloading tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting attrs>=19.2.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.8/58.8 KB 8.7 MB/s eta 0:00:00
Collecting pluggy<2.0,>=0.12
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting exceptiongroup>=1.0.0rc8
  Downloading exceptiongroup-1.0.4-py3-none-any.whl (14 kB)
Collecting pygments<3.0.0,>=2.6.0
  Downloading Pygments-2.13.0-py3-none-any.whl (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 56.7 MB/s eta 0:00:00
Collecting commonmark<0.10.0,>=0.9.0
  Downloading commonmark-0.9.1-py2.py3-none-any.whl (51 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 51.1/51.1 KB 7.1 MB/s eta 0:00:00
Collecting cython>=0.27
  Using cached Cython-0.29.32-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl (2.0 MB)
Collecting pytz>=2020.1
  Downloading pytz-2022.6-py2.py3-none-any.whl (498 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 498.1/498.1 KB 33.9 MB/s eta 0:00:00
Collecting python-dateutil>=2.8.1
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 247.7/247.7 KB 25.2 MB/s eta 0:00:00
Collecting tenacity>=6.2.0
  Downloading tenacity-8.1.0-py3-none-any.whl (23 kB)
Collecting charset-normalizer<3,>=2
  Downloading charset_normalizer-2.1.1-py3-none-any.whl (39 kB)
Collecting idna<4,>=2.5
  Downloading idna-3.4-py3-none-any.whl (61 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 61.5/61.5 KB 8.1 MB/s eta 0:00:00
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.12-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.4/140.4 KB 17.8 MB/s eta 0:00:00
Collecting certifi>=2017.4.17
  Downloading certifi-2022.9.24-py3-none-any.whl (161 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 161.1/161.1 KB 19.7 MB/s eta 0:00:00
Collecting transformers<5.0.0,>=4.6.0
  Downloading transformers-4.24.0-py3-none-any.whl (5.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 5.5/5.5 MB 62.4 MB/s eta 0:00:00
Collecting torchvision
  Downloading torchvision-0.14.0-cp39-cp39-manylinux1_x86_64.whl (24.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 24.3/24.3 MB 44.6 MB/s eta 0:00:00
Collecting sentencepiece
  Downloading sentencepiece-0.1.97-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (1.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.3/1.3 MB 51.2 MB/s eta 0:00:00
Collecting huggingface-hub>=0.4.0
  Downloading huggingface_hub-0.11.0-py3-none-any.whl (182 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 182.1/182.1 KB 22.2 MB/s eta 0:00:00
Collecting numba>=0.49
  Downloading numba-0.56.4-cp39-cp39-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (3.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.5/3.5 MB 60.4 MB/s eta 0:00:00
Collecting pynndescent>=0.5
  Downloading pynndescent-0.5.8.tar.gz (1.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.1/1.1 MB 50.1 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pyparsing!=3.0.5,>=2.0.2
  Downloading pyparsing-3.0.9-py3-none-any.whl (98 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 98.3/98.3 KB 12.8 MB/s eta 0:00:00
Collecting dnspython>=1.15.0
  Downloading dnspython-2.2.1-py3-none-any.whl (269 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 269.1/269.1 KB 26.4 MB/s eta 0:00:00
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting filelock
  Downloading filelock-3.8.0-py3-none-any.whl (10 kB)
Collecting llvmlite<0.40,>=0.39.0dev0
  Downloading llvmlite-0.39.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (34.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 34.6/34.6 MB 22.8 MB/s eta 0:00:00
Requirement already satisfied: setuptools in /usr/local/lib/python3.9/site-packages (from numba>=0.49->umap-learn>=0.5.0->BERTopic==0.12.0->twitter-topic-model==0.0.1) (58.1.0)
Collecting six>=1.5
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting tokenizers!=0.11.3,<0.14,>=0.11.1
  Downloading tokenizers-0.13.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (7.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 7.6/7.6 MB 64.6 MB/s eta 0:00:00
Collecting asgiref>=3.4.0
  Downloading asgiref-3.5.2-py3-none-any.whl (22 kB)
Collecting h11>=0.8
  Downloading h11-0.14.0-py3-none-any.whl (58 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 58.3/58.3 KB 10.1 MB/s eta 0:00:00
Collecting httptools>=0.4.0
  Downloading httptools-0.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (417 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 417.9/417.9 KB 44.8 MB/s eta 0:00:00
Collecting watchgod>=0.6
  Downloading watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting websockets>=10.0
  Downloading websockets-10.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 106.5/106.5 KB 17.4 MB/s eta 0:00:00
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Downloading uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.2/4.2 MB 58.6 MB/s eta 0:00:00
Collecting python-dotenv>=0.13
  Downloading python_dotenv-0.21.0-py3-none-any.whl (18 kB)
Collecting torchvision
  Downloading torchvision-0.13.1-cp39-cp39-manylinux1_x86_64.whl (19.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 19.1/19.1 MB 51.8 MB/s eta 0:00:00
  Downloading torchvision-0.13.0-cp39-cp39-manylinux1_x86_64.whl (19.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 19.1/19.1 MB 17.9 MB/s eta 0:00:00
Collecting sniffio>=1.1
  Downloading sniffio-1.3.0-py3-none-any.whl (10 kB)
Building wheels for collected packages: hdbscan, sentence-transformers, umap-learn, pynndescent, python-multipart
  Building wheel for hdbscan (pyproject.toml): started
  Building wheel for hdbscan (pyproject.toml): still running...
  Building wheel for hdbscan (pyproject.toml): finished with status 'done'
  Created wheel for hdbscan: filename=hdbscan-0.8.29-cp39-cp39-linux_x86_64.whl size=3659595 sha256=0e96c371f75b3b3e9f3efa5a27887450eb78b13567190312943b7ea1980faa61
  Stored in directory: /root/.cache/pip/wheels/05/6f/88/1a4c04276b98306f00217a1e300e6ba0252c6aa4f7616067ae
  Building wheel for sentence-transformers (setup.py): started
  Building wheel for sentence-transformers (setup.py): finished with status 'done'
  Created wheel for sentence-transformers: filename=sentence_transformers-2.2.2-py3-none-any.whl size=125938 sha256=ebaa78ec38b1fcd01afc98dc5c8e087ca2d904407b0d17249d1c9d42f949f7b8
  Stored in directory: /root/.cache/pip/wheels/71/67/06/162a3760c40d74dd40bc855d527008d26341c2b0ecf3e8e11f
  Building wheel for umap-learn (setup.py): started
  Building wheel for umap-learn (setup.py): finished with status 'done'
  Created wheel for umap-learn: filename=umap_learn-0.5.3-py3-none-any.whl size=82829 sha256=8780da2cc178f5ee44044b289d90df036736f5d6a17a56e88e7f5d12f2428d4c
  Stored in directory: /root/.cache/pip/wheels/f4/3e/1c/596d0a463d17475af648688443fa4846fef624d1390339e7e9
  Building wheel for pynndescent (setup.py): started
  Building wheel for pynndescent (setup.py): finished with status 'done'
  Created wheel for pynndescent: filename=pynndescent-0.5.8-py3-none-any.whl size=55513 sha256=7c8926e63bdd95c5fb14800f068d819389ba63ca94f953e32bbbce780e795bba
  Stored in directory: /root/.cache/pip/wheels/b9/89/cc/59ab91ef5b21dc2ab3635528d7d227f49dfc9169905dcb959d
  Building wheel for python-multipart (setup.py): started
  Building wheel for python-multipart (setup.py): finished with status 'done'
  Created wheel for python-multipart: filename=python_multipart-0.0.5-py3-none-any.whl size=31678 sha256=1b7c0997d89b5610348ff61226afaaf2d329a6eac07a4a44022ffc1c8a5f2be8
  Stored in directory: /root/.cache/pip/wheels/fe/04/d1/a10661cc45f03c3cecda50deb2d2c22f57b4e84a75b2a5987e
Successfully built hdbscan sentence-transformers umap-learn pynndescent python-multipart
Installing collected packages: tokenizers, sentencepiece, pytz, iniconfig, commonmark, websockets, uvloop, urllib3, ujson, typing-extensions, tqdm, tomli, threadpoolctl, tenacity, sniffio, smmap, six, regex, pyyaml, python-dotenv, pyparsing, pygments, pluggy, pillow, orjson, numpy, MarkupSafe, loguru, llvmlite, joblib, itsdangerous, idna, httptools, h11, giturlparse, filelock, fastprogress, exceptiongroup, dnspython, cython, click, charset-normalizer, certifi, attrs, asgiref, uvicorn, torch, scipy, rich, requests, python-multipart, python-dateutil, pydantic, plotly, packaging, numba, nltk, jinja2, gitdb, email_validator, anyio, watchgod, torchvision, starlette, scikit-learn, pytest, pandas, huggingface-hub, GitPython, fastscript, fastcore, transformers, pynndescent, hdbscan, fastapi, umap-learn, sentence-transformers, pymemri, BERTopic, twitter-topic-model
  Running setup.py develop for twitter-topic-model
Successfully installed BERTopic-0.12.0 GitPython-3.1.27 MarkupSafe-2.1.1 anyio-3.6.2 asgiref-3.5.2 attrs-22.1.0 certifi-2022.9.24 charset-normalizer-2.1.1 click-8.1.3 commonmark-0.9.1 cython-0.29.32 dnspython-2.2.1 email_validator-1.3.0 exceptiongroup-1.0.4 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 filelock-3.8.0 gitdb-4.0.9 giturlparse-0.10.0 h11-0.14.0 hdbscan-0.8.29 httptools-0.5.0 huggingface-hub-0.11.0 idna-3.4 iniconfig-1.1.1 itsdangerous-2.1.2 jinja2-3.0.0 joblib-1.2.0 llvmlite-0.39.1 loguru-0.6.0 nltk-3.7 numba-0.56.4 numpy-1.23.5 orjson-3.8.2 packaging-21.3 pandas-1.5.2 pillow-8.4.0 plotly-5.11.0 pluggy-1.0.0 pydantic-1.10.2 pygments-2.13.0 pymemri-0.0.34 pynndescent-0.5.8 pyparsing-3.0.9 pytest-7.2.0 python-dateutil-2.8.2 python-dotenv-0.21.0 python-multipart-0.0.5 pytz-2022.6 pyyaml-5.4.1 regex-2022.10.31 requests-2.28.1 rich-12.6.0 scikit-learn-1.1.3 scipy-1.9.3 sentence-transformers-2.2.2 sentencepiece-0.1.97 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tenacity-8.1.0 threadpoolctl-3.1.0 tokenizers-0.13.2 tomli-2.0.1 torch-1.12.0 torchvision-0.13.0 tqdm-4.64.1 transformers-4.24.0 twitter-topic-model-0.0.1 typing-extensions-4.4.0 ujson-5.5.0 umap-learn-0.5.3 urllib3-1.26.12 uvicorn-0.17.6 uvloop-0.17.0 watchgod-0.8.2 websockets-10.4
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
$ curl http://pod:3030/version
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    58  100    58    0     0  29000      0 --:--:-- --:--:-- --:--:-- 29000
{"build_profile":null,"cargo":"0.4.4","git_describe":null}$ export POD_ADDRESS='http://pod:3030'
$ pytest tests/
============================= test session starts ==============================
platform linux -- Python 3.9.15, pytest-7.2.0, pluggy-1.0.0
rootdir: /builds/memri/twitter-topic-model
plugins: anyio-3.6.2
collected 3 items
tests/test_topic_model.py ...                                            [100%]
=============================== warnings summary ===============================
../../../usr/local/lib/python3.9/site-packages/bertopic/_utils.py:4
  /usr/local/lib/python3.9/site-packages/bertopic/_utils.py:4: DeprecationWarning: Please use `csr_matrix` from the `scipy.sparse` namespace, the `scipy.sparse.csr` namespace is deprecated.
    from scipy.sparse.csr import csr_matrix
-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
=================== 3 passed, 1 warning in 263.72s (0:04:23) ===================
Cleaning up project directory and file based variables
00:01
Job succeeded```