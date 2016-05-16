# Installation

## clone patches repository including the dwm repository

    git clone https://github.com/jceb/slock-patches

## init and load dwm submodule

    cd slock-patches
    git submodule update --init --recursive

## activate all patches, including the personal configuration

    quilt push -a

## build slock (or us the ./build script)

    cd slock
    rm -f config.h
    make

## install st locally (or use ./install script)

    make DESTDIR=~/.local PREFIX= install

# Patch References

* [pam_auth.patch](patches/pam_auth.patch)                           (no URL yet)
