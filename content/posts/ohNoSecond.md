+++
title="Oh no second"
description="Most experienced people in development have experienced an oh no second at some point in their careers."
date=2023-11-30
authors = ["Mark Rainey"]
[taxonomies]
categories=["work"]
tags=[]
+++

An oh no second is that moment in time when you realise that you have done something potentially catastrophic and your stomach turns to mush with the dread and realisation.

<!-- more -->

One of the most common examples is performing some operation on a production environment when you thought you were on a "lesser" environment; classics include deleting data. If you are fortunate then you will be able to recover the data.

<img src="/posts/OhNoSecond.png" title="Oh no second" class="mid-image"></img><p></p>

I have had it happen to me, however not in the same league as this one ...

This [article](https://www.chrislewicki.com/articles/failurestory) is brilliant and well worth a read. It tells the story of how the author had an oh no second when working on the $500M Mars Rover. I won't spoilt what happens, you need to read it.

I will only say that I particularly like the bit where he explains one of the outcomes of his error:

> And I still remember the shock when Project Manager Pete delivered the decision and the follow-on news: ‘These tests will continue. And Chris will continue to lead them as we have paid for his education. He’s the last person on Earth who would make this mistake again.’

There is definitely some truth to that. 

We had an incident recently where a bunch of things conspired together to break a non-production environment right before a demo to a potential customer. It would have been very easy to look for people to blame however that rarely has a good conclusion.

The team had a post-mortem meeting and then we had a subsequent meeting to agree how things would be changed to ensure it didn't happen again. I explained to the team that we were not looking to assign blame - in fact I am happy to take all the blame but we need to work out how to reduce the risk of it happening again. Also if we don't learn from this and it happens again then I would be sharing some of the blame with the relevant people.

At the point of failure, a mistake or an oh no second, is not the time to spread blame. It is the time to work out how to fix it and then to later work out how to prevent it in future.

__Links__

[My $500M Mars Rover Mistake: A Failure Story - Chris Lewicki](https://www.chrislewicki.com/articles/failurestory)
