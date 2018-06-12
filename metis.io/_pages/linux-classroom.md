---
ID: 3590
post_title: Linux Classroom
author: stephen
post_excerpt: ""
layout: page
permalink: https://swoicik.com/linux-classroom/
published: true
post_date: 2016-10-27 00:04:43
---
This tutorial is made specifically for <a href="https://elementary.io/" target="_blank">Elementary OS 0.4 Loki</a>. Many of the concepts will work with any Ubuntu based distro.
<h3>Introduction</h3>
I started in education technology in 2007, and have since been working on incorporating open source software into the classroom. The end goal being to design a school system/district that runs entirely on open source software.

This project is an attempt to put research and ideas into one place. Providing easy to follow instructions for bringing Linux into the classroom.

Why Linux? I am not advocating Linux as the only solution, but a comparable alternative to Windows and OSX. Linux is open source and free for school to use. The costs associated with proprietary operating system and software can be a barrier for many schools. Open source software can alleviate these financial restrictions, while providing the same technology. I also want students to understand there is more to computers than Apple or Microsoft.

As more educational tools move to online sources, the role of the computer in the classroom has changed. The computer is becoming the gateway to web based learning. Whether the gate is Windows, OSX, Linux, Chromebook, or something else entirely doesn’t matter. They are all accessing the same resources online. Technology is becoming less hardware dependent.

*This is a continual work in progress. Things will be added and updated as I learn. If you have any questions or comments, feel free to <a href="http://woicik.rivikhosting.com/contact/">contact me</a>.
<h3>Choosing A Distro</h3>
The operating system, or distro (Linux distribution), I will be using is the Debian/Ubuntu based <a title="ElementaryOS" href="http://elementary.io/" target="_blank">Elementary OS Loki</a>. I considered using stock <a title="Ubuntu" href="http://www.ubuntu.com/" target="_blank">Ubuntu</a> (the usual recommendation for first time users), but Elementary OS has a clean look, easy navigation, and isn't loaded with a lot of extras.

A few things I wanted in the distro:

<strong>A Software Center</strong> - It just makes software easier to manage (install/uninstall). It is by no means a requirements for functionality though.

<strong>Debian/Ubuntu Based</strong> - This is my personal preference. I know Debian and I am more comfortable working with it. The principles I am laying out can be used across any Linux platform you are comfortable working in.

<strong>Guest Account Access</strong> - This is what we will use for our student accounts. It utilizes the <a title="LightDM" href="http://en.wikipedia.org/wiki/LightDM" target="_blank">LightDM</a> display manager.
<h3>Installing Elementary OS</h3>
There are lots of tutorials on <a href="https://elementary.io/docs/installation#installation" target="_blank">how to install Linux</a> on any kind of computer, so I won't go into much detail here.

I will mention that you should set up an administrator account during the install process. This will be the main account for managing the computer. This will either be an IT account or a teacher account (something like <strong>Teacher</strong> or <strong>Admin</strong> will work fine). Whenever changes are made to the computer or updates need to be done, this is the account you will use.

The account will need to be password protected from students and guests. If you need help creating a strong password, refer to <a href="https://xkcd.com/936/" target="_blank">XKCD</a>.
<h3>Setting Up The Desktop</h3>
Once the OS has been installed, you will need to login with the administrator account you created during set up. You should then see the default desktop of Elementary OS.

<img class="alignnone size-large wp-image-3595" src="http://swoicik.com/files/2016/10/Elementary-OS-Loki-Desktop-1024x640.png" alt="elementary-os-loki-desktop" width="660" height="413" />

To start customizing the OS for use in a classroom, we will remove some of the default applications. the desktop should be as clean and free from distractions as possible. *If you have a need for any of these programs, feel free to leave them in.

The previous versions of Elementary OS required some work in the terminal to complete this task, but since the release of Loki, an AppCenter has been added. Click the AppCenter icon at the bottom of the screen (blue with a down arrow).

<img class="alignnone wp-image-3592 size-large" src="http://swoicik.com/files/2016/10/AppCenter-Screenshot-1024x616.png" alt="The AppCenter homepage" width="660" height="397" />

After the AppCenter opens, click on the Updates tab. This will give you a list of all the software currently installed on the computer.

<img class="alignnone size-large wp-image-3594" src="http://swoicik.com/files/2016/10/AppCenter-Screenshot-Updates-1024x616.png" alt="appcenter-screenshot-updates" width="660" height="397" />

To remove the software, simply click on the software you wish to remove and hit Uninstall on the next page.

<img class="alignnone size-large wp-image-3593" src="http://swoicik.com/files/2016/10/AppCenter-Screenshot-Unistall-Web-1024x616.png" alt="appcenter-screenshot-unistall-web" width="660" height="397" />

A list of the software that will be uninstalled: Mail, Music, Photos, Web, Videos, Printers, and Calendar.

Next we will need to install some software. Go back to the main page of the AppCenter. You can use the search functionality to find the software or click through the categories.

Install: Chrome and LibreOffice.
<h3>Setting Up Student Access</h3>
Next we are going to use the LightDM funtionality built into Elementary OS to set up a student workspace and have it automatically login when the computer boots up.

This bit will take some work in the terminal. If you are uncomfortable using the terminal ask someone for assistance.

The first command is to access the LightDM configuration file. The second command is the text that needs to be added to the configuration file.

<script src="https://gist.github.com/swoicik/79bf5d772249cef0aa6c952109dfd3bf.js"></script>

<img class="alignnone size-large wp-image-3601" src="http://swoicik.com/files/2016/10/Elementary-OS-Terminal-LightDM-1-1024x640.png" alt="elementary-os-terminal-lightdm-1" width="660" height="413" />

<img class="alignnone wp-image-3602 size-large" src="http://swoicik.com/files/2016/10/Elementary-OS-Terminal-LightDM-Nano-1024x640.png" alt="elementary-os-terminal-lightdm-nano" width="660" height="413" />

After the text has been added to the configuration file. Save the file, exit the terminal, and restart the computer. After the computer boots up it should log directly into a guest desktop and prompt the user with this message.

<img class="alignnone size-large wp-image-3596" src="http://swoicik.com/files/2016/10/Student-Login-Screenshot-1024x640.png" alt="student-login-screenshot" width="660" height="413" />

This desktop is to be used by the student. There is no password to access the desktop and nothing will be saved. This means the student will need to save all of their work either on a thumb drive, network drive, or some other storage option.

The advantage is that every time the guest desktop is logged out, all changes are removed and reset to the original settings. Students will be unable to make permanent changes to the computer. This will also help prevent viruses or malware being installed on the computer.