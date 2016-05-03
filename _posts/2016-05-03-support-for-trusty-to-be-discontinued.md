---
layout: post
title: "Support for Ubuntu 14.04LTS to be discontinued"
author: Andrew Chadwick
date: 2016-05-03 00:00:00
categories: blog
discourseID: 348
---

[MyPaint's testing repository for Ubuntu
systems](https://launchpad.net/~achadwick/+archive/ubuntu/mypaint-testing/+packages)
will discontinue support for an important old Ubuntu release shortly.
Ubuntu 14.04LTS, a.k.a. "Trusty Tahr", will no longer be supported by us.
If you are using this Ubuntu release, please upgrade to the latest LTS,
16.04 "Xenial Xerus" as soon as you can. [Here's
how.](https://wiki.ubuntu.com/XenialXerus/ReleaseNotes)

As you probably know I've been maintaining the Ubuntu [mypaint-testing
PPA](https://launchpad.net/~achadwick/+archive/ubuntu/mypaint-testing/+packages)
for several years, trying to support a broad range of Ubuntu releases.
We currently have support for trusty (12.04LTS) thru xenial (16.04LTS)
with the notable gap of utopic (14.10) right now. Shortly, support will
be dropped for vivid (15.04) too.

This widening gap of support is happening because _Canonical themselves_
do not support these old non-LTS releases: check out the [support matrix
on
Wikipedia](https://en.wikipedia.org/wiki/Ubuntu_(operating_system)#Releases)
to see how they do it. Vivid has recently turned red, now that 16.04LTS
is out, and we're forced to maintain that pattern as it changes over
time.

Also, I actually want to discontinue making builds for the old LTS
release for the next MyPaint 1.2.1.beta release or 1.2.1 proper, because
supporting a 2 year old GTK platform makes development difficult and
slows down the release process. It will mean we can rip out some very
stinky old code that's just there for legacy support ☺

Looking at the PPA's download statistics, the majority of our PPA users
are still wedded to the old LTS, so it's clear we need you give folks
fair warning. However, our hands are tied about the timing; I cannot see
Canonical keeping PPA support for the old LTS around for much longer.

People using Ubuntu 14.04LTS should upgrade to 16.04 as soon as
possible. LTS→LTS upgrades are supported by Canonical.

People using earlier Ubuntu releases should begin their upgrade
treadmill now. You *might* be able to skip releases, but please check
their release notes before you try anything drastic:

* http://www.ubuntu.com/download/desktop/upgrade
* https://wiki.ubuntu.com/XenialXerus/ReleaseNotes (15.10 *or* 14.04LTS)
* https://help.ubuntu.com/community/UpgradeNotes (intervening versions)
