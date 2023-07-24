+++
title="Advice, warnings and genetic algorithms"
description="All advice has an implicit warning and this has the same issues as genetic algorithms"
date=2023-07-20
authors = ["Mark Rainey"]
[taxonomies]
categories=["life","podcast"]
tags=[]
+++

In the Knowledge Project [podcast](https://fs.blog/knowledge-project-podcast/adam-robinson-2/) with Adam Robinson there is an interesting observation about warnings.

<!-- more -->

> Human beings always ignore warnings.

It was stated in reference to a book that he had written for Warren Buffet. He shares a load of advice but some of them come with a warning. He states that most people when reading this would ignore the fact that there are warnings associated with them and take them as the truth.

He then goes on to make a very interesting observation:
 
> All advice is a warning. All wisdom is a warning. If I say the best way to boil an egg is this, there's an implicit warning. If you don't boil it like that, the egg is not going to be as good as it could have been. If I say the best way to negotiate a contract is to always let them make the first offer. There's a warning.

It is not something I'd thought about before. When we receive advice we have a choice to take it or not. If we don't take it there is a risk that we are throwing away an opportunity to lean on someone else's knowledge and experience. However we might also be missing an opportunity to learn and find out the best way ourselves.

It is similar to the problem of local maxima with genetic algorithms. A genetic algorithm generates a result and evaluates it compared to previous results. If it is the "best" result then that becomes the next starting point. However this can create a problem called local maxima. It does not always find the best result and can get stuck at a lower point.

If you imagine a map grid where the height of every point reflects how good the result is. If you pick a starting point you can then look at all the squares next to you and move to the highest one. Using this approach you can navigate the map and will eventually end up at the top of a hill. The problem comes in that you will not move from the top of that hill as no squares around are higher. However this may not be the highest hill on the map - this is called a local maxima. 

The way they solve this with genetic algorithms is through mutations - in our example this would be deciding to head off in a new direction even though it might not be the highest point.

Coming back to the advice and warnings, if everyone always takes a piece of advice and heeds the implicit warning then we could potentially get stuck at a local maxima - we wouldn't know if there is a better way to do things. If we always ignore the advice then we might find a better way or we may find a much worse way. 

*Sometimes* we may want to ignore advice and just try things. We need to take into account the risks and the impact of being wrong. The advice to not touch a hot stove should probably be followed however the advice on the best way to learn to juggle can probably be safely ignored (although it may take you longer).

__Links__

[Adam Robinson #168](https://fs.blog/knowledge-project-podcast/adam-robinson-2)