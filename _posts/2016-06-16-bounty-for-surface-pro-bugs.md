---
layout: post
title: "Bounty available for Surface Pro 3+4 pressure issues"
author: Andrew Chadwick
date: 2016-06-16 12:00
categories: blog
---

People wanting to use MyPaint fully on newer versions of the [Surface Pro][surfpro] tablet are [willing to pay a bounty][bounty] for an important bug to be fixed. It's one where our core development team don't have hardware available for testing, so not much progress has been made yet.  It's up on Bountysource right now, if you're intersted in getting this one fixed. You can help by backing the campaign, or claim the bounty by fixing the [bug][issue]!

This is MyPaint's first foray into BountySource, so I'm keen to see how it goes. It was prompted by one of our wider community, [@scooter-dangle](https://www.bountysource.com/people/24832-scott-steele), posting the first bounty. Thanks, Scott! BTW, Bountysource are quite open about [how it works][bsfaq] in case anyone has any doubts about this.

The issue might be moderately hard to fix: I kinda suspect it's actually a bug with [GDK][gdk], one of the libs MyPaint is built against. There may be things to do in MyPaint as well, we're just not certain yet.  Even if it's really a problem elsewhere, a tested fix for [GDK's win32 backend](https://git.gnome.org/browse/gtk+/tree/gdk/win32) would probably meet our backers' approval. If it is a GDK bug, it should be reported in [the GNOME gtk+ tracker][gtkbugz] as well (with a link back to ours).

Here's the bounty post: <https://www.bountysource.com/issues/28004023>. Feel free to draw us an actual wild–west–style bounty poster if you want!

[surfpro]: https://en.wikipedia.org/wiki/Surface_Pro
[bounty]: https://www.bountysource.com/issues/28004023
[issue]: https://github.com/mypaint/mypaint/issues/484
[gtkbugz]: https://bugzilla.gnome.org/page.cgi?id=browse.html&product=gtk%2B
[bsfaq]: https://github.com/bountysource/core/wiki/Frequently-Asked-Questions
[gdk]: https://git.gnome.org/browse/gtk+/tree/gdk
