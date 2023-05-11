```
$ pip install -e .[dev]
    pre-commit install
Obtaining file:///Z:/CRDAO/4%20-%20Plugins%20Batch%204%20-%20Submission%201/mastodon-dev/mastodon-dev
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Checking if build backend supports build_editable: started
  Checking if build backend supports build_editable: finished with status 'done'
  Getting requirements to build editable: started
  Getting requirements to build editable: finished with status 'done'
  Preparing editable metadata (pyproject.toml): started
  Preparing editable metadata (pyproject.toml): finished with status 'done'
Collecting pymemri==0.0.45 (from mastodon-importer==0.0.1)
  Using cached pymemri-0.0.45-py3-none-any.whl (69 kB)
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon-importer==0.0.1) (0.6.0)
Collecting mastodon.py~=1.8.0 (from mastodon-importer==0.0.1)
  Downloading Mastodon.py-1.8.0-py2.py3-none-any.whl (64 kB)
     ---------------------------------------- 64.5/64.5 kB 1.8 MB/s eta 0:00:00
Collecting pytest~=7.0 (from mastodon-importer==0.0.1)
  Downloading pytest-7.3.1-py3-none-any.whl (320 kB)
     -------------------------------------- 320.5/320.5 kB 4.9 MB/s eta 0:00:00
Requirement already satisfied: pre-commit~=2.20 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon-importer==0.0.1) (2.20.0)
Requirement already satisfied: typer in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon-importer==0.0.1) (0.7.0)
Collecting pytest-timeout~=2.1 (from mastodon-importer==0.0.1)
  Downloading pytest_timeout-2.1.0-py3-none-any.whl (12 kB)
Collecting mypy (from mastodon-importer==0.0.1)
  Downloading mypy-1.2.0-cp310-cp310-win_amd64.whl (8.9 MB)
     ---------------------------------------- 8.9/8.9 MB 14.6 MB/s eta 0:00:00
Collecting types-all (from mastodon-importer==0.0.1)
  Downloading types_all-1.0.0-py2.py3-none-any.whl (2.9 kB)
Collecting py2store (from mastodon-importer==0.0.1)
  Downloading py2store-0.1.19.tar.gz (143 kB)
     ---------------------------------------- 143.1/143.1 kB ? eta 0:00:00
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (2.28.1)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (1.0.3)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (1.0.0)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (1.3.21)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (0.78.0)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (0.10.0)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (8.4.0)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (3.1.27)
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (3.0.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (1.10.2)
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.45->mastodon-importer==0.0.1) (1.24.2)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.19.1)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.0.5)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (2.1.2)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (5.4.1)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (5.5.0)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (3.8.0)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (1.3.0)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.17.6)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.45->mastodon-importer==0.0.1) (23.1)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.45->mastodon-importer==0.0.1) (21.3)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri==0.0.45->mastodon-importer==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri==0.0.45->mastodon-importer==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri==0.0.45->mastodon-importer==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (3.6.1)
Requirement already satisfied: colorama>=0.3.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->mastodon-importer==0.0.1) (0.4.5)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->mastodon-importer==0.0.1) (1.1.0)
Requirement already satisfied: python-dateutil in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon.py~=1.8.0->mastodon-importer==0.0.1) (2.8.2)
Requirement already satisfied: six in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon.py~=1.8.0->mastodon-importer==0.0.1) (1.16.0)
Requirement already satisfied: python-magic in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon.py~=1.8.0->mastodon-importer==0.0.1) (0.4.27)
Requirement already satisfied: decorator>=4.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from mastodon.py~=1.8.0->mastodon-importer==0.0.1) (5.1.1)
Collecting blurhash>=1.1.4 (from mastodon.py~=1.8.0->mastodon-importer==0.0.1)
  Downloading blurhash-1.1.4-py2.py3-none-any.whl (5.3 kB)
Requirement already satisfied: cfgv>=2.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->mastodon-importer==0.0.1) (3.3.1)
Requirement already satisfied: identify>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->mastodon-importer==0.0.1) (2.5.9)
Requirement already satisfied: nodeenv>=0.11.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->mastodon-importer==0.0.1) (1.7.0)
Requirement already satisfied: toml in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->mastodon-importer==0.0.1) (0.10.2)
Requirement already satisfied: virtualenv>=20.0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->mastodon-importer==0.0.1) (20.17.1)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->mastodon-importer==0.0.1) (1.1.1)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->mastodon-importer==0.0.1) (0.13.1)
Requirement already satisfied: exceptiongroup>=1.0.0rc8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->mastodon-importer==0.0.1) (1.0.0rc9)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->mastodon-importer==0.0.1) (2.0.1)
Collecting mypy-extensions>=1.0.0 (from mypy->mastodon-importer==0.0.1)
  Downloading mypy_extensions-1.0.0-py3-none-any.whl (4.7 kB)
Collecting dol (from py2store->mastodon-importer==0.0.1)
  Downloading dol-0.1.133.tar.gz (174 kB)
     ---------------------------------------- 174.9/174.9 kB ? eta 0:00:00
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Collecting config2py (from py2store->mastodon-importer==0.0.1)
  Downloading config2py-0.1.2.tar.gz (17 kB)
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Collecting importlib-resources (from py2store->mastodon-importer==0.0.1)
  Downloading importlib_resources-5.12.0-py3-none-any.whl (36 kB)
Requirement already satisfied: click<9.0.0,>=7.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from typer->mastodon-importer==0.0.1) (8.1.3)
Collecting types-DateTimeRange (from types-all->mastodon-importer==0.0.1)
  Downloading types_DateTimeRange-2.0.0.5-py3-none-any.whl (3.2 kB)
Collecting types-Deprecated (from types-all->mastodon-importer==0.0.1)
  Downloading types_Deprecated-1.2.9.2-py3-none-any.whl (3.2 kB)
Collecting types-Flask (from types-all->mastodon-importer==0.0.1)
  Downloading types_Flask-1.1.6-py3-none-any.whl (13 kB)
Collecting types-JACK-Client (from types-all->mastodon-importer==0.0.1)
  Downloading types_JACK_Client-0.5.10.8-py3-none-any.whl (5.0 kB)
Collecting types-Jinja2 (from types-all->mastodon-importer==0.0.1)
  Downloading types_Jinja2-2.11.9-py3-none-any.whl (18 kB)
Collecting types-Markdown (from types-all->mastodon-importer==0.0.1)
  Downloading types_Markdown-3.4.2.7-py3-none-any.whl (16 kB)
Collecting types-MarkupSafe (from types-all->mastodon-importer==0.0.1)
  Downloading types_MarkupSafe-1.1.10-py3-none-any.whl (4.0 kB)
Collecting types-Pillow (from types-all->mastodon-importer==0.0.1)
  Downloading types_Pillow-9.5.0.1-py3-none-any.whl (48 kB)
     ---------------------------------------- 48.6/48.6 kB ? eta 0:00:00
Collecting types-PyJWT (from types-all->mastodon-importer==0.0.1)
  Downloading types_PyJWT-1.7.1-py2.py3-none-any.whl (4.7 kB)
Collecting types-PyMySQL (from types-all->mastodon-importer==0.0.1)
  Downloading types_PyMySQL-1.0.19.6-py3-none-any.whl (13 kB)
Collecting types-PyYAML (from types-all->mastodon-importer==0.0.1)
  Downloading types_PyYAML-6.0.12.9-py3-none-any.whl (14 kB)
Collecting types-Routes (from types-all->mastodon-importer==0.0.1)
  Downloading types_Routes-2.5.0-py3-none-any.whl (3.3 kB)
Collecting types-Werkzeug (from types-all->mastodon-importer==0.0.1)
  Downloading types_Werkzeug-1.0.9-py3-none-any.whl (36 kB)
Collecting types-aiofiles (from types-all->mastodon-importer==0.0.1)
  Downloading types_aiofiles-23.1.0.1-py3-none-any.whl (8.6 kB)
Collecting types-annoy (from types-all->mastodon-importer==0.0.1)
  Downloading types_annoy-1.17.8.3-py3-none-any.whl (2.7 kB)
Collecting types-atomicwrites (from types-all->mastodon-importer==0.0.1)
  Downloading types_atomicwrites-1.4.5.1-py3-none-any.whl (2.5 kB)
Collecting types-backports (from types-all->mastodon-importer==0.0.1)
  Downloading types_backports-0.1.3-py2.py3-none-any.whl (2.2 kB)
Collecting types-backports-abc (from types-all->mastodon-importer==0.0.1)
  Downloading types_backports_abc-0.5.2-py3-none-any.whl (2.0 kB)
Collecting types-bleach (from types-all->mastodon-importer==0.0.1)
  Downloading types_bleach-6.0.0.2-py3-none-any.whl (5.5 kB)
Collecting types-boto (from types-all->mastodon-importer==0.0.1)
  Downloading types_boto-2.49.18.7-py3-none-any.whl (23 kB)
Collecting types-cachetools (from types-all->mastodon-importer==0.0.1)
  Downloading types_cachetools-5.3.0.5-py3-none-any.whl (3.6 kB)
Collecting types-certifi (from types-all->mastodon-importer==0.0.1)
  Downloading types_certifi-2021.10.8.3-py3-none-any.whl (2.1 kB)
Collecting types-characteristic (from types-all->mastodon-importer==0.0.1)
  Downloading types_characteristic-14.3.7-py3-none-any.whl (2.5 kB)
Collecting types-chardet (from types-all->mastodon-importer==0.0.1)
  Downloading types_chardet-5.0.4.3-py3-none-any.whl (5.9 kB)
Collecting types-click (from types-all->mastodon-importer==0.0.1)
  Downloading types_click-7.1.8-py3-none-any.whl (12 kB)
Collecting types-click-spinner (from types-all->mastodon-importer==0.0.1)
  Downloading types_click_spinner-0.1.13.4-py3-none-any.whl (2.7 kB)
Collecting types-colorama (from types-all->mastodon-importer==0.0.1)
  Downloading types_colorama-0.4.15.11-py3-none-any.whl (5.6 kB)
Collecting types-contextvars (from types-all->mastodon-importer==0.0.1)
  Downloading types_contextvars-2.4.7.2-py3-none-any.whl (2.7 kB)
Collecting types-croniter (from types-all->mastodon-importer==0.0.1)
  Downloading types_croniter-1.3.2.9-py3-none-any.whl (3.6 kB)
Collecting types-cryptography (from types-all->mastodon-importer==0.0.1)
  Downloading types_cryptography-3.3.23.2-py3-none-any.whl (30 kB)
Collecting types-dataclasses (from types-all->mastodon-importer==0.0.1)
  Downloading types_dataclasses-0.6.6-py3-none-any.whl (2.9 kB)
Collecting types-dateparser (from types-all->mastodon-importer==0.0.1)
  Downloading types_dateparser-1.1.4.9-py3-none-any.whl (15 kB)
Collecting types-decorator (from types-all->mastodon-importer==0.0.1)
  Downloading types_decorator-5.1.8.3-py3-none-any.whl (2.8 kB)
Collecting types-docopt (from types-all->mastodon-importer==0.0.1)
  Downloading types_docopt-0.6.11.3-py3-none-any.whl (2.3 kB)
Collecting types-docutils (from types-all->mastodon-importer==0.0.1)
  Downloading types_docutils-0.19.1.7-py3-none-any.whl (16 kB)
Collecting types-emoji (from types-all->mastodon-importer==0.0.1)
  Downloading types_emoji-2.1.0.3-py3-none-any.whl (3.5 kB)
Collecting types-enum34 (from types-all->mastodon-importer==0.0.1)
  Downloading types_enum34-1.1.8-py3-none-any.whl (2.8 kB)
Collecting types-fb303 (from types-all->mastodon-importer==0.0.1)
  Downloading types_fb303-1.0.0-py3-none-any.whl (2.8 kB)
Collecting types-filelock (from types-all->mastodon-importer==0.0.1)
  Downloading types_filelock-3.2.7-py3-none-any.whl (2.5 kB)
Collecting types-first (from types-all->mastodon-importer==0.0.1)
  Downloading types_first-2.0.5.1-py3-none-any.whl (2.1 kB)
Collecting types-freezegun (from types-all->mastodon-importer==0.0.1)
  Downloading types_freezegun-1.1.10-py3-none-any.whl (2.9 kB)
Collecting types-frozendict (from types-all->mastodon-importer==0.0.1)
  Downloading types_frozendict-2.0.9-py3-none-any.whl (2.4 kB)
Collecting types-futures (from types-all->mastodon-importer==0.0.1)
  Downloading types_futures-3.3.8-py3-none-any.whl (4.4 kB)
Collecting types-geoip2 (from types-all->mastodon-importer==0.0.1)
  Downloading types_geoip2-3.0.0-py3-none-any.whl (4.7 kB)
Collecting types-ipaddress (from types-all->mastodon-importer==0.0.1)
  Downloading types_ipaddress-1.0.8-py3-none-any.whl (3.1 kB)
Collecting types-itsdangerous (from types-all->mastodon-importer==0.0.1)
  Downloading types_itsdangerous-1.1.6-py3-none-any.whl (3.4 kB)
Collecting types-kazoo (from types-all->mastodon-importer==0.0.1)
  Downloading types_kazoo-0.1.3-py3-none-any.whl (4.1 kB)
Collecting types-maxminddb (from types-all->mastodon-importer==0.0.1)
  Downloading types_maxminddb-1.5.0-py3-none-any.whl (4.3 kB)
Collecting types-mock (from types-all->mastodon-importer==0.0.1)
  Downloading types_mock-5.0.0.6-py3-none-any.whl (5.0 kB)
Collecting types-mypy-extensions (from types-all->mastodon-importer==0.0.1)
  Downloading types_mypy_extensions-1.0.0.3-py3-none-any.whl (3.3 kB)
Collecting types-nmap (from types-all->mastodon-importer==0.0.1)
  Downloading types_nmap-0.1.6-py3-none-any.whl (3.0 kB)
Collecting types-openssl-python (from types-all->mastodon-importer==0.0.1)
  Downloading types_openssl_python-0.1.3-py2.py3-none-any.whl (4.5 kB)
Collecting types-orjson (from types-all->mastodon-importer==0.0.1)
  Downloading types_orjson-3.6.2-py3-none-any.whl (2.2 kB)
Collecting types-paramiko (from types-all->mastodon-importer==0.0.1)
  Downloading types_paramiko-3.0.0.7-py3-none-any.whl (31 kB)
Collecting types-pathlib2 (from types-all->mastodon-importer==0.0.1)
  Downloading types_pathlib2-2.3.0-py3-none-any.whl (2.9 kB)
Collecting types-pkg-resources (from types-all->mastodon-importer==0.0.1)
  Downloading types_pkg_resources-0.1.3-py2.py3-none-any.whl (4.8 kB)
Collecting types-polib (from types-all->mastodon-importer==0.0.1)
  Downloading types_polib-1.2.0.0-py3-none-any.whl (3.3 kB)
Collecting types-protobuf (from types-all->mastodon-importer==0.0.1)
  Downloading types_protobuf-4.22.0.2-py3-none-any.whl (61 kB)
     ---------------------------------------- 61.3/61.3 kB ? eta 0:00:00
Collecting types-pyRFC3339 (from types-all->mastodon-importer==0.0.1)
  Downloading types_pyRFC3339-1.1.1.4-py3-none-any.whl (3.0 kB)
Collecting types-pyaudio (from types-all->mastodon-importer==0.0.1)
  Downloading types_pyaudio-0.2.16.6-py3-none-any.whl (3.6 kB)
Collecting types-pycurl (from types-all->mastodon-importer==0.0.1)
  Downloading types_pycurl-7.45.2.4-py3-none-any.whl (6.4 kB)
Collecting types-pyfarmhash (from types-all->mastodon-importer==0.0.1)
  Downloading types_pyfarmhash-0.3.1.1-py3-none-any.whl (2.1 kB)
Collecting types-pymssql (from types-all->mastodon-importer==0.0.1)
  Downloading types_pymssql-2.1.0-py3-none-any.whl (2.4 kB)
Collecting types-pysftp (from types-all->mastodon-importer==0.0.1)
  Downloading types_pysftp-0.2.17.5-py3-none-any.whl (4.2 kB)
Collecting types-python-dateutil (from types-all->mastodon-importer==0.0.1)
  Downloading types_python_dateutil-2.8.19.12-py3-none-any.whl (9.2 kB)
Collecting types-python-gflags (from types-all->mastodon-importer==0.0.1)
  Downloading types_python_gflags-3.1.7.2-py3-none-any.whl (4.2 kB)
Collecting types-python-slugify (from types-all->mastodon-importer==0.0.1)
  Downloading types_python_slugify-8.0.0.2-py3-none-any.whl (3.2 kB)
Collecting types-pytz (from types-all->mastodon-importer==0.0.1)
  Downloading types_pytz-2023.3.0.0-py3-none-any.whl (4.7 kB)
Collecting types-pyvmomi (from types-all->mastodon-importer==0.0.1)
  Downloading types_pyvmomi-8.0.0.1-py3-none-any.whl (5.9 kB)
Collecting types-redis (from types-all->mastodon-importer==0.0.1)
  Downloading types_redis-4.5.4.1-py3-none-any.whl (56 kB)
     ---------------------------------------- 56.4/56.4 kB 2.9 MB/s eta 0:00:00
Collecting types-requests (from types-all->mastodon-importer==0.0.1)
  Downloading types_requests-2.28.11.17-py3-none-any.whl (14 kB)
Collecting types-retry (from types-all->mastodon-importer==0.0.1)
  Downloading types_retry-0.9.9.3-py3-none-any.whl (2.4 kB)
Collecting types-scribe (from types-all->mastodon-importer==0.0.1)
  Downloading types_scribe-2.0.0-py3-none-any.whl (2.8 kB)
Collecting types-simplejson (from types-all->mastodon-importer==0.0.1)
  Downloading types_simplejson-3.19.0.0-py3-none-any.whl (3.9 kB)
Collecting types-singledispatch (from types-all->mastodon-importer==0.0.1)
  Downloading types_singledispatch-4.0.0.1-py3-none-any.whl (2.5 kB)
Collecting types-six (from types-all->mastodon-importer==0.0.1)
  Downloading types_six-1.16.21.8-py3-none-any.whl (14 kB)
Collecting types-tabulate (from types-all->mastodon-importer==0.0.1)
  Downloading types_tabulate-0.9.0.2-py3-none-any.whl (3.1 kB)
Collecting types-termcolor (from types-all->mastodon-importer==0.0.1)
  Downloading types_termcolor-1.1.6.2-py3-none-any.whl (2.4 kB)
Collecting types-toml (from types-all->mastodon-importer==0.0.1)
  Downloading types_toml-0.10.8.6-py3-none-any.whl (4.5 kB)
Collecting types-tornado (from types-all->mastodon-importer==0.0.1)
  Downloading types_tornado-5.1.1-py3-none-any.whl (13 kB)
Collecting types-typed-ast (from types-all->mastodon-importer==0.0.1)
  Downloading types_typed_ast-1.5.8.6-py3-none-any.whl (6.1 kB)
Collecting types-tzlocal (from types-all->mastodon-importer==0.0.1)
  Downloading types_tzlocal-4.3.0.0-py3-none-any.whl (2.7 kB)
Collecting types-ujson (from types-all->mastodon-importer==0.0.1)
  Downloading types_ujson-5.7.0.3-py3-none-any.whl (2.3 kB)
Collecting types-waitress (from types-all->mastodon-importer==0.0.1)
  Downloading types_waitress-2.1.4.7-py3-none-any.whl (12 kB)
Collecting types-xxhash (from types-all->mastodon-importer==0.0.1)
  Downloading types_xxhash-3.0.5.2-py3-none-any.whl (2.8 kB)
Requirement already satisfied: setuptools in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->mastodon-importer==0.0.1) (67.3.3)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.45->mastodon-importer==0.0.1) (2.1.1)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.45->mastodon-importer==0.0.1) (3.4)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.45->mastodon-importer==0.0.1) (1.26.12)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.45->mastodon-importer==0.0.1) (2022.9.24)
Requirement already satisfied: distlib<1,>=0.3.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->mastodon-importer==0.0.1) (0.3.6)
Requirement already satisfied: filelock<4,>=3.4.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->mastodon-importer==0.0.1) (3.8.2)
Requirement already satisfied: platformdirs<3,>=2.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->mastodon-importer==0.0.1) (2.6.0)
Collecting i2 (from config2py->py2store->mastodon-importer==0.0.1)
  Downloading i2-0.0.182.tar.gz (163 kB)
     -------------------------------------- 163.7/163.7 kB 9.6 MB/s eta 0:00:00
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri==0.0.45->mastodon-importer==0.0.1) (3.0.9)
Collecting types-cffi (from types-JACK-Client->types-all->mastodon-importer==0.0.1)
  Downloading types_cffi-1.15.1.12-py3-none-any.whl (13 kB)
Requirement already satisfied: cryptography>=37.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from types-paramiko->types-all->mastodon-importer==0.0.1) (38.0.1)
Collecting types-pyOpenSSL (from types-redis->types-all->mastodon-importer==0.0.1)
  Downloading types_pyOpenSSL-23.1.0.2-py3-none-any.whl (6.9 kB)
Collecting types-urllib3<1.27 (from types-requests->types-all->mastodon-importer==0.0.1)
  Downloading types_urllib3-1.26.25.10-py3-none-any.whl (15 kB)
Requirement already satisfied: cffi>=1.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from cryptography>=37.0.0->types-paramiko->types-all->mastodon-importer==0.0.1) (1.15.1)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri==0.0.45->mastodon-importer==0.0.1) (5.0.0)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (3.5.2)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.14.0)
Requirement already satisfied: websockets>=10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (10.3)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.5.0)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.8.2)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (0.21.0)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.45->mastodon-importer==0.0.1) (1.3.0)
Requirement already satisfied: pycparser in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from cffi>=1.12->cryptography>=37.0.0->types-paramiko->types-all->mastodon-importer==0.0.1) (2.21)
Building wheels for collected packages: mastodon-importer, py2store, config2py, dol, i2
  Building editable for mastodon-importer (pyproject.toml): started
  Building editable for mastodon-importer (pyproject.toml): finished with status 'done'
  Created wheel for mastodon-importer: filename=mastodon_importer-0.0.1-0.editable-py3-none-any.whl size=11226 sha256=c7db50a3c6182587b6b2bd7260c17a2c4816fd2ecbd4d5193f2b14233d2c371f
  Stored in directory: C:\Users\HouPha\AppData\Local\Temp\pip-ephem-wheel-cache-knin3gre\wheels\3c\a9\29\86634055b3738d429e2ff4b192d820c48f1dabd98232b77b6d
  Building wheel for py2store (pyproject.toml): started
  Building wheel for py2store (pyproject.toml): finished with status 'done'
  Created wheel for py2store: filename=py2store-0.1.19-py3-none-any.whl size=118669 sha256=c7fb5b32251769bff1a458c4d318b3b6b9e1ae7f225300c2152163efdce753a1
  Stored in directory: c:\users\houpha\appdata\local\pip\cache\wheels\d4\13\63\fc0706bb37ce9172cb9b11b6878dc70bf17b19895ce7014e5d
  Building wheel for config2py (pyproject.toml): started
  Building wheel for config2py (pyproject.toml): finished with status 'done'
  Created wheel for config2py: filename=config2py-0.1.2-py3-none-any.whl size=19436 sha256=4c4bf1865e4511359da27567da8936bbc42dbb85ad83900fef68d878f8d49385
  Stored in directory: c:\users\houpha\appdata\local\pip\cache\wheels\3d\f8\7d\876441e090950497bc2f1500ff04ae73dafff5b1535a6377f9
  Building wheel for dol (pyproject.toml): started
  Building wheel for dol (pyproject.toml): finished with status 'done'
  Created wheel for dol: filename=dol-0.1.133-py3-none-any.whl size=179801 sha256=a4575ac3313c6c581e4d2fdca8a16bbacb76d8733baaa07303d1b00b506ce55b
  Stored in directory: c:\users\houpha\appdata\local\pip\cache\wheels\9a\87\23\299a64fd051da2f4b8f69fe04723d90aaa5708ac044f28236d
  Building wheel for i2 (pyproject.toml): started
  Building wheel for i2 (pyproject.toml): finished with status 'done'
  Created wheel for i2: filename=i2-0.0.182-py3-none-any.whl size=175435 sha256=131b15c2bd9c87a26ec04f527d2ae9587dec19272ef13bee5dd8e04b33014cef
  Stored in directory: c:\users\houpha\appdata\local\pip\cache\wheels\1e\73\7e\3d3d798bbe709218f42275bc46211017d6c3e51c168959bcf9
Successfully built mastodon-importer py2store config2py dol i2
Installing collected packages: types-xxhash, types-Werkzeug, types-waitress, types-urllib3, types-ujson, types-typed-ast, types-tornado, types-toml, types-termcolor, types-tabulate, types-six, types-singledispatch, types-simplejson, types-Routes, types-retry, types-PyYAML, types-pyvmomi, types-pytz, types-python-slugify, types-python-gflags, types-python-dateutil, types-pyRFC3339, types-PyMySQL, types-pymssql, types-pyfarmhash, types-pycurl, types-pyaudio, types-protobuf, types-polib, types-pkg-resources, types-Pillow, types-pathlib2, types-orjson, types-nmap, types-mypy-extensions, types-mock, types-MarkupSafe, types-Markdown, types-kazoo, types-itsdangerous, types-ipaddress, types-futures, types-frozendict, types-freezegun, types-first, types-filelock, types-fb303, types-enum34, types-emoji, types-docutils, types-docopt, types-Deprecated, types-decorator, types-dateparser, types-dataclasses, types-cryptography, types-croniter, types-contextvars, types-colorama, types-click-spinner, types-click, types-chardet, types-characteristic, types-cffi, types-certifi, types-cachetools, types-boto, types-bleach, types-backports-abc, types-backports, types-atomicwrites, types-annoy, types-aiofiles, i2, dol, blurhash, types-tzlocal, types-scribe, types-requests, types-PyJWT, types-openssl-python, types-maxminddb, types-Jinja2, types-JACK-Client, types-DateTimeRange, mypy-extensions, importlib-resources, config2py, types-geoip2, types-Flask, pytest, py2store, mypy, mastodon.py, types-pyOpenSSL, types-paramiko, pytest-timeout, types-redis, types-pysftp, types-all, pymemri, mastodon-importer
  Attempting uninstall: pytest
    Found existing installation: pytest 6.2.4
    Uninstalling pytest-6.2.4:
      Successfully uninstalled pytest-6.2.4
  Attempting uninstall: pymemri
    Found existing installation: pymemri 0.0.46
    Uninstalling pymemri-0.0.46:
      Successfully uninstalled pymemri-0.0.46
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
whatsapp 1.0 requires protobuf==3.19.4, but you have protobuf 3.20.3 which is incompatible.
language-identification 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
zero-shot-plugin 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
gmail-oauth 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter 0.2.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter-topic-model 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.45 which is incompatible.
twitter-topic-model 0.0.1 requires torch==1.12.0, but you have torch 2.0.0 which is incompatible.
speech-to-text 0.0.1 requires pymemri==0.0.40, but you have pymemri 0.0.45 which is incompatible.
semantic-search 0.0.1 requires torch==1.13.1, but you have torch 2.0.0 which is incompatible.
google-calendar 0.0.2 requires pytest==6.2.4, but you have pytest 7.3.1 which is incompatible.
Successfully installed blurhash-1.1.4 config2py-0.1.2 dol-0.1.133 i2-0.0.182 importlib-resources-5.12.0 mastodon-importer-0.0.1 mastodon.py-1.8.0 mypy-1.2.0 mypy-extensions-1.0.0 py2store-0.1.19 pymemri-0.0.45 pytest-7.3.1 pytest-timeout-2.1.0 types-DateTimeRange-2.0.0.5 types-Deprecated-1.2.9.2 types-Flask-1.1.6 types-JACK-Client-0.5.10.8 types-Jinja2-2.11.9 types-Markdown-3.4.2.7 types-MarkupSafe-1.1.10 types-Pillow-9.5.0.1 types-PyJWT-1.7.1 types-PyMySQL-1.0.19.6 types-PyYAML-6.0.12.9 types-Routes-2.5.0 types-Werkzeug-1.0.9 types-aiofiles-23.1.0.1 types-all-1.0.0 types-annoy-1.17.8.3 types-atomicwrites-1.4.5.1 types-backports-0.1.3 types-backports-abc-0.5.2 types-bleach-6.0.0.2 types-boto-2.49.18.7 types-cachetools-5.3.0.5 types-certifi-2021.10.8.3 types-cffi-1.15.1.12 types-characteristic-14.3.7 types-chardet-5.0.4.3 types-click-7.1.8 types-click-spinner-0.1.13.4 types-colorama-0.4.15.11 types-contextvars-2.4.7.2 types-croniter-1.3.2.9 types-cryptography-3.3.23.2 types-dataclasses-0.6.6 types-dateparser-1.1.4.9 types-decorator-5.1.8.3 types-docopt-0.6.11.3 types-docutils-0.19.1.7 types-emoji-2.1.0.3 types-enum34-1.1.8 types-fb303-1.0.0 types-filelock-3.2.7 types-first-2.0.5.1 types-freezegun-1.1.10 types-frozendict-2.0.9 types-futures-3.3.8 types-geoip2-3.0.0 types-ipaddress-1.0.8 types-itsdangerous-1.1.6 types-kazoo-0.1.3 types-maxminddb-1.5.0 types-mock-5.0.0.6 types-mypy-extensions-1.0.0.3 types-nmap-0.1.6 types-openssl-python-0.1.3 types-orjson-3.6.2 types-paramiko-3.0.0.7 types-pathlib2-2.3.0 types-pkg-resources-0.1.3 types-polib-1.2.0.0 types-protobuf-4.22.0.2 types-pyOpenSSL-23.1.0.2 types-pyRFC3339-1.1.1.4 types-pyaudio-0.2.16.6 types-pycurl-7.45.2.4 types-pyfarmhash-0.3.1.1 types-pymssql-2.1.0 types-pysftp-0.2.17.5 types-python-dateutil-2.8.19.12 types-python-gflags-3.1.7.2 types-python-slugify-8.0.0.2 types-pytz-2023.3.0.0 types-pyvmomi-8.0.0.1 types-redis-4.5.4.1 types-requests-2.28.11.17 types-retry-0.9.9.3 types-scribe-2.0.0 types-simplejson-3.19.0.0 types-singledispatch-4.0.0.1 types-six-1.16.21.8 types-tabulate-0.9.0.2 types-termcolor-1.1.6.2 types-toml-0.10.8.6 types-tornado-5.1.1 types-typed-ast-1.5.8.6 types-tzlocal-4.3.0.0 types-ujson-5.7.0.3 types-urllib3-1.26.25.10 types-waitress-2.1.4.7 types-xxhash-3.0.5.2
An error has occurred: FatalError: git failed. Is it installed, and are you in a Git repository directory?
Check the log at C:\Users\HouPha\.cache\pre-commit\pre-commit.log

```