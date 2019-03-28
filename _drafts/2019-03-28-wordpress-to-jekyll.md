---
title: Jekyll & GitHub Pages
author: stephen
layout: post
published: false
post_date: 2019-03-28
---
It’s 2019 and I’m moving swoicik.com to Jekyll and GitHub Pages. 

For as long as this website has existed, it has been powered by WordPress. WordPress is an amazing platform, and has been a huge part of my career in web development. But... the platform has grown from its blogging roots into something much larger and complex. It was time to try something new. 

## Leaving WordPress  

**WordPress Baggage**

Over the past few years, WordPress has become a huge and powerful piece of software. It has become overkill for a personal blog. The maintenance required for the site is causing me to write less. I just don’t want to deal with WordPress side of WordPress. I just want to write. 

**Writing Environment**

The writing environment in WordPress has always been a bit cluttered. With the recent Gutenberg update it seems even more so. I don’t have the patience to deal with it, when all I want to publish is a simple text blog post. All the formatting and plugin options are overkill. 

**Mobile Publishing**

Publishing to a Jekyll site from my phone is simple. It’s the same workflow for any other GitHub project I may be working on. I write the post in iA Writer and Git Commit the post with Working Copy. Seconds later the post is live. 

Mobile publishing on WordPress has never been great. At best I can get a draft done in the mobile app before logging in on a desktop to actually publish the post. 

**Theme Editing**

WordPress themes have become more and more complex and harder to edit. Compared to editing a Jekyll theme it’s like night and day. 

## Why Jekyll 

I started my research by looking to other websites I liked. I found a lot of them were powered by Jekyll. Initially I though Jekyll would be too complex. After discovering how easy Jekyll is to run on GitHub Pages, I was sold. 

Jekyll is a platform focused on blog writing and not much else. It also had an active developer community that I could rely on. And the price of free is always helpful. 

**Markdown**

I take almost all of my notes in markdown. The drafts for all of the posts I write are done in markdown. Being able to keep everything in markdown from draft to publish is just easier.l and makes sense. 

**Text Backups**

All my posts live in a plain text directory, and they live on all my devices. There is something great about having everything is a truly portable format. Posts are backed up on GitHub and locally on the devices I have connected to the Git Repository. It’s a very simple and secure set up. 

**Price**

Jekyll is open source and free to use. GitHub Pages is free to use. This entire site is now free to develop and host (side note: I am a GitHub Pro subscriber). 

## How To Migrate to Jekyll 

Now that the reasons are out of the way, how did the actual migration go?

**Respository and Theme Set Up**

I started with picking a theme to use. I complied a list of many of the themes I looked at [here](https://github.com/swoicik/Jekyll-Resources). Ultimately I chose the [Tale Theme](https://github.com/chesterhow/tale) because of its simplicity and having experindce using it in the past.  

I set up a repository called swoicik.github.io and did the initail committ with the Tale Theme. I updated the config file and started editing the css to get the site you are using now. In a week or so I will release the full code for this website as it's own Jekyll Theme, just need to clean it up a bit. 

I did most of the theme editing right in GitHub, and just refreshed swoicik.github.io in the browser to see the changes. It's not the cleanest meathod, but it worked. I wanted to make the theme very simple, but still have the functionality I had on WordPress. The only difficult part (and that just means I need to look up some code) was adding the [archive page](/archive). 

**Content Migration**

I set up a seperate private repository for the content migration. I figured a complete dump of all the content in WordPress could be a mess. I didn't want to add useless or unrelated files to my clean theme respository I just completed. 

I used this great plugin, [WordPress to Jekyll Exporter](https://github.com/benbalter/wordpress-to-jekyll-exporter), to migrate all posts and pages from my WordPress site to a format Jekyll can handle. The plugin dumped the content into my new repository in a folder strucutre that Jekyll can use. 

I then went through the content to see how the export went and clean up any code. Most everything went as planned. I found some of the newer WordPress content that was written with Gutenberg had a lot of extra html tags and comments. I cleaned these up as much as I could. 

I also deleted many of the old content that was no longer needed. Burried pages, post drafts, and pending review posts. I wanted a clean start with the new Jekyll site.

Once the content was ready, I simply copied and pasted the _posts and _pages directories to the swoicik.github.io repository. Waited for everything to udpated and started testing out the site with live content. 

## The Result of All This Work? 

https://tools.pingdom.com

![WordPress Speed Test](/assets/img/wordpress-speed-test.png)

![Jekyll Speed Test](/assets/img/jekyll-speed-test.png)


