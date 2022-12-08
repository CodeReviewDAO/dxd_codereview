```
$ pip install -e .
Obtaining file:///Z:/Memri2/Plugins/telegram-dev
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting telethon@ git+https://github.com/LonamiWebs/Telethon.git@v1
  Cloning https://github.com/LonamiWebs/Telethon.git (to revision v1) to c:\users\houpha\appdata\local\temp\pip-install-6tis422p\telethon_7f0b9a68ebc5411f98b576fa000858bf
  Running command git clone --filter=blob:none --quiet https://github.com/LonamiWebs/Telethon.git 'C:\Users\HouPha\AppData\Local\Temp\pip-install-6tis422p\telethon_7f0b9a68ebc5411f98b576fa000858bf'
  Resolved https://github.com/LonamiWebs/Telethon.git to commit 83f13da420f0f581234d66dd3f5f91fd8f8fa3e3
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Collecting pymemri==0.0.35
  Downloading pymemri-0.0.35-py3-none-any.whl (69 kB)
     ---------------------------------------- 69.0/69.0 kB 1.9 MB/s eta 0:00:00
Requirement already satisfied: pytest in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from telegram==0.0.1) (7.1.3)
Collecting pytest-asyncio
  Downloading pytest_asyncio-0.20.2-py3-none-any.whl (14 kB)
Collecting markdown-it-py
  Downloading markdown_it_py-2.1.0-py3-none-any.whl (84 kB)
     ---------------------------------------- 84.5/84.5 kB 4.6 MB/s eta 0:00:00
Requirement already satisfied: pyqrcode in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from telegram==0.0.1) (1.2.1)
Collecting qrcodeT
  Downloading qrcodeT-1.0.4.tar.gz (2.6 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: pandas in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (1.5.0)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (1.0.3)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (3.0.0)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (1.0.0)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (2.28.1)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (8.4.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (0.10.0)
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (0.6.0)
Requirement already satisfied: tqdm in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (4.64.1)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (1.10.2)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (1.3.21)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (3.1.27)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.35->telegram==0.0.1) (0.78.0)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.19.1)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (1.3.0)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (6.0)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (2.1.2)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (5.5.0)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (3.8.0)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.0.5)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.17.6)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.35->telegram==0.0.1) (21.3)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.35->telegram==0.0.1) (22.2.2)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri==0.0.35->telegram==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri==0.0.35->telegram==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri==0.0.35->telegram==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (3.6.1)
Collecting mdurl~=0.1
  Downloading mdurl-0.1.2-py3-none-any.whl (10.0 kB)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->telegram==0.0.1) (2.0.1)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->telegram==0.0.1) (1.11.0)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->telegram==0.0.1) (22.1.0)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->telegram==0.0.1) (1.0.0)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->telegram==0.0.1) (1.1.1)
Requirement already satisfied: colorama in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->telegram==0.0.1) (0.4.5)
Collecting qrcode[pil]
  Downloading qrcode-7.3.1.tar.gz (43 kB)
     ---------------------------------------- 43.5/43.5 kB 2.2 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from qrcodeT->telegram==0.0.1) (1.23.3)
Collecting rsa
  Downloading rsa-4.9-py3-none-any.whl (34 kB)
Collecting pyaes
  Downloading pyaes-1.6.1.tar.gz (28 kB)
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->pymemri==0.0.35->telegram==0.0.1) (1.1.0)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.35->telegram==0.0.1) (3.4)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.35->telegram==0.0.1) (2.1.1)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.35->telegram==0.0.1) (1.26.12)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.35->telegram==0.0.1) (2022.9.24)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri==0.0.35->telegram==0.0.1) (3.0.9)
Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri==0.0.35->telegram==0.0.1) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri==0.0.35->telegram==0.0.1) (2022.4)
Requirement already satisfied: pyasn1>=0.1.3 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from rsa->telethon@ git+https://github.com/LonamiWebs/Telethon.git@v1->telegram==0.0.1) (0.4.8)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri==0.0.35->telegram==0.0.1) (5.0.0)
Requirement already satisfied: six>=1.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from python-dateutil>=2.8.1->pandas->pymemri==0.0.35->telegram==0.0.1) (1.16.0)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (3.5.2)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.14.0)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (8.1.3)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.8.2)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.5.0)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (0.21.0)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (10.3)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.35->telegram==0.0.1) (1.3.0)
Using legacy 'setup.py install' for qrcodeT, since package 'wheel' is not installed.
Using legacy 'setup.py install' for pyaes, since package 'wheel' is not installed.
Using legacy 'setup.py install' for qrcode, since package 'wheel' is not installed.
Building wheels for collected packages: telethon
  Building wheel for telethon (pyproject.toml): started
  Building wheel for telethon (pyproject.toml): finished with status 'done'
  Created wheel for telethon: filename=Telethon-1.26.0-py3-none-any.whl size=586623 sha256=6fa10a9538805a914fbc41bc4e182ec972986b60626cd6d9f2d5607a9497c737
  Stored in directory: C:\Users\HouPha\AppData\Local\Temp\pip-ephem-wheel-cache-6d2b5_0b\wheels\e4\d2\85\315d33df578990dfeab3370b47c3747343ffac6e6ce3821d85
Successfully built telethon
Installing collected packages: pyaes, rsa, qrcode, mdurl, telethon, markdown-it-py, qrcodeT, pytest-asyncio, pymemri, telegram
  Running setup.py install for pyaes: started
  Running setup.py install for pyaes: finished with status 'done'
  Running setup.py install for qrcode: started
  Running setup.py install for qrcode: finished with status 'done'
  Running setup.py install for qrcodeT: started
  Running setup.py install for qrcodeT: finished with status 'done'
  Attempting uninstall: pymemri
    Found existing installation: pymemri 0.0.24
    Uninstalling pymemri-0.0.24:
      Successfully uninstalled pymemri-0.0.24
  Running setup.py develop for telegram
Successfully installed markdown-it-py-2.1.0 mdurl-0.1.2 pyaes-1.6.1 pymemri-0.0.35 pytest-asyncio-0.20.2 qrcode-7.3.1 qrcodeT-1.0.4 rsa-4.9 telegram-0.0.1 telethon-1.26.0

[notice] A new release of pip available: 22.2.2 -> 22.3.1
[notice] To update, run: python.exe -m pip install --upgrade pip
```
