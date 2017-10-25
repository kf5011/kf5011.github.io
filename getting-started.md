---
layout: default
---
# Getting started
This is a quick guide to getting started using [Git](https://github.com), [Atom](https://atom.io), and [PlatformIO](https://platformio.org), in the context of this module.

# Workflow
The basic pattern for the lab classes, and ultimately the assignment, is:

 1. [Fork](#forking-a-repository) the repository on Github.
 2. [Clone](#cloning-the-repository) the repository on the local machine.
 3. Work on the project
    1. Edit
    2. Compile
    3. Upload
    4. Evaluate
 4. Commit changes
 5. Push updates back to Github server.

# Github repository
The exercises for the practical sessions and the base skeleton for the assignment will be distributed via Github.  Github is a very good tool for managing and distributing source code.

## Lab material
Lab material will be distributed via public repositories, linked to from the module pages.  While you can download a .zip file containing the source, or clone the public repository, a better option is to fork the repository (which requires a Github account).

![Github page](images/github-page.png){: style="width:45em" }

# Forking a repository
Look for the fork button ![fork button](images/fork-button.png){: style="height:18px"} near the top right of the page.  _You will need to be signed into your gitub account_

Creating a fork, makes a copy of the repository under your id, you can then make changes to your copy, and log them back onto github servers.

 > Since the original repositories are public, your initial repository
 > will also be public.
 >
 > To make a private copy see the Github help page on
 > [Duplicating a repository](https://help.github.com/articles/duplicating-a-repository/)

# Cloning the repository
Making a clone of the repository, makes a local copy of the files that you can work on.  Although there are some good GUI based tools, personally I've found that the command shell tool the most convenient for this stage.

To clone the repository click on the green

![git clone](images/clone-repro.png){: style="width:70%"}

   ````shell_session
    $ git clone https://github.com/control-systems-computer-networks/simple-serial
   ```
