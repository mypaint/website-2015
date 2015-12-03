---
layout: post
title: "Developer Monologue: Short History of MyPaint"
author: "Martin Renold"
date: 2009-06-18 00:00:00
categories: blog
---



Okay, this is so that everyone can just stop asking why MyPaint, etc.

Around 2004 I bought myself a wacom tablet, having checked that it 
should work with GIMP on Linux. It did work. With minor bugs and 
glitches. For example, GIMP would sometimes drop a stroke when 
scribbling too fast. I also thought I could paint more freely if the 
brush would react in different ways to pressure and velocity.

I created a small prototype to try this. It did render circular dabs 
with radius and opacity depending on pressure and velocity. I was also 
eager to use a lowpass filter when calculating the velocity, since this 
topic was covered in my engineering studies recently.

It did work – I could paint with the program, and it was fun! I saved 
by taking screenshots. I could have done the same art inside GIMP, or 
with some freeware tool on Windows, but… A co-worker once joked that, 
should I ever want to drive, I would start by building my own car.

I had some fun experimenting with other brush ideas. My simple XInput 
test program slowly turned into a brush editor. Even today, the core of 
MyPaint is still the same experimental brush editor that I wanted to 
create at this time. It allows me to try my brush ideas quickly. Since 
I already prefered it to GIMP for creating simple art, I released the 
code without much noise.

The program slowly grew after that. Around 2006, with the release of 
version 0.4, the program was everything I wanted it to be. There was 
no undo or layers, but I had a nice brush collection now. It worked 
well with my tablet, and it was fun to use. I had reached my goal.

Something must have gone wrong, since I continued development anyway. 
Users started to appear, some of them requesting features that I also 
wanted for myself anyway. When I added layer support, the project 
turned into something more serious than a brushtest. Well, as serious 
as a project can be when it ships with a debug menu and user-visible 
FIXME comments in the tool settings.

In the meantime, several people have contributed small enhancements or 
have just been enthusiastic and spread the word. And in general it 
looks like MyPaint is here to stay, since for some reason I can’t seem 
to stop working on it. Maybe for the lack of a better challenge?

And MyPaint even has some [goals now](http://mypaint.org/about/).
