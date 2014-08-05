---
layout: post
title:  Taking things for granted
date:   2012-06-06 14:00:00
categories: career hacking "software engineering"
---
During the last two years I have interviewed some candidates for software engineer positions and after analyzing those people I came up with the conclusion that the average programmer knows very little about computers.

![](/images/dog.jpg)

As languages and frameworks evolve, programmers seem to know less about how computers work. Fifty years ago men went to space with less computing power than what we have today in the mobile phones we take in our pockets. In the 70's and early 80's, Atari games developers had to cry tears of blood to make those cool games fit in a 4KB cartridge, run with 128 Bytes of RAM and no VRAM.

Nowadays we have an extremely high level of abstraction that allows programmers to write code almost in human language without taking into consideration what's behind it. As, for example:

* How many Ruby coders think about what it takes to sum two numeric variables with a dynamically typed language where numbers are objects and **+** is not an operator, but a method that can be overwritten even for an specific instance? 

* Or how many Node.js coders know how an operating system scheduler works to make it possible for them to implement those asynchronous I/O thingies?

* How many jQuery coders consider what the browser and its JavaScript engine need to do in order to execute that animation effect he called in a single line of code?

Is it a bad thing? IMHO: **yes and no**. 

You don't need to know the mechanics of your car to drive it, but you will be a better driver and take the best of your car if you know how its engine works.

A high level of abstraction usually boosts programmers productivity, but there is a balance that needs to be measured. Treating programming languages, libraries and frameworks as black boxes won't really help you compare different tools and pick the best one for a given problem. Also, as a software **engineer** you're supposed to understand the _engineering_ of the software you're building and make the best decisions about it based on the analysis you do.

Looking on the bright side we can think that there will always be people working with the nitty-gritties of Computer Science and providing abstractions that make programming accessible for the masses, giving more people the opportunity to code and build web sites with pictures of catz.