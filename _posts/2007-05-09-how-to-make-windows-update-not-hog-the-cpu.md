---
author: Ted
title: >
  How To Make Windows Update Not Hog the
  CPU
excerpt:
layout: post
category:
  - Computers
tags:
  - windows
post_format: [ ]
---
Every morning I come into work, plug my laptop in, and turn it on.  It quickly resumes from hibernation, and then forces me to wait for about three minutes while svchost.exe dominates the CPU.  This morning, however, the process never finished.

Several hours and searches later, I had my computer back as well as a new disdain for Microsoft Update.  Windows Update is a standard feature of every version of Windows since 98 (I think).  Starting with XP service pack 2, we gained the “option” to have the updates auto-downloaded.  This works fairly well.  The problem occurs when you opt to “enhance” your Windows Update and turn it into Microsoft Update.  It sounds like a good idea.  You get the Office updates and any other MS product updates.  Unfortunately the update process isn’t the most efficient.

As a software developer myself, I have learned restraint in criticizing others’ design.  I will, however, let the community speak out on this: [[link]][1]

Basically, whenever you start your machine, MS Update (via svchost.exe) checks every app that was installed with Windows Installer 3 to see if there are any updates available.  This takes forever.  I did, however find a fix, courtesy of the MS community forums [[link]][2].

Here’s what you do:

*   Download and install this HotFix: [KB927891][3] (Restart required)
*   Download and install [Windows Update Agent 3.0][4]

Now If only I could make Windows use less RAM.  (500 MB on startup vs 70 MB on my ArchLinux system at home)

 [1]: http://www.microsoft.com/communities/newsgroups/en-us/default.aspx?dg=microsoft.public.windowsupdate&tid=25062243-6614-479b-9a73-e534497e7870&p=1
 [2]: http://www.microsoft.com/communities/newsgroups/en-us/default.aspx?dg=microsoft.public.windowsupdate&tid=518785f4-c21e-4b30-a010-21b854b3438f&p=1
 [3]: http://support.microsoft.com/kb/927891
 [4]: http://download.windowsupdate.com/v7/windowsupdate/redist/standalone/WindowsUpdateAgent30-x86.exe