---
ID: 3481
post_title: Elementary OS
author: stephen
post_excerpt: ""
layout: post
published: true
post_date: 2014-06-06 18:31:23
---
Linux is my preferred desktop operating system. And given the number or great distros available, I test and try out many of different ones. My current, and longest standing set up was <a title="Ubuntu" href="http://www.ubuntu.com/" target="_blank">Ubuntu</a> running a <a title="Gnome 3" href="http://www.gnome.org/gnome-3/" target="_blank">Gnome 3</a> desktop. It was a great set up, very minimal desktop, but wasn't running as fast as I wanted. Ubuntu had a lot of software and packages I didn't want, and Gnome 3 was more graphic intense than it needed to be. I am the type of user that would rather make my software more efficient, than upgrade my hardware.

<!--more-->I was looking for the out-of-box functionality of Ubuntu with the minimalist approach of <a title="Crunchbang" href="http://crunchbang.org/" target="_blank">CrunchBang</a>. I think I found the middle ground with <a href="http://elementaryos.org/" target="_blank">Elementary OS</a>.

I installed the OS via USB using <a href="http://unetbootin.sourceforge.net/" target="_blank">UNetbootin</a>. Installation was easy and fast. After installing I made a few adjustments to get the desktop environment just how I wanted it.

Uninstalled Empathy Internet Messaging through the Software Center.

Removed scrollbar. The default scrollbar is sometimes a pain to use on a laptop. I wanted a tradition set up.

<code>$ sudo apt-get remove scrollbar*</code>

Installed Elementary Tweaks. This allows you to make some refinements not available in the default settings menu.

<code>$ sudo apt-add-repository ppa:versable/elementary-update</code>
<code>$ sudo apt-get update</code>
<code>$ sudo apt-get install elementary-tweaks</code>

Installed Wingpanel Slim

<code>$ sudo apt-get install wingpanel-slim</code>

Install Firefox from Software Center

That's all the post installation changes I've made so far. I'm sure I will be making some more tweaks as I go. It's been a week so far and I'm very happy with the set up and speed improvements.