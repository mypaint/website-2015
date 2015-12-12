---
layout: page
title: Downloads
permalink: /downloads/
---

You can download our latest builds from
our [GitHub releases page][downloads.releases].
The releases page also contains an archive of all historical releases.

We only make official builds for a limited number of platforms
due to time and resource constraints.
Many third parties release builds for other systems.

The latest stable release is version 1.1
which was released on Jan. 4, 2013.

The next stable release will be version 1.2.0,
and betas are available for testing right now.

We no longer provide support for version 1.0 or earlier versions.
If you are using 1.1,
we may ask you to try one of the more recent builds
if you ask for support on our issue tracker.

### Linux

The latest stable version of MyPaint is available on most distributions
as third-party builds.
Use your normal package manager to install the program.
We will try to support these builds if they are recent.

We maintain an [Ubuntu PPA][linux.ppa] which is a rolling build of 
the “master” branch on GitHub.
We try to keep things on the master branch fairly stable and tested,
but there are bound to be bugs.

### Mac OS X

The latest stable and development builds of MyPaint are available via 
[MacPorts][mac.ports].
Please contact us in the issue tracker if you want to do something
for other distribution channels.

### Windows

An official build of MyPaint is available on our 
[GitHub releases page][gh.releases] for both Win32 and Win64.

In addition, long-time MyPaint porter TumaGonx 
has [builds available for Windows][windows.tumagonx].
These may be better tested than the official builds,
and sometimes do not suffer from the same issues.

We do not support any other Windows builds or installers.
Please do not install MyPaint using downloads
from any other site on the Windows platform.
Please contact us in the issue tracker
if you want to do something for Chocolatey or PortableApps.

### Source

MyPaint is actively developed and hosted on [GitHub][source.github] 
and the build is automatically tested on [Travis-CI][source.travis]
every time a commit is made.

If you want the absolute very latest development version,
or are interested in helping MyPaint evolve,
see the [README.md][source.build] file in the source to get started.

We are looking for more people willing to maintain builds
for Mac OS X, Windows, or Linux distributions.
If you want to help us port MyPaint to your OS or Linux Distribution,
please visit our community forums under the 
[Porting MyPaint Category][source.porting], and ask away there.
You can also ask questions there if you are having trouble building MyPaint.

### Brush Packages

We host a list of brushpacks available for download via 
[MyPaint's Brush Packages wiki page][brush.wiki].
You are welcome to post links to your own brushpacks on our Wiki.
Files are typically not hosted on the wiki, just linked,
so you can use any license you want.
However the preview thumbnails should be public domain.
If you release brushpacks which meet our [Licensing Policy][brush.policy],
they could be considered for inclusion in the next release.

[downloads.releases]: https://github.com/mypaint/mypaint/releases

[linux.ppa]: https://launchpad.net/~achadwick/+archive/ubuntu/mypaint-testing
[linux.build]: https://github.com/mypaint/mypaint/blob/master/README_LINUX.md

[mac.ports]: https://www.macports.org/ports.php?by=name&substr=mypaint

[windows.tumagonx]: http://www.opensourcepack.blogspot.fr/2013/01/mypaint-and-pygi.html

[source.github]: https://github.com/mypaint
[source.travis]: https://travis-ci.org/mypaint
[source.build]: https://github.com/mypaint/mypaint/blob/master/README.md
[source.porting]: http://community.mypaint.org/c/development/porting

[brush.wiki]: https://github.com/mypaint/mypaint/wiki/Brush-Packages
[brush.policy]: https://github.com/mypaint/mypaint/wiki/Licensing-policy
