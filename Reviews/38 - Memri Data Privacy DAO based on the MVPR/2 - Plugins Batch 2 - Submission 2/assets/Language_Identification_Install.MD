```
$ pip install -e .
Obtaining file:///Z:/Memri2/Plugins/language-identification-dev
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: pymemri==0.0.34 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from language-identification==0.0.1) (0.0.34)
Collecting fasttext-wheel==0.9.2
  Downloading fasttext_wheel-0.9.2-cp310-cp310-win_amd64.whl (241 kB)
     -------------------------------------- 241.5/241.5 kB 2.1 MB/s eta 0:00:00
Collecting langcodes[data]
  Downloading langcodes-3.3.0-py3-none-any.whl (181 kB)
     -------------------------------------- 181.6/181.6 kB 2.7 MB/s eta 0:00:00
Collecting rich
  Downloading rich-12.6.0-py3-none-any.whl (237 kB)
     -------------------------------------- 237.5/237.5 kB 3.6 MB/s eta 0:00:00
Requirement already satisfied: pytest in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from language-identification==0.0.1) (7.1.3)
Collecting pybind11>=2.2
  Downloading pybind11-2.10.1-py3-none-any.whl (216 kB)
     -------------------------------------- 216.1/216.1 kB 3.3 MB/s eta 0:00:00
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fasttext-wheel==0.9.2->language-identification==0.0.1) (1.23.3)
Requirement already satisfied: setuptools>=0.7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fasttext-wheel==0.9.2->language-identification==0.0.1) (63.2.0)
Requirement already satisfied: tqdm in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (4.64.1)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (8.4.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (1.10.2)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (1.0.3)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (2.28.1)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (1.0.0)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (1.3.21)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (3.1.27)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (3.0.0)
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (0.6.0)
Requirement already satisfied: pandas in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (1.5.0)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (0.78.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->language-identification==0.0.1) (0.10.0)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.19.1)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (1.3.0)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.0.5)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (2.1.2)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (3.8.0)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (5.5.0)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (6.0)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.17.6)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.34->language-identification==0.0.1) (21.3)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.34->language-identification==0.0.1) (22.2.2)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri==0.0.34->language-identification==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri==0.0.34->language-identification==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri==0.0.34->language-identification==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (3.6.1)
Collecting language-data<2.0,>=1.1
  Downloading language_data-1.1-py3-none-any.whl (4.9 MB)
     ---------------------------------------- 4.9/4.9 MB 7.9 MB/s eta 0:00:00
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->language-identification==0.0.1) (2.0.1)
Requirement already satisfied: colorama in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->language-identification==0.0.1) (0.4.5)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->language-identification==0.0.1) (1.1.1)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->language-identification==0.0.1) (1.0.0)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->language-identification==0.0.1) (22.1.0)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->language-identification==0.0.1) (1.11.0)
Requirement already satisfied: pygments<3.0.0,>=2.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from rich->language-identification==0.0.1) (2.13.0)
Collecting commonmark<0.10.0,>=0.9.0
  Downloading commonmark-0.9.1-py2.py3-none-any.whl (51 kB)
     ---------------------------------------- 51.1/51.1 kB ? eta 0:00:00
Collecting marisa-trie<0.8.0,>=0.7.7
  Downloading marisa_trie-0.7.8-cp310-cp310-win_amd64.whl (130 kB)
     ---------------------------------------- 130.2/130.2 kB ? eta 0:00:00
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->pymemri==0.0.34->language-identification==0.0.1) (1.1.0)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->language-identification==0.0.1) (1.26.12)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->language-identification==0.0.1) (2.1.1)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->language-identification==0.0.1) (2022.9.24)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->language-identification==0.0.1) (3.4)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri==0.0.34->language-identification==0.0.1) (3.0.9)
Requirement already satisfied: pytz>=2020.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri==0.0.34->language-identification==0.0.1) (2022.4)
Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri==0.0.34->language-identification==0.0.1) (2.8.2)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri==0.0.34->language-identification==0.0.1) (5.0.0)
Requirement already satisfied: six>=1.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from python-dateutil>=2.8.1->pandas->pymemri==0.0.34->language-identification==0.0.1) (1.16.0)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.14.0)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (3.5.2)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (8.1.3)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.5.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.8.2)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (0.21.0)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (10.3)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.34->language-identification==0.0.1) (1.3.0)
Installing collected packages: commonmark, rich, pybind11, marisa-trie, langcodes, language-data, fasttext-wheel, language-identification
  Running setup.py develop for language-identification
Successfully installed commonmark-0.9.1 fasttext-wheel-0.9.2 langcodes-3.3.0 language-data-1.1 language-identification-0.0.1 marisa-trie-0.7.8 pybind11-2.10.1 rich-12.6.0

[notice] A new release of pip available: 22.2.2 -> 22.3.1
[notice] To update, run: python.exe -m pip install --upgrade pip
```