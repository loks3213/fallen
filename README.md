# fallen
Welcome to Termux!

Wiki:            https://wiki.termux.com
Community forum: https://termux.com/community
Gitter chat:     https://gitter.im/termux/termux
IRC channel:     #termux on freenode

Working with packages:

* Search packages:   pkg search <query>
* Install a package: pkg install <package>
* Upgrade packages:  pkg upgrade

Subscribing to additional repositories:

* Root:     pkg install root-repo
* Unstable: pkg install unstable-repo
* X11:      pkg install x11-repo

Report issues at https://termux.com/issues

$
$ curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && chmod 755 msfinstall && ./msfinstall
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- -  0     0    0     0    0     0      0      0 --:--:-- -  0     0    0     0    0     0      0      0 --:--:--  100  6034  100  6034    0     0   3165      0  0:00:01  0:00:01 --:--:--  3165
This script must be executed as the 'root' user or with sudo
$  adduser msf #Add msf user
No command adduser found, did you mean:
Command fuser in package psmisc
$  su msf #Switch to msf user
No su program found on this device. Termux
does not supply tools for rooting, see e.g.
http://www.androidcentral.com/root for
information about rooting Android.
$  cd /opt/metasploit-framework/bin #Switch to the directory where msf is located
bash: cd: /opt/metasploit-framework/bin: No such file or directory
$  ./msfconsole #After starting msfconsole, switch to the msf user to start, so that the database will be synchronized. If you start with the root user, the database will not be synchronized
bash: ./msfconsole: No such file or directory
$
$  You can also add msfconsole to the execution directory, so you can directly msfconsole in any directory
No command You found, did you mean:
Command du in package coreutils
Command go in package golang
Command dot in package graphviz
Command jo in package jo
Command joe in package joe
Command joe in package jupp
Command ksu in package krb5
Command mdu in package mtools
Command mu in package mu
Command toe in package ncurses-utils
Command nu in package nushell
Command o in package o
Command o in package o-editor
Command moc in package qt5-base from the x11-repo repository
Command co in package rcs
Command sox in package sox
Command su in package termux-tools
Command tor in package tor
Command tsu in package tsu
Command col in package util-linux
Command cu in package uucp
Command wol in package wol
$ ln -s /opt/metasploit-framework/bin/msfconsole /usr/bin/msfconsole
ln: failed to create symbolic link '/usr/bin/msfconsole': No such file or directory
$
$  #Remarks:
$  #The first run of msf will create a database, but the PostgreSQL database used by msf by default cannot be associated with the root user, which is why you need to create a new user msf to run metasploit. If you shook your hand accidentally, the first time you run it under the root user, please use the msfdb reinit command, and then use a non-root user to initialize the database.        $
$  MSf no root
No command MSf found, did you mean:
Command ef in package electric-fence
Command fzf in package fzf
Command lf in package lf
Command rmf in package nmh from the unstable-repo repository
Command df in package termux-tools
Command mf in package texlive-bin
Command tf in package tinyfugue
$ install pkg electric fence
install: target 'fence' is not a directory
$ create new user
No command create found, did you mean:
Command createdb in package postgresql
Command cweave in package texlive-bin
$ install target
install: missing destination file operand after 'target'
Try 'install --help' for more information.
$ install taget 'fence'create user
install: target 'user' is not a directory
$ create user
No command create found, did you mean:
Command createdb in package postgresql
Command cweave in package texlive-bin
$ install 'user' create user
install: target 'user' is not a directory
$ pam_mkhomedir
pam_mkhomedir: command not found
$ pkg install ncurses-utils
Testing the available mirrors:
[*] https://dl.bintray.com/termux/termux-packages-24: bad
[*] https://grimler.se/termux-packages-24: ok
[*] https://main.termux-mirror.ml: ok
[*] https://termux.mentality.rip/termux-packages-24: ok
Picking mirror: https://grimler.se/termux-packages-24
Ign:1 https://dl.bintray.com/grimler/game-packages-24 games InRelease
Ign:2 https://dl.bintray.com/grimler/science-packages-24 science InRelease
Err:3 https://dl.bintray.com/grimler/game-packages-24 games Release
  403  Forbidden
