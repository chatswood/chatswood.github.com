---
layout: post
title: "Working With Drafts in Octopress"
date: 2012-10-20 21:45
comments: false
tags: [Octopress, Blogging]
categories: [Technology]
published: false
---

Having recently moved to an Octopress blog I've been revelling in the geekery of managing my posts from the command line. I was previously using MarsEdit to manage my posting to Tumblr, but that's not as viable an option any more. This is a shame because I like MarsEdit and I especially liked the ability to work with local draft posts, something that Octopress (and the underlying Jekyll framework) does not natively provide.

Judging by a quick Google search on the subject I'm not the only person who has been thinking about this and even the mighty [Brett Terpstra][] recently [posted to App.net][] saying that he'd implemented a "rake draft" option (among other goodies) that stores drafts to an `_drafts` folder. This seems to be an avenue that [other people are going down][Yang Meyer] but I'm not sure about the need for this separation.

Jekyll already offers the facility to mark a post as published using an attribute in the YAML front matter. When `published: false` is specified the post will not be output to the `public` folder as part of the `rake generate` task. It therefore will not be included in a `deploy` operation, which is exactly as we would expect, but makes it harder to see the draft posts in the context of the blog.

Interestingly though, when using the `rake watch` or `rake preview` tasks posts with an attribute of `published: false` *are* included in the generation of posts. When you point your browser to `localhost:4000` (or via a [Pow][] configuration) then you'll see you unpublished posts included as though they were published. For me, this negates the need to create dedicated drafts folder.

There are still failings with this approach: drafts are mixed in with published posts requiring file inspection to manually separate them, and the date given to the post (in both the YAML front matter and the filename) will be the creation date rather than the publishing date.






[Yang Meyer]: http://blog.yangmeyer.de/blog/2012/05/28/octopress-drafts
[posted to App.net]: https://posts.app.net/1076717
[Brett Terpstra]: http://brettterpstra.com/
[Pow]: http://pow.cx