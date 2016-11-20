---
layout: post
title: "Fixes are in the pipeline for GDK Wintab"
author: Andrew Chadwick
date: 2016-11-20 17:00
categories: blog
---

I've been submitting a lot of patches to GDK recently,
trying to get some of our Windows tablet bugs fixed up.
The good news is that I think we're turning the corner on
reliability over there.
Tilt should be working soon for fancy devices like the Intuos 5,
and I've fixed a pair of really nasty crashers for non-Wacom devices.
There was also a silly regression that caused
pressure to be ignored depending on
whether your tablet had an odd ID or an even one
(don't ask, but I'm hoping we'll be able to close
a ton of our own bug reports before long).

* <https://bugzilla.gnome.org/show_bug.cgi?id=774265>
* <https://bugzilla.gnome.org/show_bug.cgi?id=774379>
* <https://bugzilla.gnome.org/show_bug.cgi?id=774699>

I'm really happy about this.
It's my first proper foray into dealing with the
incompatible nonsense values that real hardware sends,
and it's nice to be actually be pushing back the tide for once.

![Test graphics tablets](/assets/posts/2016-11-20-hardware-pile.jpg)
