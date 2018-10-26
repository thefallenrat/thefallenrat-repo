# thefallenrat-repo

This repository contains set of AUR packages that I used daily. Some of which are `aurutils`, `f3-qt`, `neofetch`, `steamguard-cli` and many more.
**x86_64 only**

GPG key : 
```
2F098DADBC8550A774A055773017FBAA4ECA6CEC
```

GPG key block : 

http://pgp.mit.edu/pks/lookup?op=get&search=0x3017FBAA4ECA6CEC


Build Flags :
```
CPPFLAGS="-D_FORTIFY_SOURCE=2"
CFLAGS="-march=x86-64 -mtune=generic -O2 -pipe -fstack-protector-strong -fno-plt"
CXXFLAGS="-march=x86-64 -mtune=generic -O2 -pipe -fstack-protector-strong -fno-plt"
LDFLAGS="-Wl,-O1,--sort-common,--as-needed,-z,relro,-z,now"
```

Script used : 

https://github.com/thefallenrat/thefallenrat-repo/blob/master/thefallenrat


## Installation

* Edit `/etc/pacman.conf` and add these in the end of the file :
```
[thefallenrat-repo]
Server = https://raw.github.com/thefallenrat/$repo/master/
```
* Refresh pacman database (`-Syy`) and install `artix-keyring` package
* Done!
