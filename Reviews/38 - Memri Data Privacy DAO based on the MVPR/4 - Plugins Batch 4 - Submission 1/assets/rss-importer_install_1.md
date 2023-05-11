```
$ pip install -e .
Obtaining file:///Z:/CRDAO/4%20-%20Plugins%20Batch%204%20-%20Submission%201/rss-importer-dev/rss-importer-dev
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: pymemri in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from rss-importer==0.0.1) (0.0.45)
Requirement already satisfied: beautifulsoup4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from rss-importer==0.0.1) (4.11.1)
Collecting feedparser
  Downloading feedparser-6.0.10-py3-none-any.whl (81 kB)
     ---------------------------------------- 81.1/81.1 kB 2.3 MB/s eta 0:00:00
Requirement already satisfied: pytest in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from rss-importer==0.0.1) (7.1.3)
Requirement already satisfied: soupsieve>1.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from beautifulsoup4->rss-importer==0.0.1) (2.3.2.post1)
Collecting sgmllib3k
  Downloading sgmllib3k-1.0.0.tar.gz (5.8 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (0.6.0)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (1.0.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (0.10.0)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (3.1.27)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (8.4.0)
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (1.24.2)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (3.0.0)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (0.78.0)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (2.28.1)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (1.10.2)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (1.0.3)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri->rss-importer==0.0.1) (1.3.21)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.19.1)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.0.5)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (5.4.1)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (1.3.0)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (2.1.2)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (5.5.0)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (3.8.0)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.17.6)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri->rss-importer==0.0.1) (23.0.1)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri->rss-importer==0.0.1) (21.3)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri->rss-importer==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri->rss-importer==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri->rss-importer==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (3.6.1)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->rss-importer==0.0.1) (1.1.1)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->rss-importer==0.0.1) (1.0.0)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->rss-importer==0.0.1) (2.0.1)
Requirement already satisfied: colorama in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->rss-importer==0.0.1) (0.4.5)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->rss-importer==0.0.1) (1.11.0)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->rss-importer==0.0.1) (22.1.0)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->pymemri->rss-importer==0.0.1) (1.1.0)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->rss-importer==0.0.1) (2022.9.24)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->rss-importer==0.0.1) (1.26.12)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->rss-importer==0.0.1) (2.1.1)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri->rss-importer==0.0.1) (3.4)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri->rss-importer==0.0.1) (3.0.9)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri->rss-importer==0.0.1) (5.0.0)
Requirement already satisfied: six>=1.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from python-multipart<0.0.6,>=0.0.5->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (1.16.0)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (8.1.3)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (3.5.2)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.14.0)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (10.3)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.5.0)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.21.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (0.8.2)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri->rss-importer==0.0.1) (1.3.0)
Installing collected packages: sgmllib3k, feedparser, rss-importer
  DEPRECATION: sgmllib3k is being installed using the legacy 'setup.py install' method, because it does not have a 'pyproject.toml' and the 'wheel' package is not installed. pip 23.1 will enforce this behaviour change. A possible replacement is to enable the '--use-pep517' option. Discussion can be found at https://github.com/pypa/pip/issues/8559
  Running setup.py install for sgmllib3k: started
  Running setup.py install for sgmllib3k: finished with status 'done'
  Running setup.py develop for rss-importer
Successfully installed feedparser-6.0.10 rss-importer-0.0.1 sgmllib3k-1.0.0

[notice] A new release of pip is available: 23.0.1 -> 23.1
[notice] To update, run: python.exe -m pip install --upgrade pip

```