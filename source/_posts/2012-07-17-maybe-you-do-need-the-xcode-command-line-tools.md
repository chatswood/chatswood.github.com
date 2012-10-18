---
layout: post
title: You *Do* Need The Xcode Command Line Tools
date: 2012-07-17
categories: [Homebrew, Xcode, Command Line Tools, Oliver Drobnik, Cocoanetics, Mac OS X]
comments: false
permalink: /post/27400566838/maybe-you-do-need-the-xcode-command-line-tools
categories: [Development, Apple]
---

Oliver Drobnik over at [Cocoanetics][] wrote a [very detailed guide][guide] on how to get by without the Xcode Command Line Tools package, and how to remove them if you want to save a bit of space. He makes some compelling arguments as to why you don't need them around (tl;dr - they all live inside the Xcode.app package and you can access most of them using the `xcrun` command) but he also missed a very good reason to keep them installed on your system. While Oliver did point out that the tools are needed for *"compiling stuff outside of Xcode… [y]ou know, bare knuckles, command line geekery"*, this completely neglects an extremely useful source of software that you don't need to engage your bare knuckles to take advantage of.

The [Homebrew][] package management system provides third-party UNIX tools to supplement or replace those tools provided by Apple. There is a huge list of available software ranging from simple tools like `wget` to complex software like MySQL. For example, if you wanted to install an up-to-date version of `bash` you just type: `brew install bash`

Homebrew will consult it's formula for brewing `bash`, fetch the source archives, fetch any patches required, compile and install to `/usr/local`. Oh, and it'll also download and compile any dependencies you might need. Considering it has to compile the software you ask it to install, one key toolchain in this system is the Xcode Command Line Tools - without these installed Homebrew won't be able to compile the code it downloads.

So if you use Homebrew and are thinking of getting rid of the Xcode CLTs, then don't. And if you have never used [Homebrew][] and are about to remove the CLTs, then give them a stay of execution, and try out Homebrew instead. You may find it a compelling reason to keep those pesky tools hanging around.

[Cocoanetics]: http://www.cocoanetics.com/
[guide]: http://www.cocoanetics.com/2012/07/you-dont-need-the-xcode-command-line-tools/
[Homebrew]: http://mxcl.github.com/homebrew/