---
author: Ted
title: Sending Legitimate Bulk Email
excerpt:
layout: post
category:
  - Computers
  - Stupidity
tags:
  - bulk
  - development
  - dkim
  - email
  - filter
  - gmail
  - software
  - spam
  - web
post_format: [ ]
---
This is for all those people who are trying to run a web business that need to send bulk email messages and don’t want them to go directly into their recipients’ spam folders.

Yesterday, I (and several others) dedicated several hours to the task of determining why every email we sent went directly into the spam folders of those we were trying to reach. When you search Google for information about spam filters, you find plenty of information about blocking unwanted email, but hardly anything about making sure your legitimate bulk email is not discarded with the trash. We were able to solve our issues, and so I thought I’d share our findings with the community.

*   Send only plain text. Attachments and HTML content raise flags with content filters.
*   Set the message header: “Precedence: bulk”
*   You must set a subject, body, from address, and reply-to address (not having reply-to was my problem

In addition, if you are hosting your own mail server you should:

*   Publish an [SPF record][1] in your DNS configuration
*   Configure your MTA to and DNS to use [DKIM][2]. (Acronyms FTW!)

I hope this info is helpful to someone. I wish I had it.

Sources:

*   [http://mail.google.com/support/bin/answer.py?hl=en&answer=81126][3]
*   <http://domainkeys.sourceforge.net/>
*   <http://www.skylist.net/resources/authentication.php>

 [1]: http://old.openspf.org/wizard.html
 [2]: http://www.dkim.org/
 [3]: http://www.skylist.net/resources/authentication.php