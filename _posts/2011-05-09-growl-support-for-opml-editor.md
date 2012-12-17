---
author: Ted
title: Growl Support for OPML Editor
excerpt:
layout: post
category:
  - Uncategorized
tags: [ ]
post_format: [ ]
---
[From blogs.tedchoward.com][1]. 

I’ve been privilaged to be part of a bootstrapping comminuty using a collaboration tool called an [Instant Outliner][2]. It’s an interesting tool built around the concept of a shared outline. I’ll probably write more about this at some point, but for now I have one specific point I want to talk about.

When the outine is updated, the computer beeps, and the person’s node that updated is bolded. This works fine when I’m at home and at my computer. But when I’m at work, I often have the volume down and the outline in the background. I found myself wanting a visual notification of some sort when the outline updated.

I’m on a Mac, so the obvious solution is to use [Growl][3].

Like all the other tools for this community, the Instant Outliner is built on top of the [OPML Editor][4], which I have previously described as a [Swiss Army Knife][5]. If I want Growl notifications for my Instant Outline updates, the OPML Editor needs to know how to talk to Growl. So, I wrote a tool.

Growl.root adds support for sending Growl notifications from scripts written in the OPML Editor. There are basically 2 verbs (OPML-speak for functions) that you need to care about.

`growlSuite.newNotification(title, enabled)` will tell Growl about a type of notification I want to send. For the instant outliner I would execute:

    growlSuite.newNotification("Instant Outliner", true)

`growlSuite.sendNotification(name, title, description)` will actually send the notification. The first parameter(`name`) must match a notification type from the previous verb. The second parameter is the title of the notification and the third parameter is the text of the notification. To notify that I updated my outline I would execute:

    growlSuite.sendNotification("Instant Outliner", "tedhoward", "Guys, check out my new growl scripts")

If you’re interested in this sort of thing, you can download growl.root [here][6].

 [1]: http://blogs.tedchoward.com/ted/stories/2011/05/09/growlSupportForOpmlEditor.html
 [2]: http://bhc3.wordpress.com/2009/01/16/before-there-was-twitter-there-was-dave-winers-instant-outliner/
 [3]: http://growl.info/
 [4]: http://editor.opml.org/
 [5]: http://blogs.tedchoward.com/ted/stories/2011/03/24/aSwissArmyKnife.html
 [6]: http://static.tedchoward.com/tools/growl.root.zip
