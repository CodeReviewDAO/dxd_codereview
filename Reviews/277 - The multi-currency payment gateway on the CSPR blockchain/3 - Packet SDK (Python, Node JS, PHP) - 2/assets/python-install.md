```
yusuf@Yusuf-MacBook-Pro ~ % git clone https://github.com/DHFinance/dhf-pay-python
Cloning into 'dhf-pay-python'...
remote: Enumerating objects: 190, done.
remote: Counting objects: 100% (190/190), done.
remote: Compressing objects: 100% (134/134), done.
remote: Total 190 (delta 87), reused 121 (delta 48), pack-reused 0
Receiving objects: 100% (190/190), 49.39 KiB | 1.10 MiB/s, done.
Resolving deltas: 100% (87/87), done.
yusuf@Yusuf-MacBook-Pro ~ % cd dhf-pay-python 
yusuf@Yusuf-MacBook-Pro dhf-pay-python % ls
CONTRIBUTING.md	README.rst	dhf_wrapper	setup.py
LICENSE		SECURITY.md	setup.cfg	tests
yusuf@Yusuf-MacBook-Pro dhf-pay-python % ls
CONTRIBUTING.md	README.rst	dhf_wrapper	setup.py
LICENSE		SECURITY.md	setup.cfg	tests
yusuf@Yusuf-MacBook-Pro dhf-pay-python % python setup.py install --user
running install
running bdist_egg
running egg_info
creating dhf_sdk.egg-info
writing dhf_sdk.egg-info/PKG-INFO
writing dependency_links to dhf_sdk.egg-info/dependency_links.txt
writing requirements to dhf_sdk.egg-info/requires.txt
writing top-level names to dhf_sdk.egg-info/top_level.txt
writing manifest file 'dhf_sdk.egg-info/SOURCES.txt'
reading manifest file 'dhf_sdk.egg-info/SOURCES.txt'
writing manifest file 'dhf_sdk.egg-info/SOURCES.txt'
installing library code to build/bdist.macosx-10.9-x86_64/egg
running install_lib
running build_py
creating build
creating build/lib
creating build/lib/dhf_wrapper
copying dhf_wrapper/base_client.py -> build/lib/dhf_wrapper
copying dhf_wrapper/client.py -> build/lib/dhf_wrapper
copying dhf_wrapper/__init__.py -> build/lib/dhf_wrapper
copying dhf_wrapper/base_dto.py -> build/lib/dhf_wrapper
copying dhf_wrapper/exceptions.py -> build/lib/dhf_wrapper
creating build/lib/dhf_wrapper/entities
copying dhf_wrapper/entities/store.py -> build/lib/dhf_wrapper/entities
copying dhf_wrapper/entities/params.py -> build/lib/dhf_wrapper/entities
copying dhf_wrapper/entities/transaction.py -> build/lib/dhf_wrapper/entities
copying dhf_wrapper/entities/__init__.py -> build/lib/dhf_wrapper/entities
copying dhf_wrapper/entities/payment.py -> build/lib/dhf_wrapper/entities
creating build/bdist.macosx-10.9-x86_64
creating build/bdist.macosx-10.9-x86_64/egg
creating build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper
copying build/lib/dhf_wrapper/base_client.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper
copying build/lib/dhf_wrapper/client.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper
copying build/lib/dhf_wrapper/__init__.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper
copying build/lib/dhf_wrapper/base_dto.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper
copying build/lib/dhf_wrapper/exceptions.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper
creating build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities
copying build/lib/dhf_wrapper/entities/store.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities
copying build/lib/dhf_wrapper/entities/params.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities
copying build/lib/dhf_wrapper/entities/transaction.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities
copying build/lib/dhf_wrapper/entities/__init__.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities
copying build/lib/dhf_wrapper/entities/payment.py -> build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/base_client.py to base_client.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/client.py to client.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/base_dto.py to base_dto.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/exceptions.py to exceptions.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities/store.py to store.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities/params.py to params.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities/transaction.py to transaction.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities/__init__.py to __init__.cpython-39.pyc
byte-compiling build/bdist.macosx-10.9-x86_64/egg/dhf_wrapper/entities/payment.py to payment.cpython-39.pyc
creating build/bdist.macosx-10.9-x86_64/egg/EGG-INFO
copying dhf_sdk.egg-info/PKG-INFO -> build/bdist.macosx-10.9-x86_64/egg/EGG-INFO
copying dhf_sdk.egg-info/SOURCES.txt -> build/bdist.macosx-10.9-x86_64/egg/EGG-INFO
copying dhf_sdk.egg-info/dependency_links.txt -> build/bdist.macosx-10.9-x86_64/egg/EGG-INFO
copying dhf_sdk.egg-info/requires.txt -> build/bdist.macosx-10.9-x86_64/egg/EGG-INFO
copying dhf_sdk.egg-info/top_level.txt -> build/bdist.macosx-10.9-x86_64/egg/EGG-INFO
zip_safe flag not set; analyzing archive contents...
creating dist
creating 'dist/dhf_sdk-0.0.3-py3.9.egg' and adding 'build/bdist.macosx-10.9-x86_64/egg' to it
removing 'build/bdist.macosx-10.9-x86_64/egg' (and everything under it)
Processing dhf_sdk-0.0.3-py3.9.egg
Copying dhf_sdk-0.0.3-py3.9.egg to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding dhf-sdk 0.0.3 to easy-install.pth file

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/dhf_sdk-0.0.3-py3.9.egg
Processing dependencies for dhf-sdk==0.0.3
Searching for nose>=1.3.7
Reading https://pypi.org/simple/nose/
Downloading https://files.pythonhosted.org/packages/15/d8/dd071918c040f50fa1cf80da16423af51ff8ce4a0f2399b7bf8de45ac3d9/nose-1.3.7-py3-none-any.whl#sha256=9ff7c6cc443f8c51994b34a667bbcf45afd6d945be7477b52e97516fd17c53ac
Best match: nose 1.3.7
Processing nose-1.3.7-py3-none-any.whl
Installing nose-1.3.7-py3-none-any.whl to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding nose 1.3.7 to easy-install.pth file
Installing nosetests script to /Users/yusuf/Library/Python/3.9/bin
Installing nosetests-3.4 script to /Users/yusuf/Library/Python/3.9/bin

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/nose-1.3.7-py3.9.egg
Searching for requests>=2.27.1
Reading https://pypi.org/simple/requests/
Downloading https://files.pythonhosted.org/packages/ca/91/6d9b8ccacd0412c08820f72cebaa4f0c0441b5cda699c90f618b6f8a1b42/requests-2.28.1-py3-none-any.whl#sha256=8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
Best match: requests 2.28.1
Processing requests-2.28.1-py3-none-any.whl
Installing requests-2.28.1-py3-none-any.whl to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding requests 2.28.1 to easy-install.pth file

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/requests-2.28.1-py3.9.egg
Searching for urllib3<1.27,>=1.21.1
Reading https://pypi.org/simple/urllib3/
Downloading https://files.pythonhosted.org/packages/68/47/93d3d28e97c7577f563903907912f4b3804054e4877a5ba6651f7182c53b/urllib3-1.26.10-py2.py3-none-any.whl#sha256=8298d6d56d39be0e3bc13c1c97d133f9b45d797169a0e11cdd0e0489d786f7ec
Best match: urllib3 1.26.10
Processing urllib3-1.26.10-py2.py3-none-any.whl
Installing urllib3-1.26.10-py2.py3-none-any.whl to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding urllib3 1.26.10 to easy-install.pth file

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/urllib3-1.26.10-py3.9.egg
Searching for idna<4,>=2.5
Reading https://pypi.org/simple/idna/
Downloading https://files.pythonhosted.org/packages/04/a2/d918dcd22354d8958fe113e1a3630137e0fc8b44859ade3063982eacd2a4/idna-3.3-py3-none-any.whl#sha256=84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff
Best match: idna 3.3
Processing idna-3.3-py3-none-any.whl
Installing idna-3.3-py3-none-any.whl to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding idna 3.3 to easy-install.pth file

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/idna-3.3-py3.9.egg
Searching for charset-normalizer<3,>=2
Reading https://pypi.org/simple/charset-normalizer/
Downloading https://files.pythonhosted.org/packages/94/69/64b11e8c2fb21f08634468caef885112e682b0ebe2908e74d3616eb1c113/charset_normalizer-2.1.0-py3-none-any.whl#sha256=5189b6f22b01957427f35b6a08d9a0bc45b46d3788ef5a92e978433c7a35f8a5
Best match: charset-normalizer 2.1.0
Processing charset_normalizer-2.1.0-py3-none-any.whl
Installing charset_normalizer-2.1.0-py3-none-any.whl to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding charset-normalizer 2.1.0 to easy-install.pth file
Installing normalizer script to /Users/yusuf/Library/Python/3.9/bin

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/charset_normalizer-2.1.0-py3.9.egg
Searching for certifi>=2017.4.17
Reading https://pypi.org/simple/certifi/
Downloading https://files.pythonhosted.org/packages/e9/06/d3d367b7af6305b16f0d28ae2aaeb86154fa91f144f036c2d5002a5a202b/certifi-2022.6.15-py3-none-any.whl#sha256=fe86415d55e84719d75f8b69414f6438ac3547d2078ab91b67e779ef69378412
Best match: certifi 2022.6.15
Processing certifi-2022.6.15-py3-none-any.whl
Installing certifi-2022.6.15-py3-none-any.whl to /Users/yusuf/Library/Python/3.9/lib/python/site-packages
Adding certifi 2022.6.15 to easy-install.pth file

Installed /Users/yusuf/Library/Python/3.9/lib/python/site-packages/certifi-2022.6.15-py3.9.egg
Finished processing dependencies for dhf-sdk==0.0.3
```
