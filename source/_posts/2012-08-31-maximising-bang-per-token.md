---
layout: post
title: Maximising Bang Per Token
date: 2012-08-31
comments: false
categories: [Twitter, Tweetbot for Mac, TapBots, Access Tokens]
permalink: /post/30606832645/maximising-bang-per-token
---

The brouhaha over third-party Twitter clients continues with the news of the release of a [beta version][] of Tweetbot for Mac. Just 4 days ago the [alpha version was withdrawn][] with Tapbots citing as a reason the "finite limit on the number of user tokens we can get for Tweetbot for Mac".

This was a fair move by the developers - any Mac user could download the alpha, sign in and obtain a limited Tweetbot for Mac token. If they subsequently decided they were not interested in buying the application they can discard it without releasing the token they use. It was a problem with only one resolution - withdraw the app and preserve the tokens.

Today Tapbots came back with a beta version and some new rules:

* new users can install the beta but they'll not be able to add a Twitter account;
* users of the alpha version can use the same Twitter account they used before;
* users of the alpha version cannot add extra Twitter accounts;
* users of the alpha who revoke their access token on the Twitter site cannot add their account again.

All of this makes perfect sense from the point of view of token preservation. Unfortunately in this [post-announcement][] landscape these once common items are now a scarce resource. They've become the fossil fuels of the technology world, and like fossil fuels they're limited and easily wasted. They used to be very disposable - a quick look at my [Apps section][] on twitter.com lists 34 tokens on one account alone, and that's after a prune earlier this week.

## Efficient Token Usage

Like many people I have a number of Twitter accounts, and on each of my clients I like to have all of my accounts signed in. This was never a problem before but now it just exacerbates the issues faced by app developers. They have a limited number of access tokens that can be used with their apps and users like me with multiple accounts end up using more tokens than other people.

To make an app commercially viable developers need to squeeze as much money per token as possible. One way to do this would be to increase the cost of their apps to cover the average number of accounts per user. Alternatively they could keep the initial purchase price the same while limiting the number of accounts that can be signed in through the app. Power users could then be offered the option to use in-app purchases to effectively buy extra access tokens.

There has been a lot of discussion recently on the devaluing of software through bargain basement prices and this is really going to hit home to Twitter client developers now. Maybe the scarcity of access tokens will encourage users to value the software higher and pay more for it. Remember, you're not just paying for the software anymore - you're also paying for the privilege of connecting to the service through your favourite client.

[beta version]: http://tapbots.com/blog/news/tweetbot-for-mac-beta-sort-of
[alpha version was withdrawn]: http://tapbots.com/news/where-did-the-tweetbot-for-mac-alpha-go
[post-announcement]: https://dev.twitter.com/blog/changes-coming-to-twitter-api
[Apps section]: https://twitter.com/settings/applications