---
layout: post
title: php-mcrypt on Mountain Lion
external-url: 
published: true
comments: false
date: 2012-07-29
tags:
- Apache
- Mountain Lion
- OS X
- PHP
- homebrew
- mcrypt
permalink: /post/28261274431/php-mcrypt-on-mountain-lion
categories: [Programming]
---

I was having a few PHP problems post-Mountain Lion upgrade. Specifically I couldn't get any sites working that utilised `mcrypt` with PHP.

Executing `php` at the command line told me the following:

> PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/local/Cellar/php53-mcrypt/5.3.13/mcrypt.so' - dlopen(/usr/local/Cellar/php53-mcrypt/5.3.13/mcrypt.so, 9): Library not loaded: /usr/lib/libltdl.7.dylib
>  Referenced from: /usr/local/Cellar/php53-mcrypt/5.3.13/mcrypt.so
>  Reason: image not found in Unknown on line 0

I decided to reinstall Jose Gonzalez' convenient php53-mcrypt formula. Post install, the PHP was able to start up without error and a quick `otool -L` on `mcrypt.so`revealed that it no longer had a dependency on `libltdl.7.dylib`.
