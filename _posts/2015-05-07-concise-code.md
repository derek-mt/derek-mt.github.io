---
title: Drawing the line&colon; Concision vs. Complexity
tags: code, thoughts
layout: post
---

As a programmer, I strive to write readable, maintainable code. That includes ensuring that my code is DRY -- as non-repetitive and concise as it can be. I often end up obsessing over the smallest of details, the tiniest little changes I can make to ensure that it is *nearly impossible* to condense my code any further.

There is, however, a limit to compressing one's code:

> **readability > concision**
>
> *Do not obfuscate code to make it shorter.*

Take a look at this program for example (I find it easiest to illustrate my point with Python):
<script src="https://gist.github.com/AjayMT/c3fc571517ed862ba20f.js"></script>

The objective here is immediately apparent: to add the 'super rich' tag to anyone who is tagged 'billionaire' in the dictionary 'people'.

Here's another script that does exactly the same thing:
<script src="https://gist.github.com/AjayMT/dc0cdf397d16cd5ab254.js"></script>

Unless the person reading this piece of code knows what it's supposed to do, they'll take longer to understand it than the first example. It's still relatively simple, but (in my experience) programs become exponentially more complex the larger they are and the more they are shortened.

The more code there is, the more complexity condensing it will create.

However, it's also important to ensure that you're not writing *too much* code: moderately concise code is simple and easy to read, and too much code can be hard to understand.

It seems like the best way to program is to condense code only to the point that it is still simple and easy to understand. A programmer who has achieved the balance between simplicity and concision has written *beautiful code*.

But 'beautiful code' is different for everyone because 'easy' and 'hard' to understand are subjective terms. Thus the question arises:

> How does one distinguish between complexity and concision?
>
> **Where does one draw the line?**

Such is the art of programming.

(You could also choose to be like Ryan Dahl and [not give a fuck](https://gist.github.com/cookrn/4015437#file-rant-md).)
