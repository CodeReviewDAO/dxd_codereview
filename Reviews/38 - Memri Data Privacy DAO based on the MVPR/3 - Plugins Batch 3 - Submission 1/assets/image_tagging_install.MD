```
$ pip install -e .
Obtaining file:///Z:/CRDAO/Memri_Milestone3/image-tagging-dev
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: pymemri in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from image-tagging==0.0.1) (0.0.45)
Collecting torch>=1.13.0
  Downloading torch-1.13.1-cp310-cp310-win_amd64.whl (162.6 MB)
     ------------------------------------- 162.6/162.6 MB 31.2 MB/s eta 0:00:00
Requirement already satisfied: transformers in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from image-tagging==0.0.1) (4.25.1)
Requirement already satisfied: pytest in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from image-tagging==0.0.1) (7.1.3)
Requirement already satisfied: typing-extensions in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from torch>=1.13.0->image-tagging==0.0.1) (4.4.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (0.10.0)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (3.1.27)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (8.4.0)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (1.0.3)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (1.0.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (1.10.2)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (1.3.21)
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (0.6.0)
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (1.23.3)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (3.0.0)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (2.28.1)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->image-tagging==0.0.1) (0.78.0)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.19.1)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.17.6)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (5.5.0)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (1.3.0)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (2.1.2)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (3.8.0)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (5.4.1)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.0.5)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri->image-tagging==0.0.1) (22.3.1)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri->image-tagging==0.0.1) (21.3)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri->image-tagging==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri->image-tagging==0.0.1) (2.1.1)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (3.6.1)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->image-tagging==0.0.1) (2.0.1)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->image-tagging==0.0.1) (22.1.0)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->image-tagging==0.0.1) (1.0.0)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->image-tagging==0.0.1) (1.11.0)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->image-tagging==0.0.1) (1.1.1)
Requirement already satisfied: colorama in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->image-tagging==0.0.1) (0.4.5)
Requirement already satisfied: filelock in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers->image-tagging==0.0.1) (3.8.2)
Requirement already satisfied: tqdm>=4.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers->image-tagging==0.0.1) (4.64.1)
Requirement already satisfied: huggingface-hub<1.0,>=0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers->image-tagging==0.0.1) (0.11.1)
Requirement already satisfied: regex!=2019.12.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers->image-tagging==0.0.1) (2022.9.13)
Requirement already satisfied: tokenizers!=0.11.3,<0.14,>=0.11.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers->image-tagging==0.0.1) (0.13.2)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->pymemri->image-tagging==0.0.1) (1.1.0)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri->image-tagging==0.0.1) (3.0.9)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->image-tagging==0.0.1) (3.4)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->image-tagging==0.0.1) (2.1.1)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->image-tagging==0.0.1) (1.26.12)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->image-tagging==0.0.1) (2022.9.24)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri->image-tagging==0.0.1) (5.0.0)
Requirement already satisfied: six>=1.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from python-multipart<0.0.6,>=0.0.5->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (1.16.0)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.14.0)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (8.1.3)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (3.5.2)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.21.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.8.2)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (10.3)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (0.5.0)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri->image-tagging==0.0.1) (1.3.0)
Installing collected packages: torch, image-tagging
  Attempting uninstall: torch
    Found existing installation: torch 1.12.0
    Uninstalling torch-1.12.0:
      Successfully uninstalled torch-1.12.0
  Running setup.py develop for image-tagging
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
torchvision 0.13.0 requires torch==1.12.0, but you have torch 1.13.1 which is incompatible.
zero-shot-plugin 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter-topic-model 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter-topic-model 0.0.1 requires torch==1.12.0, but you have torch 1.13.1 which is incompatible.
speech-to-text 0.0.1 requires pymemri==0.0.40, but you have pymemri 0.0.45 which is incompatible.
Successfully installed image-tagging-0.0.1 torch-1.13.1

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: python.exe -m pip install --upgrade pip

```