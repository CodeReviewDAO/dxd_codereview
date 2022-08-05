```sh
gitpod /workspace/casperfyre-backend (main) $ sudo apt update
gitpod /workspace/casperfyre-backend (main) $ sudo apt install mysql-server
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  libaio1 libcgi-fast-perl libcgi-pm-perl libencode-locale-perl libfcgi-perl
  libhtml-parser-perl libhtml-tagset-perl libhtml-template-perl
  libhttp-date-perl libhttp-message-perl libio-html-perl
  liblwp-mediatypes-perl libmecab2 libnuma1 libtimedate-perl liburi-perl
  mecab-ipadic mecab-ipadic-utf8 mecab-utils mysql-client-8.0
  mysql-client-core-8.0 mysql-server-8.0 mysql-server-core-8.0 psmisc
Suggested packages:
  libdata-dump-perl libipc-sharedcache-perl libwww-perl mailx tinyca
The following NEW packages will be installed:
  libaio1 libcgi-fast-perl libcgi-pm-perl libencode-locale-perl libfcgi-perl
  libhtml-parser-perl libhtml-tagset-perl libhtml-template-perl
  libhttp-date-perl libhttp-message-perl libio-html-perl
  liblwp-mediatypes-perl libmecab2 libnuma1 libtimedate-perl liburi-perl
  mecab-ipadic mecab-ipadic-utf8 mecab-utils mysql-client-8.0
  mysql-client-core-8.0 mysql-server mysql-server-8.0 mysql-server-core-8.0
  psmisc
0 upgraded, 25 newly installed, 0 to remove and 21 not upgraded.
Need to get 32.1 MB of archives.
After this operation, 264 MB of additional disk space will be used.
Do you want to continue? [Y/n] 
Get:1 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-client-core-8.0 amd64 8.0.30-0ubuntu0.20.04.2 [4,521 kB]
Get:2 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-client-8.0 amd64 8.0.30-0ubuntu0.20.04.2 [22.0 kB]
Get:3 http://archive.ubuntu.com/ubuntu focal/main amd64 libaio1 amd64 0.3.112-5 [7,184 B]
Get:4 http://archive.ubuntu.com/ubuntu focal/main amd64 libmecab2 amd64 0.996-10build1 [233 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal/main amd64 libnuma1 amd64 2.0.12-1 [20.8 kB]
Get:6 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-server-core-8.0 amd64 8.0.30-0ubuntu0.20.04.2 [18.6 MB]
Get:7 http://archive.ubuntu.com/ubuntu focal/main amd64 psmisc amd64 23.3-1 [53.3 kB]
Get:8 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-server-8.0 amd64 8.0.30-0ubuntu0.20.04.2 [1,292 kB]
Get:9 http://archive.ubuntu.com/ubuntu focal/main amd64 libhtml-tagset-perl all 3.20-4 [12.5 kB]
Get:10 http://archive.ubuntu.com/ubuntu focal/main amd64 liburi-perl all 1.76-2 [77.5 kB]
Get:11 http://archive.ubuntu.com/ubuntu focal/main amd64 libhtml-parser-perl amd64 3.72-5 [86.3 kB]
Get:12 http://archive.ubuntu.com/ubuntu focal/main amd64 libcgi-pm-perl all 4.46-1 [186 kB]
Get:13 http://archive.ubuntu.com/ubuntu focal/main amd64 libfcgi-perl amd64 0.79-1 [33.1 kB]
Get:14 http://archive.ubuntu.com/ubuntu focal/main amd64 libcgi-fast-perl all 1:2.15-1 [10.5 kB]
Get:15 http://archive.ubuntu.com/ubuntu focal/main amd64 libencode-locale-perl all 1.05-1 [12.3 kB]
Get:16 http://archive.ubuntu.com/ubuntu focal/main amd64 libhtml-template-perl all 2.97-1 [59.0 kB]
Get:17 http://archive.ubuntu.com/ubuntu focal/main amd64 libtimedate-perl all 2.3200-1 [34.0 kB]
Get:18 http://archive.ubuntu.com/ubuntu focal/main amd64 libhttp-date-perl all 6.05-1 [9,920 B]
Get:19 http://archive.ubuntu.com/ubuntu focal/main amd64 libio-html-perl all 1.001-1 [14.9 kB]
Get:20 http://archive.ubuntu.com/ubuntu focal/main amd64 liblwp-mediatypes-perl all 6.04-1 [19.5 kB]
Get:21 http://archive.ubuntu.com/ubuntu focal/main amd64 libhttp-message-perl all 6.22-1 [76.1 kB]
Get:22 http://archive.ubuntu.com/ubuntu focal/main amd64 mecab-utils amd64 0.996-10build1 [4,912 B]
Get:23 http://archive.ubuntu.com/ubuntu focal/main amd64 mecab-ipadic all 2.7.0-20070801+main-2.1 [6,714 kB]
Get:24 http://archive.ubuntu.com/ubuntu focal/main amd64 mecab-ipadic-utf8 all 2.7.0-20070801+main-2.1 [4,380 B]
Get:25 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-server all 8.0.30-0ubuntu0.20.04.2 [9,540 B]
Fetched 32.1 MB in 2s (18.2 MB/s)
debconf: delaying package configuration, since apt-utils is not installed
Selecting previously unselected package mysql-client-core-8.0.
(Reading database ... 36091 files and directories currently installed.)
Preparing to unpack .../00-mysql-client-core-8.0_8.0.30-0ubuntu0.20.04.2_amd64.deb ...
Unpacking mysql-client-core-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Selecting previously unselected package mysql-client-8.0.
Preparing to unpack .../01-mysql-client-8.0_8.0.30-0ubuntu0.20.04.2_amd64.deb ...
Unpacking mysql-client-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Selecting previously unselected package libaio1:amd64.
Preparing to unpack .../02-libaio1_0.3.112-5_amd64.deb ...
Unpacking libaio1:amd64 (0.3.112-5) ...
Selecting previously unselected package libmecab2:amd64.
Preparing to unpack .../03-libmecab2_0.996-10build1_amd64.deb ...
Unpacking libmecab2:amd64 (0.996-10build1) ...
Selecting previously unselected package libnuma1:amd64.
Preparing to unpack .../04-libnuma1_2.0.12-1_amd64.deb ...
Unpacking libnuma1:amd64 (2.0.12-1) ...
Selecting previously unselected package mysql-server-core-8.0.
Preparing to unpack .../05-mysql-server-core-8.0_8.0.30-0ubuntu0.20.04.2_amd64.deb ...
Unpacking mysql-server-core-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Selecting previously unselected package psmisc.
Preparing to unpack .../06-psmisc_23.3-1_amd64.deb ...
Unpacking psmisc (23.3-1) ...
Selecting previously unselected package mysql-server-8.0.
Preparing to unpack .../07-mysql-server-8.0_8.0.30-0ubuntu0.20.04.2_amd64.deb ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 76.)
debconf: falling back to frontend: Readline
Unpacking mysql-server-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Selecting previously unselected package libhtml-tagset-perl.
Preparing to unpack .../08-libhtml-tagset-perl_3.20-4_all.deb ...
Unpacking libhtml-tagset-perl (3.20-4) ...
Selecting previously unselected package liburi-perl.
Preparing to unpack .../09-liburi-perl_1.76-2_all.deb ...
Unpacking liburi-perl (1.76-2) ...
Selecting previously unselected package libhtml-parser-perl.
Preparing to unpack .../10-libhtml-parser-perl_3.72-5_amd64.deb ...
Unpacking libhtml-parser-perl (3.72-5) ...
Selecting previously unselected package libcgi-pm-perl.
Preparing to unpack .../11-libcgi-pm-perl_4.46-1_all.deb ...
Unpacking libcgi-pm-perl (4.46-1) ...
Selecting previously unselected package libfcgi-perl.
Preparing to unpack .../12-libfcgi-perl_0.79-1_amd64.deb ...
Unpacking libfcgi-perl (0.79-1) ...
Selecting previously unselected package libcgi-fast-perl.
Preparing to unpack .../13-libcgi-fast-perl_1%3a2.15-1_all.deb ...
Unpacking libcgi-fast-perl (1:2.15-1) ...
Selecting previously unselected package libencode-locale-perl.
Preparing to unpack .../14-libencode-locale-perl_1.05-1_all.deb ...
Unpacking libencode-locale-perl (1.05-1) ...
Selecting previously unselected package libhtml-template-perl.
Preparing to unpack .../15-libhtml-template-perl_2.97-1_all.deb ...
Unpacking libhtml-template-perl (2.97-1) ...
Selecting previously unselected package libtimedate-perl.
Preparing to unpack .../16-libtimedate-perl_2.3200-1_all.deb ...
Unpacking libtimedate-perl (2.3200-1) ...
Selecting previously unselected package libhttp-date-perl.
Preparing to unpack .../17-libhttp-date-perl_6.05-1_all.deb ...
Unpacking libhttp-date-perl (6.05-1) ...
Selecting previously unselected package libio-html-perl.
Preparing to unpack .../18-libio-html-perl_1.001-1_all.deb ...
Unpacking libio-html-perl (1.001-1) ...
Selecting previously unselected package liblwp-mediatypes-perl.
Preparing to unpack .../19-liblwp-mediatypes-perl_6.04-1_all.deb ...
Unpacking liblwp-mediatypes-perl (6.04-1) ...
Selecting previously unselected package libhttp-message-perl.
Preparing to unpack .../20-libhttp-message-perl_6.22-1_all.deb ...
Unpacking libhttp-message-perl (6.22-1) ...
Selecting previously unselected package mecab-utils.
Preparing to unpack .../21-mecab-utils_0.996-10build1_amd64.deb ...
Unpacking mecab-utils (0.996-10build1) ...
Selecting previously unselected package mecab-ipadic.
Preparing to unpack .../22-mecab-ipadic_2.7.0-20070801+main-2.1_all.deb ...
Unpacking mecab-ipadic (2.7.0-20070801+main-2.1) ...
Selecting previously unselected package mecab-ipadic-utf8.
Preparing to unpack .../23-mecab-ipadic-utf8_2.7.0-20070801+main-2.1_all.deb ...
Unpacking mecab-ipadic-utf8 (2.7.0-20070801+main-2.1) ...
Selecting previously unselected package mysql-server.
Preparing to unpack .../24-mysql-server_8.0.30-0ubuntu0.20.04.2_all.deb ...
Unpacking mysql-server (8.0.30-0ubuntu0.20.04.2) ...
Setting up libmecab2:amd64 (0.996-10build1) ...
Setting up mysql-client-core-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Setting up psmisc (23.3-1) ...
Setting up libhtml-tagset-perl (3.20-4) ...
Setting up liblwp-mediatypes-perl (6.04-1) ...
Setting up libencode-locale-perl (1.05-1) ...
Setting up mecab-utils (0.996-10build1) ...
Setting up libio-html-perl (1.001-1) ...
Setting up libtimedate-perl (2.3200-1) ...
Setting up libnuma1:amd64 (2.0.12-1) ...
Setting up mysql-client-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Setting up libfcgi-perl (0.79-1) ...
Setting up libaio1:amd64 (0.3.112-5) ...
Setting up liburi-perl (1.76-2) ...
Setting up libhttp-date-perl (6.05-1) ...
Setting up mecab-ipadic (2.7.0-20070801+main-2.1) ...
Compiling IPA dictionary for Mecab.  This takes long time...
reading /usr/share/mecab/dic/ipadic/unk.def ... 40
emitting double-array: 100% |###########################################| 
/usr/share/mecab/dic/ipadic/model.def is not found. skipped.
reading /usr/share/mecab/dic/ipadic/Adj.csv ... 27210
reading /usr/share/mecab/dic/ipadic/Adnominal.csv ... 135
reading /usr/share/mecab/dic/ipadic/Adverb.csv ... 3032
reading /usr/share/mecab/dic/ipadic/Auxil.csv ... 199
reading /usr/share/mecab/dic/ipadic/Conjunction.csv ... 171
reading /usr/share/mecab/dic/ipadic/Filler.csv ... 19
reading /usr/share/mecab/dic/ipadic/Interjection.csv ... 252
reading /usr/share/mecab/dic/ipadic/Noun.adjv.csv ... 3328
reading /usr/share/mecab/dic/ipadic/Noun.adverbal.csv ... 795
reading /usr/share/mecab/dic/ipadic/Noun.csv ... 60477
reading /usr/share/mecab/dic/ipadic/Noun.demonst.csv ... 120
reading /usr/share/mecab/dic/ipadic/Noun.nai.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.name.csv ... 34202
reading /usr/share/mecab/dic/ipadic/Noun.number.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.org.csv ... 16668
reading /usr/share/mecab/dic/ipadic/Noun.others.csv ... 151
reading /usr/share/mecab/dic/ipadic/Noun.place.csv ... 72999
reading /usr/share/mecab/dic/ipadic/Noun.proper.csv ... 27328
reading /usr/share/mecab/dic/ipadic/Noun.verbal.csv ... 12146
reading /usr/share/mecab/dic/ipadic/Others.csv ... 2
reading /usr/share/mecab/dic/ipadic/Postp-col.csv ... 91
reading /usr/share/mecab/dic/ipadic/Postp.csv ... 146
reading /usr/share/mecab/dic/ipadic/Prefix.csv ... 221
reading /usr/share/mecab/dic/ipadic/Suffix.csv ... 1393
reading /usr/share/mecab/dic/ipadic/Symbol.csv ... 208
reading /usr/share/mecab/dic/ipadic/Verb.csv ... 130750
emitting double-array: 100% |###########################################| 
reading /usr/share/mecab/dic/ipadic/matrix.def ... 1316x1316
emitting matrix      : 100% |###########################################| 

done!
update-alternatives: using /var/lib/mecab/dic/ipadic to provide /var/lib/mecab/dic/debian (mecab-dictionary) in auto mode
Setting up mysql-server-core-8.0 (8.0.30-0ubuntu0.20.04.2) ...
Setting up mecab-ipadic-utf8 (2.7.0-20070801+main-2.1) ...
Compiling IPA dictionary for Mecab.  This takes long time...
reading /usr/share/mecab/dic/ipadic/unk.def ... 40
emitting double-array: 100% |###########################################| 
/usr/share/mecab/dic/ipadic/model.def is not found. skipped.
reading /usr/share/mecab/dic/ipadic/Adj.csv ... 27210
reading /usr/share/mecab/dic/ipadic/Adnominal.csv ... 135
reading /usr/share/mecab/dic/ipadic/Adverb.csv ... 3032
reading /usr/share/mecab/dic/ipadic/Auxil.csv ... 199
reading /usr/share/mecab/dic/ipadic/Conjunction.csv ... 171
reading /usr/share/mecab/dic/ipadic/Filler.csv ... 19
reading /usr/share/mecab/dic/ipadic/Interjection.csv ... 252
reading /usr/share/mecab/dic/ipadic/Noun.adjv.csv ... 3328
reading /usr/share/mecab/dic/ipadic/Noun.adverbal.csv ... 795
reading /usr/share/mecab/dic/ipadic/Noun.csv ... 60477
reading /usr/share/mecab/dic/ipadic/Noun.demonst.csv ... 120
reading /usr/share/mecab/dic/ipadic/Noun.nai.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.name.csv ... 34202
reading /usr/share/mecab/dic/ipadic/Noun.number.csv ... 42########..........] 
reading /usr/share/mecab/dic/ipadic/Noun.org.csv ... 16668
reading /usr/share/mecab/dic/ipadic/Noun.others.csv ... 151
reading /usr/share/mecab/dic/ipadic/Noun.place.csv ... 72999
reading /usr/share/mecab/dic/ipadic/Noun.proper.csv ... 27328
reading /usr/share/mecab/dic/ipadic/Noun.verbal.csv ... 12146
reading /usr/share/mecab/dic/ipadic/Others.csv ... 2
reading /usr/share/mecab/dic/ipadic/Postp-col.csv ... 91
reading /usr/share/mecab/dic/ipadic/Postp.csv ... 146
reading /usr/share/mecab/dic/ipadic/Prefix.csv ... 221
reading /usr/share/mecab/dic/ipadic/Suffix.csv ... 1393
reading /usr/share/mecab/dic/ipadic/Symbol.csv ... 208
reading /usr/share/mecab/dic/ipadic/Verb.csv ... 130750
emitting double-array: 100% |###########################################| 
reading /usr/share/mecab/dic/ipadic/matrix.def ... 1316x1316
emitting matrix      : 100% |###########################################| 

done!
update-alternatives: using /var/lib/mecab/dic/ipadic-utf8 to provide /var/lib/mecab/dic/debian (mecab-dictionary) in auto mode
Setting up libhtml-parser-perl (3.72-5) ...
Setting up libhttp-message-perl (6.22-1) ...
Setting up mysql-server-8.0 (8.0.30-0ubuntu0.20.04.2) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 76.)
debconf: falling back to frontend: Readline
invoke-rc.d: could not determine current runlevel
invoke-rc.d: policy-rc.d denied execution of stop.
update-alternatives: using /etc/mysql/mysql.cnf to provide /etc/mysql/my.cnf (my.cnf) in auto mode
Renaming removed key_buffer and myisam-recover options (if present)
mysqld will log errors to /var/log/mysql/error.log
mysqld is running as pid 2143
Created symlink /etc/systemd/system/multi-user.target.wants/mysql.service → /lib/systemd/system/mysql.service.
invoke-rc.d: could not determine current runlevel
invoke-rc.d: policy-rc.d denied execution of start.
Setting up libcgi-pm-perl (4.46-1) ...
Setting up libhtml-template-perl (2.97-1) ...
Setting up mysql-server (8.0.30-0ubuntu0.20.04.2) ...
Setting up libcgi-fast-perl (1:2.15-1) ...
Processing triggers for systemd (245.4-4ubuntu3.17) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.9) ...
```

