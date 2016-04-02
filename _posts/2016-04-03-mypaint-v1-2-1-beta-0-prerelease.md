---
layout: post
title: "MyPaint 1.2.1-beta.0 prerelease"
author: Andrew Chadwick
date: 2016-04-03 00:06:00
categories: blog
comments: off
---

We have a new prerelease out for you to test:
MyPaint version **1.2.1-beta.0**.

When 1.2.1 is ready, it will be a minor bugfix release.
We're hoping to keep its beta cycle short,
so please test and feed back.

Binaries are available right now for Ubuntu and Windows systems,
and this prerelease is available in official source tarball form too.
MyPaint v1.2.1-beta.0 can be downloaded from its
[release page on github](https://github.com/mypaint/mypaint/releases/tag/v1.2.1-beta.0)
or from the
[MyPaint-testing PPA](https://launchpad.net/~achadwick/+archive/ubuntu/mypaint-testing).

-------------------

## MyPaint v1.2.1-beta.0 (2016-04-02)

_“We Thought It Was Just Another Snake Cult”_

When it's ready, MyPaint version 1.2.1 will be a minor bugfix release.
This means that it fixes bugs present in v1.2.0 without adding new
features.

### Changes since 1.2.0

* Fix failure to start under GLib 2.48.
* Fix failure to start when config and user data dirs are missing.
* GNOME: Update mypaint.appdata.xml.
* Fix failure to start when no translations are present.
* Fix pure-black being duplicated in the colour history.
* Fix glitch stroke when Inking is exited & the default tool entered.
* OSX: fix exception if AppKit isn't installed.
* Fix mispositioned windows in multi-monitor setups.
* Windows: fix inability to paste more than the 1st copied image.
* Fix exception when pasting into a layer group.
* Fix incorrect numeric range check on x-axis tilts.
* Fix layers blinking when selected in layer-solo mode.
