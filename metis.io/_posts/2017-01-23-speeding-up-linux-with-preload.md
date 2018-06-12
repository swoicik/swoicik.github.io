---
ID: 3615
post_title: Speeding Up Linux With Preload
author: stephen
post_excerpt: ""
layout: post
permalink: >
  https://swoicik.com/2017/speeding-up-linux-with-preload/
published: true
post_date: 2017-01-23 01:45:20
---
I've been a long time Linux user. One of the great things about it, is that I rarely need the latest and greatest hardware. Linux can be as fast or faster than Windows or OSX on older hardware. It helps me save money when buying a new computer and extend the life of my current computer.

One way to do this is using Preload

<script src="https://gist.github.com/swoicik/41dd8af507794d905fdcb6f18106d30c.js"></script>

Preload is a background service for Linux that will monitor what processes and resources you use most often and help load them quicker. For example, almost every time I start up my laptop, I will open the terminal and Firefox. Preload will learn this behavior and add these applications to my memory on startup so they open even faster.

It's a small but very useful Linux trick that doesn't get enough attention. You can find more information about Preload on the <a href="https://sourceforge.net/projects/preload/">SourceForge</a> page.