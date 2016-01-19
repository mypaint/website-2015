---
layout: post
title: "Final translation push for 1.2.0"
author: Andrew Chadwick
date: 2015-11-21 03:55:10
categories: blog
---

<p style="text-align: center; display: block;">
<img src="/assets/posts/2015-11-21-languages-world-map-gfdl.png"
alt="Map of world languages"
title="Languages world map, by Julien1311"
/>
</p>
MyPaint is nearing its next stable release, v1.2.0,
and that means it's time to get the translations finalized.
Today marks the start of a week-long translation effort for MyPaint,
and we need your help!

### Translation status

At the time of writing,
the 33 languages we support are just under 50% translated.
We’d like that figure to be much higher!
Can we get to 55% or 60% within a week,
or complete one or more of the smaller languages?

Latest figure: <a href="https://hosted.weblate.org/engage/mypaint/"><img
src="https://hosted.weblate.org/widgets/mypaint/-/svg-badge.svg"
title="Please help translate MyPaint into your language on Weblate"
/></a>

### How you can help

If you’re new to translating software, welcome!
We've made it as simple as possible to help.
All of the program text is available for translation on
[WebLate](https://hosted.weblate.org/engage/mypaint/).
WebLate is a collaborative online tool
that presents each fragment of text in turn,
and asks you to translate it.
If you're not sure,
you can type in suggestions for other translators.

<div style="align: center; text-align: center; padding: 0.5em;">
<p
style="border: solid 2px; padding: 0.5em 1.0em; width: auto;"
>
<strong style="font-size: 150%;">
<a
href="https://hosted.weblate.org/engage/mypaint/">Click here to start translating</a>
</strong>
<br/>
<em>(and please share the link with your friends!)</em>
</p>
</div>

You can log in with social media accounts,
or your Github account if you are already a developer.
The account name is recorded in the commit log,
and you can add your name to the credits by adding it to
the translation of the “translator-credits” marker string.

### What needs translating?

MyPaint has two components which can be translated:

* [libmypaint](https://hosted.weblate.org/projects/mypaint/libmypaint/):
  This is MyPaint’s dynamic brush engine.
  The strings for translation are all brush setings, inputs, etc.
  Without context, this can be somewhat hard to translate.
* [MyPaint](https://hosted.weblate.org/projects/mypaint/mypaint/):
  The main GUI for the program.
  Context is present for a subset of these,
  and the strings don't require as much domain-specific knowledge.
  However, there are a lot of them.

### Translation workflow

The main translation interface looks like this:

![Screengrab of the WebLate interface](/assets/posts/2015-11-21-weblate-interface-small.png)

1. Source texts in the program are written in US English.
2. The translation text box is where you write your translated text.
3. When you're confident the translation is correct,
   click on Save to move on to the next string in the
   current list.

The **fuzzy** checkbox is an indication that this translation is a guess.
Sometimes this is because the tools we use have been forced to make
an estimate about which ild translation is which (it happens, sorry!)
Alternatively, other translators may have flagged the string as erroneous.
Fuzzy strings are not presented in the user interface,
so reviewing and cleaning up fuzzy translations will really help
a translation present much more usefully.

One hidden feature in the WebLate UI is the **Machine Translation** tab.
It's pictured above, but it isn't open by default.
Machine translation can be used as a starting point,
but please don't machine-translate the entire program!

You will sometimes see **formatting codes** in strings that need
translating. These might look like any of the following:

* “%s”, “%r”, “%d”, etc. (python-format)
* “{like_this}” (python-brace-format)

These need to stay in the translated text.
The MyPaint program will try to replace them
with other fragments of text at runtime,
for example the name of a file, or a pixel size.
If they are omitted, the program may crash
or present the user with an error message.

If you're an expert in MyPaint and want to help out other translators of
your language who don't know the program that well,
please consider adding to its **glossary**.
This is also a good place to write up a style guide for your language's
translation.

Even if your language is complete, you can help by sharing the link
above among your colleagues and friends on social media.

Page image:
<https://commons.wikimedia.org/wiki/File:Languages_world_map.svg> by
Bardion and Julien1311, GFDL/cc-by-sa-3.0.

