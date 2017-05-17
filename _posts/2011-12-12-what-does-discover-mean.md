---
layout: post
title: "Lessons from TileStack: What Does '#Discover' Mean?"
date: 2011-12-12 15:37:00 -0600
---

So, last week Twitter debuted a new interface with the stated intent of
[simplifying the experience][1]. This new interface has drawn [criticism][2]
[from][3] [many][4] [bloggers][9]. Most of the discussion centered around
Twitter organizing their user interface under two categories: *Connect*
and *Discover*.

Their PR explains it this way (emphasis mine):
> We've simplified the design to make it easier than ever to follow what
> you care about, **connect** with others and **discover** something new.

The problem with *Connect* and *Discover* is that they are not words
people use to describe routine actions. Instead they are vague
words that convey a range of meanings instead of describing specific
activities[^1].

I actually get where they're coming from. There is a perceived problem
that people don't really know how to use Twitter. In the old days of
boxed software, this would be a documentation issue. In the post-manual
world that we live in today, the user interface is to blame.

The answer is to simplify, which means we need less options. Before
there were @replies, #hashtags, lists, search, followers and people you
follow. I can imagine the meeting where someone asks: 
> What if we could reduce all those features to two sections. Two is
> less than six, so that makes it simpler which makes it better. We
> just need to name the two options in a way that conveys the full
> power behind them.

That's how you come up with *Connect* and *Discover*. These are abstract
concepts, not product features. To someone
who already knows what Twitter is capable of, *Connect* and *Discover*
are great words that succinctly distill the full potential of Twitter.
To someone that doesn't know anything about Twitter, these words mean
nothing. They need to be explained in the context of Twitter.

The reason I know this is because [Josh Gertzen][8] and I made the same
mistake with [TileStack][5].

We needed a name for the button that brought up the
stack editor.[^2] We wanted to convey to the user that launching the
editor was a safe operation, that any changes they made would not be
applied to the stack they were viewing.[^3] For that reason, we didn't
want to use '*Edit*', because '*Edit*' made it sound like you could
modify something that someone else had made. We had many long
conversations and debates about what to call the button. The thesaurus
was consulted. Finally we chose a word[^4]: '*Customize this stack*'.

The idea was that '*Customize*' implied that you were creating a custom
version of the stack you were modifying instead of modifying the
original. This was the exact behavior we wanted to encourage: see a cool
stack, make some changes and save a new copy with your changes. We
really wanted to grow a community of re-mixers.

There was just one problem: people didn't click the button. We knew this
not by using fancy analytics tools, but by the questions we were asked
by email or in our forums. One of the top questions we got was a feature
request for a stack editor. We were completely befuddled. The stack
editor was **the** core of what we had built, and most people didn't
even know it existed!

Back to the drawing board. The problem with '*Customize*' was that it
*always* implied that the intent was to make a new creation. Early on,
there was no community. People just wanted to upload their
[HyperCard][6] stacks and edit them in the browser. We needed something
that would convey this ability as well as the fact that it is still a
*safe operation* on someone else's public stack.

After another long round, we finally settled on '*Inspect*'. The word
sounds pretty harmless. You're just looking around to see how something
worked. There's also the notion of an [Inspector Window][7] which was
essentially what our editor was.[^5]

Do you care to guess what the impact of that change was? How about
*nothing*? We ended up making a series of videos showing how to use the
site, which did help a lot, but we still got questions about where to
find the stack editor.

To be fair, both *Customize* and *Inspect* are actually pretty concrete
words, but they were the wrong words. How do I know they were the wrong
words? I didn't use them myself. I would always say *Edit*. In fact, the
tool palette that appeared was called the *Editor* (not *Customizer* or
*Inspector*). Those words were forced because the natural word wasn't
deemed to be good enough. This just exposes that we weren't as smart as
we thought we were.  Eventually we broke down and just called the
button '*Edit*'[^6]


[^1]: When was the last time you went to Twitter to *Connect*?
[^2]: By default, stacks were loaded in *play mode*. If a user wanted to modify the stack (or see how it was built), they needed to launch the editor.
[^3]: You could launch the editor on any public stack on the site, so that you could see how they worked.
[^4]: Err... phrase.
[^5]: Without the window.
[^6]: If you edited someone else's stack, we indicated that it was a *safe operation* by changing the *Save* button to a *Save As* button.

[1]: http://blog.twitter.com/2011/12/lets-fly.html
[2]: http://inessential.com/2011/12/08/on_the_tab_labels_in_the_new_twitter_app
[3]: http://daringfireball.net/2011/12/new_twitter
[4]: https://twitter.com/amyhoy/status/146286890641928192
[5]: http://youtu.be/fwlJGLIsT-M
[6]: http://en.wikipedia.org/wiki/HyperCard#Similar_systems
[7]: http://en.wikipedia.org/wiki/Inspector_window
[8]: http://twitter.com/#!/gertzen
[9]: http://scripting.com/stories/2011/12/10/newnewTwitterNotSoNew.html
