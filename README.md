# Installation for Ubuntu

## install dependencies
```sh
 sudo apt update
 sudo apt install autoconf automake libtool m4 gcc build-essential
```
## config build and installation
```sh
 touch AUTHORS ChangeLog NEWS README & aclocal & autoconf & automake --add-missing
 ./configure
 make
 make install
```
