---
layout: post
title: "MyPaint v2.0.0-alpha.13 Released"
author: Jesper Lloyd
date: 2019-11-09 14:40:00
categories: blog
excerpt: "A new alpha release is upon us, and we look back on the alphas in between."
---

For those who don't spend their days spamming `git fetch` in their local 
clone of the mypaint repo, eagerly waiting for the latest changes, it might
seem like nothing much has happened recently. To allay such notions,
there is now a new alpha release with the latest and greatest changes 
(as a matter of fact, all changes) as we make our steady crawl towards
the beta phase.

Get yourself over to the [release page][release.src] for a list of changes
and a list of files!

Unfortunately we don't have the ppa or other deb builds up to date, so users
on Debian/Ubuntu will have to make do with the AppImage builds for the time
being.

## A Tale of Alphas Past

Since there were no blog posts about the alpha releases after the first one,
here is a quick summary in reverse chronological order.

### Alpha 12

These were the new features added in alpha 12:

* Faster floodfill
* Offset/Blur options added to floodfill
* Gap-detecting floodfill
* Erase/Lock Alpha/Colorize now work with floodfill
* Click-drag floodfill (fill multiple separate areas in one go)
* Separate source-selection (you can fill _based on_ a specific layer)
* Cancellable floodfill (if you made a mistake on a _huge_ canvas or with a
slow computer, most people should never see the cancellation dialog)
* Adjustable opacity and blendmode for floodfill (sometimes useful)
* Ability to fill _with reference to_ vector layers.
* Viewport-limited floodfill (useful for erasing and
adjusting gap-detection settings)

There may be a pattern in those additions, I'm not sure.

### Alpha 11

* Floating subwindows brought back on Windows
* Weighted subtractive smudging - using the spectral model for sampling colors

### Alpha 10-9

* Tweaks and fixes to rendering/compositing of the new color representations

### Alpha 8

* Keyboard-controlled drawing inputs for pressure and barrel rotation
* Improvements to layer merging for the new Pigment layer type

### Alpha 7-1

* Minor changes, preparations for barrel rotation input

[release.src]: https://github.com/mypaint/mypaint/releases/tag/v2.0.0-alpha.13
