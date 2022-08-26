+++
title="Solving a Dell laptop freezing"
date=2022-08-28
[taxonomies]
categories=["howto"]
tags=[]

+++

I have a Dell XPS13 laptop and it developed this really annoying habit of randomly freezing for a few seconds and then carrying on as if nothing had happened. It quite often happened in the middle of a work call which made it pretty much unusable.

<!-- more -->

I checked the Windows event viewer and there was nothing in there that stood out at the time it happened. I trawled the web for a solution but didn't find anything.

I can't remember how I found the solution; it may have been from watching the task manager when it froze, however it turns out it is due to the Dell SupportAssist and related processes. If I turn off these services then I remove all the freezing issues.

I initially just disabled the one service but it would sometimes magically start again - no doubt triggered by another service.

So the solution for me is to open the "services" app. Sort the entries so all the "Dell" services are together and then disable them all. I have seen no side-effects on my machine (your experience may differ I guess). Every few months I run SupportAssist manually to check for updates and the disable them all again.