Err:4 https://dl.bintray.com/grimler/science-packages-24 science Release
  403  Forbidden
Get:5 https://grimler.se/termux-packages-24 stable InRelease [16.8 kB]
Get:6 https://grimler.se/termux-packages-24 stable/main aarch64 Packages [246 kB]
Get:7 https://grimler.se/termux-packages-24 stable/main all Packages [18.2 kB]
Reading package lists... Done
E: The repository 'https://dl.bintray.com/grimler/game-packages-24 games Release' does not have a Release file.
N: Metadata integrity can't be verified, repository is disabled now.
N: Possible cause: repository is under maintenance or down (wrong sources.list URL?).
E: The repository 'https://dl.bintray.com/grimler/science-packages-24 science Release' does not have a Release file.
N: Metadata integrity can't be verified, repository is disabled now.
N: Possible cause: repository is under maintenance or down (wrong sources.list URL?).
$ pkg install git clone https://github.com/htr-tech/termux-login.git
Checking availability of current mirror: ok
Reading package lists... Done
Building dependency tree
Reading state information... Done
E: Unable to locate package clone
E: Unable to locate package https://github.com/htr-tech
E: Couldn't find any package by glob 'https://github.com/htr-tech'
E: Couldn't find any package by regex 'https://github.com/htr-tech'
$ $ls
$ ls
div  msfinstall
$ ls
div  msfinstall
$
$ CMSeeK knock termux-lazysqlmap ToolB0x p€ntest
CMSeeK: command not found
$
$ $ cd ..
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ ls
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ home usr
No command home found, did you mean:
Command comm in package coreutils
Command host in package dnsutils
Command hors in package hors
Command joe in package joe
Command joe in package jupp
Command lame in package lame
Command toe in package ncurses-utils
Command comp in package nmh from the unstable-repo repository
Command node in package nodejs
Command node in package nodejs-lts
Command ode in package plotutils from the x11-repo repository
Command htmex in package texlive-bin
Command more in package util-linux
$
$ $ cd usr
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ ls
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ bin include libexec src var etc lib share tmp
No command bin found, did you mean:
Command bat in package bat
Command bc in package bc
Command bsh in package beanshell
Command bison in package bison
Command bmon in package bmon
Command boinc in package boinc
Command bvi in package bvi
Command dir in package coreutils
Command dig in package dnsutils
Command mix in package elixir
Command find in package findutils
Command git in package git
Command gio in package glib-bin
Command i3 in package i3 from the x11-repo repository
Command iw in package iw from the root-repo repository
Command man in package man
Command tic in package ncurses-utils
Command nim in package nim
Command inc in package nmh from the unstable-repo repository
Command nnn in package nnn
Command pil in package picolisp
Command gie in package proj
Command uic in package qt5-base from the x11-repo repository
Command ci in package rcs
Command ri in package ruby-ri
Command svn in package subversion
Command ip in package termux-tools
Command tie in package texlive-bin
Command tig in package tig
Command sn in package tin-summer
Command vi in package vim
Command vi in package vim-gtk from the x11-repo repository
Command vi in package vim-python
Command vis in package vis
Command zip in package zip
$
$ $ cd src
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ ls
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ libsqlite
libsqlite: command not found
$
$ $ cd ..
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ cd bin
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ ls
div  msfinstall
$ 1CMSeeK knock termux-lazysqlmap ToolB0x p€ntest
1CMSeeK: command not found
$ add user
No command add found, did you mean:
Command atd in package at from the unstable-repo repository
Command ldd in package binutils
Command dd in package coreutils
$  apt update && apt upgrade
Ign:1 https://dl.bintray.com/grimler/game-packages-24 games InRelease
Ign:2 https://dl.bintray.com/grimler/science-packages-24 science InRelease
Err:3 https://dl.bintray.com/grimler/game-packages-24 games Release
  403  Forbidden
