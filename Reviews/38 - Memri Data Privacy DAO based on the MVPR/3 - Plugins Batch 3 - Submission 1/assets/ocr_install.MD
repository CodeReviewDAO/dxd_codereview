```
$ pip install -e .
Obtaining file:///Z:/CRDAO/Memri_Milestone3/ocr-main
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: pytest~=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from ocr==0.0.1) (7.1.3)
Collecting pymemri~=0.0.41
  Downloading pymemri-0.0.45-py3-none-any.whl (69 kB)
     ---------------------------------------- 69.9/69.9 kB 1.9 MB/s eta 0:00:00
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from ocr==0.0.1) (0.6.0)
Requirement already satisfied: pre-commit~=2.20 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from ocr==0.0.1) (2.20.0)
Collecting easyocr~=1.6.2
  Downloading easyocr-1.6.2-py3-none-any.whl (2.9 MB)
     ---------------------------------------- 2.9/2.9 MB 6.3 MB/s eta 0:00:00
Collecting python-bidi
  Downloading python_bidi-0.4.2-py2.py3-none-any.whl (30 kB)
Collecting scikit-image
  Downloading scikit_image-0.19.3-cp310-cp310-win_amd64.whl (12.0 MB)
     --------------------------------------- 12.0/12.0 MB 17.2 MB/s eta 0:00:00
Requirement already satisfied: Pillow in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from easyocr~=1.6.2->ocr==0.0.1) (8.4.0)
Requirement already satisfied: torchvision>=0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from easyocr~=1.6.2->ocr==0.0.1) (0.13.0)
Requirement already satisfied: PyYAML in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from easyocr~=1.6.2->ocr==0.0.1) (5.4.1)
Collecting pyclipper
  Downloading pyclipper-1.3.0.post4-cp310-cp310-win_amd64.whl (94 kB)
     ---------------------------------------- 94.5/94.5 kB 5.3 MB/s eta 0:00:00
Requirement already satisfied: torch in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from easyocr~=1.6.2->ocr==0.0.1) (1.12.0)
Collecting ninja
  Downloading ninja-1.11.1-py2.py3-none-win_amd64.whl (313 kB)
     ------------------------------------- 313.0/313.0 kB 18.9 MB/s eta 0:00:00
Collecting Shapely
  Downloading shapely-2.0.1-cp310-cp310-win_amd64.whl (1.4 MB)
     ---------------------------------------- 1.4/1.4 MB 28.9 MB/s eta 0:00:00
Collecting opencv-python-headless<=4.5.4.60
  Downloading opencv_python_headless-4.5.4.60-cp310-cp310-win_amd64.whl (35.0 MB)
     --------------------------------------- 35.0/35.0 MB 50.4 MB/s eta 0:00:00
Requirement already satisfied: scipy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from easyocr~=1.6.2->ocr==0.0.1) (1.9.3)
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from easyocr~=1.6.2->ocr==0.0.1) (1.23.3)
Requirement already satisfied: colorama>=0.3.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->ocr==0.0.1) (0.4.5)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->ocr==0.0.1) (1.1.0)
Requirement already satisfied: nodeenv>=0.11.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->ocr==0.0.1) (1.7.0)
Requirement already satisfied: cfgv>=2.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->ocr==0.0.1) (3.3.1)
Requirement already satisfied: toml in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->ocr==0.0.1) (0.10.2)
Requirement already satisfied: virtualenv>=20.0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->ocr==0.0.1) (20.17.1)
Requirement already satisfied: identify>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->ocr==0.0.1) (2.5.9)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (3.0.0)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (1.0.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (1.10.2)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (3.1.27)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (0.78.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (0.10.0)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (1.3.21)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (2.28.1)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri~=0.0.41->ocr==0.0.1) (1.0.3)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.19.1)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (2.1.2)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (3.8.0)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.0.5)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (5.5.0)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.17.6)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (1.3.0)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri~=0.0.41->ocr==0.0.1) (22.3.1)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri~=0.0.41->ocr==0.0.1) (21.3)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri~=0.0.41->ocr==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri~=0.0.41->ocr==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri~=0.0.41->ocr==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (3.6.1)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->ocr==0.0.1) (1.11.0)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->ocr==0.0.1) (1.1.1)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->ocr==0.0.1) (22.1.0)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->ocr==0.0.1) (2.0.1)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->ocr==0.0.1) (1.0.0)
Requirement already satisfied: setuptools in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->ocr==0.0.1) (63.2.0)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri~=0.0.41->ocr==0.0.1) (3.4)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri~=0.0.41->ocr==0.0.1) (2.1.1)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri~=0.0.41->ocr==0.0.1) (1.26.12)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri~=0.0.41->ocr==0.0.1) (2022.9.24)
Requirement already satisfied: filelock<4,>=3.4.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->ocr==0.0.1) (3.8.2)
Requirement already satisfied: distlib<1,>=0.3.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->ocr==0.0.1) (0.3.6)
Requirement already satisfied: platformdirs<3,>=2.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->ocr==0.0.1) (2.6.0)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri~=0.0.41->ocr==0.0.1) (3.0.9)
Requirement already satisfied: six in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from python-bidi->easyocr~=1.6.2->ocr==0.0.1) (1.16.0)
Collecting networkx>=2.2
  Downloading networkx-3.0-py3-none-any.whl (2.0 MB)
     ---------------------------------------- 2.0/2.0 MB 65.6 MB/s eta 0:00:00
Collecting imageio>=2.4.1
  Downloading imageio-2.25.1-py3-none-any.whl (3.4 MB)
     ---------------------------------------- 3.4/3.4 MB 71.4 MB/s eta 0:00:00
Collecting PyWavelets>=1.1.1
  Downloading PyWavelets-1.4.1-cp310-cp310-win_amd64.whl (4.2 MB)
     ---------------------------------------- 4.2/4.2 MB 67.0 MB/s eta 0:00:00
Collecting tifffile>=2019.7.26
  Downloading tifffile-2023.2.3-py3-none-any.whl (215 kB)
     ---------------------------------------- 215.1/215.1 kB ? eta 0:00:00
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri~=0.0.41->ocr==0.0.1) (5.0.0)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.14.0)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (8.1.3)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (3.5.2)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.5.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.8.2)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (10.3)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (0.21.0)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri~=0.0.41->ocr==0.0.1) (1.3.0)
Installing collected packages: pyclipper, ninja, tifffile, Shapely, PyWavelets, python-bidi, opencv-python-headless, networkx, imageio, scikit-image, easyocr, pymemri, ocr
  Attempting uninstall: pymemri
    Found existing installation: pymemri 0.0.40
    Uninstalling pymemri-0.0.40:
      Successfully uninstalled pymemri-0.0.40
  Running setup.py develop for ocr
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
whatsapp 1.0 requires protobuf==3.19.4, but you have protobuf 4.21.10 which is incompatible.
language-identification 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
zero-shot-plugin 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
gmail-oauth 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter 0.2.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter-topic-model 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
speech-to-text 0.0.1 requires pymemri==0.0.40, but you have pymemri 0.0.45 which is incompatible.
Successfully installed PyWavelets-1.4.1 Shapely-2.0.1 easyocr-1.6.2 imageio-2.25.1 networkx-3.0 ninja-1.11.1 ocr-0.0.1 opencv-python-headless-4.5.4.60 pyclipper-1.3.0.post4 pymemri-0.0.45 python-bidi-0.4.2 scikit-image-0.19.3 tifffile-2023.2.3

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: python.exe -m pip install --upgrade pip

```