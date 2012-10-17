---
layout: post
title: Give Up GitHub (sort of)
external-url: 
published: true
comments: false
date: 2012-04-08
tags:
- BitBucket
- Git
- GitHub
- SCM
---

[GitHub][] is an amazing place. There are so many diverse projects hosted there, and it's fantastic to be able to quickly create a repo and share code with the world. I've been a member for just under a year, and in that time I've gone from just downloading other people's projects, to forking and contributing to Open Source projects, to creating my own public and private repositories.

If you're familiar with GitHub and it's pricing plans, you'll know that you can create unlimited public projects with an unlimited number of contributors for free. This is probably one of the reasons why GitHub has become a de facto standard for public projects[^1].

About eight months ago I started working on some personal projects, which I just wasn't prepared to share with the world. I did some due diligence had a look at the various options available to me (including [BitBucket][] and [Beanstalk][]), and made the decision to pay for the GitHub Micro account (at $7 per month). I don't regret that decision, as I think GitHub was definitely the best option at the time.

Things are different now though. In October last year [BitBucket announced][announcement] that they were now going to offer support for Git repositories (prior to that they'd only had a [Mercurial][] offering). This was a pretty big deal for many potential users and they offer a very attractive pricing scheme to sweeten the deal.

With GitHub I was getting 5 private repos and 1 collaborator for $7 per month. With [BitBucket][BB Pricing] I can get unlimited private repos with 5 collaborators for free. I also get tighter integration with Atlassian's [JIRA][], which I use for issue tracking over the GitHub system. At first glance this seems like a no-brainer, except…

## Community

There's only one real problem with BitBucket. It's not GitHub. Don't get me wrong, [it tries very hard to be GitHub][ripoff], but there's one area where GitHub beats the competition hands down - community.

GitHub is home to so many public projects that it's the natural place to fork a project or create a new one. There is no way that I know of to fork/pull request between GitHub and BitBucket. It's also hard to justify moving public repos from GitHub when people who may find them use might not want to fork on a "smaller" site like BitBucket.

As of today, I've imported my private repos into BitBucket, and have downgraded my GitHub account. Anything I want to keep private will now go to BitBucket, and I'm going public only on GitHub. If I want to fork a project I'll do it on GitHub, or if I want to share a repo making it as easy as possible for other people to use, I'll do that on GitHub as well.

I was concerned that some of my private projects wouldn't move to BitBucket cleanly - I have a couple of Xcode projects that utilise Open Source frameworks to provide core functionality. I've already forked these on GitHub and I didn't want to lose that flexibility. Thankfully Git submodules allows me to get the best of both worlds. Even though my parent repos now originate on BitBucket, I was still able to define submodules which are originated on GitHub with no ill effects.

Now, GitHub, please don't announce any pricing plan changes for the next few months so that I can at least get settled in over at BitBucket.


[^1]: That and the fact that forking/pull requests is a great model for controlled collaboration. Oh, and Git has been flavour of the month for SCM for a while now.

[GitHub]: http://github.com/
[BitBucket]: https://bitbucket.org/
[Beanstalk]: http://beanstalkapp.com/
[announcement]: http://blog.bitbucket.org/2011/10/03/bitbucket-now-rocks-git/
[Mercurial]: http://mercurial.selenic.com/
[BB Pricing]: https://bitbucket.org/plans
[JIRA]: http://www.atlassian.com/software/jira/overview
[ripoff]: http://www.pocoo.org/~blackbird/github-vs-bitbucket/bitbucket.html
