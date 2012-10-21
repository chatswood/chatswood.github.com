---
layout: post
title: Working With Drafts in Octopress
date: 2012-10-21 18:03
comments: false
tags:
- Octopress
- Blogging
categories:
- Technology
published: true
---

Having recently moved to an Octopress blog I've been revelling in the geekery of managing my posts from the command line. I was previously using [MarsEdit][] to manage my posting to Tumblr, but that's not as viable an option any more. This is a shame because I like MarsEdit and I especially liked the ability to work with local draft posts, something that Octopress (and the underlying Jekyll framework) does not natively provide.

Judging by a quick Google search on the subject I'm not the only person who has been thinking about this. Even the mighty [Brett Terpstra][] recently [posted to App.net][] saying that he'd implemented a `rake draft` option (among other goodies) that stores drafts to a `_drafts` folder. This seems to be an avenue that [other people are going down][Yang Meyer] but I'm not sure about the need for this separation.

Jekyll already offers the facility to mark a post as published using an attribute in the YAML front matter. When `published: false` is specified the post will not be output to the `public` folder as part of the `rake generate` task. It therefore will not be included in a `deploy` operation, which is exactly as we would expect, but makes it harder to see the draft posts in the context of the blog.

Interestingly though when using the `rake watch` or `rake preview` tasks, posts with an attribute of `published: false` *are* included in the generation of posts. When you point your browser to `localhost:4000` (or via a [Pow][] configuration) then you'll see your unpublished posts included as though they were published. For me, this negates the need to create a dedicated drafts folder.

There are still failings with this approach: drafts are mixed in with published posts requiring file inspection to manually separate them, and the date given to the post (crucially updating both the YAML front matter and the filename) will be the creation date rather than the publishing date.

To facilitate this workflow I updated the Rakefile to include a few more default YAML attributes for a new post (defaulting `published` to `false`). Most importantly it includes a Rake task called `publish_draft` that lists all the posts with a `published` status of `false` and allows the user to select a post. The post can then be published using the current date (updating the YAML and the filename) or it can simply be published with the original date. You can find this Rake task in the Gist below - please take care as it has not been made 100% foolproof that this stage.

{% gist 3927558 %}





[MarsEdit]: http://www.red-sweater.com/marsedit
[Yang Meyer]: http://blog.yangmeyer.de/blog/2012/05/28/octopress-drafts
[posted to App.net]: https://posts.app.net/1076717
[Brett Terpstra]: http://brettterpstra.com/
[Pow]: http://pow.cx
