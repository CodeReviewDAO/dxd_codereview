```
$ pip install -e .
Obtaining file:///Z:/CRDAO/Memri_Milestone3/speech-to-text-main
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Collecting whisper@ git+https://github.com/openai/whisper.git@f82bc59
  Cloning https://github.com/openai/whisper.git (to revision f82bc59) to c:\users\houpha\appdata\local\temp\pip-install-69_4v41u\whisper_e47bad4783c848a0b39ba26da83b0f7a
  Running command git clone --filter=blob:none --quiet https://github.com/openai/whisper.git 'C:\Users\HouPha\AppData\Local\Temp\pip-install-69_4v41u\whisper_e47bad4783c848a0b39ba26da83b0f7a'
  WARNING: Did not find branch or tag 'f82bc59', assuming revision or ref.
  Running command git checkout -q f82bc59
  Resolved https://github.com/openai/whisper.git to commit f82bc59
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: pytest~=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from speech-to-text==0.0.1) (7.1.3)
Collecting pymemri==0.0.40
  Downloading pymemri-0.0.40-py3-none-any.whl (69 kB)
     ---------------------------------------- 69.6/69.6 kB 1.9 MB/s eta 0:00:00
Requirement already satisfied: loguru~=0.6.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from speech-to-text==0.0.1) (0.6.0)
Requirement already satisfied: pre-commit~=2.20 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from speech-to-text==0.0.1) (2.20.0)
Collecting yt-dlp
  Downloading yt_dlp-2023.2.17-py2.py3-none-any.whl (2.9 MB)
     ---------------------------------------- 2.9/2.9 MB 8.7 MB/s eta 0:00:00
Requirement already satisfied: jinja2==3.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (3.0.0)
Requirement already satisfied: pydantic==1.10.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (1.10.2)
Requirement already satisfied: fastapi[all]==0.78.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (0.78.0)
Requirement already satisfied: fastcore==1.3.21 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (1.3.21)
Requirement already satisfied: numpy in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (1.23.3)
Requirement already satisfied: giturlparse==0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (0.10.0)
Requirement already satisfied: GitPython==3.1.27 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (3.1.27)
Requirement already satisfied: fastprogress in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (1.0.3)
Requirement already satisfied: pillow==8.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (8.4.0)
Requirement already satisfied: requests in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (2.28.1)
Requirement already satisfied: fastscript in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pymemri==0.0.40->speech-to-text==0.0.1) (1.0.0)
Requirement already satisfied: starlette==0.19.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.19.1)
Requirement already satisfied: email_validator<2.0.0,>=1.1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (1.3.0)
Requirement already satisfied: uvicorn[standard]<0.18.0,>=0.12.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.17.6)
Requirement already satisfied: orjson<4.0.0,>=3.2.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (3.8.0)
Requirement already satisfied: python-multipart<0.0.6,>=0.0.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.0.5)
Requirement already satisfied: pyyaml<7.0.0,>=5.3.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (5.4.1)
Requirement already satisfied: itsdangerous<3.0.0,>=1.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (2.1.2)
Requirement already satisfied: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (5.5.0)
Requirement already satisfied: pip in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.40->speech-to-text==0.0.1) (22.3.1)
Requirement already satisfied: packaging in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from fastcore==1.3.21->pymemri==0.0.40->speech-to-text==0.0.1) (21.3)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from GitPython==3.1.27->pymemri==0.0.40->speech-to-text==0.0.1) (4.0.9)
Requirement already satisfied: MarkupSafe>=2.0.0rc2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from jinja2==3.0.0->pymemri==0.0.40->speech-to-text==0.0.1) (2.1.1)
Requirement already satisfied: typing-extensions>=4.1.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pydantic==1.10.2->pymemri==0.0.40->speech-to-text==0.0.1) (4.4.0)
Requirement already satisfied: anyio<5,>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (3.6.1)
Requirement already satisfied: win32-setctime>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->speech-to-text==0.0.1) (1.1.0)
Requirement already satisfied: colorama>=0.3.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from loguru~=0.6.0->speech-to-text==0.0.1) (0.4.5)
Requirement already satisfied: identify>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->speech-to-text==0.0.1) (2.5.9)
Requirement already satisfied: cfgv>=2.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->speech-to-text==0.0.1) (3.3.1)
Requirement already satisfied: nodeenv>=0.11.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->speech-to-text==0.0.1) (1.7.0)
Requirement already satisfied: virtualenv>=20.0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->speech-to-text==0.0.1) (20.17.1)
Requirement already satisfied: toml in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pre-commit~=2.20->speech-to-text==0.0.1) (0.10.2)
Requirement already satisfied: attrs>=19.2.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->speech-to-text==0.0.1) (22.1.0)
Requirement already satisfied: iniconfig in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->speech-to-text==0.0.1) (1.1.1)
Requirement already satisfied: py>=1.8.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->speech-to-text==0.0.1) (1.11.0)
Requirement already satisfied: pluggy<2.0,>=0.12 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->speech-to-text==0.0.1) (1.0.0)
Requirement already satisfied: tomli>=1.0.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from pytest~=7.0->speech-to-text==0.0.1) (2.0.1)
Requirement already satisfied: torch in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (1.12.0)
Requirement already satisfied: tqdm in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (4.64.1)
Collecting more-itertools
  Downloading more_itertools-9.0.0-py3-none-any.whl (52 kB)
     ---------------------------------------- 52.8/52.8 kB ? eta 0:00:00
Requirement already satisfied: transformers>=4.19.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (4.25.1)
Collecting ffmpeg-python==0.2.0
  Downloading ffmpeg_python-0.2.0-py3-none-any.whl (25 kB)
Collecting future
  Downloading future-0.18.3.tar.gz (840 kB)
     ------------------------------------- 840.9/840.9 kB 10.6 MB/s eta 0:00:00
  Preparing metadata (setup.py): started
  Preparing metadata (setup.py): finished with status 'done'
Requirement already satisfied: certifi in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from yt-dlp->speech-to-text==0.0.1) (2022.9.24)
Requirement already satisfied: websockets in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from yt-dlp->speech-to-text==0.0.1) (10.3)
Collecting brotli
  Downloading Brotli-1.0.9-cp310-cp310-win_amd64.whl (383 kB)
     ------------------------------------- 383.3/383.3 kB 12.0 MB/s eta 0:00:00
Collecting mutagen
  Downloading mutagen-1.46.0-py3-none-any.whl (193 kB)
     ---------------------------------------- 193.6/193.6 kB ? eta 0:00:00
Collecting pycryptodomex
  Downloading pycryptodomex-3.17-cp35-abi3-win_amd64.whl (1.7 MB)
     ---------------------------------------- 1.7/1.7 MB 13.8 MB/s eta 0:00:00
Requirement already satisfied: setuptools in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from nodeenv>=0.11.1->pre-commit~=2.20->speech-to-text==0.0.1) (63.2.0)
Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.40->speech-to-text==0.0.1) (2.1.1)
Requirement already satisfied: idna<4,>=2.5 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.40->speech-to-text==0.0.1) (3.4)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from requests->pymemri==0.0.40->speech-to-text==0.0.1) (1.26.12)
Requirement already satisfied: filelock in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers>=4.19.0->whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (3.8.2)
Requirement already satisfied: tokenizers!=0.11.3,<0.14,>=0.11.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers>=4.19.0->whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (0.13.2)
Requirement already satisfied: regex!=2019.12.17 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers>=4.19.0->whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (2022.9.13)
Requirement already satisfied: huggingface-hub<1.0,>=0.10.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from transformers>=4.19.0->whisper@ git+https://github.com/openai/whisper.git@f82bc59->speech-to-text==0.0.1) (0.11.1)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from packaging->fastcore==1.3.21->pymemri==0.0.40->speech-to-text==0.0.1) (3.0.9)
Requirement already satisfied: platformdirs<3,>=2.4 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->speech-to-text==0.0.1) (2.6.0)
Requirement already satisfied: distlib<1,>=0.3.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from virtualenv>=20.0.8->pre-commit~=2.20->speech-to-text==0.0.1) (0.3.6)
Requirement already satisfied: dnspython>=1.15.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from email_validator<2.0.0,>=1.1.1->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (2.2.1)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from gitdb<5,>=4.0.1->GitPython==3.1.27->pymemri==0.0.40->speech-to-text==0.0.1) (5.0.0)
Requirement already satisfied: six>=1.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from python-multipart<0.0.6,>=0.0.5->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (1.16.0)
Requirement already satisfied: h11>=0.8 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.14.0)
Requirement already satisfied: click>=7.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (8.1.3)
Requirement already satisfied: asgiref>=3.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (3.5.2)
Requirement already satisfied: watchgod>=0.6 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.8.2)
Requirement already satisfied: httptools>=0.4.0 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.5.0)
Requirement already satisfied: python-dotenv>=0.13 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from uvicorn[standard]<0.18.0,>=0.12.0->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (0.21.0)
Requirement already satisfied: sniffio>=1.1 in c:\users\houpha\appdata\local\programs\python\python310\lib\site-packages (from anyio<5,>=3.4.0->starlette==0.19.1->fastapi[all]==0.78.0->pymemri==0.0.40->speech-to-text==0.0.1) (1.3.0)
Installing collected packages: brotli, pycryptodomex, mutagen, more-itertools, future, yt-dlp, ffmpeg-python, whisper, pymemri, speech-to-text
  DEPRECATION: future is being installed using the legacy 'setup.py install' method, because it does not have a 'pyproject.toml' and the 'wheel' package is not installed. pip 23.1 will enforce this behaviour change. A possible replacement is to enable the '--use-pep517' option. Discussion can be found at https://github.com/pypa/pip/issues/8559
  Running setup.py install for future: started
  Running setup.py install for future: finished with status 'done'
  DEPRECATION: whisper is being installed using the legacy 'setup.py install' method, because it does not have a 'pyproject.toml' and the 'wheel' package is not installed. pip 23.1 will enforce this behaviour change. A possible replacement is to enable the '--use-pep517' option. Discussion can be found at https://github.com/pypa/pip/issues/8559
  Running setup.py install for whisper: started
  Running setup.py install for whisper: finished with status 'done'
  Attempting uninstall: pymemri
    Found existing installation: pymemri 0.0.34
    Uninstalling pymemri-0.0.34:
      Successfully uninstalled pymemri-0.0.34
  Running setup.py develop for speech-to-text
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
whatsapp 1.0 requires protobuf==3.19.4, but you have protobuf 4.21.10 which is incompatible.
language-identification 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.40 which is incompatible.
zero-shot-plugin 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.40 which is incompatible.
gmail-oauth 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.40 which is incompatible.
twitter 0.2.1 requires pymemri==0.0.34, but you have pymemri 0.0.40 which is incompatible.
twitter-topic-model 0.0.1 requires pymemri==0.0.34, but you have pymemri 0.0.40 which is incompatible.
Successfully installed brotli-1.0.9 ffmpeg-python-0.2.0 future-0.18.3 more-itertools-9.0.0 mutagen-1.46.0 pycryptodomex-3.17 pymemri-0.0.40 speech-to-text-0.0.1 whisper-1.0 yt-dlp-2023.2.17

[notice] A new release of pip available: 22.3.1 -> 23.0.1
[notice] To update, run: python.exe -m pip install --upgrade pip

```