Hit:4 https://grimler.se/termux-packages-24 stable InRelease
Err:5 https://dl.bintray.com/grimler/science-packages-24 science Release
  403  Forbidden
Reading package lists... Done
E: The repository 'https://dl.bintray.com/grimler/game-packages-24 games Release' does not have a Release file.
N: Metadata integrity can't be verified, repository is disabled now.
N: Possible cause: repository is under maintenance or down (wrong sources.list URL?).
E: The repository 'https://dl.bintray.com/grimler/science-packages-24 science Release' does not have a Release file.
N: Metadata integrity can't be verified, repository is disabled now.
N: Possible cause: repository is under maintenance or down (wrong sources.list URL?).
$ 7z
The program 7z is not installed. Install it by executing:
pkg install p7zip
$ installp7zip
installp7zip: command not found
$ install p7zip
install: missing destination file operand after 'p7zip'
Try 'install --help' for more information.
$ p7a
No command p7a found, did you mean:
Command pr in package coreutils
Command pub in package dart
Command exa in package exa
Command jp2a in package jp2a
Command lha in package lhasa
Command psl in package libpsl
Command lua in package lua
Command pee in package moreutils
Command 7z in package p7zip
Command ptar in package perl
Command phar in package php
Command pil in package picolisp
Command pmap in package procps
Command pup in package pup
Command pv in package pv
Command psc in package sc
Command play in package sox
Command pkg in package termux-tools
$ install pkg termux-tools
install: cannot stat 'pkg': No such file or directory
$ termux tools
No command termux found, did you mean:
Command tmux in package tmux
$ tmux tools.install pkg
The program tmux is not installed. Install it by executing:
pkg install tmux
$ pkg install tmux
Checking availability of current mirror: ok
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
  libevent
The following NEW packages will be installed:
  libevent tmux
0 upgraded, 2 newly installed, 0 to remove and 39 not upgraded.
Need to get 466 kB of archives.
After this operation, 1942 kB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 https://grimler.se/termux-packages-24 stable/main aarch64 libevent aarch64 2.1.12 [189 kB]
Get:2 https://grimler.se/termux-packages-24 stable/main aarch64 tmux aarch64 3.2 [277 kB]
Fetched 466 kB in 1s (245 kB/s)
Selecting previously unselected package libevent.
(Reading database ... 3765 files and directories currently installed.)
Preparing to unpack .../libevent_2.1.12_aarch64.deb ...
Unpacking libevent (2.1.12) ...
Selecting previously unselected package tmux.
Preparing to unpack .../archives/tmux_3.2_aarch64.deb ...
Unpacking tmux (3.2) ...
Setting up libevent (2.1.12) ...
Setting up tmux (3.2) ...
$ apt instsll
E: Invalid operation instsll
$ apt install python2
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
  binutils clang gdbm glib libffi libllvm libsqlite
  libxml2 make ncurses ncurses-ui-libs ndk-sysroot
  pkg-config
The following NEW packages will be installed:
  binutils clang gdbm glib libffi libllvm libsqlite
  libxml2 make ncurses-ui-libs ndk-sysroot pkg-config
  python2
The following packages will be upgraded:
  ncurses
