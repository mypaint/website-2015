---
layout: post
title: "MyPaint v2.0.1 Released"
author: Jesper Lloyd
date: 2020-05-29 22:30
categories: blog
excerpt: "Bugs were squashed and things were made a bit better."
---

[MyPaint v2.0.1](https://github.com/mypaint/mypaint/releases/tag/v2.0.1) is out!

This is a bugfix release, so no new features, but quite a few improvements.
The most important bug that has been fixed, for those who work in 2.x mode, is the rounding error bug.
If you do most of your work in that mode, updating is strongly recommended!

Here is a selection of the changes. The full (condensed) changelog can be read on the release page.

* HSV/HCY brush dynamics in 2.x mode have been fixed.
* Undo/Redo stack size is now configurable, and the default size is increased to 40.
* An image-degrading rounding error when saving files in 2.x mode has been fixed.
* Translations have been updated, and some invalid translations have been corrected.
* Translations in the brush editor now works correctly in the AppImage builds.
* Invalid (technically) svg icons have been fixed, and reduced in size.
* Performance for the Windows builds have been improved (they now use openmp)
* Windows build sizes have been significantly reduced. (extracted size by ~50%, compressed size by ~70% for installers)
* AppImage file sizes have been reduced by ~9MB (a ~30% reduction for the English-only version).
* AppImages can now launch external editors without causing dependency conflicts.
