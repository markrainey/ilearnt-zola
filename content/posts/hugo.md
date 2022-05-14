+++
title="Getting started with the Hugo static site generator"
date=2018-01-20
[taxonomies]
categories=["technology", "howto"]
tags=[]
+++
This blog is being powered by a static content generator called [Hugo](https://gohugo.io/) and hosted on GitHub Pages. Getting Hugo up and running was relatively easy. Download the relevant version and installation was just copying it to a folder.
<!-- more -->

Once installed, create a new site:

​	`hugo new site mySite`

In the site folder edit the config.toml file to change the baseUrl, the language and the title.

Use git to clone a theme from the [available themes](https://themes.gohugo.io/) to a folder under the themes folder in your site.

A page can be added by typing:

​	`hugo new post/somepost.md`

and then editing the file generated under the content/post folder. You might want to remove the "draft" line".

To test the site, run:

​	`hugo server -t thethemename`

where the _thethemename_ is the name of the theme folder and then go to the url given in the console output.

To build the static content:

​	`hugo -t thethemename --destination=/somefolder`

where _somefolder_ is the name of the folder to build the content to.

This can then be pushed to GitHub.

Side note: You might also want to "*git config core.safecrlf false*" on the github folder to remove some CRLF warnings when pushing on Windows.

__Links__

[Hugo](https://gohugo.io/)

[Available themes](https://themes.gohugo.io/)

