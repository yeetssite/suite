# scripts  
My bash and other assorted scripts

# use  
This repo is actually a github pages site at [https://yeetssite.github.io/suite/](https://yeetssite.github.io/suite/)(formely [https://yeetssite.github.io/scripts](https://yeetssite.github.io/scripts)), but it has no content as it's specifically made to host files only.

It's meant to be used with bash, but can contain other script types, too.

# Available programs and scripts:

### Termux Bash scripts:  

*Available from `Termux/`*

> [Termux](https://termux.dev) is a non-[FHS compliant](https://en.m.wikipedia.org/wiki/Filesystem_Hierarchy_Standard) unix-like system-within-a-system/terminal emulator/linux environment for Android that isn't compatible with normal bash scripts (cuz of the FHS thingy), and thus needs its own special scripts.


`yeetsmemes v1.4-alpha` - downloads memes from [yeet's memes](https://github.com/yeetssite/memes# "GitHub source code for Yeet's memes")
`qls v1.2-alpha` - Quickly lists home/ and bin/ directories
`yeetsinstaller v1.3-alpha` - installs these bash scripts

### BASIC programs:

*Available from `1.BASIC/`*

> NOTE: These BASIC scripts use the [TinyBASIC](https://github.com/cyningstan/tinybasic) interpeter. See [1.BASIC/README.md](./1.BASIC/README.md).

`myFirstBASICcode.bas` - To be honest, idek(it has swearing(NOT FOR SENSITIVE CRYBABY MFS))

### C Scripts/compilable source code:

*Available from `2.C-Scripts/`*

`helloearl.c` - (Has swears) My first C program (I didnt wanna make some dumb hello world)

### Python 3 scripts

*Available from `3.Python/`*

> IMPORTANT: see [`3.Python/README.md`](./3.Python/README.md)

`yourmom.py` - (Guess what? Has swears? CORRECT!) - Once again, idek

# Installing

### You can install my scripts using these methods:

#### The installer ~~(The recommended way)~~~~(broken)~~(super broken)

> Somehow, I broke all the non-termux scripts, and the installer. please use the [git](https://github.com/yeetssite/scripts#clone-via-git) method to install instead, and please remember that normal bash scripts aren't available.

The installer is the recommended way to get my scripts because you don't have to specify the path to scripts you want to run if you use this method.  
To use the installer, enter or copypasta these commands: 

```console
~$ curl -O https://yeetssite.github.io/scripts/yeetsinstaller
~$ chmod u+r+x ./yeetsinstaller 
~$ # ^^^Downloads the installer and marks it executable
~$ ./yeetsinstaller 
~$ # ^^^runs the installer
 ```   

The installer will download scripts to your `BIN/` directory so they can be executed as normal commands.

You can also use `wget` to download the installer:

```console
~$ wget https://yeetssite.github.io/suite/yeetsinstaller && chmod u+r+x ./yeetsinstaller
~$ ./yeetsinstaller
```

#### Clone Via Git:

Check if git is installed:

```console
~$ git version
```

If git is installed, it should say something like "`git version 2.45.1`".


If git isn't installed, it will give you an error like "`command not found: git`". You'll have to [install git](https://github.com/git-guides/install-git#install-git-using-github-desktop) if this happens.

##### Clone the repo:

```console
~$ git clone https://github.com/yeetssite/suite.git
```

But using this method to install will require you to specify the path to your scripts every time you want to run them, e.g.:

```console
~$ ./suite/yeetsmemes
```

Using the installer will download scripts to your BIN and mark them executable, letting them be run like this:

```console
~$ yeetsmemes
```

*...however*, since the installer is broken, simply run these commands:

```console
~$ chmod u+r+x ./suite/Termux/*
~$ cp ./suite/Termux/* $PREFIX/bin/
```

Adding scripts to `bin/` will allow them to be run as if the installer installed them(because you basically just did the installer's job manually).
