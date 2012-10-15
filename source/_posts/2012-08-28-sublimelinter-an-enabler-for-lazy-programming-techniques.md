---
layout: post
title: SublimeLinter - an Enabler for Lazy Programming Techniques
date: 2012-08-28
categories: [Sublime Text 2, Ruby, Rails, Development, Programming]
comments: off
---

Recently I've been experimenting with *text-editor-du-jour* [Sublime Text 2][] in parallel with coming late to the [Rails][] party. Sublime Text 2 has a great plugin ecosystem that seems to be growing by the day and one plugin (or *package* in ST2 parlance) that I find indispensible is [SublimeLinter][].

As a developer I've always written code in an iterative fashion - write a couple of lines, compile, edit those lines to fix the bugs, compile, write a few more lines, and so on. In my career this has occasionally been problematic, as I've sometimes had to work with unwieldy and inefficient `make`-based build systems that unnecessarily rebuilt large swathes of code instead of a single source file. In recent years I've been spoilt by some excellent IDEs (such as Eclipse/STS and Xcode) that have been kind enough to alert me to syntactical errors before I invest time in a build. 

While playing with [Rails][] I found that I was regularly coming across syntactical errors only when it came to testing out the application. It wasn't the horrible build systems of yore, but it wasn't exactly the convenience of a nice IDE. So I hunted around for a linter that I could integrate with ST2 and quickly came across [SublimeLinter][]. A couple of seconds later (thanks to the ridiculously useful [Package Control][]) and I had it up and running and I was getting lots of notifications about errors in my Ruby code.

Unfortunately I soon realised that I was getting too many errors, to the extent that I was getting errors on perfectly valid code. The code ran fine in my Rails app, but still SublimeLinter was bitching and moaning about it. I had a look around the SublimeLinter documentation, and noticed that they recommended using the full path to the `ruby` executable if using a Ruby interpreter provided by [rvm][]. On OS X this comes down to the fact that the default Ruby is 1.8.7 whereas most people will be using code written against Ruby 1.9.X, which they've usually installed themselves.

Thankfully SublimeLinter makes it easy to customise the Ruby interpreter to use, so if you're having trouble with syntax errors in your Ruby code, just chose the menu item *Sublime Text 2 -> Preferences -> Package Settings -> SublimeLinter -> Settings - User*. This will open up the user preferences file for SublimeLinter and you can enter the following snippet (substituting in your own username of course, and remembering to merge the JSON with any settings you may already have in there):

    {
        "sublimelinter_executable_map": {
            "ruby": "/Users/username/.rvm/rubies/default/bin/ruby"
        }
    }

May you continue to be a lazy, iterative developer like me.



[Sublime Text 2]: http://www.sublimetext.com/2
[Rails]: http://rubyonrails.org/
[SublimeLinter]: https://github.com/SublimeLinter/SublimeLinter
[Package Control]: http://wbond.net/sublime_packages/package_control
[rvm]: http://rvm.io/