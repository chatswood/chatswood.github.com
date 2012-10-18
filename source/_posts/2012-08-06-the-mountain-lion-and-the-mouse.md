---
layout: post
title: The (Mountain) Lion And The Mouse
date: 2012-08-06
tags: [Mountain Lion, OS X, Dropbox]
categories: [Apple, Technology]
permalink: /post/28825879449/the-mountain-lion-and-the-mouse
---

Mountain Lion has been running really well on *almost* all the machines I've installed it to, with just one exception - my (employer's) 17" MacBook Pro. This is unfortunate, as it's the machine that I spend the most time on - if it's not running smoothly I feel the "pain" all day, every day.

Specifically I was experiencing severe cursor lag when using the mouse (or trackpad) on an intermittent basis. It wasn't caused by any one application that I could isolate, but some apps did seem to trigger it more frequently. I couldn't see anything under Activity Monitor to indicate what the problem could be - there were no CPU or I/O spikes. I resolved to just sit it out waiting for the inevitable 10.8.1.

Then I experienced a bout of constant lag. At first it seemed like a curse, but I realised that I had a recently booted system with few applications running - this is as close as I get to laboratory conditions. A quick glance at the process list showed that only one was running a little high - [Dropbox][][^1]. It was only consuming 17% of a single core, but it still seemed a little high. When I finally got the cursor under control I was able to quit Dropbox and the lag ceased immediately. I'm guessing it might have been something to do with the methods by which Dropbox monitors the filesystem for changes.

A quick inspection of the Account pane under the Dropbox preferences revealed that I was still running the 1.4.7 version, rather than the Mountain Lion-compatible 1.4.12. This wasn't all sloppiness on my part - as usual Dropbox have said that the clients should auto-update, but, also as usual, Dropbox's auto-update facility is woefully behind the time.

All good [fables][] need a moral, so here goes: *"If your Dropbox client hasn't updated itself, then you might want to do so manually."*


[Dropbox]: http:://www.dropbox.com
[referral link]: http://db.tt/LNlAuHd
[fables]: http://en.wikipedia.org/wiki/The_Lion_and_the_Mouse

[^1]: If you've not yet used Dropbox and would like to sign up, here's a [referral link][].