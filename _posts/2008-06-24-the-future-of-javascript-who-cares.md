---
author: Ted
title: 'The Future of Javascript -- Who Cares?!?'
excerpt:
layout: post
category:
  - Thoughts
tags:
  - firefox
  - javascript
  - mozilla
  - slashdot
  - Stupidity
post_format: [ ]
---
[Yesterday on Slashdot][1], someone posted an [InfoWorld interview][2] of Brendan Eich (the creator of JavaScript).  In the interview he lays out his plans of the evolution of JavaScript into what he calls JS2.  The discussion on Slashdot was over the details of whether the language changes made things better or worse.  The thing about programmers is that they won’t all agree on anything.  Everyone has their own understanding of how software should be written.  My critique isn’t on any of the details of the language changes, its the premise itself.

First of all, let me say that I don’t believe JavaScript to be the Holy Grail of languages.  It’s not perfect, there are things about it that I find irritating.  There are also things about it that I like.  This is true of any language with any competent hacker.

**Why JavaScript Matters:**

More and more software is being designed to run “in the cloud”.  The benefits are obvious.  Deployment is trivial, as are upgrades.  Developing for the web means not having to care about the users’ platforms.  Connectivity is becoming faster and more ubiquitous every day.  JavaScript matters because it is the language of the web.  It excels not on technical merit, but out of necessity.

In the 1990s, Netscape was in a unique position.  It essentially owned the web platform.  Whatever they decided became standard.  When Microsoft built IE, they had to include JavaScript support so their browser could compete.  Every new browser since then had to include a JavaScript engine.

In todays market, every computer has a web browser and therefore has a JavaScript engine.  JavaScript matters for one reason, and only one reason: ***i******t is ubiquitous***.

**Why JS2 Does Not Matter:**

Although Mozilla acts as if they inherited Netscape’s mid 90s status as keeper of the web platform, this is not the case.  They say that it doesn’t matter is Microsoft adopts JS2 or not, they’ll just write an IE plugin.  This may work to increase JS2 adoption, but it doesn’t actually solve any real problems.  JS2 is a solution looking for a problem.

When building TileStack, my main problem with JS isn’t some language feature (native classes, typed variables, etc.) it’s the lack of consistency between browsers.  Granted this isn’t something the Mozilla Foundation can fix, but a new version of the JS language does more harm than good in this context. 

**Why JS2 is Harmful to Mozilla:**

While Mozilla has the best of their JavaScript team busy writing new language features, the competition is getting tough.  Apple continues to push the limits of WebKit.  The next version of Safari will smoke the competition when it comes to JS performance.  They are packing so much stuff into the browser, that web developers will start to question the need for Flash.  Meanwhile, Mozilla is working on the syntax for the “let” keyword.  Hey Mozilla, where’s mobile FireFox?  How come the poster boy for open source isn’t part of the first open source mobile phone platform (Android)?  Congratulations on all the downloads of FireFox 3.  Too bad it’s killer feature is that it doesn’t suck down resources like FireFox 2.  Wake up guys, you’re starting to lose!

I guess the point is that language syntax is one of the least important features of a platform.  Do developers use .Net for C#’s syntax?  Is Objective-C’s syntax the reason for Apple’s recent successes?  Will the declarative structure of JavaFX Script save the Java platform?  I could go on with more examples, but I wont.  The answer is a resounding NO!  There are much more important things to ensuring the success of a platform than language syntax.

I suppose this doesn’t really need to concern me.  The web as a platform will continue to exist and grow and mature.  It’s just frustrating to observe this waste of time and energy.

UPDATE: I want to give credit where credit is due.  My colleague Josh Gertzen was quoted in [AjaxWorld magazine][3] on the irrelevancy of JS2 in an article that ran on [Slashdot][4] for a while.

 [1]: http://tech.slashdot.org/article.pl?sid=08/06/23/2112213&from=rss
 [2]: http://www.infoworld.com/archives/emailPrint.jsp?R=printThis&A=/article/08/06/23/eich-javascript-interview_1.html
 [3]: http://ajax.sys-con.com/read/456101_2.htm
 [4]: http://developers.slashdot.org/article.pl?sid=07/12/11/1947240