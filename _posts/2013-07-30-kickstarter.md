---
title: Kickstarter - An Experiment With Cocoa Development
tags: code cocoa project
layout: post
---

In case you didn't know, I do most of my work on a Mac (a beautiful 21-inch iMac, for those of you who care), and I appreciate functional, well-designed, useful, and to-the-point apps. So, using a Mac drew me towards Cocoa development, and an aspiration to create a really good Mac app. This eventually led to the creation of Kickstarter, an app that I hope will (someday) be useful to those of you that use OS X.

This blog post will be more about the development experience than the app itself. If you want to know more about Kickstarter, visit its project page [here](http://ajaymt.github.com/Kickstarter).

Creating a Cocoa app was certainly an interesting experience. It took a while for me to get a 'feel' for the framework and how I'm supposed to use it. I knew some Objective-C, so I wasn't completely lost, but I still wasn't very sure *where* my code was supposed to go. After a few days of experimentation, things started to make sense. So, I decided to start working on an app.

After some thinking, I (kind of) knew what my app was going to do -- launch other apps. I realized that, every time I needed to edit a few configuration files, or write some code, I was always launching the same apps (iTerm and Emacs). So I decided that my app would automate this repetitive app-launching process, by letting the user capture 'setups' -- lists of apps to launch, and some shell commands to run. Launching a setup would launch all the apps in the setup, and run the shell commands (with the shell that you choose). This would (hopefully) speed up the process of getting into workflows, and would also let you perform complicated tasks that can only be done through a shell.

After weeks of coding and debugging, I had a very basic first version that I could unleash upon the world. So I did, and discovered a few bugs. I pushed an update, and realized that the self-updating system didn't work. So I pushed a few more updates, and I had a usable app. Of course, I will update it and improve it, but, for now, it works.

Get Kickstarter [here](http://ajaymt.github.com/Kickstarter).
