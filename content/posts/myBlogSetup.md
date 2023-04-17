+++
title="My Free Blog Setup"
date=2023-04-17
authors = ["Mark Rainey"]
[taxonomies]
categories=["technology","howto"]
tags=[]
+++

I thought it was worth documenting my current setup for this blog. Most of it is automated and it costs me nothing to host it.

<!-- more -->

I use [Zola](https://www.getzola.org/) to generate the site. It is a static website generator that effectively takes markdown documents and a theme and produces the site.

The theme I use is based on [DeepThought](https://www.getzola.org/themes/deepthought) with a few tweaks and customisations. I like this theme as it supports all the features I wanted - such as search, static pages - in a nice clean way.

When I have written a post I test the site using:

> zola serve

And once I am happy with it I build the site with:

> zola build --output-dir docs

I host the site using [Github Pages](<[GitHub Pages](https://pages.github.com)>) so publishing the site is simply a case of submitting the changes - I use [GitHub Desktop](https://desktop.github.com/) as it is very simple.

I have also setup the site to use a free [Cloudflare](https://www.cloudflare.com/en-gb/plans/free/) account to handle the HTTPS and also improve performance.

The latest change I have introduced is to use [Obsidian](https://obsidian.md/) for creating the posts. I have created a draft folder under the posts folder and set Zola to ignore this folder. I can now create posts whenever I want and only have to move them and update the post date to make them visible.

I have a template set for each new post so it simplifies the post creation significantly.

__Links__

[Zola](https://www.getzola.org/)

[DeepThought](https://www.getzola.org/themes/deepthought)

[GitHub Pages](https://pages.github.com)

[GitHub Desktop](https://desktop.github.com/)

[Cloudflare](https://www.cloudflare.com/en-gb/plans/free/)

[Obsidian](https://obsidian.md/)