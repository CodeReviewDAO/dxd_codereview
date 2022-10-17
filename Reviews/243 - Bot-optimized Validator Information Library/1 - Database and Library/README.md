Grant Proposal | [243 - Bot-optimized Validator Information Library](https://portal.devxdao.com/public-proposals/243)
------------ | -------------
Milestone | 1
Milestone Title | Database and Library
OP | furkanahmetk
Reviewer | Chad <elmabahma@gmail.com>

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

-Mysql or MongoDB database will be created to store and map status metrics about validators.
-Getting information from Casper Network about validators and sending them to the database.
-API development : Developing API to get requested information from database. API will be developed with python.

**Acceptance criteria:**

-Code of database and database itself will be available to review.
-List of tools that are used for the database and methods will be explained and available.
-API repository and API itself will be available with README and HOW TOs.


**Additional notes regarding submission from OP:**

API is deployed on an Ubuntu 20.04 server and can be found here for testing endpoints with auto generated API documentation:

http://38.242.242.73:5555/swagger-ui/#/

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/furkanahmetk/Casper-Bot-Optimized-API | 18c665c

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/furkanahmetk/Casper-Bot-Optimized-API, reviewer was
able to successfully install Prerequisites ,build and run the source code for this milestone :


````bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/243/Casper-Bot-Optimized-API$ make run
pip3 install virtualenv==20.16.5
Collecting virtualenv==20.16.5
  Downloading virtualenv-20.16.5-py3-none-any.whl (8.8 MB)
     |████████████████████████████████| 8.8 MB 40.7 MB/s
Collecting filelock<4,>=3.4.1
  Downloading filelock-3.8.0-py3-none-any.whl (10 kB)
Collecting distlib<1,>=0.3.5
  Downloading distlib-0.3.6-py2.py3-none-any.whl (468 kB)
     |████████████████████████████████| 468 kB 106.7 MB/s
Collecting platformdirs<3,>=2.4
  Downloading platformdirs-2.5.2-py3-none-any.whl (14 kB)
Installing collected packages: filelock, distlib, platformdirs, virtualenv
Successfully installed distlib-0.3.6 filelock-3.8.0 platformdirs-2.5.2 virtualenv-20.16.5
python3 -m virtualenv env
created virtual environment CPython3.8.10.final.0-64 in 193ms
  creator CPython3Posix(dest=/home/abahmane/reviews/243/Casper-Bot-Optimized-API/env, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, setuptools=bundle, wheel=bundle, via=copy, app_data_dir=/home/abahmane/.local/share/virtualenv)
    added seed packages: pip==22.2.2, setuptools==65.3.0, wheel==0.37.1
  activators BashActivator,CShellActivator,FishActivator,NushellActivator,PowerShellActivator,PythonActivator
. env/bin/activate
pip3 install -r requirements.txt
Collecting pytest==4.0.0
  Downloading pytest-4.0.0-py2.py3-none-any.whl (217 kB)
     |████████████████████████████████| 217 kB 52.3 MB/s
Collecting Flask==2.0.0
  Downloading Flask-2.0.0-py3-none-any.whl (93 kB)
     |████████████████████████████████| 93 kB 15.2 MB/s
Collecting marshmallow==3.15.0
  Downloading marshmallow-3.15.0-py3-none-any.whl (47 kB)
     |████████████████████████████████| 47 kB 42.2 MB/s
Collecting requests==2.27.1
  Downloading requests-2.27.1-py2.py3-none-any.whl (63 kB)
     |████████████████████████████████| 63 kB 12.1 MB/s
Collecting python-dotenv==0.19.2
  Downloading python_dotenv-0.19.2-py2.py3-none-any.whl (17 kB)
Collecting pymongo==4.2.0
  Downloading pymongo-4.2.0-cp38-cp38-manylinux2014_x86_64.whl (506 kB)
     |████████████████████████████████| 506 kB 155.8 MB/s
Collecting APScheduler==3.9.1
  Downloading APScheduler-3.9.1-py2.py3-none-any.whl (59 kB)
     |████████████████████████████████| 59 kB 43.6 MB/s
Collecting mongomock==4.1.2
  Downloading mongomock-4.1.2-py2.py3-none-any.whl (60 kB)
     |████████████████████████████████| 60 kB 54.7 MB/s
Collecting Flask-APScheduler==1.12.4
  Downloading Flask-APScheduler-1.12.4.tar.gz (12 kB)
Collecting webargs==8.2.0
  Downloading webargs-8.2.0-py3-none-any.whl (30 kB)
Collecting flask-apispec==0.11.4
  Downloading flask_apispec-0.11.4-py2.py3-none-any.whl (2.4 MB)
     |████████████████████████████████| 2.4 MB 83.4 MB/s
Collecting apispec==5.2.2
  Downloading apispec-5.2.2-py3-none-any.whl (29 kB)
Requirement already satisfied: setuptools in /usr/lib/python3/dist-packages (from pytest==4.0.0->-r requirements.txt (line 1)) (45.2.0)
Collecting py>=1.5.0
  Downloading py-1.11.0-py2.py3-none-any.whl (98 kB)
     |████████████████████████████████| 98 kB 37.5 MB/s
Collecting atomicwrites>=1.0
  Downloading atomicwrites-1.4.1.tar.gz (14 kB)
Collecting more-itertools>=4.0.0
  Downloading more_itertools-8.14.0-py3-none-any.whl (52 kB)
     |████████████████████████████████| 52 kB 9.6 MB/s
Collecting attrs>=17.4.0
  Downloading attrs-22.1.0-py2.py3-none-any.whl (58 kB)
     |████████████████████████████████| 58 kB 47.6 MB/s
Collecting pluggy>=0.7
  Downloading pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Requirement already satisfied: six>=1.10.0 in /usr/lib/python3/dist-packages (from pytest==4.0.0->-r requirements.txt (line 1)) (1.14.0)
Collecting Werkzeug>=2.0
  Downloading Werkzeug-2.2.2-py3-none-any.whl (232 kB)
     |████████████████████████████████| 232 kB 120.4 MB/s
Collecting click>=7.1.2
  Downloading click-8.1.3-py3-none-any.whl (96 kB)
     |████████████████████████████████| 96 kB 47.2 MB/s
Collecting itsdangerous>=2.0
  Downloading itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting Jinja2>=3.0
  Downloading Jinja2-3.1.2-py3-none-any.whl (133 kB)
     |████████████████████████████████| 133 kB 81.3 MB/s
Requirement already satisfied: packaging in /usr/lib/python3/dist-packages (from marshmallow==3.15.0->-r requirements.txt (line 3)) (20.3)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /usr/lib/python3/dist-packages (from requests==2.27.1->-r requirements.txt (line 4)) (1.25.8)
Requirement already satisfied: certifi>=2017.4.17 in /usr/lib/python3/dist-packages (from requests==2.27.1->-r requirements.txt (line 4)) (2019.11.28)
Requirement already satisfied: idna<4,>=2.5; python_version >= "3" in /usr/lib/python3/dist-packages (from requests==2.27.1->-r requirements.txt (line 4)) (2.8)
Collecting charset-normalizer~=2.0.0; python_version >= "3"
  Downloading charset_normalizer-2.0.12-py3-none-any.whl (39 kB)
Collecting pytz
  Downloading pytz-2022.4-py2.py3-none-any.whl (500 kB)
     |████████████████████████████████| 500 kB 139.4 MB/s
Collecting tzlocal!=3.*,>=2.0
  Downloading tzlocal-4.2-py3-none-any.whl (19 kB)
Collecting sentinels
  Downloading sentinels-1.0.0.tar.gz (4.1 kB)
Collecting python-dateutil>=2.4.2
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     |████████████████████████████████| 247 kB 123.1 MB/s
Collecting MarkupSafe>=2.1.1
  Downloading MarkupSafe-2.1.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting pytz-deprecation-shim
  Downloading pytz_deprecation_shim-0.1.0.post0-py2.py3-none-any.whl (15 kB)
Collecting backports.zoneinfo; python_version < "3.9"
  Downloading backports.zoneinfo-0.2.1-cp38-cp38-manylinux1_x86_64.whl (74 kB)
     |████████████████████████████████| 74 kB 22.6 MB/s
Collecting tzdata; python_version >= "3.6"
  Downloading tzdata-2022.5-py2.py3-none-any.whl (336 kB)
     |████████████████████████████████| 336 kB 130.9 MB/s
Building wheels for collected packages: Flask-APScheduler, atomicwrites, sentinels
  Building wheel for Flask-APScheduler (setup.py) ... done
  Created wheel for Flask-APScheduler: filename=Flask_APScheduler-1.12.4-py3-none-any.whl size=15725 sha256=a36021ceac3bfb5b33e39b0e23c6738e0443f22aa77758868f5a7e8db0f2bcda
  Stored in directory: /home/abahmane/.cache/pip/wheels/83/89/54/0f51ff73f88b28b6d0af3dad42efed206c732fd5edec3fcb08
  Building wheel for atomicwrites (setup.py) ... done
  Created wheel for atomicwrites: filename=atomicwrites-1.4.1-py2.py3-none-any.whl size=6943 sha256=cac12e1dfe943bbea59862e4150dbf3221e2599fa604ae35f7206dba50261322
  Stored in directory: /home/abahmane/.cache/pip/wheels/ce/24/c1/56b1ca77dda9577b75eb88d7ec50425f103ec2f6170c6e97df
  Building wheel for sentinels (setup.py) ... done
  Created wheel for sentinels: filename=sentinels-1.0.0-py3-none-any.whl size=3186 sha256=ff3c82e4c237114898a2e47af0841f1acc286c06e7379f06992a6bb048a6ca1b
  Stored in directory: /home/abahmane/.cache/pip/wheels/52/6d/1d/f8b21b7cc5b50cba5e5744c06f71fdac7d7464cb6f35e61abf
Successfully built Flask-APScheduler atomicwrites sentinels
Installing collected packages: py, atomicwrites, more-itertools, attrs, pluggy, pytest, MarkupSafe, Werkzeug, click, itsdangerous, Jinja2, Flask, marshmallow, charset-normalizer, requests, python-dotenv, pymongo, pytz, tzdata, backports.zoneinfo, pytz-deprecation-shim, tzlocal, APScheduler, sentinels, mongomock, python-dateutil, Flask-APScheduler, webargs, apispec, flask-apispec
Successfully installed APScheduler-3.9.1 Flask-2.0.0 Flask-APScheduler-1.12.4 Jinja2-3.1.2 MarkupSafe-2.1.1 Werkzeug-2.2.2 apispec-5.2.2 atomicwrites-1.4.1 attrs-22.1.0 backports.zoneinfo-0.2.1 charset-normalizer-2.0.12 click-8.1.3 flask-apispec-0.11.4 itsdangerous-2.1.2 marshmallow-3.15.0 mongomock-4.1.2 more-itertools-8.14.0 pluggy-1.0.0 py-1.11.0 pymongo-4.2.0 pytest-4.0.0 python-dateutil-2.8.2 python-dotenv-0.19.2 pytz-2022.4 pytz-deprecation-shim-0.1.0.post0 requests-2.27.1 sentinels-1.0.0 tzdata-2022.5 tzlocal-4.2 webargs-8.2.0
python3 run.py
 * Serving Flask app 'src.app' (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: off
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:5555
 * Running on http://65.108.1.10:5555
Press CTRL+C to quit
````

The source code was build and run on an Ubuntu 20.04 server.

The reviewer was then able to connect to Swagger REST endpoint that was deployed on the server : http://65.108.1.10:5555

**The reviewer recommends the OP to add a section on how to Run the application as a Service**

![243](../assets/swagger_Rest.png "endpoint")

The reviewer checked the endpoint exposes the four following methods : 

/delegationRate <br>/state<br>/totalDelegators<br>/totalStake

* Example of usage :

1- delegationRate

![243](../assets/delegationRate.png "delegationRate")

2- state

![243](../assets/state.png "state")

3- totalDelegators

![243](../assets/total_delegators.png "total_delegators")

3- totalStake

![243](../assets/total_stake.png "total_stake")

## Overall Impression of usage testing

The reviewer was able to build and run the application.
For a small project like this the build instructions are sufficient and clear. The OP also provides the list of prerequisites to install and in particular MongoDB.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS
Can connect to a Casper node | PASS

# Unit / Automated Testing

The project contains 15 unit tests which covers the 4 methods above.
The tests can be executed from the console and cover both positive and negative test paths.
**For the next milestone, the OP is encouraged to :<br>
1- Add more negative path tests <br>
2- Add logging to tests. Reviewer was not able to know what test scenarios are running while executing tests**

```bash
make test
```

```bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/243/Casper-Bot-Optimized-API$ make test
python3 -m pytest
====================================================================================================== test session starts =======================================================================================================
platform linux -- Python 3.8.10, pytest-4.0.0, py-1.11.0, pluggy-1.0.0
rootdir: /home/abahmane/reviews/243/Casper-Bot-Optimized-API, inifile:
collected 5 items

tests/integration/test_endpoints.py ....                                                                                                                                                                                   [ 80%]
tests/unit/test_models.py .                                                                                                                                                                                                [100%]

==================================================================================================== 5 passed in 0.04 seconds ====================================================================================================
```


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS/A

# Documentation

### Code Documentation

The code is now overall well documented and almost all classes and critical functions have acceptable code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

The project documentation is generally sufficient and the instructions for building and running project are clear.
The -Example Usage- paragraph in the Readme file details the different operations exposed by the endpoint.
The Rest API deployed  through Swagger once the application is launched  is well documented.
For a project of this size, documentation is clear and sufficient.


Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The Project is released under the Apache License

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

The project contains a CONTRIBUTING policy that links to a Code of Conduct policy. Pull requests and Issues are enabled.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

Code is generally well-structured and very readable. The project as committed to GitHub and both the unit tests and the manual tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS 
------------ | -------------