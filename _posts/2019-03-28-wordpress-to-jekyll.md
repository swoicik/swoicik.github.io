---
title: Jekyll & GitHub Pages
author: stephen
layout: post
published: true
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

I started with picking a theme to use. I complied a list of some themes I looked at [here](https://github.com/swoicik/Jekyll-Resources). Ultimately I chose the [Tale Theme](https://github.com/chesterhow/tale) because of its simplicity and having experience using it in the past.  

I set up a repository called swoicik.github.io and did the initial commit with the default Tale Theme. I updated the config file and started editing the css to build the site you are using now. In a week or so I will release the full code for this website as its own Jekyll Theme (need to clean it up a bit). 

Most of the theme editing was done right in GitHub. I just refreshed swoicik.github.io in the browser to see the changes. It's not the cleanest method, but it worked. I wanted to make the theme very simple, but still have the functionality I had on WordPress. The only difficult part (that just means I needed to look up some code) was adding the [archive page](/archive). 

**Content Migration**

I set up a separate private repository for the content migration. I figured a complete dump of all the content from WordPress would be a mess. I didn't want to add useless or unrelated files to my clean theme repository I just completed. 

I used this great plugin, [WordPress to Jekyll Exporter](https://github.com/benbalter/wordpress-to-jekyll-exporter), to migrate all posts and pages from WordPress to a format Jekyll can handle. The plugin dumped the content to the repository in a folder structure that Jekyll uses.

I then went through the content to check the export and clean up any code. Most everything went as planned. I found some of the newer WordPress content that was written with Gutenberg had a lot of extra html tags and comments. I cleaned these up as I went through. 

I deleted the old content that was no longer needed. Burried pages, post drafts, and pending review posts mostly. I wanted a clean start with the new Jekyll site.

Once the content was ready, I copied and pasted the _posts and _pages directories to the swoicik.github.io repository. Waited for everything to updated and started testing out the site with live content. 

## The Result of All This Work? 

Before I migrated I knew Jekyll would provide the writing experience and post updating style I wanted. I didn’t need to check if this worked, I knew it would. 

One things I did want to make sure was speed of the site. I had felt that my WordPress was loading slower. And Jekyll is prompted as being much faster (static content vs dynamic). 

I used [Pingdom](https://tools.pingdom.com) to test the site before and after the migrations. 

Wordpress Test Results
| Performance   | Load Time | Page Size | Requests  |
| ---           | ---       | ---       | ---       |
| C - 76        | 1.26 s    | 1.9 MB    | 112       |

Here is a screenshot of the results from the WordPress site. 
![WordPress Speed Test](/assets/img/wordpress-speed-test.png)

Here is a screenshot of the result from the Jeyll site. 
![Jekyll Speed Test](/assets/img/jekyll-speed-test.png)

Jekyll Test Results
| Performance   | Load Time | Page Size | Requests  |
| ---           | ---       | ---       | ---       |
| A - 93        | 177 ms    | 49.0 KB   | 8         |

I think the numbers speak for themselves, but the site also feels much faster. It loads quicker on my phone or tablet and is easier to use. 

## Not All Perfect

It can’t all be perfect. There are a few features I lost in the migration. Some of them I will be adding back in later, some of them are just going away. They a things you should be aware of if you plan on making this same migration. 

**Categories and Tags**

I no longer have my posts organized by categories and tags. It was more effort than it was worth to get this working with my Jekyll theme. It was also a function that was barely used by my end users on WordPress. I may add as implied version back in at a later time. 

**Search**

The Jekyll site no longer has search built in. I’ll need to come up with a solution to fix this. 

**Contact Form**

Jekyll is a static site. I can’t have a built in contact form as I did on WordPress. There are third party options available to embed a form. I hav opted to just exclude it for now. 

**RSS**

My new site doesn’t have an RSS feed right now. I’ll need to add that back in later. I still rely pretty heavily on RSS from other websites. I should provide the same functionality on my site. 

**Comments**

No more comments on Jekyll. Much like the contact form, you can use an embed option if you wanted, but I don’t. I removed comments entirely. I added a message at the end of each post to either contact me on [twitter](https://twitter.com/swoicik) or email me to discuss anything. 

That’s everything. I hope you found something useful in it. I’m happy overall with the migration process and the new site. I’m sure I’ll have more updates, let me know if there is anything specific you’d like the to discuss. 



