```sh
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo apt -y install apache2
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  apache2-bin apache2-data apache2-utils libaprutil1-dbd-sqlite3 libaprutil1-ldap libjansson4 liblua5.2-0 ssl-cert
Suggested packages:
  apache2-doc apache2-suexec-pristine | apache2-suexec-custom ufw openssl-blacklist
The following NEW packages will be installed:
  apache2 apache2-bin apache2-data apache2-utils libaprutil1-dbd-sqlite3 libaprutil1-ldap libjansson4 liblua5.2-0 ssl-cert
0 upgraded, 9 newly installed, 0 to remove and 4 not upgraded.
Need to get 1,691 kB of archives.
After this operation, 7,527 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1-dbd-sqlite3 amd64 1.6.1-4ubuntu2 [10.5 kB]
Get:2 http://archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1-ldap amd64 1.6.1-4ubuntu2 [8,736 B]
Get:3 http://archive.ubuntu.com/ubuntu focal/main amd64 libjansson4 amd64 2.12-1build1 [28.9 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal/main amd64 liblua5.2-0 amd64 5.2.4-1.1build3 [106 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-bin amd64 2.4.41-4ubuntu3.12 [1,181 kB]
Get:6 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-data all 2.4.41-4ubuntu3.12 [159 kB]
Get:7 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-utils amd64 2.4.41-4ubuntu3.12 [84.5 kB]
Get:8 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2 amd64 2.4.41-4ubuntu3.12 [95.6 kB]
Get:9 http://archive.ubuntu.com/ubuntu focal/main amd64 ssl-cert all 1.0.39 [17.0 kB]
Fetched 1,691 kB in 1s (1,621 kB/s)
Preconfiguring packages ...
Selecting previously unselected package libaprutil1-dbd-sqlite3:amd64.
(Reading database ... 70604 files and directories currently installed.)
Preparing to unpack .../0-libaprutil1-dbd-sqlite3_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1-dbd-sqlite3:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libaprutil1-ldap:amd64.
Preparing to unpack .../1-libaprutil1-ldap_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1-ldap:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libjansson4:amd64.
Preparing to unpack .../2-libjansson4_2.12-1build1_amd64.deb ...
Unpacking libjansson4:amd64 (2.12-1build1) ...
Selecting previously unselected package liblua5.2-0:amd64.
Preparing to unpack .../3-liblua5.2-0_5.2.4-1.1build3_amd64.deb ...
Unpacking liblua5.2-0:amd64 (5.2.4-1.1build3) ...
Selecting previously unselected package apache2-bin.
Preparing to unpack .../4-apache2-bin_2.4.41-4ubuntu3.12_amd64.deb ...
Unpacking apache2-bin (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package apache2-data.
Preparing to unpack .../5-apache2-data_2.4.41-4ubuntu3.12_all.deb ...
Unpacking apache2-data (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package apache2-utils.
Preparing to unpack .../6-apache2-utils_2.4.41-4ubuntu3.12_amd64.deb ...
Unpacking apache2-utils (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package apache2.
Preparing to unpack .../7-apache2_2.4.41-4ubuntu3.12_amd64.deb ...
Unpacking apache2 (2.4.41-4ubuntu3.12) ...
Selecting previously unselected package ssl-cert.
Preparing to unpack .../8-ssl-cert_1.0.39_all.deb ...
Unpacking ssl-cert (1.0.39) ...
Setting up libaprutil1-ldap:amd64 (1.6.1-4ubuntu2) ...
Setting up libaprutil1-dbd-sqlite3:amd64 (1.6.1-4ubuntu2) ...
Setting up libjansson4:amd64 (2.12-1build1) ...
Setting up ssl-cert (1.0.39) ...
Setting up liblua5.2-0:amd64 (5.2.4-1.1build3) ...
Setting up apache2-data (2.4.41-4ubuntu3.12) ...
Setting up apache2-utils (2.4.41-4ubuntu3.12) ...
Setting up apache2-bin (2.4.41-4ubuntu3.12) ...
Setting up apache2 (2.4.41-4ubuntu3.12) ...
Enabling module mpm_event.
Enabling module authz_core.
Enabling module authz_host.
Enabling module authn_core.
Enabling module auth_basic.
Enabling module access_compat.
Enabling module authn_file.
Enabling module authz_user.
Enabling module alias.
Enabling module dir.
Enabling module autoindex.
Enabling module env.
Enabling module mime.
Enabling module negotiation.
Enabling module setenvif.
Enabling module filter.
Enabling module deflate.
Enabling module status.
Enabling module reqtimeout.
Enabling conf charset.
Enabling conf localized-error-pages.
Enabling conf other-vhosts-access-log.
Enabling conf security.
Enabling conf serve-cgi-bin.
Enabling site 000-default.
Created symlink /etc/systemd/system/multi-user.target.wants/apache2.service → /lib/systemd/system/apache2.service.
Created symlink /etc/systemd/system/multi-user.target.wants/apache-htcacheclean.service → /lib/systemd/system/apache-htcacheclean.service.
invoke-rc.d: could not determine current runlevel
invoke-rc.d: policy-rc.d denied execution of start.
Processing triggers for systemd (245.4-4ubuntu3.17) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.9) ...
```
```
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo a2enmod rewrite
Enabling module rewrite.
To activate the new configuration, you need to run:
  service apache2 restart
```
```
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo a2enmod headers
Enabling module headers.
To activate the new configuration, you need to run:
  service apache2 restart
```
```
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo a2enmod ssl
Considering dependency setenvif for ssl:
Module setenvif already enabled
Considering dependency mime for ssl:
Module mime already enabled
Considering dependency socache_shmcb for ssl:
Enabling module socache_shmcb.
Enabling module ssl.
See /usr/share/doc/apache2/README.Debian.gz on how to configure SSL and create self-signed certificates.
To activate the new configuration, you need to run:
  service apache2 restart
```
```
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo apt -y install software-properties-common
Reading package lists... Done
Building dependency tree       
Reading state information... Done
software-properties-common is already the newest version (0.99.9.8).
0 upgraded, 0 newly installed, 0 to remove and 4 not upgraded.
```
```
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo add-apt-repository ppa:ondrej/php
 Co-installable PHP versions: PHP 5.6, PHP 7.x and most requested extensions are included. Only Supported Versions of PHP (http://php.net/supported-versions.php) for Supported Ubuntu Releases (https://wiki.ubuntu.com/Releases) are provided. Don't ask for end-of-life PHP versions or Ubuntu release, they won't be provided.

Debian oldstable and stable packages are provided as well: https://deb.sury.org/#debian-dpa

You can get more information about the packages at https://deb.sury.org

IMPORTANT: The <foo>-backports is now required on older Ubuntu releases.

BUGS&FEATURES: This PPA now has a issue tracker:
https://deb.sury.org/#bug-reporting

CAVEATS:
1. If you are using php-gearman, you need to add ppa:ondrej/pkg-gearman
2. If you are using apache2, you are advised to add ppa:ondrej/apache2
3. If you are using nginx, you are advised to add ppa:ondrej/nginx-mainline
   or ppa:ondrej/nginx

PLEASE READ: If you like my work and want to give me a little motivation, please consider donating regularly: https://donate.sury.org/

WARNING: add-apt-repository is broken with non-UTF-8 locales, see
https://github.com/oerdnj/deb.sury.org/issues/56 for workaround:

# LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php
 More info: https://launchpad.net/~ondrej/+archive/ubuntu/php
Press [ENTER] to continue or Ctrl-c to cancel adding it.

Get:1 https://packages.microsoft.com/repos/microsoft-ubuntu-focal-prod focal InRelease [10.5 kB]
Hit:2 https://cli.github.com/packages stable InRelease                                                                    
Hit:3 https://repo.anaconda.com/pkgs/misc/debrepo/conda stable InRelease                                                  
Get:4 http://ppa.launchpad.net/ondrej/php/ubuntu focal InRelease [23.9 kB]                                                
Hit:5 http://ppa.launchpad.net/xapienz/curl34/ubuntu focal InRelease                                                      
Hit:6 http://archive.ubuntu.com/ubuntu focal InRelease                     
Get:7 https://packages.microsoft.com/repos/microsoft-ubuntu-focal-prod focal/main amd64 Packages [185 kB]
Get:8 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]                                   
Get:9 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Get:10 http://ppa.launchpad.net/ondrej/php/ubuntu focal/main amd64 Packages [169 kB]
Get:11 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]                                                
Get:12 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages [1,161 kB]
Get:13 http://security.ubuntu.com/ubuntu focal-security/main amd64 Packages [1,979 kB]
Get:14 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages [2,420 kB]                               
Get:16 http://archive.ubuntu.com/ubuntu focal-updates/restricted amd64 Packages [1,437 kB]                                
Get:17 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 Packages [1,339 kB]        
Hit:15 https://packagecloud.io/github/git-lfs/ubuntu focal InRelease              
Fetched 9,061 kB in 2s (4,480 kB/s)
Reading package lists... Done
```
```
@ggurbet ➜ /workspaces/devxdao-backend (master) $ sudo apt-get update
Hit:1 https://cli.github.com/packages stable InRelease
Hit:2 http://security.ubuntu.com/ubuntu focal-security InRelease                                                          
Hit:3 http://ppa.launchpad.net/ondrej/php/ubuntu focal InRelease                                                          
Hit:4 https://repo.anaconda.com/pkgs/misc/debrepo/conda stable InRelease                                                  
Hit:5 http://ppa.launchpad.net/xapienz/curl34/ubuntu focal InRelease                                                      
Hit:6 https://packages.microsoft.com/repos/microsoft-ubuntu-focal-prod focal InRelease                                    
Hit:7 http://archive.ubuntu.com/ubuntu focal InRelease                                                                    
Hit:8 http://archive.ubuntu.com/ubuntu focal-updates InRelease       
Hit:9 http://archive.ubuntu.com/ubuntu focal-backports InRelease     
Hit:10 https://packagecloud.io/github/git-lfs/ubuntu focal InRelease 
Reading package lists... Done
```
```

```