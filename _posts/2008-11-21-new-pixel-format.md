---
layout: post
title: "New Pixel Format"
author: Martin Renold
date: 2008-11-21 00:00:00
categories: blog
comments: off
---

GEGL (the upcoming GIMP backend) uses linear-light floating point as 
the main pixel format. Krita allows several colorspaces and color 
management through LittleCMS. What about MyPaint? Version 0.5.x uses 
8bit sRGB without any alpha channel. Time for a change.

I have settled now with a 16bit integer for each channel, permultiplied 
alpha, no linear light (gamma as in sRGB). The extra precision helps 
against the noise when blitting many faint dabs on top of each other. 
Here you can see the difference (click to enlarge):

![8bit vs 16bit](/assets/posts/2009-07-23-8bit_vs_16bit.png)

A more subtle point is that white (or opaque alpha) is not stored as 
2^16-1 but as 2^15. So, after multiplying a component with the alpha 
channel, the neccessary division by 2^15 can be done with a simple bit 
shift (fixed-point arithmetic). So effectively only 15 bits are used. 
Nobody will miss that final bit of precision.

I also have read quite a bit about linear light and even did a test 
implementation. But after a short painting session I came to the 
conclusion that, while the effect for painting is subtle, it is mostly 
counter-intuitive. Especially the fact that white is “stronger” than 
black. I’m sure there are some special situations where it works better 
(eg zooming, and maybe layer compositing in some special cases), but 
right now, linear light is no longer a topic for me.

The advantages of premultiplied alpha have been discussed more than 
enough elsewhere. I just want to share one little pleasant surprise: my 
almost unoptimized C implementation blitting 16bit premultiplied RGBA 
onto 8bit RGB is three times faster than gdk-pixbuf blitting 8bit RGBA 
onto 8bit RGB.

