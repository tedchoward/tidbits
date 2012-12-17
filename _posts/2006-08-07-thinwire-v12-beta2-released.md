---
author: Ted
title: ThinWire v1.2 beta2 Released
excerpt:
layout: post
category:
  - ThinWire
tags: [ ]
post_format: [ ]
---
After several weeks of hard work, the next beta has been released.  You can read all about it at the [ThinWire Blog][1].  The main two things are the ability to change the style of each component or the entire application at a global level through a properties file, and a major performance enhancement minimizing client-server traffic.

My main contribution to this release is the RangeComponent interface and two component implementations of this interface: Slider and ProgressBar.  The progress bar is very useful for providing feedback to the user while your application is doing some sort of processing.  The slider is used for selecting a numeric value from a specified range of values.

As this release was mainly about style, I have revamped the look of ThinWire Mail (my demo application built in my spare time).  Today we are also announcing live demos of ThinWire, so you can click [here][2] to try out ThinWire Mail without having to download anything.

[ThinWire Mail Demo][2]

[Playground Demo][3]

[Download ThinWire v1.2 beta2 SDK][4]

 [1]: http://thinwire.com/blog/
 [2]: http://207.200.22.70:8086/mail/
 [3]: http://207.200.22.70:8086/playground/
 [4]: http://thinwire.com/download.html