---
layout    : post
categories: [blog]
date      : 2014-06-18 14:43:00
title     : "The value of code quality"
author    : "Frank Sons"
---
[1]: http://blog.innogames.com/
[2]: http://c2.com/cgi/wiki?CodeForTheMaintainer


(I published a first version of this on the [InnoGames Inside blog][1])

Before I can talk about the value of code quality, I should define what I mean with code quality. Usually a user or player only sees the result of a game or product. He will notice good and bad quality in the User Interface or in the game mechanics, but these may or may not be the result of bad code quality. Defining bad code / quality by itself is not an easy task, as code may look fine to one developer, while another one may think it is really, really bad.

<!--more-->

Why? Well, this has a lot to do with experience and personal preferences. Most developers have experienced fights about coding style guides (e.g. tabs vs. spaces), but this is just the top. Some developers like a big object-oriented architecture, while others prefer functional or even procedural architectures. So let's try to just define code quality from my point of view:

* **Understandable**: It should be easy to read and to understand by other developers
* **Testable**: It should be possible - and easy - to write unit tests for the code
* **Maintainable**: It should be easy to fix bugs in the code (usually related to all other points)
* **Flexible**: It should be possible and easy (not too hard) to add new features later on

Sounds easy, right? Well, I can go on and try to define all these terms in more detail and talk about SOLID principles and other clean code practices, but I want to focus on the value of the code quality. One problem for code quality in general is, that it is very hard, if not impossible, to put a real quantified value on it. What are you going to tell your project manager, when he or she asks you about the costs and value calculation of better code quality? As explained before, most non programmers just judge quality by the User Interface - does it look great and does it work? Great! Developers have a gut feeling about bad code, especially if they know they are the ones who will have to fix all the bugs and problems in a few months.

Without being able to put some real value (in terms of money or time) on code quality, how can we describe and understand the value of better code? As I defined code quality, there are two terms that are really important to take into account: maintainability and flexibility. Why are they important? Because these two can differ from project to project. For example think of a website for a special one time only event or raffle. The code will be created only for this specific tasks. Typically it will only be online for a short amount of time. On the other hand, take our browser games. Tribal Wars is more than 10 years old, our other games are online for multiple years as well, and all of them are still getting new features and events.

In the first case maintainability and flexibility don't really matter at all. The code is just there for this specific tasks. It will - hopefully! - not be reused once the event or raffle is over and no new features will be added half a year later. In our second case, for our browser games, we face the complete opposite. Our games will be online for a very long time, there will be new features and we will have to maintain the code. So code quality is much, much more important for any project that will be online for a longer time and/or will have changes after the initial development. My rule of thumb: the longer the estimated lifetime and the higher the chance for new features and changes after release, the more important code quality will be for the project! This is why we always keep an eye on code quality in our games, and why we try to get better with every new game. The real value of code quality will show up a long time after the initial development and will decide how easy and fast it will then be to make changes to the game.

But just in case you want to completely skip code quality for a smaller project: Always keep in mind that throw away code very often ends up not being thrown away. I've seen code from "specific one time only events with a short lifetime and no changes", that was still being maintained and new features were still added after years. So just to be sure, when you write code as a developer, always [code for the maintainer][2] and remember this old quote: "Always code as if the person who ends up maintaining your code is a violent psychopath who knows where you live." :-)