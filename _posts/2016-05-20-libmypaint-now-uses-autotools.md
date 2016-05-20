---
layout: post
title: "libMyPaint now uses autotools"
author: Andrew Chadwick
date: 2016-05-20 02:45:00
categories: blog
---

MyPaint's brush engine, [libmypaint](https://github.com/mypaint/libmypaint), now needs to be built with [autotools](https://en.wikipedia.org/wiki/GNU_Build_System). This reduces its dependencies on things like Python, which is good for projects like GIMP which build against libmypaint. If you used to build MyPaint from git with special _scons_ flags just to make libmypaint as a dependency for some other project, you don't need to do that any more!

This is pretty much the final stage of making libmypaint a fully independent module. To reflect its new status, we will be making formal releases of libmypaint shortly for other projects to build with.

#### Build/install

See the updated build documentation in [libmypaint's README](https://github.com/mypaint/libmypaint/blob/master/README.md). It's all fairly standard stuff:

    $ ./autogen.sh     # only needed when building from git
    $ ./configure --prefix=/some/where
    $ make distcheck

You can install it in the usual way too. However we will be making [Debian-style packages](https://github.com/mypaint/libmypaint.deb) available via the PPA shortly, including developer ones. There is already a [git PKGBUILD](https://github.com/Alexpux/MINGW-packages/tree/master/mingw-w64-libmypaint-git) for [Windows MSYS2](https://msys2.github.io/), and updates will be available shortly for Arch Linux.

*****

Development of MyPaint will continue of course; in fact making this split happen has improved a lot of things in the codebases of both projects ☺  Big thanks to [@Jehan](https://github.com/Jehan) for making this all work so well!
