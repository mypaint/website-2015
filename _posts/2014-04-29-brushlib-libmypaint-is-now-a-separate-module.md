---
layout: post
title:  "Brushlib is Now a Separate Module"
author: Andrew Chadwick
date:   2014-04-29 00:00:00
categories: blog
---

The MyPaint brushlib(libmypaint) is now maintained in a separate git repository. Its
new home is also on Gitorious, at
<https://gitorious.org/mypaint/libmypaint/>, so it hasn’t moved far!
We’ve done this because there are more projects using this code, or
wanting to use it, than just MyPaint. The MyPaint project now includes
brushlib as a git [submodule](http://www.git-scm.com/book/en/Git-Tools-Submodules).

The practical upshot of this for users is that you may see some
unexpected errors if you’ve been tracking MyPaint development through
git for a long time. If you’ve just updated your clone using “git pull”,
and your build is failing due to a missing file:

    $ scons
    [...]
    In file included from lib/mypaintlib.hpp:13:0,
     from lib/mypaintlib_wrap.cpp:3071:
    lib/mapping.hpp:20:21: fatal error: mapping.h: No such file or directory
     #include "mapping.h"
     ^
    compilation terminated.
    scons: *** [lib/mypaintlib_wrap.os] Error 1
    scons: building terminated because of errors.
    $

then you may need to remove a local copy of brushlib that git has
somewhat unhelpfully left lying around. You will also need to tell git
to pull in the submodules MyPaint needs for building:

    $ rm -fr brushlib
    $ git submodule update --init
    Submodule path 'brushlib': checked out 'f9fd9[...]'
    $ scons

After fetching the missing dependencies, the build procedure should work
as it did before.

If you switch between branches a lot, you may find yourself having to do
this quite a lot: not every branch of MyPaint out there know about the
submodule yet. Sorry about that; please excuse the dust.

The basics of this are recapped in the updated [README](https://gitorious.org/mypaint/mypaint/source/f8d48ad9b91866eab1fa5fe6946f0ae2354534fe:README) file, and more
information on working with git and submodules is available online or in
print in the Pro Git book, chapter [6.6 Git Tools –
Submodules](http://www.git-scm.com/book/en/Git-Tools-Submodules).

