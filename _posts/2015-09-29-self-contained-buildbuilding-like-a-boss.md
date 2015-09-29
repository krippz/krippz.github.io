---
layout: post
title: Self-Contained Build...building like a boss
categories: [build]
tags: [cake]
published: True

---

So this past week I've had the plesure of working with a sane build system written in C#.


It's called `cake` a word play on make :) and I really enjoy working with it's DSL.
You can find it here [www.cakebuild.net](http://www.cakebuild.net)


I have written build scripts before and in diffrents languages, but this was the first time I've written any _sane_ C# script. I have written C# as a `MSBuild` task, but that was not so pleasent and for the rest of MSBuild you write xml for your script, but that model is really really *REALLY hard* to understand and write.


With `cake` I've written a _self-contained build_, hmm you say what is that, yet another buzz word online. Well as I understand it's more of a preparation of the repo in such a way that a new dev can perform some simple steps and be off **building** and **debugging** and **developing**.

In my self-contained build I have these steps:

- clone the repo
- run build.sh on Linux and OS X
- run build.ps1 on Windows

Simple right!
And I have a really quick demo :)

![Build Like A Boss](/assets/github-self-contained-build.gif)

You can find the demo here [https://github.com/krippz/build-demo.git](https://github.com/krippz/build-demo.git)