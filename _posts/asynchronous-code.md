---
title: Writing asynchronous code nicely
tags: code, node.js, async
layout: post
---

I first became familiar with asynchronous programming when I used [node.js](http://nodejs.org).

> Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.
> -- *<http://nodejs.org>*

At first, I found it strange--it wasn't *natural* for programs to *not* run sequentially and synchronously. As I continued to use node, however, I started to enjoy the benefits of asynchronous programming. I felt like *everything* should be non-blocking and event-driven.

## The Problem
Being able to write non-blocking code without too much effort in more languages and platforms than javascript and node seems like a great idea, except for one problem:

**callbacks.**

Javascript's function syntax lends itself pretty easily to node's callback style:
<script src="https://gist.github.com/AjayMT/4b441a958e5e0aa4d9c6.js"></script>

Although that works, it won't save you from [callback hell](http://callbackhell.com):
<script src="https://gist.github.com/AjayMT/7e8b3aea242fb2a442dc.js"></script>

And with a language like python that doesn't allow inline function declarations (other that `lambda`s, which are very limited), it only gets worse:
<script src="https://gist.github.com/AjayMT/b1cae05a873342858b5c.js"></script>

This isn't the same as javascript's callback hell, but the code is still very hard to read. And when you encounter more complex code (which you probably will since this example was pretty simple) you will begin to really appreciate how *nice* synchronous code looks.

So callbacks start to look bad pretty quickly. How do we write *synchronous-looking* asynchronous code?

## The Solution

**Use promises.**

Promises allow us to write reasonably sync-looking code while still being 100% async:
<script src="https://gist.github.com/AjayMT/98aa9944995908b7b9ba.js"></script>

Now you can write nice-looking readable code without compromising on asynchrony or performance.
