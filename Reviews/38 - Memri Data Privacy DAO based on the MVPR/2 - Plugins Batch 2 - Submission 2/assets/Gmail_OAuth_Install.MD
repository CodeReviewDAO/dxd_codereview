```
$ pip install -e .
Obtaining file:///Z:/Memri2/Plugins/gmail_oauth-dev
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting simplegmail~=4.0.4
  Downloading simplegmail-4.0.4-py3-none-any.whl (18 kB)
Requirement already satisfied: pytest~=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gmail-oauth==0.0.1) (7.1.3)
Collecting pymemri==0.0.34
  Using cached pymemri-0.0.34-py3-none-any.whl (68 kB)
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gmail-oauth==0.0.1) (0.6.0)
Collecting pre-commit~=2.20
  Downloading pre_commit-2.20.0-py2.py3-none-any.whl (199 kB)
     -------------------------------------- 199.5/199.5 kB 4.0 MB/s eta 0:00:00
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (1.3.21)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (1.0.0)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (1.0.3)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (2.28.1)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (0.10.0)
Requirement already satisfied: pandas in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (1.5.0)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (0.78.0)
Requirement already satisfied: tqdm in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (4.64.1)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (3.0.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (1.10.2)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (8.4.0)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.34->gmail-oauth==0.0.1) (3.1.27)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.19.1)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (3.8.0)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (1.3.0)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.17.6)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (5.5.0)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (2.1.2)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (6.0)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.0.5)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.34->gmail-oauth==0.0.1) (22.2.2)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.34->gmail-oauth==0.0.1) (21.3)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri==0.0.34->gmail-oauth==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri==0.0.34->gmail-oauth==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri==0.0.34->gmail-oauth==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (3.6.1)
Requirement already satisfied: colorama>=0.3.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->gmail-oauth==0.0.1) (0.4.5)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->gmail-oauth==0.0.1) (1.1.0)
Collecting virtualenv>=20.0.8
  Downloading virtualenv-20.17.1-py3-none-any.whl (8.8 MB)
     ---------------------------------------- 8.8/8.8 MB 22.7 MB/s eta 0:00:00
Collecting identify>=1.0.0
  Downloading identify-2.5.9-py2.py3-none-any.whl (98 kB)
     ---------------------------------------- 98.8/98.8 kB 5.5 MB/s eta 0:00:00
Requirement already satisfied: toml in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->gmail-oauth==0.0.1) (0.10.2)
Collecting nodeenv>=0.11.1
  Downloading nodeenv-1.7.0-py2.py3-none-any.whl (21 kB)
Collecting cfgv>=2.0.0
  Downloading cfgv-3.3.1-py2.py3-none-any.whl (7.3 kB)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->gmail-oauth==0.0.1) (1.11.0)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->gmail-oauth==0.0.1) (1.0.0)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->gmail-oauth==0.0.1) (2.0.1)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->gmail-oauth==0.0.1) (22.1.0)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->gmail-oauth==0.0.1) (1.1.1)
Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from simplegmail~=4.0.4->gmail-oauth==0.0.1) (2.8.2)
Collecting oauth2client>=4.1.3
  Downloading oauth2client-4.1.3-py2.py3-none-any.whl (98 kB)
     ---------------------------------------- 98.2/98.2 kB ? eta 0:00:00
Requirement already satisfied: lxml>=4.4.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from simplegmail~=4.0.4->gmail-oauth==0.0.1) (4.9.1)
Collecting bs4>=0.0.1
  Downloading bs4-0.0.1.tar.gz (1.1 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting google-api-python-client>=1.7.3
  Downloading google_api_python_client-2.68.0-py2.py3-none-any.whl (10.6 MB)
     --------------------------------------- 10.6/10.6 MB 32.8 MB/s eta 0:00:00
Requirement already satisfied: beautifulsoup4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from bs4>=0.0.1->simplegmail~=4.0.4->gmail-oauth==0.0.1) (4.11.1)
Collecting google-auth<3.0.0dev,>=1.19.0
  Downloading google_auth-2.15.0-py2.py3-none-any.whl (177 kB)
     ---------------------------------------- 177.0/177.0 kB ? eta 0:00:00
Collecting uritemplate<5,>=3.0.1
  Downloading uritemplate-4.1.1-py2.py3-none-any.whl (10 kB)
Collecting google-auth-httplib2>=0.1.0
  Downloading google_auth_httplib2-0.1.0-py2.py3-none-any.whl (9.3 kB)
Collecting httplib2<1dev,>=0.15.0
  Downloading httplib2-0.21.0-py3-none-any.whl (96 kB)
     ---------------------------------------- 96.8/96.8 kB ? eta 0:00:00
Collecting google-api-core!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0,<3.0.0dev,>=1.31.5
  Downloading google_api_core-2.11.0-py3-none-any.whl (120 kB)
     ---------------------------------------- 120.3/120.3 kB ? eta 0:00:00
Requirement already satisfied: setuptools in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->gmail-oauth==0.0.1) (63.2.0)
Requirement already satisfied: rsa>=3.1.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from oauth2client>=4.1.3->simplegmail~=4.0.4->gmail-oauth==0.0.1) (4.9)
Requirement already satisfied: pyasn1>=0.1.7 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from oauth2client>=4.1.3->simplegmail~=4.0.4->gmail-oauth==0.0.1) (0.4.8)
Requirement already satisfied: pyasn1-modules>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from oauth2client>=4.1.3->simplegmail~=4.0.4->gmail-oauth==0.0.1) (0.2.8)
Requirement already satisfied: six>=1.6.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from oauth2client>=4.1.3->simplegmail~=4.0.4->gmail-oauth==0.0.1) (1.16.0)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->gmail-oauth==0.0.1) (1.26.12)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->gmail-oauth==0.0.1) (2.1.1)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->gmail-oauth==0.0.1) (2022.9.24)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.34->gmail-oauth==0.0.1) (3.4)
Collecting distlib<1,>=0.3.6
  Downloading distlib-0.3.6-py2.py3-none-any.whl (468 kB)
     ------------------------------------- 468.5/468.5 kB 28.6 MB/s eta 0:00:00
Collecting platformdirs<3,>=2.4
  Downloading platformdirs-2.6.0-py3-none-any.whl (14 kB)
Requirement already satisfied: filelock<4,>=3.4.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->gmail-oauth==0.0.1) (3.8.2)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri==0.0.34->gmail-oauth==0.0.1) (3.0.9)
Requirement already satisfied: pytz>=2020.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri==0.0.34->gmail-oauth==0.0.1) (2022.4)
Requirement already satisfied: numpy>=1.21.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri==0.0.34->gmail-oauth==0.0.1) (1.23.3)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri==0.0.34->gmail-oauth==0.0.1) (5.0.0)
Collecting googleapis-common-protos<2.0dev,>=1.56.2
  Downloading googleapis_common_protos-1.57.0-py2.py3-none-any.whl (217 kB)
     ---------------------------------------- 218.0/218.0 kB ? eta 0:00:00
Collecting protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
  Downloading protobuf-4.21.10-cp310-abi3-win_amd64.whl (525 kB)
     ------------------------------------- 525.5/525.5 kB 32.2 MB/s eta 0:00:00
Collecting cachetools<6.0,>=2.0.0
  Downloading cachetools-5.2.0-py3-none-any.whl (9.3 kB)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (8.1.3)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.14.0)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (3.5.2)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.21.0)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (10.3)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.5.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (0.8.2)
Requirement already satisfied: soupsieve>1.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from beautifulsoup4->bs4>=0.0.1->simplegmail~=4.0.4->gmail-oauth==0.0.1) (2.3.2.post1)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.34->gmail-oauth==0.0.1) (1.3.0)
Using legacy 'setup.py install' for bs4, since package 'wheel' is not installed.
WARNING: Error parsing requirements for pymemri: [Errno 2] No such file or directory: 'c:\\users\\houpha\\appdata\\local\\programs\\python\\python310\\lib\\site-packages\\pymemri-0.0.35.dist-info\\METADATA'
Installing collected packages: distlib, uritemplate, protobuf, platformdirs, nodeenv, identify, httplib2, cfgv, cachetools, virtualenv, oauth2client, googleapis-common-protos, google-auth, bs4, pre-commit, google-auth-httplib2, google-api-core, google-api-python-client, simplegmail, pymemri, gmail-oauth
  Attempting uninstall: protobuf
    Found existing installation: protobuf 3.19.4
    Uninstalling protobuf-3.19.4:
      Successfully uninstalled protobuf-3.19.4
  Running setup.py install for bs4: started
  Running setup.py install for bs4: finished with status 'done'
  Attempting uninstall: pymemri
    WARNING: No metadata found in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages
    Found existing installation: pymemri 0.0.35
    Can't uninstall 'pymemri'. No files were found to uninstall.
  Running setup.py develop for gmail-oauth
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
whatsapp 1.0 requires protobuf==3.19.4, but you have protobuf 4.21.10 which is incompatible.
telegram 0.0.1 requires pymemri==0.0.35, but you have pymemri 0.0.34 which is incompatible.
Successfully installed bs4-0.0.1 cachetools-5.2.0 cfgv-3.3.1 distlib-0.3.6 gmail-oauth-0.0.1 google-api-core-2.11.0 google-api-python-client-2.68.0 google-auth-2.15.0 google-auth-httplib2-0.1.0 googleapis-common-protos-1.57.0 httplib2-0.21.0 identify-2.5.9 nodeenv-1.7.0 oauth2client-4.1.3 platformdirs-2.6.0 pre-commit-2.20.0 protobuf-4.21.10 pymemri-0.0.34 simplegmail-4.0.4 uritemplate-4.1.1 virtualenv-20.17.1

[notice] A new release of pip available: 22.2.2 -> 22.3.1
[notice] To update, run: python.exe -m pip install --upgrade pip

```