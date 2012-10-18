---
layout: post
title: Maplin 500Mb/s Powerline Adapters - A Rambling Review
date: 2012-08-14
comments: false
tags: [WiFi,Powerline,Networking,Airport Extreme,Review]
categories: [Review, Technology]
published: true
permalink: /post/29405190084/maplin-500mb-s-powerline-adapters-a-rambling-review
---

I'm stuck between a rock and a hard place. I have a beautiful home of timberframe construction where every internal wall is a stud wall. What this really means is that every wall is a candidate for being stuffed full of cables. My biggest home-improvement desire is to get every room wired with Gigabit Ethernet, but if possible I'd like to get every type of cable under the sun in there. If it's possible to generate enough heat from those cables to remove the need for central heating then I'll consider that to be a bonus.

The problem is that all those lovely wall cavities are hiding behind plasterboard that my wife does not want me to remove. I'm convinced that I could do it in a surgical manner - in and out with minimal disruption and a nice new shiny coat of paint in every room. She's convinced that I'll leave gaping holes running down the walls that never get patched up, and that the painting won't get beyond the colour-picking stage. She's probably right.

## Enter stage left: 802.11n WiFi

With the *right hardware* 802.11n WiFi could very easily have been the answer to my (or my wife's) prayers. The *theoretical* maximum is 600Mb/s - it's not quite Gigabit Ethernet, but is still capable of delivering a large amount of data quickly. Theoretically. With the right hardware.

At the minute I only have one weak spot in the home network - the link between a Gigabit network upstairs and a Gigabit network downstairs in the office. I invested in the latest Apple Airport Extreme base station that I paired up with a 2nd generation Time Capsule. The Airport Extreme was configured to establish a 5GHz 802.11n network using the wide-band settings.

I had hoped to see a pretty fast link between the two base stations, but unfortunately the data rate reported by the Extreme was just 180Mb/s. Testing the network for "real-world" performance resulted in just 93.43Mb/s (using zPerf as a test tool). This isn't a bad speed, but I do tend to fling a large amount of data around the network. It also gets extremely frustrating to be limited to Fast Ethernet speeds when I know there's a Gigabit network up there just waiting to be saturated.


## Enter stage right: powerline networking adapters

I'd considered powerline adapters in the past, but had always balked at the relatively low speeds they offered. Having discovered just how poor the WiFi connection was I decided that the newer 500Mb/s models might be worth a blast - even at 50% of the theoretical maximum I could still get 2.5 times the performance of the WiFi link. When an offer for [Maplin powerline network adapters][] came up they were hastily purchased. Once received I got to testing, and the results were extremely disappointing.

I know that the 500Mb/s is an ideal scenario and many things will conspire to reduce this figure in the real world. Old wiring, interference from other devices and use of extension cables amongst other factors. Our home is fairly modern, and has wiring that is only 8 years old. I tried to improve things by avoiding extension cables, and plugging directly into the mains sockets at both ends, but to no avail. The best rate I could get was a paltry 53.21Mb/s. WiFi it is then.

Not wanting to return the product without trying to find a use for it, I decided to try using the powerline adapters to connect my ADSL modem/router from downstairs to the upstairs network. We only get 5.5-6Mb/s from our ADSL connection so 50+Mb/s is plenty of bandwidth. Unfortunately since doing so, I noticed regular breaks in the connection from the home network to the ADSL router.

The only new factor there is the powerline adapters, so they've had to come out and are currently on their way back to Maplin. Rather than post them, my kind wife agreed to drop them into the store as she was going to be passing it. She'll probably be away for a few hours at least. Now to find my hammer, some Cat6, and the crimping tool.


[Maplin powerline network adapters]: http://www.maplin.co.uk/500mbps-twin-powerline-starter-kit-626154