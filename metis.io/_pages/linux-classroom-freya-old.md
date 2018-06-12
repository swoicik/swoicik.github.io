---
ID: 3546
post_title: Linux Classroom Freya Old
author: stephen
post_excerpt: ""
layout: page
permalink: >
  https://swoicik.com/linux-classroom-freya-old/
published: true
post_date: 2016-03-05 03:23:15
---
<h3>Introduction</h3>
I started in education technology in 2007, and have since been working on incorporating open source software into the classroom. The end goal being to design a school system/district that runs entirely on open source software.

This project is an attempt to put research and ideas into one place. Providing easy to follow instructions for bringing Linux into the classroom.

Why Linux? I am not advocating Linux as the only solution, but a comparable alternative to Windows and OSX. Linux is open source and free for school to use. The costs associated with proprietary operating system and software can be a barrier for many schools. Open source software can alleviate these financial restrictions, while providing the same technology. I also want students to understand there is more to computers than Apple or Microsoft.

As more educational tools move to online sources, the role of the computer in the classroom has changed. The computer is becoming the gateway to web based learning. Whether the gate is Windows, OSX, Linux, Chromebook, or something else entirely doesn’t matter. They are all accessing the same resources online. Technology is becoming less hardware dependent.

*This is a continual work in progress. Things will be added and updated as I learn. If you have any questions or comments, feel free to <a href="http://woicik.rivikhosting.com/contact/">contact me</a>.
<h3>Choosing A Distro</h3>
The operating system, or distro, I will be using is the debian/ubuntu based <a title="ElementaryOS" href="http://elementary.io/" target="_blank">Elementary OS Freya</a>. I considered using stock <a title="Ubuntu" href="http://www.ubuntu.com/" target="_blank">Ubuntu</a> (the usual recommendation for first time users), but Elementary OS has a  clean look, easy navigation, and isn't loaded with a lot of extras.

A few things I wanted in my distro:

A Software Center - It just makes software easier to manage (install/uninstall). It is by no means a requirements for functionality though.

Debian/Ubuntu Based - This is my personal preference. I know Debian and I am more comfortable working with it. The principles I am laying out can be used across any Linux platform you are comfortable working in.

Guest Account Access - This is what we will use for our student accounts. It utilizes the <a title="LightDM" href="http://en.wikipedia.org/wiki/LightDM" target="_blank">LightDM</a> display manager.
<h3>Installing Elementary OS</h3>
There are lots of tutorials on <a href="https://elementary.io/docs/installation#installation" target="_blank">how to install Linux</a> on any kind of computer, so I won't go into much detail here.

I will mention that you should set up an administrator account during the install process. This will be the main account for managing the computer. This will either be an IT account or a teacher account. Whenever changes are made to the computer or updates need to be done, this is the account you will use. It will need to be password protected from students or guests.
<h3>Setting Up The Desktop</h3>
Once the OS has been installed, you will need to login with the adminstrator account your just created. You should then see the default desktop of Elementary OS.

To start customizing the OS for the classroom, we will remove some of the default applications. I want a desktop that is as clean and free from distractions as possible. *If you have a need for any of these programs, feel free to leave them in.

Open the terminal and run the following commands to remove some of the built in software.

<script src="https://gist.github.com/swoicik/fd7296857a3609fe06f63423522d7a15.js"></script>

With the terminal open, run the following commands to install Chrome. This will be the default browser.
<script src="https://gist.github.com/swoicik/b22071ab40b41205a69b9cfce6668cb0.js"></script>

After Chrome installs, open the program and set it as the default browser.

Open the Software Center to remove the following software.
Remove Empathy Internet Messaging
Remove Keyboard Input Methods
Remove Printing

Set up the Guest Account to login automatically.
<script src="https://gist.github.com/swoicik/79bf5d772249cef0aa6c952109dfd3bf.js"></script>