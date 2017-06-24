---
layout: post
title:  "Auto-clearing Chromium data with Tasker"
date:   2017-06-24 00:00:00 +0000
category: android
comments: true
---
One of the many perks of using Brave as your PC browser is that there's an option to clear specific data upon exiting the application. Unfortunately, the Android counterpart and other Chromium-based browsers lack this feature - something they desparately require, given how many mobile devices are tight on storage. Fortunately, I was able to modify a StackExchange answer into a seamless solution. Well, provided your device is rooted. And has Tasker (though another automation app should suffice).

* *(Optional)* In Tasker's monitoring preferences, I unchecked 'Run In Foreground' and 'Show Notification Icon' - and the Task still ran perfectly.

1. On Tasker, create a new **Application Profile** with only your Chromium-based browser selected; press the toolbar back button to save.

2. Subsequently create a new Task, and then add a Code -> Run Shell action.

3. *(For History)* Type:{% highlight shell %}rm -f /data/data/com.browser.name/app_chrome/Default/History{% endhighlight %}in the 'Command' field. To clear other types of data, enter their respective path instead.

4. Select 'Use Root'; press the toolbar back button to save.

And there you have it. When you switch between apps and leave Brave open - the data will still be saved; but when you remove it from recents and relaunch - it's all gone, thus saving your device a good amount of space.