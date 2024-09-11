---
layout: single
title:  "Formatting the Blog"
date:   2024-09-01 23:27:31 -0500
categories: jekyll update
author: AliasJeer
header:
    image: /assets/images/jekyllrb-screenshot.png
    teaser: /assets/images/jekyllrb-screenshot.png
---
After installing Jekyll I started learning my way around the structure of the blog. Jekll is a site builder that uses Ruby to parse through partial html files and yaml configs and assemble webpages based on componenets. This allows modular formats to be used with pre-made styles. I followed the guide here to install jekyll locally and created a github repo to connect it. I will be using Github Pages and since this is my portfolio it will be hosted at aliasjeer.github.io.

To install Jekyll, first make sure you have ruby and all needed dependencies. You can follow the guide that applies to your setup here:

<a href="https://jekyllrb.com/docs/installation/#requirements" target="_blank"> Jekyll Requirements</a>

Once complete, use the following commands to install jekyll and create the site foundation:

`gem install bundler jekyll` #Install the jekyll gem package

`jekyll new SITE-TITLE-HERE` #Run the jekyll creator to make a new site base

Now navigate to directory that was just created. You will see some directories and files here. Before going any further, you can load up the site by running:

`bundle exec jekyll serve --livereload` #The livereload is optional but convenient

Then visit your site by navigating to http://127.0.0.1:4000/

Open up your index.md file in your favorite text editor or IDE and make a change. Then navigate back to your local host and refresh to see the changes. One of the best things about using jekyll is that you can quickly iterate and write posts, preview them locally with no risk to your live site, and then push changes to publish on your github pages profile site.

I may write a post in the future about how to connect the jekyll site wth github.

For a guide on generating a new post from the terminal, you can <a href="https://limemangler.github.io/2024/09/10/testing-post-from-terminal-and-editing-using-obsidian.html" target="_blank">check out limemangler's post here</a>

The rest of the steps you take will depend on what kind of site you're hoping to build. You can choose on a theme and follow their guide to install it.

This process will vary, but in most cases you can load the theme and then further customize using a CSS override file. Again, you will want to consult your theme's documentation. I am using the <a href="https://github.com/mmistakes/minimal-mistakes" target="_blank">minimal-mistakes theme which you can find here.</a> Once you have a theme, you can customize, publish, add new pages, etc. The main thing is to make it your own and have fun with it. 