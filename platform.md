---
layout: default
title: Development Platform
---

# Development platform

The [Atom](http://atom.io) editor is available for Windows, Linux, and Mac's.  By itself it has good support for programming.   The plugin/extension [PlatformIO](http://platformIO.org) adds specific support for embedded systems.  These make a good pairing, are freely available (Open-source), and I've successfully build code for the current ARM boards (as long as you avoid the Embedded artists library `EALib`), and Arduino Uno.  Using both C and assembly language.

# Github
I plan to use Github for disseminating material (code examples) to the students.  Getting them used to using version control as a matter of routine.  The  Github classrooms provide a very convenient way of handling submission of software projects.

# Installing on Ubuntu

{% highlight bash %}
#!/bin/sh
# install atom with platformio and dependencies
# Alun  5/05/2017


# platform IO needs clang, it has quite a few dependencies
# so the  --yes just installs the lot
sudo  apt-get install --yes git git-man liberror-perl clang

# atom isn't in the debian archives yet
# download the deb file and install it
wget -c https://atom-installer.github.com/v1.16.0/atom-amd64.deb
sudo  dpkg -i atom-amd64.deb
{% endhighlight %}

# Installing on Windows
To install on Windows, you will need
 * the LLVM compliler system (for clang) from [http://releases.llvm.org/download.html](http://releases.llvm.org/download.html) ([64bit installer](http://releases.llvm.org/4.0.0/LLVM-4.0.0-win64.exe))
 * the Atom [installer](https://atom.io/download/windows_x64)
Once you have thses installed, fire up Atom.
From the preferences (Ctrl-comma) you can install the platformIO packages.