1 upgraded, 13 newly installed, 0 to remove and 38 not upgraded.
Need to get 45.8 MB/50.6 MB of archives.
After this operation, 298 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 https://grimler.se/termux-packages-24 stable/main aarch64 ncurses aarch64 6.2.20200725-4 [494 kB]
Get:2 https://grimler.se/termux-packages-24 stable/main aarch64 libllvm aarch64 12.0.0-1 [19.2 MB]
Get:3 https://grimler.se/termux-packages-24 stable/main aarch64 clang aarch64 12.0.0-1 [19.3 MB]
Get:4 https://grimler.se/termux-packages-24 stable/main aarch64 gdbm aarch64 1.19 [104 kB]
Get:5 https://grimler.se/termux-packages-24 stable/main aarch64 glib aarch64 2.66.1 [1094 kB]
Get:6 https://grimler.se/termux-packages-24 stable/main aarch64 libsqlite aarch64 3.35.5-1 [528 kB]
Get:7 https://grimler.se/termux-packages-24 stable/main aarch64 make aarch64 4.3-1 [219 kB]
Get:8 https://grimler.se/termux-packages-24 stable/main aarch64 ncurses-ui-libs aarch64 6.2.20200725-4 [29.1 kB]
Get:9 https://grimler.se/termux-packages-24 stable/main aarch64 pkg-config aarch64 0.29.2 [25.9 kB]
Get:10 https://grimler.se/termux-packages-24 stable/main aarch64 python2 aarch64 2.7.18-5 [4864 kB]
Fetched 45.8 MB in 17s (2588 kB/s)
(Reading database ... 3822 files and directories currently installed.)
Preparing to unpack .../ncurses_6.2.20200725-4_aarch64.deb ...
Unpacking ncurses (6.2.20200725-4) over (6.2.20200725) ...
Setting up ncurses (6.2.20200725-4) ...
Selecting previously unselected package binutils.
(Reading database ... 3827 files and directories currently installed.)
Preparing to unpack .../00-binutils_2.36.1_aarch64.deb ...
Unpacking binutils (2.36.1) ...
Selecting previously unselected package ndk-sysroot.
Preparing to unpack .../01-ndk-sysroot_21d-1_aarch64.deb ...
Unpacking ndk-sysroot (21d-1) ...
Selecting previously unselected package libffi.
Preparing to unpack .../02-libffi_3.3-2_aarch64.deb ...
Unpacking libffi (3.3-2) ...
Selecting previously unselected package libxml2.
Preparing to unpack .../03-libxml2_2.9.12_aarch64.deb ...
Unpacking libxml2 (2.9.12) ...
Selecting previously unselected package libllvm.
Preparing to unpack .../04-libllvm_12.0.0-1_aarch64.deb ...
Unpacking libllvm (12.0.0-1) ...
Selecting previously unselected package clang.
Preparing to unpack .../05-clang_12.0.0-1_aarch64.deb ...
Unpacking clang (12.0.0-1) ...
Selecting previously unselected package gdbm.
Preparing to unpack .../06-gdbm_1.19_aarch64.deb ...
Unpacking gdbm (1.19) ...
Selecting previously unselected package glib.
Preparing to unpack .../07-glib_2.66.1_aarch64.deb ...
Unpacking glib (2.66.1) ...
Selecting previously unselected package libsqlite.
Preparing to unpack .../08-libsqlite_3.35.5-1_aarch64.deb ...
Unpacking libsqlite (3.35.5-1) ...
Selecting previously unselected package make.
Preparing to unpack .../09-make_4.3-1_aarch64.deb ...
Unpacking make (4.3-1) ...
Selecting previously unselected package ncurses-ui-libs.
Preparing to unpack .../10-ncurses-ui-libs_6.2.20200725-4_aarch64.deb ...
Unpacking ncurses-ui-libs (6.2.20200725-4) ...
Selecting previously unselected package pkg-config.
Preparing to unpack .../11-pkg-config_0.29.2_aarch64.deb ...
Unpacking pkg-config (0.29.2) ...
Selecting previously unselected package python2.
Preparing to unpack .../12-python2_2.7.18-5_aarch64.deb ...
Unpacking python2 (2.7.18-5) ...
Setting up gdbm (1.19) ...
Setting up ndk-sysroot (21d-1) ...
Setting up binutils (2.36.1) ...
Setting up libsqlite (3.35.5-1) ...
Setting up libffi (3.3-2) ...
Setting up ncurses-ui-libs (6.2.20200725-4) ...
Setting up make (4.3-1) ...
Setting up glib (2.66.1) ...
Setting up libxml2 (2.9.12) ...
Setting up python2 (2.7.18-5) ...
Setting up pip2...
DEPRECATION: Python 2.7 will reach the end of its life on January 1st, 2020. Please upgrade your Python as Python 2.7 won't be maintained after that date. A future version of pip will drop support for Python 2.7. More details about Python 2 support in pip, can be found at https://pip.pypa.io/en/latest/development/release-process/#python-2-support
Looking in links: /data/data/com.termux/files/usr/tmp/tmpeA7d6B
Collecting setuptools
Collecting pip
Installing collected packages: setuptools, pip
Successfully installed pip-19.2.3 setuptools-41.2.0
Setting up pkg-config (0.29.2) ...
Setting up libllvm (12.0.0-1) ...
Setting up clang (12.0.0-1) ...
$ install python pkg 2.7
install: target '2.7' is not a directory
$ add apt key
No command add found, did you mean:
Command atd in package at from the unstable-repo repository
Command ldd in package binutils
Command dd in package coreutils
$ add-apt-repository
add-apt-repository: command not found
$
$ $ git clone https://github.com/Tuhinshubhra/CMSeeK
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$ install package editor
install: cannot stat 'package': No such file or directory
$
$ $ apt update && apt upgrade
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$ apt-get update
Ign:1 https://dl.bintray.com/grimler/game-packages-24 games InRelease
Ign:2 https://dl.bintray.com/grimler/science-packages-24 science InRelease
Ign:3 https://dl.bintray.com/grimler/game-packages-24 games Release
Ign:4 https://dl.bintray.com/grimler/science-packages-24 science Release
Get:5 https://grimler.se/termux-packages-24 stable InRelease [16.8 kB]
Ign:6 https://dl.bintray.com/grimler/game-packages-24 games/stable aarch64 Packages
Ign:7 https://dl.bintray.com/grimler/game-packages-24 games/stable all Packages
Ign:8 https://dl.bintray.com/grimler/science-packages-24 science/stable aarch64 Packages
Ign:9 https://dl.bintray.com/grimler/science-packages-24 science/stable all Packages
Ign:6 https://dl.bintray.com/grimler/game-packages-24 games/stable aarch64 Packages
Ign:7 https://dl.bintray.com/grimler/game-packages-24 games/stable all Packages
Ign:8 https://dl.bintray.com/grimler/science-packages-24 science/stable aarch64 Packages
Ign:9 https://dl.bintray.com/grimler/science-packages-24 science/stable all Packages
Ign:6 https://dl.bintray.com/grimler/game-packages-24 games/stable aarch64 Packages
Ign:7 https://dl.bintray.com/grimler/game-packages-24 games/stable all Packages
Ign:8 https://dl.bintray.com/grimler/science-packages-24 science/stable aarch64 Packages
Ign:9 https://dl.bintray.com/grimler/science-packages-24 science/stable all Packages
Ign:6 https://dl.bintray.com/grimler/game-packages-24 games/stable aarch64 Packages
Ign:7 https://dl.bintray.com/grimler/game-packages-24 games/stable all Packages
Ign:8 https://dl.bintray.com/grimler/science-packages-24 science/stable aarch64 Packages
Ign:9 https://dl.bintray.com/grimler/science-packages-24 science/stable all Packages
Err:6 https://dl.bintray.com/grimler/game-packages-24 games/stable aarch64 Packages
  403  Forbidden
