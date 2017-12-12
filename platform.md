---
layout: default
title: Software Platform
---
* toc
{:toc}

# Software platform
The [Atom](http://atom.io) editor is available for Windows, Linux, and Mac's.  By itself it has good support for programming.   The plugin/extension [PlatformIO](http://platformIO.org) adds specific support for embedded systems.  These make a good pairing, are freely available (Open-source), and I've successfully build code for the LPC4088 ARM boards (as long as you avoid the Embedded artists library `EALib`), and Arduino Uno.  Using both C and assembly language.

## Computing Lab machines
The Linux (Ububtu)  Machines in the Department's Off-Campus labs are the ones we will be using.  They do need some installation/updates of software.   If they aren't set up right the instructions are below.

### Checking version numbers
I have a copy of [Ubuntu's Desktop](https://www.ubuntu.com/download/desktop) (which is what we have in the labs) that I use to make sure material works on the lab machines.   My setup is:

    alun@Ubuntu:~$ git --version
    git version 2.7.4

    alun@Ubuntu:~$ atom --version
    Atom    : 1.22.1
    Electron: 1.6.15
    Chrome  : 56.0.2924.87
    Node    : 7.4.0

    alun@Ubuntu:~$ clang --version
    clang version 3.8.0-2ubuntu4 (tags/RELEASE_380/final)
    Target: x86_64-pc-linux-gnu
    Thread model: posix
    InstalledDir: /usr/bin

    alun@Ubuntu:~$ apm list | grep platformio
    ├── platformio-ide@2.0.0-rc.4
    ├── platformio-ide-debugger@1.2.4
    ├── platformio-ide-terminal@2.7.0

    alun@Ubuntu:~$ hg --version
    Mercurial Distributed SCM (version 3.7.3)
    (see https://mercurial-scm.org for more information)

    Copyright (C) 2005-2016 Matt Mackall and others
    This is free software; see the source for copying conditions. There is NO
    warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

    alun@Ubuntu:~$
{: .example}
_as of 12/12/2017_

---

# Github
I plan to use Github for disseminating material (code examples) to the students.  Getting them used to using version control as a matter of routine.  The  Github classrooms provide a very convenient way of handling submission of software projects.

There are several alternatives for accessing, cloning, and updating git repositories.

## GitHub Account
We will be using [git](https://git-scm.com/) as our version control system.  Example code, exercises, and assignment will use [GitHub](https://github.com/)
as the master store for the repositories.

> A GitHub account will be __*essential*__ for submitting the code for your assignment.

## Github Education
Once you have your Github account, it is well worth signing up for a [Student Developer Pack](https://education.github.com/pack).  There are plenty of useful resources, and you get more private repositories for your account.

## On Ubuntu
To install on ubuntu

    sudo apt install git
{: .example}

---

# Atom
You will need an up-to-date version of Atom.  The Linux version does not automatically track the up-to-date version on the website, so you may have to install the latest version manually.

## Installing on Ubuntu
Atom isn't in the debian archives yet, so you will need to manually download and install Atom.

Download the deb file and install it.  To get the link go to the [releases page](https://github.com/atom/atom/releases/latest) and copy the link address for the `.deb` file.

    wget  https://github.com/atom/atom/releases/download/v1.22.1/atom-amd64.deb
    sudo  dpkg -i atom-amd64.deb
{: .example}

## Installing on Windows
To install on Windows, you will need
 the Atom [installer](https://atom.io/download/windows_x64)

---

# LLVM and Clang
PlatformIO uses Clang and LLVM for code highlighting and syntax checking.

## Installing on Ubuntu
Clang has quite a few dependencies so the  `--yes` option
just installs the lot

    sudo  apt install --yes  clang
{: .example}

## Installing on Windows
To install on Windows, you will need  the LLVM compliler system (for clang) from [http://releases.llvm.org/download.html](http://releases.llvm.org/download.html) ([64bit installer](http://releases.llvm.org/4.0.0/LLVM-4.0.0-win64.exe))

---

# PlatformIO
Once you have Atom and LLVM/Clang installed you can install PlatformIO.

Start up Atom and from the preferences (Ctrl-comma/⌘-comma) you can install the platformIO packages.   The first time atom starts it does go through an installation process of its own, be patient.

## Command line
Atom has a command line package manager `apm` you can install the PlatformIO package with

    apm install platformio-ide
{: .example}
Note on Unixes you don't need to use `sudo`

---

# Mercurial
The [MBED libraries](https://os.mbed.com/code) use [Mercuial](https://www.mercurial-scm.org/) as their version control system.  If you have mercurial installed, PlatformIO can automatically download libraries from the MBED site.

## Installing on Ubuntu
For Ubuntu

    sudo  apt install mercurial
{: .example}

## Other OSes
The Mercurial website has downloads for other Operating Systems.
