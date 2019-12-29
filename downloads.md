---
layout: page
title: Downloads
permalink: /downloads/
---

You can download our latest builds from
our [GitHub releases page][downloads.releases].
The releases page also contains an archive of all historical releases.

The MyPaint team only makes builds for a limited number of platforms
due to time and resource constraints.
Many third parties release builds for other systems.

The latest stable release is version 1.2
which was released on Jan. 15, 2016.

We no longer provide support for version 1.1 or earlier versions.
If you are using those versions,
we will ask you to try one of the more recent builds
if you ask for support on our issue tracker.

### Linux

The latest stable version of MyPaint is available on most distributions
as third-party builds.
Use your normal package manager to install the program.
We will try to support these builds if they are recent.

#### Appimages

We have two versions of our Appimages.

[Rolling Release][downloads.rolling]: This where we store our Rolling
Releases which build directly from Master. Beware may be unstable.

[Standard Release][downloads.releases]: This where you can get any stable
and Alpha/Beta Builds we tag and release. The Alpha/Beta may be unstable, 
but for the most part will work compared to our Rolling Releases.


#### Flatpak:

MyPaint is now also availble as Flatpak and should be installable on
all major Linux distributions that support it like Fedora, Debian,
Ubuntu, elementaryOS, Arch, openSuSE, and many more.

-->[Click to install Flatpak][linux.flatpak]<--

Click to install is not yet availble in all distributions.  If you are
lucky it will open your Software application.  Otherwise you can use
the command line:

```
flatpak install --from https://raw.githubusercontent.com/mypaint/mypaint/master/flatpak/mypaint-stable.flatpakref
```

After installing the Flatpak, the applications should show up in your
system, but because Flatpak is very new, you may need to log out and
log in again to see the launcher in your desktop.  You can also launch
it from the commandline:

```
flatpak run org.mypaint.MyPaint
```

### Mac OS X

The latest stable and development builds of MyPaint are available via
[MacPorts][mac.ports].
Please contact us in the issue tracker if you want to do something
for other distribution channels.

### Windows

We have stable builds and prerelease builds available on our
[GitHub releases page][downloads.releases] for both Win32 and Win64.

#### Rolling Release

We also have continuous builds available which are updated 
everytime a new change is made in our [Github Repository][source.github].

->[Latest Windows Alpha Builds from Appveyor.][downloads.alpha]<-

*Just select whether build(i686/MINGW32=32bit build or x86_64/MINGW64=64bit build) 
you are using and navigate to the Artifacts tab to download the exe file. 
Be aware, the “latest build” can likely be a very very beta “Pull Request” 
with some random feature. Make sure it doesn’t say “Pull Request”. If it 
does, click on “build history” and select one that does NOT say “Pull 
Request” on it.*

#### Chocolatey

If you prefer to use the Chocolatey repository, both
[stable releases][choco.prerel] and [pre-releases][choco.stable]
can be found there. This is maintained by a third party so be warned.

__Apart from the two mentioned above, we do not officially support any 
other Windows builds or installers.__

### Source

MyPaint is actively developed and hosted on [GitHub][source.github]
and the build is automatically tested on [Travis-CI][source.travis] for 
Linux and [AppVeyor][downloads.alpha] for Windows every time a commit 
is made on Repsitory.

If you want the absolute very latest development version, or are interested 
in helping MyPaint evolve,see the [README.md][source.build] file in the 
source to get started.

We are always open for more people willing to maintain buildsfor Mac 
OS X, Windows, or Linux distributions.If you want to help us port 
MyPaint to your OS or Linux Distribution,please visit our community 
forums under the [Porting MyPaint Category][source.porting], and ask away 
there.You can also ask questions there if you are having trouble 
building MyPaint.

### Brush Packages

We host a list of brushpacks available for download via
[MyPaint's Brush Packages wiki page][brush.wiki].
You are welcome to post links to your own brushpacks on our Wiki.
Files are typically not hosted on the wiki, just linked,
so you can use any license you want.
However the preview thumbnails should be public domain.
If you release brushpacks which meet our [Licensing Policy][brush.policy],
they could be considered for inclusion in the next release.

[downloads.rolling]: https://github.com/mypaint/mypaint-appimage/releases
[downloads.releases]: https://github.com/mypaint/mypaint/releases
[downloads.alpha]: https://ci.appveyor.com/project/achadwick/mypaint

[choco.prerel]: https://chocolatey.org/packages/mypaint/
[choco.stable]: https://chocolatey.org/packages/mypaint/1.2.1

[linux.flatpak]: https://flathub.org/repo/appstream/org.mypaint.MyPaint.flatpakref
[linux.build]: https://github.com/mypaint/mypaint/blob/master/README_LINUX.md

[mac.ports]: https://www.macports.org/ports.php?by=name&substr=MyPaint

[windows.tumagonx]: http://www.opensourcepack.blogspot.fr/2013/01/mypaint-and-pygi.html

[source.github]: https://github.com/mypaint
[source.travis]: https://travis-ci.org/mypaint
[source.build]: https://github.com/mypaint/mypaint/blob/master/README.md
[source.porting]: http://community.mypaint.org/c/development/porting

[brush.wiki]: https://github.com/mypaint/mypaint/wiki/Brush-Packages
[brush.policy]: https://github.com/mypaint/mypaint/wiki/Licensing-policy
