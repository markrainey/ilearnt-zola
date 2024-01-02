+++
title="Speeding up Windows PC"
description="Some things you can do to make your Windows PC boot more quickly and potentially run faster"
date=2024-01-02
authors = ["Mark Rainey"]
[taxonomies]
categories=["howto","technology"]
tags=[]
+++

My dad is pretty tech-savvy (he was an electronic engineer) however he was having problems with how long it took his Windows PC to become usable.

<!-- more -->

As he has helped me with loads of tasks (mostly DIY) over the years I thought  that the least I could do was try and help him out.

**I have not included detailed instructions on how to do each step as you probably need some knowledge before enabling and disabling applications and services but this post should give some ideas what to look at.**

The first thing we did was to reboot the machine and, as soon as he had logged in, press CTRL+Shift+Escape to bring up Task Manager. This is much quicker that trying to right click on the task bar and open it that way. We sorted it by CPU usage to see the most expensive applications.

Within task manager we looked at the "startup apps" tab to see what was enabled and executing. Some of the applications we saw in there were not needed so we disabled them.

We looked in the registry at:

*HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run*
*HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run*

We removed some applications from here that were not needed as well. We also looked at the scheduled tasks and were able to remove some more from there.

The next step was to look at the Services being run. We disabled the indexing service as well as a service that was used to prioritise network streaming traffic as he had no need for that.

The last step was something I'd come across when running a Dell machine. The Support Assist software is dreadful and can cause slow performance and even random hanging. So we disabled this and he can run it when he needs - instructions for this can be found [here](@/posts/dellFreezing.md).