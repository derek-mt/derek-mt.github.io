---
title: Drawing the line&colon; Concision vs. Complexity
tags: code, thoughts
layout: post
---

As a coder, I strive to write readable, maintainable code. That often includes ensuring that my code is DRY -- as non-repetitive as it can be. I often end up obsessing over the smallest of details, the tiniest little changes I can make to ensure that it is *nearly impossible* to make my code any more concise.

There is, however, a limit to DRYing out one's code:

> **readability > concision**
>
> *Do not condense your code to the extent that it becomes hard to understand.*

Take a look at, for example, this piece of code (I find it easiest to illustrate my point with Python):
<script src="https://gist.github.com/AjayMT/c3fc571517ed862ba20f.js"></script>

The objective here is quite apparent: to add the 'super rich' tag to anyone who is tagged 'billionaire' in the dictionary 'people'.

Here's another snippet of code that accomplishes exactly the same thing:
<script src="https://gist.github.com/AjayMT/dc0cdf397d16cd5ab254.js"></script>

For someone who doesn't know what it's supposed to do, it'll take a little longer to understand this piece of code than the previous example. It's still pretty simple, but (in my experience) the complexity of code created by unnecessary concision increases nearly exponentially as more code is added.

*Note:* I use the term 'complexity' to describe how easy/hard some code is to understand, not the complexity of the algorithm(s) used.

Basically, the more code you have, the more complexity you will create by condensing it (because it will do more stuff).

However, it's also important to ensure that you're not writing *too much* code: that can also be hard to understand.

It seems like the best way to write code is to condense it only to the point that it is still easy to understand. Once you have achieved that balance between simplicity and concision, you have written *beautiful code*.

But 'beautiful code' is different for everyone because *easy* and *hard* to understand are subjective terms. Thus the question arises:

> How does one distinguish between the two?
>
> **Where does one draw the line?**

Such is the art of programming.

(You could also choose to be like Ryan Dahl and [not give a fuck](https://gist.github.com/cookrn/4015437#file-rant-md).)
