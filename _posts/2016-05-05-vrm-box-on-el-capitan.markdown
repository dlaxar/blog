---
layout: post
title:  "Focusrite VRM Box on El Capitan"
date:   2016-05-05 19:13:27 +0200
categories: posts
---
Many people have struggled with running their Focusrite VRM Box with OS X El Capitan. Here's how I got it working:

- Power down your Mac
- Boot it up and press Cmd+R immediately to boot into Recovery Mode
- In Recovery find Utilities>Terminal and type `csrutil disable` to (temporarily) disable [SIP][sip]
- Reboot your Mac and install the latest drivers from the Focusrite Website
- *Reboot and then stop at this point if you'd like to use the VRM Feature. If you just need an interface continue*
- Power down and boot up pressing Cmd+R
- In Recovery find Utilities>Terminal and type `csrutil enable` to reenable SIP
- Boot up and enjoy

[sip]: https://developer.apple.com/library/mac/documentation/Security/Conceptual/System_Integrity_Protection_Guide/ConfiguringSystemIntegrityProtection/ConfiguringSystemIntegrityProtection.html