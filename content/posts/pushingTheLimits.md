+++
title="Pushing The Limits"
description="Going beyond what would normally be expected when coding"
date=2024-01-04
authors = ["Mark Rainey"]
[taxonomies]
categories=["life","technology"]
tags=[]
+++

A lot of coding jobs can involve fairly "normal" tasks - create a page, write to and read from a database, add a new field to this screen. These tasks have been done numerous times by numerous developers around the world in different flavours.

<!-- more -->

I came across someone who is absolutely pushing the limits of what is possible with C#. This [article](https://migeel.sk/blog/2024/01/02/building-a-self-contained-game-in-csharp-under-2-kilobytes/) describes how they wrote a simple game in C# and then through a number of more and more obscure approaches managed to get the size of the self contained application from an initial  64MB down to an incredible 2KB. 

I am never likely to need to use many, if any, of the techniques it documents but it is firstly an incredible bit of technical work to show what is possible and secondly a very well written article explaining each step involved and why it was done.

In my first real job after university I was writing Pascal for a system that was used by public libraries all over Europe. The code would be compiled and then blown onto a physical prom pack that would then be slotted into a terminal to run the application. The application we produced had a number of different features and each library not only had their own combination of features but also their own localisation of the text.

This was back in the early 1990s so it was unusual to have to support localisation at the time and it was a nightmare doing the builds and the testing as each was unique.

Anyway, one day they told me they needed to fit a combination of features that were much larger than could fit on the prom pack. The prom pack could handle about 768KB but the code when compiled was about 1300KB. My job was to try and get it to fit.

<img src="/posts/PushingLimits.png" title="Pushing Limits" class="mid-image"></img>

The first step was to replace the original Pascal compiler with a compatible optimising compiler (Stony Brook). This had a whole set of different flags that claimed to produce smaller and/or faster code. Unfortunately some of them, or at least some of the combinations of them, were buggy and would cause crashes. However with a certain amount of trial and error I managed to get it to compile and reduce the size by a chunk.

The next step was to go through the code and find ways to make it compile smaller. I found that the way it handled certain data structures could be tweaked to significantly reduce the code size. Along with a whole set of other changes I was getting closer to the target. I went through over 200k+ lines of code line by line and hand optimised it for speed. 

I got to the point where I was dreaming about it in my sleep.

I got within about 30KB of the target when they decided that actually they didn't need all the features and I could stop optimising the code. I was glad to put that task behind me but also a little disappointed that I didn't quite hit the target.

On a side note, I  found out that the designer of the Pascal language, Niklaus Wirth, passed away this week. His language, Pascal, set the basis for my career.

Back on topic, the distributed ledger platform that we are developing at the moment is another example where it is going beyond the normal. Some of the things we have had to design and implement are definitely not your "run of the mill" code. Pretty much every task is different from every other task and involves working out new ways of doing things.

There are definitely challenges in going beyond the normal - sometimes you don't even know if it is possible - but it is the challenge and the learning that can make things fun.

__Links__

[Building a self-contained game in C# under 2 kilobytes](https://migeel.sk/blog/2024/01/02/building-a-self-contained-game-in-csharp-under-2-kilobytes)
