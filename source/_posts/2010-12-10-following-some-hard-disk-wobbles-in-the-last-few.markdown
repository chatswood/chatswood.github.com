---
layout: post
title: Daily Backups
date: 2010-12-10
tags:
- Backup
- Growl
- Mac
- OS X
- Prowl
- SuperDuper!
- iOS
permalink: /post/2163692626/following-some-hard-disk-wobbles-in-the-last-few
categories: [Technology]
---

Following some hard disk wobbles in the last few weeks I decided to take a more rigorous approach to my backup strategy. I've been using [SuperDuper!][] for some time now but my backups were infrequent to say the least. So I bit the bullet and set up a scheduled backup for myself to run every lunchtime when I was away from my desk.

After a couple of days I decided that wasn't quite enough - what I really wanted was a backup at the end of the day to complement the lunchtime backup. However I'm too impatient to sit around waiting for a backup to complete when I could be hitting the road and avoiding rush hour traffic. So I went for the next best thing and went for a morning backup instead. Because my arrival time to work can vary a bit depending on morning traffic I simply enabled the *"When you connect [drive name] to your Macintosh"* option in [SuperDuper!][] which allowed it to start as soon as my boot procedure finished and I'd attached the drive to the Mac.

This was working well, however it did leave me checking back occasionally to see when I could get started on some work. This is when [Prowl][] came to the rescue. Prowl is a fantastic [iOS app][iTunes] that receives notifications from my desktop applications and forwards them to my iOS device using Apple's push notification service. Prowl receives these notifications from my Mac via it's custom [Growl][] plugin - this plugin receives the Growl notifications and sends them to my account with Prowl (and also displays the notification to the computer screen).

Once [Prowl][] has sent the notification to my device I get a nice alert (as seen above) informing me that the backup has completed or failed (which has never happened to date thankfully). All of which means that I can continue to enjoy my breakfast until my iPhone alerts me to the fact that it's time to get stuck into a days work.

Speaking of which...

[SuperDuper!]: http://www.shirt-pocket.com/SuperDuper/SuperDuperDescription.html
[Prowl]: http://prowl.weks.net/
[iTunes]: http://itunes.apple.com/app/prowl-growl-client/id320876271?mt=8
[Growl]: http://growl.info/
