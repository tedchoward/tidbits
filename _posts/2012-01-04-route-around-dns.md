---
layout: post
title: How to Route Around DNS
date: 2012-01-04 09:43:00
published: false
---

Background
==========

There's been a lot of talk recently about [SOPA][1] and what it will do to the internet. The general consensus is that it will [destroy the internet][2]. The basic premise is this: if someone complains that your site is hosting copyrighted material, the federal government will have the authority to seize your domain name.

What does that mean? Every computer connected to the internet has a number called an IP address. It's kind of like how every telephone connected to the phone network has a phone number. If you want to call your friend, you have to type their phone number into your phone. Over the years, we have built several systems to manage phone numbers from the phone book published by the phone company to the built in address book in most modern cell phones. Today, there are very few phone numbers that I have memorized.

The internet essentially has a worldwide address book that knows each computer's unique number. I don't know Google Search's number, but when I type [google.com](http://google.com) into my web browser, it looks up google's number in the global address book (called the domain name system). This system makes the internet usable. (Imagine having to look up IP addresses in a giant phone book every time).

How To Route Around
===================

If this law passes, we can no longer trust that when we type in google.com our browser will take us to Google Search. Here's what we can do about it.

Step 1: Know the IP Addresses of Your Favorite Sites
----------------------------------------------------
Every computer has a tool called <code>ping</code> that is normally used to test whether another computer is connected to the internet. It has a nice side effect of displaying the ip address if you give it a domain name. <code>ping</code> is a command line tool so you will first need to open Terminal on the Mac or cmd.exe on Windows.

Example:
<pre>
$ ping google.com
PING google.com (74.125.227.112): 56 data bytes
64 bytes from 74.125.227.112: icmp_seq=0 ttl=60 time=2.894 ms
</pre>



[1]: http://en.wikipedia.org/wiki/Stop_Online_Piracy_Act
[2]: http://www.google.com/search?client=safari&rls=en&q=sopa+will+destroy+the+internet&ie=UTF-8&oe=UTF-8
