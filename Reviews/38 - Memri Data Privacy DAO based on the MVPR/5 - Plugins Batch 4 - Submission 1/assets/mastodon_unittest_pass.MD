```
[0KRunning with gitlab-runner 15.7.1 (6d480948)[0;m
[0K  on gitlab memri public docker-runner Ryesm3zY[0;m
section_start:1679642011:prepare_executor
[0K[0K[36;1mPreparing the "docker" executor[0;m[0;m
[0KUsing Docker executor with image python:3.9 ...[0;m
[0KStarting service gitlab.memri.io/memri/pod:dev-5f7f5e38 ...[0;m
[0KAuthenticating with credentials from job payload (GitLab Registry)[0;m
[0KPulling docker image gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 ...[0;m
[0KUsing docker image sha256:f1c9374b7ec1c085f6380164d0114f3a85486b34e4679850d715c35b276cd4a7 for gitlab.memri.io:5050/memri/pod:dev-5f7f5e38 with digest gitlab.memri.io:5050/memri/pod@sha256:4a88a9d71e775f3e2dc29af47aa69cc51b8b48c58a25767c2fc767ceef124f10 ...[0;m
[0KWaiting for services to be up and running (timeout 30 seconds)...[0;m
[0KPulling docker image python:3.9 ...[0;m
[0KUsing docker image sha256:e20b16618982799ec7f28ff6a45da7819702a231e952aa8280047e042f5885f7 for python:3.9 with digest python@sha256:7ac171271f185d4f05824b68ab1995981872e8f9b0cac262fe7da138fbd82e9a ...[0;m
section_end:1679642017:prepare_executor
[0Ksection_start:1679642017:prepare_script
[0K[0K[36;1mPreparing environment[0;m[0;m
Running on runner-ryesm3zy-project-712-concurrent-0 via cab6f0e97d50...
section_end:1679642018:prepare_script
[0Ksection_start:1679642018:get_sources
[0K[0K[36;1mGetting source from Git repository[0;m[0;m
[32;1mFetching changes with git depth set to 20...[0;m
Reinitialized existing Git repository in /builds/memri/plugins/mastodon/.git/
[32;1mChecking out c35d2a8f as dev...[0;m
Removing .cache/
Removing .pytest_cache/
Removing build/
Removing mastodon_importer.egg-info/
Removing mastodon_importer/__pycache__/
Removing tests/__pycache__/

[32;1mSkipping Git submodules setup[0;m
section_end:1679642020:get_sources
[0Ksection_start:1679642020:restore_cache
[0K[0K[36;1mRestoring cache[0;m[0;m
[32;1mChecking cache for default-protected...[0;m
No URL provided, cache will not be downloaded from shared cache server. Instead a local version of cache will be extracted.[0;m 
[32;1mSuccessfully extracted cache[0;m
section_end:1679642022:restore_cache
[0Ksection_start:1679642022:step_script
[0K[0K[36;1mExecuting "step_script" stage of the job script[0;m[0;m
[0KUsing docker image sha256:e20b16618982799ec7f28ff6a45da7819702a231e952aa8280047e042f5885f7 for python:3.9 with digest python@sha256:7ac171271f185d4f05824b68ab1995981872e8f9b0cac262fe7da138fbd82e9a ...[0;m
[32;1m$ pip install .[dev][0;m
Processing /builds/memri/plugins/mastodon
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting pymemri==0.0.45
  Using cached pymemri-0.0.45-py3-none-any.whl (69 kB)
Collecting loguru~=0.6.0
  Using cached loguru-0.6.0-py3-none-any.whl (58 kB)
Collecting mastodon.py~=1.8.0
  Using cached Mastodon.py-1.8.0-py2.py3-none-any.whl (64 kB)
Collecting pytest~=7.0
  Using cached pytest-7.2.2-py3-none-any.whl (317 kB)
Collecting pre-commit~=2.20
  Using cached pre_commit-2.21.0-py2.py3-none-any.whl (201 kB)
Collecting typer
  Using cached typer-0.7.0-py3-none-any.whl (38 kB)
Collecting pytest-timeout~=2.1
  Using cached pytest_timeout-2.1.0-py3-none-any.whl (12 kB)
Collecting mypy
  Using cached mypy-1.1.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (12.1 MB)
Collecting types-all
  Using cached types_all-1.0.0-py2.py3-none-any.whl (2.9 kB)
Collecting py2store
  Using cached py2store-0.1.18-py3-none-any.whl
Collecting numpy
  Using cached numpy-1.24.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.3 MB)
Collecting requests
  Using cached requests-2.28.2-py3-none-any.whl (62 kB)
Collecting fastapi[all]==0.78.0
  Using cached fastapi-0.78.0-py3-none-any.whl (54 kB)
Collecting pillow==8.4.0
  Using cached Pillow-8.4.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (3.1 MB)
Collecting fastprogress
  Using cached fastprogress-1.0.3-py3-none-any.whl (12 kB)
Collecting GitPython==3.1.27
  Using cached GitPython-3.1.27-py3-none-any.whl (181 kB)
Collecting jinja2==3.0.0
  Using cached Jinja2-3.0.0-py3-none-any.whl (133 kB)
Collecting pydantic==1.10.2
  Using cached pydantic-1.10.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (13.2 MB)
Collecting giturlparse==0.10.0
  Using cached giturlparse-0.10.0-py2.py3-none-any.whl (14 kB)
Collecting fastcore==1.3.21
  Using cached fastcore-1.3.21-py3-none-any.whl (53 kB)
Collecting fastscript
  Using cached fastscript-1.0.0-py3-none-any.whl (11 kB)
Collecting starlette==0.19.1
  Using cached starlette-0.19.1-py3-none-any.whl (63 kB)
Collecting orjson<4.0.0,>=3.2.1
  Using cached orjson-3.8.8-cp39-cp39-manylinux_2_28_x86_64.whl (143 kB)
Collecting pyyaml<7.0.0,>=5.3.1
  Using cached PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl (661 kB)
Collecting itsdangerous<3.0.0,>=1.1.0
  Using cached itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting uvicorn[standard]<0.18.0,>=0.12.0
  Using cached uvicorn-0.17.6-py3-none-any.whl (53 kB)
Collecting python-multipart<0.0.6,>=0.0.5
  Using cached python_multipart-0.0.5-py3-none-any.whl
Collecting email_validator<2.0.0,>=1.1.1
  Using cached email_validator-1.3.1-py2.py3-none-any.whl (22 kB)
Collecting ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1
  Using cached ujson-5.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (52 kB)
Collecting packaging
  Using cached packaging-23.0-py3-none-any.whl (42 kB)
Requirement already satisfied: pip in /usr/local/lib/python3.9/site-packages (from fastcore==1.3.21->pymemri==0.0.45->mastodon-importer==0.0.1) (22.0.4)
Collecting gitdb<5,>=4.0.1
  Using cached gitdb-4.0.10-py3-none-any.whl (62 kB)
Collecting MarkupSafe>=2.0.0rc2
  Using cached MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting typing-extensions>=4.1.0
  Using cached typing_extensions-4.5.0-py3-none-any.whl (27 kB)
Collecting anyio<5,>=3.4.0
  Using cached anyio-3.6.2-py3-none-any.whl (80 kB)
Collecting six
  Using cached six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting decorator>=4.0.0
  Using cached decorator-5.1.1-py3-none-any.whl (9.1 kB)
Collecting python-magic
  Using cached python_magic-0.4.27-py2.py3-none-any.whl (13 kB)
Collecting blurhash>=1.1.4
  Using cached blurhash-1.1.4-py2.py3-none-any.whl (5.3 kB)
Collecting python-dateutil
  Using cached python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
Collecting virtualenv>=20.10.0
  Using cached virtualenv-20.21.0-py3-none-any.whl (8.7 MB)
Collecting identify>=1.0.0
  Using cached identify-2.5.21-py2.py3-none-any.whl (98 kB)
Collecting cfgv>=2.0.0
  Using cached cfgv-3.3.1-py2.py3-none-any.whl (7.3 kB)
Collecting nodeenv>=0.11.1
  Using cached nodeenv-1.7.0-py2.py3-none-any.whl (21 kB)
Collecting exceptiongroup>=1.0.0rc8
  Using cached exceptiongroup-1.1.1-py3-none-any.whl (14 kB)
Collecting tomli>=1.0.0
  Using cached tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting pluggy<2.0,>=0.12
  Using cached pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting iniconfig
  Using cached iniconfig-2.0.0-py3-none-any.whl (5.9 kB)
Collecting attrs>=19.2.0
  Using cached attrs-22.2.0-py3-none-any.whl (60 kB)
Collecting mypy-extensions>=1.0.0
  Using cached mypy_extensions-1.0.0-py3-none-any.whl (4.7 kB)
Collecting dol
  Using cached dol-0.1.124-py3-none-any.whl
Collecting config2py
  Using cached config2py-0.1.0-py3-none-any.whl
Collecting importlib-resources
  Using cached importlib_resources-5.12.0-py3-none-any.whl (36 kB)
Collecting click<9.0.0,>=7.1.1
  Using cached click-8.1.3-py3-none-any.whl (96 kB)
Collecting types-filelock
  Using cached types_filelock-3.2.7-py3-none-any.whl (2.5 kB)
Collecting types-backports
  Using cached types_backports-0.1.3-py2.py3-none-any.whl (2.2 kB)
Collecting types-PyYAML
  Using cached types_PyYAML-6.0.12.8-py3-none-any.whl (14 kB)
Collecting types-Deprecated
  Using cached types_Deprecated-1.2.9.1-py3-none-any.whl (3.2 kB)
Collecting types-pyaudio
  Using cached types_pyaudio-0.2.16.6-py3-none-any.whl (3.6 kB)
Collecting types-kazoo
  Using cached types_kazoo-0.1.3-py3-none-any.whl (4.1 kB)
Collecting types-chardet
  Using cached types_chardet-5.0.4.2-py3-none-any.whl (5.9 kB)
Collecting types-pysftp
  Using cached types_pysftp-0.2.17.2-py3-none-any.whl (4.2 kB)
Collecting types-Werkzeug
  Using cached types_Werkzeug-1.0.9-py3-none-any.whl (36 kB)
Collecting types-toml
  Using cached types_toml-0.10.8.5-py3-none-any.whl (4.5 kB)
Collecting types-click-spinner
  Using cached types_click_spinner-0.1.13.3-py3-none-any.whl (2.7 kB)
Collecting types-tornado
  Using cached types_tornado-5.1.1-py3-none-any.whl (13 kB)
Collecting types-click
  Using cached types_click-7.1.8-py3-none-any.whl (12 kB)
Collecting types-first
  Using cached types_first-2.0.5.1-py3-none-any.whl (2.1 kB)
Collecting types-Routes
  Using cached types_Routes-2.5.0-py3-none-any.whl (3.3 kB)
Collecting types-typed-ast
  Using cached types_typed_ast-1.5.8.5-py3-none-any.whl (6.0 kB)
Collecting types-Markdown
  Using cached types_Markdown-3.4.2.5-py3-none-any.whl (16 kB)
Collecting types-mypy-extensions
  Using cached types_mypy_extensions-1.0.0.3-py3-none-any.whl (3.3 kB)
Collecting types-simplejson
  Using cached types_simplejson-3.18.0.1-py3-none-any.whl (4.0 kB)
Collecting types-protobuf
  Using cached types_protobuf-4.22.0.0-py3-none-any.whl (61 kB)
Collecting types-tabulate
  Using cached types_tabulate-0.9.0.1-py3-none-any.whl (3.1 kB)
Collecting types-DateTimeRange
  Using cached types_DateTimeRange-2.0.0.3-py3-none-any.whl (3.2 kB)
Collecting types-retry
  Using cached types_retry-0.9.9.2-py3-none-any.whl (2.4 kB)
Collecting types-termcolor
  Using cached types_termcolor-1.1.6.1-py3-none-any.whl (2.4 kB)
Collecting types-mock
  Using cached types_mock-5.0.0.5-py3-none-any.whl (5.0 kB)
Collecting types-waitress
  Using cached types_waitress-2.1.4.5-py3-none-any.whl (12 kB)
Collecting types-Flask
  Using cached types_Flask-1.1.6-py3-none-any.whl (13 kB)
Collecting types-PyJWT
  Using cached types_PyJWT-1.7.1-py2.py3-none-any.whl (4.7 kB)
Collecting types-pyfarmhash
  Using cached types_pyfarmhash-0.3.1.1-py3-none-any.whl (2.1 kB)
Collecting types-PyMySQL
  Using cached types_PyMySQL-1.0.19.5-py3-none-any.whl (13 kB)
Collecting types-bleach
  Using cached types_bleach-6.0.0.1-py3-none-any.whl (5.5 kB)
Collecting types-docopt
  Using cached types_docopt-0.6.11.3-py3-none-any.whl (2.3 kB)
Collecting types-pymssql
  Using cached types_pymssql-2.1.0-py3-none-any.whl (2.4 kB)
Collecting types-docutils
  Using cached types_docutils-0.19.1.6-py3-none-any.whl (16 kB)
Collecting types-singledispatch
  Using cached types_singledispatch-4.0.0.1-py3-none-any.whl (2.5 kB)
Collecting types-pathlib2
  Using cached types_pathlib2-2.3.0-py3-none-any.whl (2.9 kB)
Collecting types-Jinja2
  Using cached types_Jinja2-2.11.9-py3-none-any.whl (18 kB)
Collecting types-pyRFC3339
  Using cached types_pyRFC3339-1.1.1.3-py3-none-any.whl (3.0 kB)
Collecting types-aiofiles
  Using cached types_aiofiles-23.1.0.0-py3-none-any.whl (8.5 kB)
Collecting types-maxminddb
  Using cached types_maxminddb-1.5.0-py3-none-any.whl (4.3 kB)
Collecting types-openssl-python
  Using cached types_openssl_python-0.1.3-py2.py3-none-any.whl (4.5 kB)
Collecting types-python-slugify
  Using cached types_python_slugify-8.0.0.1-py3-none-any.whl (3.2 kB)
Collecting types-pytz
  Using cached types_pytz-2022.7.1.2-py3-none-any.whl (4.7 kB)
Collecting types-tzlocal
  Using cached types_tzlocal-4.3.0.0-py3-none-any.whl (2.7 kB)
Collecting types-dataclasses
  Using cached types_dataclasses-0.6.6-py3-none-any.whl (2.9 kB)
Collecting types-python-gflags
  Using cached types_python_gflags-3.1.7.2-py3-none-any.whl (4.2 kB)
Collecting types-fb303
  Using cached types_fb303-1.0.0-py3-none-any.whl (2.8 kB)
Collecting types-enum34
  Using cached types_enum34-1.1.8-py3-none-any.whl (2.8 kB)
Collecting types-contextvars
  Using cached types_contextvars-2.4.7.1-py3-none-any.whl (2.6 kB)
Collecting types-decorator
  Using cached types_decorator-5.1.8.3-py3-none-any.whl (2.8 kB)
Collecting types-annoy
  Using cached types_annoy-1.17.8.2-py3-none-any.whl (2.7 kB)
Collecting types-croniter
  Using cached types_croniter-1.3.2.6-py3-none-any.whl (3.6 kB)
Collecting types-MarkupSafe
  Using cached types_MarkupSafe-1.1.10-py3-none-any.whl (4.0 kB)
Collecting types-ipaddress
  Using cached types_ipaddress-1.0.8-py3-none-any.whl (3.1 kB)
Collecting types-requests
  Downloading types_requests-2.28.11.16-py3-none-any.whl (14 kB)
Collecting types-geoip2
  Using cached types_geoip2-3.0.0-py3-none-any.whl (4.7 kB)
Collecting types-boto
  Using cached types_boto-2.49.18.6-py3-none-any.whl (23 kB)
Collecting types-freezegun
  Using cached types_freezegun-1.1.10-py3-none-any.whl (2.9 kB)
Collecting types-backports-abc
  Using cached types_backports_abc-0.5.2-py3-none-any.whl (2.0 kB)
Collecting types-paramiko
  Using cached types_paramiko-3.0.0.4-py3-none-any.whl (31 kB)
Collecting types-itsdangerous
  Using cached types_itsdangerous-1.1.6-py3-none-any.whl (3.4 kB)
Collecting types-orjson
  Using cached types_orjson-3.6.2-py3-none-any.whl (2.2 kB)
Collecting types-characteristic
  Using cached types_characteristic-14.3.7-py3-none-any.whl (2.5 kB)
Collecting types-pkg-resources
  Using cached types_pkg_resources-0.1.3-py2.py3-none-any.whl (4.8 kB)
Collecting types-pycurl
  Using cached types_pycurl-7.45.2.3-py3-none-any.whl (6.4 kB)
Collecting types-nmap
  Using cached types_nmap-0.1.6-py3-none-any.whl (3.0 kB)
Collecting types-futures
  Using cached types_futures-3.3.8-py3-none-any.whl (4.4 kB)
Collecting types-xxhash
  Using cached types_xxhash-3.0.5.2-py3-none-any.whl (2.8 kB)
Collecting types-pyvmomi
  Using cached types_pyvmomi-8.0.0.1-py3-none-any.whl (5.9 kB)
Collecting types-redis
  Downloading types_redis-4.5.3.0-py3-none-any.whl (55 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 55.6/55.6 KB 2.2 MB/s eta 0:00:00
Collecting types-JACK-Client
  Using cached types_JACK_Client-0.5.10.7-py3-none-any.whl (5.0 kB)
Collecting types-colorama
  Using cached types_colorama-0.4.15.8-py3-none-any.whl (5.5 kB)
Collecting types-python-dateutil
  Using cached types_python_dateutil-2.8.19.10-py3-none-any.whl (9.1 kB)
Collecting types-six
  Using cached types_six-1.16.21.7-py3-none-any.whl (14 kB)
Collecting types-atomicwrites
  Using cached types_atomicwrites-1.4.5.1-py3-none-any.whl (2.5 kB)
Collecting types-dateparser
  Using cached types_dateparser-1.1.4.8-py3-none-any.whl (15 kB)
Collecting types-Pillow
  Using cached types_Pillow-9.4.0.17-py3-none-any.whl (46 kB)
Collecting types-cachetools
  Using cached types_cachetools-5.3.0.4-py3-none-any.whl (3.6 kB)
Collecting types-frozendict
  Using cached types_frozendict-2.0.9-py3-none-any.whl (2.4 kB)
Collecting types-certifi
  Using cached types_certifi-2021.10.8.3-py3-none-any.whl (2.1 kB)
Collecting types-emoji
  Using cached types_emoji-2.1.0.2-py3-none-any.whl (3.5 kB)
Collecting types-scribe
  Using cached types_scribe-2.0.0-py3-none-any.whl (2.8 kB)
Collecting types-ujson
  Using cached types_ujson-5.7.0.1-py3-none-any.whl (2.2 kB)
Collecting types-polib
  Using cached types_polib-1.2.0.0-py3-none-any.whl (3.3 kB)
Collecting types-cryptography
  Using cached types_cryptography-3.3.23.2-py3-none-any.whl (30 kB)
Requirement already satisfied: setuptools in /usr/local/lib/python3.9/site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->mastodon-importer==0.0.1) (58.1.0)
Collecting certifi>=2017.4.17
  Using cached certifi-2022.12.7-py3-none-any.whl (155 kB)
Collecting urllib3<1.27,>=1.21.1
  Using cached urllib3-1.26.15-py2.py3-none-any.whl (140 kB)
Collecting idna<4,>=2.5
  Using cached idna-3.4-py3-none-any.whl (61 kB)
Collecting charset-normalizer<4,>=2
  Using cached charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (199 kB)
Collecting platformdirs<4,>=2.4
  Using cached platformdirs-3.1.1-py3-none-any.whl (14 kB)
Collecting filelock<4,>=3.4.1
  Downloading filelock-3.10.3-py3-none-any.whl (10 kB)
Collecting distlib<1,>=0.3.6
  Using cached distlib-0.3.6-py2.py3-none-any.whl (468 kB)
Collecting zipp>=3.1.0
  Using cached zipp-3.15.0-py3-none-any.whl (6.8 kB)
Collecting types-cffi
  Downloading types_cffi-1.15.1.8-py3-none-any.whl (13 kB)
Collecting cryptography>=37.0.0
  Downloading cryptography-40.0.0-cp36-abi3-manylinux_2_28_x86_64.whl (3.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 3.7/3.7 MB 50.3 MB/s eta 0:00:00
Collecting types-pyOpenSSL
  Using cached types_pyOpenSSL-23.0.0.4-py3-none-any.whl (6.9 kB)
Collecting types-urllib3<1.27
  Using cached types_urllib3-1.26.25.8-py3-none-any.whl (15 kB)
Collecting cffi>=1.12
  Using cached cffi-1.15.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (441 kB)
Collecting dnspython>=1.15.0
  Using cached dnspython-2.3.0-py3-none-any.whl (283 kB)
Collecting smmap<6,>=3.0.1
  Using cached smmap-5.0.0-py3-none-any.whl (24 kB)
Collecting h11>=0.8
  Using cached h11-0.14.0-py3-none-any.whl (58 kB)
Collecting asgiref>=3.4.0
  Using cached asgiref-3.6.0-py3-none-any.whl (23 kB)
Collecting uvloop!=0.15.0,!=0.15.1,>=0.14.0
  Using cached uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.2 MB)
Collecting python-dotenv>=0.13
  Using cached python_dotenv-1.0.0-py3-none-any.whl (19 kB)
Collecting httptools>=0.4.0
  Using cached httptools-0.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (417 kB)
Collecting watchgod>=0.6
  Using cached watchgod-0.8.2-py3-none-any.whl (12 kB)
Collecting websockets>=10.0
  Using cached websockets-10.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (106 kB)
Collecting sniffio>=1.1
  Using cached sniffio-1.3.0-py3-none-any.whl (10 kB)
Collecting pycparser
  Using cached pycparser-2.21-py2.py3-none-any.whl (118 kB)
Building wheels for collected packages: mastodon-importer
  Building wheel for mastodon-importer (setup.py): started
  Building wheel for mastodon-importer (setup.py): finished with status 'done'
  Created wheel for mastodon-importer: filename=mastodon_importer-0.0.1-py3-none-any.whl size=20318 sha256=437978059d105033ce170546eb9438a96300c1213a580158109741b27e3254da
  Stored in directory: /tmp/pip-ephem-wheel-cache-wy0wjv4z/wheels/7d/f7/a7/dfc4be396d24447b346982bea51b462508f41a7750797c40e2
Successfully built mastodon-importer
Installing collected packages: types-xxhash, types-Werkzeug, types-waitress, types-urllib3, types-ujson, types-typed-ast, types-tornado, types-toml, types-termcolor, types-tabulate, types-six, types-singledispatch, types-simplejson, types-Routes, types-retry, types-PyYAML, types-pyvmomi, types-pytz, types-python-slugify, types-python-gflags, types-python-dateutil, types-pyRFC3339, types-PyMySQL, types-pymssql, types-pyfarmhash, types-pycurl, types-pyaudio, types-protobuf, types-polib, types-pkg-resources, types-Pillow, types-pathlib2, types-orjson, types-nmap, types-mypy-extensions, types-mock, types-MarkupSafe, types-Markdown, types-kazoo, types-itsdangerous, types-ipaddress, types-futures, types-frozendict, types-freezegun, types-first, types-filelock, types-fb303, types-enum34, types-emoji, types-docutils, types-docopt, types-Deprecated, types-decorator, types-dateparser, types-dataclasses, types-cryptography, types-croniter, types-contextvars, types-colorama, types-click-spinner, types-click, types-chardet, types-characteristic, types-cffi, types-certifi, types-cachetools, types-boto, types-bleach, types-backports-abc, types-backports, types-atomicwrites, types-annoy, types-aiofiles, dol, distlib, blurhash, zipp, websockets, uvloop, urllib3, ujson, typing-extensions, types-tzlocal, types-scribe, types-requests, types-PyJWT, types-openssl-python, types-maxminddb, types-Jinja2, types-DateTimeRange, tomli, sniffio, smmap, six, pyyaml, python-magic, python-dotenv, pycparser, pluggy, platformdirs, pillow, packaging, orjson, numpy, nodeenv, mypy-extensions, MarkupSafe, loguru, itsdangerous, iniconfig, idna, identify, httptools, h11, giturlparse, filelock, fastprogress, exceptiongroup, dnspython, decorator, config2py, click, charset-normalizer, cfgv, certifi, attrs, asgiref, virtualenv, uvicorn, types-JACK-Client, types-geoip2, types-Flask, typer, requests, python-multipart, python-dateutil, pytest, pydantic, mypy, jinja2, importlib-resources, gitdb, fastscript, fastcore, email_validator, cffi, anyio, watchgod, starlette, pytest-timeout, py2store, pre-commit, mastodon.py, GitPython, cryptography, types-pyOpenSSL, types-paramiko, fastapi, types-redis, types-pysftp, types-all, pymemri, mastodon-importer
Successfully installed GitPython-3.1.27 MarkupSafe-2.1.2 anyio-3.6.2 asgiref-3.6.0 attrs-22.2.0 blurhash-1.1.4 certifi-2022.12.7 cffi-1.15.1 cfgv-3.3.1 charset-normalizer-3.1.0 click-8.1.3 config2py-0.1.0 cryptography-40.0.0 decorator-5.1.1 distlib-0.3.6 dnspython-2.3.0 dol-0.1.124 email_validator-1.3.1 exceptiongroup-1.1.1 fastapi-0.78.0 fastcore-1.3.21 fastprogress-1.0.3 fastscript-1.0.0 filelock-3.10.3 gitdb-4.0.10 giturlparse-0.10.0 h11-0.14.0 httptools-0.5.0 identify-2.5.21 idna-3.4 importlib-resources-5.12.0 iniconfig-2.0.0 itsdangerous-2.1.2 jinja2-3.0.0 loguru-0.6.0 mastodon-importer-0.0.1 mastodon.py-1.8.0 mypy-1.1.1 mypy-extensions-1.0.0 nodeenv-1.7.0 numpy-1.24.2 orjson-3.8.8 packaging-23.0 pillow-8.4.0 platformdirs-3.1.1 pluggy-1.0.0 pre-commit-2.21.0 py2store-0.1.18 pycparser-2.21 pydantic-1.10.2 pymemri-0.0.45 pytest-7.2.2 pytest-timeout-2.1.0 python-dateutil-2.8.2 python-dotenv-1.0.0 python-magic-0.4.27 python-multipart-0.0.5 pyyaml-6.0 requests-2.28.2 six-1.16.0 smmap-5.0.0 sniffio-1.3.0 starlette-0.19.1 tomli-2.0.1 typer-0.7.0 types-DateTimeRange-2.0.0.3 types-Deprecated-1.2.9.1 types-Flask-1.1.6 types-JACK-Client-0.5.10.7 types-Jinja2-2.11.9 types-Markdown-3.4.2.5 types-MarkupSafe-1.1.10 types-Pillow-9.4.0.17 types-PyJWT-1.7.1 types-PyMySQL-1.0.19.5 types-PyYAML-6.0.12.8 types-Routes-2.5.0 types-Werkzeug-1.0.9 types-aiofiles-23.1.0.0 types-all-1.0.0 types-annoy-1.17.8.2 types-atomicwrites-1.4.5.1 types-backports-0.1.3 types-backports-abc-0.5.2 types-bleach-6.0.0.1 types-boto-2.49.18.6 types-cachetools-5.3.0.4 types-certifi-2021.10.8.3 types-cffi-1.15.1.8 types-characteristic-14.3.7 types-chardet-5.0.4.2 types-click-7.1.8 types-click-spinner-0.1.13.3 types-colorama-0.4.15.8 types-contextvars-2.4.7.1 types-croniter-1.3.2.6 types-cryptography-3.3.23.2 types-dataclasses-0.6.6 types-dateparser-1.1.4.8 types-decorator-5.1.8.3 types-docopt-0.6.11.3 types-docutils-0.19.1.6 types-emoji-2.1.0.2 types-enum34-1.1.8 types-fb303-1.0.0 types-filelock-3.2.7 types-first-2.0.5.1 types-freezegun-1.1.10 types-frozendict-2.0.9 types-futures-3.3.8 types-geoip2-3.0.0 types-ipaddress-1.0.8 types-itsdangerous-1.1.6 types-kazoo-0.1.3 types-maxminddb-1.5.0 types-mock-5.0.0.5 types-mypy-extensions-1.0.0.3 types-nmap-0.1.6 types-openssl-python-0.1.3 types-orjson-3.6.2 types-paramiko-3.0.0.4 types-pathlib2-2.3.0 types-pkg-resources-0.1.3 types-polib-1.2.0.0 types-protobuf-4.22.0.0 types-pyOpenSSL-23.0.0.4 types-pyRFC3339-1.1.1.3 types-pyaudio-0.2.16.6 types-pycurl-7.45.2.3 types-pyfarmhash-0.3.1.1 types-pymssql-2.1.0 types-pysftp-0.2.17.2 types-python-dateutil-2.8.19.10 types-python-gflags-3.1.7.2 types-python-slugify-8.0.0.1 types-pytz-2022.7.1.2 types-pyvmomi-8.0.0.1 types-redis-4.5.3.0 types-requests-2.28.11.16 types-retry-0.9.9.2 types-scribe-2.0.0 types-simplejson-3.18.0.1 types-singledispatch-4.0.0.1 types-six-1.16.21.7 types-tabulate-0.9.0.1 types-termcolor-1.1.6.1 types-toml-0.10.8.5 types-tornado-5.1.1 types-typed-ast-1.5.8.5 types-tzlocal-4.3.0.0 types-ujson-5.7.0.1 types-urllib3-1.26.25.8 types-waitress-2.1.4.5 types-xxhash-3.0.5.2 typing-extensions-4.5.0 ujson-5.7.0 urllib3-1.26.15 uvicorn-0.17.6 uvloop-0.17.0 virtualenv-20.21.0 watchgod-0.8.2 websockets-10.4 zipp-3.15.0
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
WARNING: You are using pip version 22.0.4; however, version 23.0.1 is available.
You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.
[32;1m$ curl http://pod:3030/version[0;m
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100    58  100    58    0     0  19333      0 --:--:-- --:--:-- --:--:-- 29000
{"build_profile":null,"cargo":"0.4.4","git_describe":null}[32;1m$ export POD_ADDRESS='http://pod:3030'[0;m
[32;1m$ pytest -s[0;m
The user_configs_dirpath doesn't exist. Making it: /root/.py2store_configs
The myconfigs_dirpath doesn't exist. Making it: /root/.py2store_configs/my
============================= test session starts ==============================
platform linux -- Python 3.9.16, pytest-7.2.2, pluggy-1.0.0
rootdir: /builds/memri/plugins/mastodon, configfile: setup.cfg
plugins: timeout-2.1.0, anyio-3.6.2
collected 3 items

tests/test_plugin.py 2023-03-24 07:14:41.642 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
2023-03-24 07:14:42.000 | INFO     | mastodon_importer.plugin:sync:124 - Starting import of tweets
2023-03-24 07:14:42.092 | INFO     | mastodon_importer.plugin:sync:128 - Importing me
2023-03-24 07:14:42.098 | INFO     | mastodon_importer.plugin:sync:131 - Importing friends
2023-03-24 07:14:42.110 | INFO     | mastodon_importer.plugin:sync:134 - Waiting for futures to complete
2023-03-24 07:14:42.111 | INFO     | mastodon_importer.plugin:wait_for_futures:139 - Waiting for futures to complete and join consumer thread
2023-03-24 07:14:42.178 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 90/90 items/edges
2023-03-24 07:14:42.220 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 90 items/edges
2023-03-24 07:14:42.222 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {'Tweet': 20, 'Account': 4})
2023-03-24 07:14:42.226 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 15/15 items/edges
2023-03-24 07:14:42.236 | INFO     | mastodon_importer.plugin:sync:136 - Futures are completed
2023-03-24 07:14:42.249 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 15 items/edges
2023-03-24 07:14:42.250 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {'Tweet': 20, 'Account': 4, 'Photo': 3, 'File': 3})
2023-03-24 07:14:42.251 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 5/5 items/edges
2023-03-24 07:14:42.271 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 5 items/edges
2023-03-24 07:14:42.271 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {'Tweet': 20, 'Account': 4, 'Photo': 4, 'File': 4})
2023-03-24 07:14:42.309 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
.2023-03-24 07:14:42.522 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
2023-03-24 07:14:42.810 | INFO     | mastodon_importer.plugin:sync:124 - Starting import of tweets
2023-03-24 07:14:42.890 | INFO     | mastodon_importer.plugin:sync:128 - Importing me
2023-03-24 07:14:42.913 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 36/36 items/edges
2023-03-24 07:14:42.925 | INFO     | mastodon_importer.plugin:sync:131 - Importing friends
2023-03-24 07:14:42.934 | INFO     | mastodon_importer.plugin:sync:134 - Waiting for futures to complete
2023-03-24 07:14:42.935 | INFO     | mastodon_importer.plugin:wait_for_futures:139 - Waiting for futures to complete and join consumer thread
2023-03-24 07:14:42.951 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 36 items/edges
2023-03-24 07:14:42.953 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {'Tweet': 20, 'Account': 1})
2023-03-24 07:14:42.986 | INFO     | mastodon_importer.plugin:sync:136 - Futures are completed
2023-03-24 07:14:43.003 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 74/74 items/edges
2023-03-24 07:14:43.030 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 74 items/edges
2023-03-24 07:14:43.032 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {'Tweet': 20, 'Account': 4, 'Photo': 4, 'File': 4})
2023-03-24 07:14:43.188 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
2023-03-24 07:14:43.698 | INFO     | mastodon_importer.plugin:sync:124 - Starting import of tweets
2023-03-24 07:14:43.769 | INFO     | mastodon_importer.plugin:sync:128 - Importing me
2023-03-24 07:14:43.772 | INFO     | mastodon_importer.plugin:sync:131 - Importing friends
2023-03-24 07:14:43.777 | INFO     | mastodon_importer.plugin:sync:134 - Waiting for futures to complete
2023-03-24 07:14:43.778 | INFO     | mastodon_importer.plugin:wait_for_futures:139 - Waiting for futures to complete and join consumer thread
2023-03-24 07:14:43.778 | INFO     | mastodon_importer.plugin:sync:136 - Futures are completed
2023-03-24 07:14:43.836 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 6/6 items/edges
2023-03-24 07:14:43.849 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 6 items/edges
2023-03-24 07:14:43.849 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {})
.
tests/test_twitter_users.py 2023-03-24 07:14:43.988 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
2023-03-24 07:14:44.343 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 30/30 items/edges
2023-03-24 07:14:44.370 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 30 items/edges
2023-03-24 07:14:44.371 | INFO     | mastodon_importer.consumer:add_count:42 - defaultdict(<class 'int'>, {'Account': 4, 'Photo': 4, 'File': 4})
2023-03-24 07:14:44.385 | WARNING  | pymemri.pod.client:create_account:81 - 404 Endpoint not found
.

=============================== warnings summary ===============================
tests/test_plugin.py::test_benchmark
tests/test_plugin.py::test_duplicates
tests/test_twitter_users.py::test_following
  /usr/local/lib/python3.9/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    warnings.warn(

tests/test_plugin.py: 65 warnings
tests/test_twitter_users.py: 11 warnings
  /builds/memri/plugins/mastodon/mastodon_importer/pod_update_queue.py:89: DeprecationWarning: `copy_on_model_validation` should be a string: 'deep', 'shallow' or 'none'
    pod_update = PodUpdate(

tests/test_plugin.py: 574 warnings
tests/test_twitter_users.py: 38 warnings
  /builds/memri/plugins/mastodon/mastodon_importer/pod_update_queue.py:28: DeprecationWarning: `copy_on_model_validation` should be a string: 'deep', 'shallow' or 'none'
    return PodUpdate(

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
======================= 3 passed, 691 warnings in 2.97s ========================
section_end:1679642085:step_script
[0Ksection_start:1679642085:archive_cache
[0K[0K[36;1mSaving cache for successful job[0;m[0;m
[32;1mCreating cache default-protected...[0;m
.cache/pip: found 1530 matching files and directories[0;m 
No URL provided, cache will not be uploaded to shared cache server. Cache will be stored only locally.[0;m 
[32;1mCreated cache[0;m
section_end:1679642090:archive_cache
[0Ksection_start:1679642090:cleanup_file_variables
[0K[0K[36;1mCleaning up project directory and file based variables[0;m[0;m
section_end:1679642090:cleanup_file_variables
[0K[32;1mJob succeeded[0;m
```