```sh
gitpod /workspace/casperfyre-backend (main) $ sudo mysql -u root
ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/run/mysqld/mysqld.sock' (2)
gitpod /workspace/casperfyre-backend (main) $ sudo service mysql status
 * MySQL is stopped.
gitpod /workspace/casperfyre-backend (main) $ sudo service mysql start
 * Starting MySQL database server mysqld                                                   su: warning: cannot change directory to /nonexistent: No such file or directory
                                                                                    [ OK ]
gitpod /workspace/casperfyre-backend (main) $ sudo mysql -u root
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 10
Server version: 8.0.30-0ubuntu0.20.04.2 (Ubuntu)

Copyright (c) 2000, 2022, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'crdao';
Query OK, 0 rows affected (0.00 sec)

mysql> create database casperfyre;
Query OK, 1 row affected (0.00 sec)

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| casperfyre         |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)

mysql> exit
Bye
gitpod /workspace/casperfyre-backend (main) $ 

```

```sh
gitpod /workspace/casperfyre-backend (main) $ sudo mkdir /var/www
gitpod /workspace/casperfyre-backend (main) $ cd /var/www
gitpod /var/www $ sudo git clone https://github.com/ledgerleapllc/casperfyre-backend casperfyre-api
Cloning into 'casperfyre-api'...
remote: Enumerating objects: 1659, done.
remote: Counting objects: 100% (443/443), done.
remote: Compressing objects: 100% (219/219), done.
remote: Total 1659 (delta 284), reused 352 (delta 219), pack-reused 1216
Receiving objects: 100% (1659/1659), 14.66 MiB | 17.78 MiB/s, done.
Resolving deltas: 100% (1043/1043), done.
gitpod /var/www $ sudo chown root:www-data /tmp/
gitpod /var/www $ ls -l / | grep tmp
drwxrwxrwt   3 root   www-data  140 Aug  5 17:36 tmp
gitpod /var/www $ sudo chown -R www-data:www-data casperfyre-api/
gitpod /var/www $ ls -l
total 4
drwxr-xr-x 9 www-data www-data 4096 Aug  5 17:33 casperfyre-api
drwxr-xr-x 2 root     root       55 Jul 26 02:34 html
gitpod /var/www $ cd casperfyre-api/
gitpod /var/www/casperfyre-api (main) $ ./setup.sh 


```