Ign:7 https://dl.bintray.com/grimler/game-packages-24 games/stable all Packages
Err:8 https://dl.bintray.com/grimler/science-packages-24 science/stable aarch64 Packages
  403  Forbidden
Ign:9 https://dl.bintray.com/grimler/science-packages-24 science/stable all Packages
Reading package lists... Done
E: The repository 'https://dl.bintray.com/grimler/game-packages-24 games Release' does not have a Release file.
N: Metadata integrity can't be verified, repository is disabled now.
N: Possible cause: repository is under maintenance or down (wrong sources.list URL?).
E: The repository 'https://dl.bintray.com/grimler/science-packages-24 science Release' does not have a Release file.
N: Metadata integrity can't be verified, repository is disabled now.
N: Possible cause: repository is under maintenance or down (wrong sources.list URL?).
$ Installation :
Installation: command not found
$
$ $ apt update && apt upgrade
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ apt install git 
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ apt install python2
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ git clone https://github.com/m4ll0k/Infoga
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ cd Infoga
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ chmod +x *
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ $ pip2 install requests
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ usage : 
No command usage found, did you mean:
Command osage in package graphviz
$
$ $ python2 infoga.py
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$
$ Now it shows all options to use this tool
No command Now found, did you mean:
Command od in package coreutils
Command go in package golang
Command dot in package graphviz
Command iw in package iw from the root-repo repository
Command jo in package jo
Command joe in package joe
Command joe in package jupp
Command toe in package ncurses-utils
Command forw in package nmh from the unstable-repo repository
Command o in package o
Command o in package o-editor
Command moc in package qt5-base from the x11-repo repository
Command co in package rcs
Command sox in package sox
Command stow in package stow
Command top in package termux-tools
Command tor in package tor
Command col in package util-linux
Command wol in package wol
$
$ $ python2 infoga.py -t gmail.com -s all
No command $ found, did you mean:
Command [ in package coreutils
Command k in package kona
Command o in package o
Command o in package o-editor
Command v in package vlang from the unstable-repo repository
$ dot
The program dot is not installed. Install it by executing:
pkg install graphviz
$ install graghiv
install: missing destination file operand after 'graghiv'
Try 'install --help' for more information.
$ install graphiv pkg
install: cannot stat 'graphiv': No such file or directory
$ col
installapt update && apt upgrade

$ apt install git 

$ git clone https://github.com/thelinuxchoice/userrecon

$ cd userrecon

$ chmod +X *

usage :

$ ./userrecon.sh
loks13
click jacking scanner..

this script scans target site is vulnerable for this attack

Installation :

$ apt update && apt upgrade

$ apt install git 

$ apt install python2

$ apt install python

$ git clone https://github.com/D4Vinci/Clickjacking-Tester

$ cd Clickjacking-Tester

$ chmod +x *

Now create here file.txt file, in this file paste victem website and save it

usage : 

$ python3 Clickjacking-Tester.py file.txt

Now it starts scanning if target is vulnerable then it shows you..scan
star scannijb^[[Aapt update && apt upgrade

$ apt install git 

$ apt install python2

$ apt install python

$ git clone https://github.com/medbenali/CyberScan.git

$ cd CyberScan

usage :

$ python2 CyberScan.py -v

$ CyberScan -h
install.cynerscan.py
install cyberscan.py
git clone https://github.com/shawarkhanethicalhacker/D-TECT

$ cd D-TECT

$ chmod +x *

$ pip2 install requests

usage :

$ python2 d-tect.py
,apt update && apt upgrade

$ apt install git 

$ apt install python2

$ apt install python

$ pip2 install requests

$ git clone https://github.com/Gameye98/santet-online

$ santet-online

$ chmod +x *

usage :

$ python2 santet.py

apt-get update -y

$ apt-get upgrade -y

$ pkg install python -y

$ pkg install python2 -y

$ pkg install git -y

$ pip install lolcat

$ git clone https://github.com/noob-hackers/mrphish

$ cd $HOME

$ ls

$ cd mrphish

$ ls

$ bash setup

$ bash mrphish
start
^[end] 
