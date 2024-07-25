# Installation for Ubuntu

# install dependencies
$: sudo apt update
$: sudo apt install autoconf automake libtool m4 gcc build-essential

# config build and installation

$: touch AUTHORS ChangeLog NEWS README & aclocal & autoconf & automake --add-missing
$: ./configure
$: make
$: make install