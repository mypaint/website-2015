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

#### Ubuntu PPA:

We maintain an [Ubuntu PPA][linux.ppa] which is a rolling build of
the “master” branch on GitHub.
We try to keep things on the master branch fairly stable and tested,
but there are bound to be bugs.

#### Appimage

We have appimages available in our [Github Release][downloads.releases]
page which are images of the alpha builds of mypaint. We hope to 
have stable versions out soon

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

#### Flatpak Nightly:

There is also a Flatpak package which is a rolling build of the
“master” branch on GitHub.  You can install it from the command line:

```
flatpak remote-add --no-gpg-verify --user mypaint-master-repo http://flatpak-repo.manuq.com.ar
flatpak --user install mypaint-master-repo org.mypaint.MyPaint-Nightly
```

And then run from your desktop or with this command:

```
flatpak run org.mypaint.MyPaint-Nightly
```

Note this process is not automated yet.  The package is updated
manually. Your Software application should notify you on any
update. Otherwise you can update with this command:

```
flatpak --user update org.mypaint.MyPaint-Nightly
```

### Mac OS X

The latest stable and development builds of MyPaint are available via
[MacPorts][mac.ports].
Please contact us in the issue tracker if you want to do something
for other distribution channels.

### Windows

We have stable builds and prerelease builds available on our
[GitHub releases page][downloads.releases] for both Win32 and Win64.

We also have continuous alpha builds available which are updated 
everytime a new change is made in our [Github Repository][source.github].

->[Grab the latest Windows Alpha Builds from Appveyor here.][downloads.alpha]<-

Just select whether build(i686/MINGW32=32bit build or x86_64/MINGW64=64bit build) 
you are using and navigate to the Artifacts tab to download the exe file.

Be aware, the “latest build” is likely to be a very very beta “Pull Request” 
with some random feature. Make sure it doesn’t say “Pull Request”, or 
click “build history” and select one that does NOT say “pull request” on it.

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

[downloads.releases]: https://github.com/mypaint/mypaint-appimage/releases
[downloads.alpha]: https://ci.appveyor.com/project/achadwick/mypaint

[linux.ppa]: https://launchpad.net/~achadwick/+archive/ubuntu/mypaint-testing
[linux.flatpak]: https://raw.githubusercontent.com/mypaint/mypaint/master/flatpak/mypaint-stable.flatpakref
[linux.build]: https://github.com/mypaint/mypaint/blob/master/README_LINUX.md

[mac.ports]: https://www.macports.org/ports.php?by=name&substr=MyPaint

[windows.tumagonx]: http://www.opensourcepack.blogspot.fr/2013/01/mypaint-and-pygi.html

[source.github]: https://github.com/mypaint
[source.travis]: https://travis-ci.org/mypaint
[source.build]: https://github.com/mypaint/mypaint/blob/master/README.md
[source.porting]: http://community.mypaint.org/c/development/porting

[brush.wiki]: https://github.com/mypaint/mypaint/wiki/Brush-Packages
[brush.policy]: https://github.com/mypaint/mypaint/wiki/Licensing-policy
