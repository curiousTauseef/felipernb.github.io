---
layout: post
title: Design Patterns can be evil
date: 2013-12-08 23:05:24
categories: hacking software engineering
---

Experience working with good developers can teach you a lot of things, but one that I really appreciate is learning how to be **pragmatic**.

> ### pragmatic
> /pragˈmatɪk/
>
> _adjective_
> 
> 1. dealing with things sensibly and realistically in a way that is based on practical rather than theoretical considerations.

Academic background is great and I probably wouldn't be half the programmer I am now if I hadn't gone to university. But on the other hand there is an _impedance mismatch_ between the academia and the market, where people leave school and start working with a fake sense of _purity_ with their J2EE shaped minds ignoring that there are many things you can only learn hands-on - and that's why there are so many self-taught developers doing great and revolutionary stuff out there by thinking out of the box.

I've been there, I used to know by heart pretty much every pattern from the Gang of Four and tried to use them whenever I had a chance. But one thing I've learned since I left the university and started coding in the **real world** is that the _right thing®_ to do is not always the winning choice. In my opinion, one major example of this _phenomenon_ is JavaScript: _With so many good languages around, how come a "**platypus**" language like JavaScript became the most popular and universal one?_ (I'm just going to leave this here for you to discuss in the comments, or for a future post :))

![](/images/platypus.png)

But back to design patterns: _**they are examples of good and reusable solutions to recurring problems**_. That's a great thing to have, right? How could they possibly be evil?

The problem is not with the design patterns per se, but with the mentality of forcing their usage indiscriminately, as if it was always the right thing to do.

This approach can lead to changing the problems to adapt them to the proposed solutions and not the other way around as it is supposed to be, and it can also lead to over-engineering and unnecessary complexity that will cause frustration in the future.

![](/images/design_patterns.jpg)

In the pragmatic approach, design patterns arise in the code naturally. You've seen them before, you know they exist but you're not explicitly thinking about them while you're implementing a solution. Instead, with your experience they start popping up in your code in a natural and adapted way that fits the problem without being _cumbersome_. You maybe don't even know the name of the pattern you're using and that's OK, but if you know it, it can be useful to document the solution and make it simpler for other developers to know what you're doing without the need to read the whole code, since you're following a pattern.

So I think it's important to know design patterns and get familiar with them - as well as it's good to read other people's code to see how they solve problems in different ways -, but don't try to force their way into your code. Just let things flow and _keep it simple, stupid®_!
