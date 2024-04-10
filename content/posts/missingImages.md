+++
title="Missing images"
description="The images on my blog all suddenly disappeared and I didn't know why"
date=2024-04-10
authors = ["Mark Rainey"]
[taxonomies]
categories=["technology"]
tags=[]
+++

I hadn't updated my blog for a while so I thought I would write a short post about [The Keeper Test](/posts/thekeepertest/). That is when all the images suddenly stopped displaying on this blog.

<!-- more -->

I happened to publish to Github Pages, where this is hosted, just as Github threw a wobbly. This meant the site partially built but never deployed. Once Github recovered it kept saying the Action job was queued but it was stuck and would not run again. I found out the solution to this was to make a minor change and commit that to create a new Action and that executed fine.

At the same time I noticed that I was getting a message in Github Desktop that it was changing the line endings for some of the files. So to fix that I changed the line in .gitattributes from 

> \* text=auto

 to

> \* text eol=lf

I republished my site and left it at that. 

A few days later I decided to write another post and noticed that there were no images appearing on the deployed site. I used the developer tools in Chrome  to work out that they were being returned by the server but they looked wrong. 

I went into Github to examine them in the repository and it refused to preview the image files - but they looked fine locally on my machine. Strange.

For my next step I tried to force the images to be resubmitted in case the wobble had caused some form of corruption. I forced all their timestamps to be updated using the DOS command: 

> copy *.png+ /Y

Committing these changes still made no difference.

The only thing I could think to try was to revert the .gitattributes change - maybe it affected image files as well as the markdown files.

And now all the images were uploaded correctly and now they appear again. 

Of course, it was user error on my part.

I should have looked at that change more closely - the asterisk at the beginning means apply it to all files, not just the markdown files. I should have taken a moment to understand the change I was making and not just blindly make the change. I should have specified the .md file extension and potentially excluded .png files.

It is through making mistakes that we learn.
