---
layout: post
title:  "Alesis IO 26 and El Capitan"
date:   2016-05-16 20:52:27 +0200
categories: posts
---
Getting your audio interface to live under El Capitan can be quite difficult. Just last week I've struggled to
get my Focusrite VRM Box up & running with El Capitan. Today I've updated my Mac to OS X 10.11.5 and suddenly
my Alesis IO 26 wasn't recognized as audio device. If you have the same issue here's what resolved it for me:

* Power down your mac
* Reboot into recovery and run `csrutil disable` in terminal
* Reboot and install drivers
* Reboot
* Voila

If you've had the drivers installed previously and reenabled SIP afterwards (as I have) disabling SIP fixes the issue.
Unfortunately you need to leave SIP disabled. I'm not too happy about it but I'm afraid that's all I can do
until I buy a new interface.