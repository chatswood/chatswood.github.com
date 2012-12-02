---
layout: post
title: Mail.app and Power Nap
date: 2012-12-02 12:05
comments: false
tags:
- OS X
- Mountain Lion
- Mail
- Power Nap
categories:
- Apple
published: true
---

Mountain Lion has been with us for several months now and has been a pretty solid release with some nice new features. One of those [features is Power Nap][OSXFeatures] - the ability for a certain Macs to sleep with one eye open. It allows for the updating of data (fetching mail, contact updates, etc) and the performing of housekeeping tasks (carrying out backups and downloading software updates) while your Mac give sthe impression of being asleep.

I have a nice shiny 2012 [MacBook Air][] so I've been getting these Power Nap features for free since upgrading to Mountain Lion. Generally I don't notice it much - I have notifications from Messages already onscreen when I open my machine in the morning, software updates are quick to apply because they have already been downloaded and, most usefully, I can see new entries in my mailbox that arrived overnight.

So far, so good. There's just one gripe with the way the mail messages arrive. I have an IMAP account that gets updated with new messages. But if I have viewed those messages on my iPhone/iPad or on another Mac, they don't get marked as read via Power Nap. This seems like a minor inconvenience as the next refresh of the IMAP account should update their read/unread status.

Nope. Checking for new mail in all accounts doesn't change the status. In fact, basic testing has shown that once woken from Power Nap I can't even pick up new items in the IMAP mailbox. A restart of Mail.app is required before any updates to that mailbox are detected. It just seems to be the one IMAP account though - I have 3 other mail accounts (2 GMail and 1 iCloud) that update fine.

I guess it's time to file a bug.



[OSXFeatures]: http://www.apple.com/osx/whats-new/
[MacBook Air]: http://www.apple.com/macbookair/
