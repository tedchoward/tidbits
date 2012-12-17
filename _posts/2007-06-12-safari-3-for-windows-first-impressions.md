---
author: Ted
title: 'Safari 3 For Windows -- First Impressions'
excerpt:
layout: post
category:
  - Computers
  - programming
  - ThinWire
tags:
  - ajax
  - apple
  - corefoundation
  - coregraphics
  - firefox
  - internet explorer
  - opera
  - safari
  - web
  - webkit
  - windows
post_format: [ ]
---
As soon as I heard the announcement, I downloaded the public beta of [Safari 3 for Windows][1].  So far I’m pretty impressed.  The memory usage seems to come in between Firefox (the worst) and Opera (the best).  [ThinWire][2], my web application framework, works beautifully.  Gmail works fine, but Yahoo Mail has some issues (I get lots of JS errors).

I did a quick performance benchmark.  ThinWire has a [Grid][3] component that can display lots of data.  I fired up my benchmark app for the Grid, and added 10,000 rows.  Here’s the performance results: 

*   Internet Explorer 7: 1 minute 33.66 seconds
*   Opera 9: 27.93 seconds
*   Firefox 2: 23.24 seconds
*   Safari 3 Beta: 18.91 seconds

I realize that there is only approximately a 4 second improvment over Firefox 2 in this test, but 4 seconds is a lifetime in terms of waiting for a web application to load.

Also, while the Grid was loading, the rest of the app was still responsive; I could even start browsing and scrolling the Grid.Also, a quick look in the install directory reveals some interesting libraries.  WebKit was there as expected, but also CoreFoundation (Apple’s base C library) and CoreGraphics (the main OS X graphics library).  Very interesting.

 [1]: http://www.apple.com/safari/
 [2]: http://www.thinwire.com
 [3]: http://thinwire.com/api/thinwire/ui/GridBox.html
