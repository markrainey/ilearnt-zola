+++
title="How to run a planning workshop"
date=2019-03-13
[taxonomies]
categories=["work"]
tags=[]
+++
We have just completed a two week exercise with the whole development team to identify, design and estimate the next phase of work. It started as an organic process as we found the best way to do this and then developed into a repeatable process for the latter functionality.
<!-- more -->

Before starting on the individual breakdowns we produced a list of things to consider for everything we were estimating. This mostly consisted of a list of functional requirements like logging, testing, documentation, etc. as sometimes these can have a significant impact on the work.

The first step was to break down the work into "EPICs". For us these are the deliverables to the business. At the completion of each of these we should be able to demonstrate a significant piece of functionality.

For each of the EPICs we then generated high level user stories and also acceptance criteria at the EPIC level. We set in stone that we could not move on to generating the backlog of tasks and estimates until the whole team agreed on both of these. These could be revisited if needed if the next step revealed any changes were required.

Once these had been agreed we discussed the tasks involved in each of the stories. If the story was small enough we would not break it down any further at this point however we would still agree what would be involved in the implementation and make note of any important points.

For larger stories we broke these down into smaller tasks. In most cases this created three to four tasks.

The next step was estimation. The team decided that they wanted to use story points. To achieve this we went through the process of looking at the work we had done previously and identifying tasks that took a similar amount of work and were differing sizes relatively to the rest. 

We identified three tasks for each of 1, 3 and 8 story points. When we get to estimating these provide a way to compare with what is being estimated and gauge relative size.

For the estimating itself we used a Slack plugin called Pokerbot with Fibonacci story points. This actually worked really well. For each task every developer would use this to vote in secret. We displayed the comparison tasks while voting was done.

At this point we also reminded them to consider the earlier list of things to consider.

Once all the votes had been cast we used the following rules:

- We only accept a vote with adjacent scores (only 1's and 2's, only 5's and 8's, etc.)
- If there are non-adjacent scores, start by asking the small outliers "what work is involved?" Then ask the large outliers "what [other] work is involved"? And then do a revote for the whole team.
- If you have adjacent scores, but 2 or more are the higher number, take the higher number.
- If you have adjacent scores, but only 1 of the higher number, they get to choose between the two numbers.
- For the question mark option: Use it sparingly, but it lets someone ask a question and force a revote
- Infinity: Something's gone wrong. It's the wrong work, or can't be done.

We generated estimates for each task and then summed them to produce estimates for each story.

The last step is to take these and map them to dates for reporting to management. To achieve this we needed to generate an initial velocity value that will obviously change as the project progresses. 

As a one off we did this by estimating in days how long some of the tasks would take and then mapping these to the story points to get the initial value.

The thing that amazed me most was how much the team bought into the process. Admittedly they are all senior level developers but they fully engaged in all the discussions and the process and, hopefully, we have a much clearer view on what we need to do and much better estimates (we'll see soon!).

