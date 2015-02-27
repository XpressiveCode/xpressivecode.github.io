---
layout: post
title: "Better Growl Notifications"
description: ""
category:
tags: [OSX,Growl,TDD]
---
{% include JB/setup %}
## TL;DR
- Do not install terminal-notifier
- Install <a href="http://growl.info/purchase#AppStore" target="_blank">growl</a>
- Install <a href="http://growl.info/downloads#generaldownloads" target="_blank">growlnotify</a>
<!--more-->
Now when growl is called from an application like mocha, it will use the growl notification system instead of the notification center. Your icons will show up as expected, and you can key off of visual cues instead of having to read the test results.

Keep in mind, that going the traditional growl route costs money. Using the terminal-notifier doesn't. But the cheap cost of growl is worth it to me, as I find the visual cue better/faster for TDD.

## POST
<p>
	I have been doing more and more work lately on OSX for a few clients. One thing that I wanted to achieve was to have better feedback from my tests on whether they passed or failed. I find it important to have rapid feedback while doing TDD, as the sooner you correct the last error, the sooner you move onto the next.
</p>
<p>
	I heard mention of growl notifcations before. However, with the latest OSX update, we have access to the notification center. I have to say, I'm not a huge fan, at least not while doing TDD.
</p>
<p>
	I would rather be able to key off visual cues, then read whether or not my tests passed or failed. Unfortunately, the notification center doesn't allow you (at least at this moment) to override the application icon. So if you're running your tests in a terminal window and they make a call out to show a notification, it's going to use the terminal windows app icon. That means, I would be left with having to read whether my tests passed or failed.
</p>
<p>
	Alternatively, if you leverage growl notifications, you get a green checkmark or red x. The visual cue is much faster and easier for you to glance at.
</p>
