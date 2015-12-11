---
layout: page
title: Downloads
permalink: /downloads/
---

The Latest build release of MyPaint is version `1.2.0-beta.3` which was 
released on Nov. 21, 2015. The latest stable build is version `1.1` 
which was released on Jan. 4, 2013. 

We no longer provide support for version `1.0`. For Version `1.1` , we 
may ask you to try one of the more recent builds if you ask for support 
on our issue tracker.

### Linux

The latest stable version of MyPaint is available via 
`apt-get install mypaint` in the terminal on Debian and Ubuntu based 
distributions. 

We do maintain a [Ubuntu PPA][linux.ppa] which is a rolling build of 
MyPaint's "Master" branch on Github. We try to keep things on the master 
branch fairly stable and tested, but there are bound to be bugs.

All other major Linux Distributions will most likely include the most 
recent stable MyPaint package. To get the latest version of MyPaint, 
[it will have to be build from the source][linux.build]. We do not 
maintain packages for other distributions besides Ubuntu and Debian.

### Mac OSX

The latest stable and development builds of MyPaint are available via 
[MacPorts][mac.ports]. 

You can also build MyPaint on Mac OSX with MacPorts as well. Please go 
to our [README_OSX.md][mac.build] in our Github repository for more 
information.

### Windows

Our latest build of MyPaint is available via our 
[Github Releases Page][gh.releases] for both Win32 and Win64. The 
latest build version is `v1.2.0-beta.3`.

Long-time MyPaint porter TumaGonix 
[has builds available for windows as well][windows.tumagonx]. The 
latest build version on TumaGonix's blog is `mypaint-1.2.0.7z` which 
was released on Sep. 19, 2015. We recommend you look at these builds 
first if you are looking for a stable build of MyPaint on Windows.

You can also build MyPaint from source as well. We use 
[MSYS2][windows.msys2] as our build environment to build a windows 
version. For more information please go to our 
[README_WINDOWS.md][windows.build] for information on how to build on 
windows.

### Source

MyPaint is actively developed and hosted on [Github][source.github] 
and is always actively tested by [Travis-CI][source.travis] every time a 
commit is made. If you want the absolute very latest development 
version, or are interested in helping MyPaint evolve, please follow the 
instructions in the [README.md][source.build] file to get started.

We are looking for builders who will be willing to maintain a builds 
for Mac OSX and Windows. If you wish to help us port MyPaint to your OS 
or Linux Distribution. Please visit our Discourse forums under the 
[Porting MyPaint Category][source.porting]. You can also ask questions 
there if you are having a trouble building MyPaint.

### Brush Packages

We host a list of brushpacks available download on 
[MyPaint's Brush Packages Wiki][brush.wiki]. You are welcome to post 
you own brushpacks on that Wiki provided your brushpacks abides by our 
[Licensing Policy][brush.policy].


[gh.releases]: https://github.com/mypaint/mypaint/releases

[linux.ppa]: https://launchpad.net/~achadwick/+archive/ubuntu/mypaint-testing
[linux.build]: https://github.com/mypaint/mypaint/blob/master/README_LINUX.md

[mac.ports]: https://www.macports.org/ports.php?by=name&substr=mypaint
[mac.build]: https://github.com/mypaint/mypaint/blob/master/README_OSX.md

[windows.tumagonx]: http://www.opensourcepack.blogspot.fr/2013/01/mypaint-and-pygi.html
[windows.msys2]: https://github.com/msys2
[windows.build]: https://github.com/mypaint/mypaint/blob/master/README_WINDOWS.md

[source.github]: https://github.com/mypaint
[source.travis]: https://travis-ci.org/mypaint
[source.build]: https://github.com/mypaint/mypaint/blob/master/README.md
[source.porting]: http://community.mypaint.org/c/development/porting

[brush.wiki]: https://github.com/mypaint/mypaint/wiki/Brush-Packages
[brush.policy]: https://github.com/mypaint/mypaint/wiki/Licensing-policy
