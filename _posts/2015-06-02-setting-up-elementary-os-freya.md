---
ID: 3515
post_title: Setting Up Elementary OS Freya
author: stephen
post_excerpt: ""
layout: post
published: true
post_date: 2015-06-02 17:27:01
---
I  upgraded my laptop to Freya, the latest version of Elementary OS, and wanted to go over the changes I made to customize my setup. You can grab the download from the Elementary OS <a href="http://elementary.io" target="_blank">website</a>. If you need help installing it, there are a number of tutorials online.

<!--more-->After booting up the computer for the first time, it's a good idea to run any updates before making changes. Open the terminal and run;

<code>$ sudo apt-get update</code>

<code>$ sudo apt-get upgrade</code>

Next, I install Firefox and uninstall Midori. Although Midori is a good browser, I am more comfortable in Firefox and have a number of add-ons I like using.

<code>$ sudo apt-get install firefox</code>

<code>$ sudo apt-get remove midori*</code>

Install Elementary Tweaks for Freya. If you used Luna, you are probably familiar with Elementary Tweaks. A nice little program that lets you make some visual changes to the desktop. In Freya, the program has been completely re-done and improved, so you'll need to add a new repository and install.

<code>$ sudo add-apt-repository ppa:mpstark/elementary-tweaks-daily
$ sudo apt-get update
$ sudo apt-get install elementary-tweaks</code>

Once Elementary Tweaks is installed. Go to Settings -&gt; Tweaks.

Under Appearance, I  turned on Prefer Dark Theme.

Under Plank, I changed Icon Size to 42, hide mode to Auto hide, theme to transparent, and position to Left.

I liked the wallpaper I had on my old Luna installation, so I just re-installed them in Freya.
<code>
$ sudo apt-get install elementary-wallpaper-extra</code>

Sublime Text 3 is my go-to text editor and where most my work is done. It's a must on any machine. There isn't an official PPA, but the always helpful <a href="http://www.webupd8.org/" target="_blank">Web Updt8 Team</a> has a solution.

<code>$ sudo add-apt-repository ppa:webupd8team/sublime-text-3
$ sudo apt-get update
$ sudo apt-get install sublime-text-installer</code>

Now for my graphics program. I have come to really like Krita.

<code>$ sudo apt-get install krita</code>

Lastly I wanted to include a couple keyboard shortcuts I use constantly.

Super + Space - Open the Application menu and lets you search for a program to launch.

Super + S - Opens the desktop and window switcher

One thing still missing, Wing-Panel-Slim. I used this on Elementary OS Luna. It made it possible to customize the top bar on the desktop. It's not a huge concern, but a little tweak that made the desktop just a little more customized.

If you have anything to add to this initial setup, let me know in the comments.