---
layout: post
title: Shifting the blame won't help
external-url: http://allthingsd.com/20120406/whats-this-a-mac-virus-no-actually-its-a-weakness-in-java/
published: true
comments: false
date: 2012-04-08
tags:
- AllThingsD
- Apple
- Flashback
- Java
- Malware
- Trojan
permalink: /post/20724352391/shifting-the-blame-wont-help
categories: [Apple, Opinion]
---

In a recent article about the Flashback Trojan that's been infecting many Macs Arik Hesseldahl at AllThingsD led off with the title *[What’s This? A Mac Virus? No, Actually It’s a Weakness in Java][Source]*. Intentional or not, this title contains the suggestion that it's not Apple's fault, it's Oracle's (with a hint of "Macs are still invulnerable" thrown in for good measure).

He's right of course - it's not a Mac virus. (If we want to be pedantic it's not even a [virus][], it's a [trojan][].) But Arik goes on to try to diminish the importance of this trojan, and worse, he seems to try to admonish Apple of their responsibility:

> Does that let Apple off the hook entirely? No, though to its credit, Apple had a fix ready within a week of learning of this vulnerability. That’s not exactly a pokey response, especially when the problem lies not directly within Apple’s software, but in Oracle’s.

The exploit in Java that is used by the Flashback Trojan has existed for some time. It was reported in September 2011 in [CVE-2011-3544][] and Oracle themselves [put out patched Java runtimes][Oracle] in October 2011.

Contrary to the quote above, rather than getting a patch out within a week, Apple have actually sat on this one for a long time. Disappointingly they only released their updates after the [initial announcement][Dr Web] by Dr. Web caused the story to blow up.

So, Arik, let's not give Apple any credit on this one. The current estimate is 600,000 Macs infected with this malware. Yes, it's an Java vulnerability, but it is Apple who distributes the Java runtime for OS X, not Oracle. They had the opportunity to fix this in a timely fashion, and chose not to, putting many of their customers systems at risk by not doing so.

Rather than deserving credit, I rather think they owe their customers instead.

[Source]: http://allthingsd.com/20120406/whats-this-a-mac-virus-no-actually-its-a-weakness-in-java/
[virus]: http://en.wikipedia.org/wiki/Computer_virus
[trojan]: http://en.wikipedia.org/wiki/Trojan_horse_(computing)
[CVE-2011-3544]: http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2011-3544
[Oracle]: http://www.oracle.com/technetwork/topics/security/javacpuoct2011-443431.html
[Dr Web]: http://news.drweb.com/show/?i=2341
