---
layout: default
title: Development Platform
---

# Development platform

The [Atom](http://atom.io) editor is available for Windows, Linux, and Mac's.  By itself it has good support for programming.   The plugin/extension [PlatformIO](http://platformIO.org) adds specific support for embedded systems.  These make a good pairing, are freely available (Open-source), and I've successfully build code for the LPC4088 ARM boards (as long as you avoid the Embedded artists library `EALib`), and Arduino Uno.  Using both C and assembly language.

# Github
I plan to use Github for disseminating material (code examples) to the students.  Getting them used to using version control as a matter of routine.  The  Github classrooms provide a very convenient way of handling submission of software projects.

There are several alternatives for accessing, cloning, and updating git repositories.

# Atom
You will need an up-to-date version of Atom.  The Linux version does not automatically track the up-to-date version on the website, so you may have to install the latest version manually.

## Installing on Ubuntu
Atom isn't in the debian archives yet, so you will need to manually download and install Atom.

Download the deb file and install it
{% highlight bash %}
wget -c https://atom-installer.github.com/v1.16.0/atom-amd64.deb
sudo  dpkg -i atom-amd64.deb
{% endhighlight %}{: .example}

## Installing on Windows
To install on Windows, you will need
 the Atom [installer](https://atom.io/download/windows_x64)

# LLVM and Clang
PlatformIO uses Clang and LLVM for code highlighting and syntax checking.
## Installing on Ubuntu

Clang has quite a few dependencies so the  `--yes` option
just installs the lot
{% highlight bash %}
sudo  apt-get install --yes git git-man liberror-perl clang
{% endhighlight %}{: .example}

## Installing on Windows
To install on Windows, you will need  the LLVM compliler system (for clang) from [http://releases.llvm.org/download.html](http://releases.llvm.org/download.html) ([64bit installer](http://releases.llvm.org/4.0.0/LLVM-4.0.0-win64.exe))


# PlatformIO
Once you have Atom and LLVM/Clang installed you can install PlatformIO.
Start up Atom and from the preferences (Ctrl-comma/⌘-comma) you can install the platformIO packages.   The first time atom starts it does go through an installation process of its own, be patient.
