```
$ pip install -e .
Obtaining file:///Z:/CRDAO/Memri_FinalWork/whatsapp-multi-device-dev
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31
  Cloning https://gitlab.memri.io/memri/pymemri.git (to revision v0.0.31) to c:\users\houpha\appdata\local\temp\pip-install-ivalfq6s\pymemri_36c04b688f9e405f8a198ab2a8789056
  Running command git clone --filter=blob:none --quiet https://gitlab.memri.io/memri/pymemri.git 'C:\Users\HouPha\AppData\Local\Temp\pip-install-ivalfq6s\pymemri_36c04b688f9e405f8a198ab2a8789056'
  Running command git checkout -q a9cecb620c4b6dde75405a17801cade497c63995
  Resolved https://gitlab.memri.io/memri/pymemri.git to commit a9cecb620c4b6dde75405a17801cade497c63995
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting wamd@ git+https://github.com/alpdeniz/wamd.git@main
  Cloning https://github.com/alpdeniz/wamd.git (to revision main) to c:\users\houpha\appdata\local\temp\pip-install-ivalfq6s\wamd_70509571926646e280f91a078742df70
  Running command git clone --filter=blob:none --quiet https://github.com/alpdeniz/wamd.git 'C:\Users\HouPha\AppData\Local\Temp\pip-install-ivalfq6s\wamd_70509571926646e280f91a078742df70'
  Resolved https://github.com/alpdeniz/wamd.git to commit 2d6b9662f03edbc83ea80d95053a7bb887a9e3a7
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: websocket-client in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whatsapp==1.0) (1.4.1)
Requirement already satisfied: curve25519-donna in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whatsapp==1.0) (1.3)
Requirement already satisfied: pyqrcode in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whatsapp==1.0) (1.2.1)
Requirement already satisfied: protobuf==3.19.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whatsapp==1.0) (3.19.4)
Requirement already satisfied: pytest in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whatsapp==1.0) (7.1.3)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2.28.1)
Requirement already satisfied: tqdm in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (4.64.1)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.0.3)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.0.0)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.3.21)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.78.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.10.0)
Requirement already satisfied: pandas in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.5.0)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (8.4.0)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.1.27)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.0.0)
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.6.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.10.2)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.19.1)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.8.0)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2.1.2)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (6.0)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.0.5)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.17.6)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (5.5.0)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.3.0)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (21.3)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (22.2.2)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.6.1)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->whatsapp==1.0) (22.1.0)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->whatsapp==1.0) (1.1.1)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->whatsapp==1.0) (1.0.0)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->whatsapp==1.0) (2.0.1)
Requirement already satisfied: colorama in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->whatsapp==1.0) (0.4.5)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest->whatsapp==1.0) (1.11.0)
Requirement already satisfied: twisted in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (22.8.0)
Requirement already satisfied: PyOpenSSL in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (22.1.0)
Requirement already satisfied: service_identity in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (21.1.0)
Requirement already satisfied: autobahn in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (22.7.1)
Requirement already satisfied: dissononce in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.34.3)
Requirement already satisfied: consonance in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.1.5)
Requirement already satisfied: python-axolotl in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.2.3)
Requirement already satisfied: python-magic in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.4.27)
Requirement already satisfied: setuptools-rust in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (1.5.2)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.1.0)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.4)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.26.12)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2.1.1)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2022.9.24)
Requirement already satisfied: txaio>=21.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (22.2.1)
Requirement already satisfied: cryptography>=3.4.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (38.0.1)
Requirement already satisfied: hyperlink>=21.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (21.0.0)
Requirement already satisfied: setuptools in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (63.2.0)
Requirement already satisfied: python-axolotl-curve25519 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from consonance->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.4.1.post2)
Requirement already satisfied: transitions in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from consonance->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.9.0)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.0.9)
Requirement already satisfied: numpy>=1.21.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.23.3)
Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pandas->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2022.4)
Requirement already satisfied: six in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from service_identity->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (1.16.0)
Requirement already satisfied: pyasn1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from service_identity->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.4.8)
Requirement already satisfied: pyasn1-modules in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from service_identity->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (0.2.8)
Requirement already satisfied: semantic-version<3,>=2.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from setuptools-rust->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (2.10.0)
Requirement already satisfied: incremental>=21.3.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from twisted->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (22.10.0)
Requirement already satisfied: Automat>=0.8.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from twisted->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (20.2.0)
Requirement already satisfied: constantly>=15.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from twisted->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (15.1.0)
Requirement already satisfied: zope.interface>=4.4.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from twisted->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (5.5.0)
Requirement already satisfied: twisted-iocpsupport<2,>=1.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from twisted->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (1.0.2)
Requirement already satisfied: cffi>=1.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from cryptography>=3.4.6->autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (1.15.1)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (5.0.0)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (8.1.3)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (3.5.2)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.14.0)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (10.3)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.21.0)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.5.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (0.8.2)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri@ git+https://gitlab.memri.io/memri/pymemri.git@v0.0.31->whatsapp==1.0) (1.3.0)
Requirement already satisfied: pycparser in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from cffi>=1.12->cryptography>=3.4.6->autobahn->wamd@ git+https://github.com/alpdeniz/wamd.git@main->whatsapp==1.0) (2.21)
Installing collected packages: whatsapp
  Running setup.py develop for whatsapp
Successfully installed whatsapp-1.0

[notice] A new release of pip available: 22.2.2 -> 22.3
[notice] To update, run: python.exe -m pip install --upgrade pip
```