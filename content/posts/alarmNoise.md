+++
title="Alarms lost in the noise"
date=2023-05-07
authors = ["Mark Rainey"]
[taxonomies]
categories=["life","book","work"]
tags=[]
+++

Adding an alert or alarm for a situation you need to monitor should be a good thing but sometimes, depending on how it is done, it can actually make things worse or at a minimum not work as expected.

<!-- more -->

In the book [Upstream](https://www.amazon.co.uk/Upstream-solve-problems-before-happen-ebook/dp/B07VMVZ9MN) by Dan Heath there is a section about alarms (my emphasis) ...

>Have you ever rolled your eyes when you heard a fire alarm? That’s alarm fatigue, and it’s a critical problem. A group of researchers studied five ICUs (intensive care units), treating 461 patients, for a month in 2013. There were almost 400,000 audible alarms logged in a month, which broke down to 187 audible alarms per bed per day. **When everything is cause for alarm, nothing is cause for alarm**. As we design early-warning systems, we should keep these questions in mind: 
>- Will the warning give us enough time to act effectively? (If not, why bother?) 
>- What rate of false positives can we expect? Our comfort with that level of false positives may, in turn, hinge on the relative cost of handling false positives versus the possibility of missing a real problem.

I had two experiences of alarms during the last week.

We were using an office in a large building in Vienna. Suddenly the fire alarm went off. As we were only using the office for the day we checked whether it was a test or we had to leave the building. It was real so we all evacuated - along with hundreds of other people. 

By the time we were outside the first fire engine had turned up. Within five minutes there were at least another nine appliances present. Fortunately they were able to deal with the situation and we could return after just over an hour. 

This is an example of an alarm that should always be investigated. They are relatively rare and could involve a risk to life or significant damage to property. Yet, our previous experience of fire alarms meant that there was an element of doubt on whether we needed to act on it.

The second experience was at work. We have recently added a new monitoring tool that alerts us if data is missing. This is something that should never happen but if it happens we would like to know about it as quickly as possible.

The tool got deployed to an environment and we noticed that it was generating an alert every few hours saying there was an issue and then a short while later effectively cancelling that by saying everything was okay.

In investigating the cause we identified that it was due to one part of the workflow not reliably generating all the data required by the next step. This meant that sometimes it would not provide everything needed and hence the tool would generate an alert - even though there was no real underlying problem with the system being monitored.

In this instance we were getting frequent alerts of something important but they were wrong. However this meant that we also didn't know when a "real" alert was generated as it was lost in the noise. This made the tool effectively useless as this alert would be missed. In the short term we have disabled the monitoring tool while the issue is fixed.

Alarms are important and useful but there must be a high signal to noise ratio otherwise there is a risk they will be ignored and not achieve their aim.

__Links__

[Upstream: How to solve problems before they happen](https://www.amazon.co.uk/Upstream-solve-problems-before-happen-ebook/dp/B07VMVZ9MN)
