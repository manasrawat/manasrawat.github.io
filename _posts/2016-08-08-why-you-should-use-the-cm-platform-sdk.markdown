---
layout: post
title:  "Why you should use the CM Platform SDK"
date:   2016-08-08 00:00:00 +0000
category: android
description: "Find out why you should be using the CyanogenMod Platform SDK to develop apps"
---
CyanogenMod is the largest Android custom ROM by far - and for many reasons, the best. Smooth (mostly), highly customizable and developer-friendly - it's got all the perks a custom ROM can offer. Something that's not as popular as the ROM itself, but is just as great, is the CyangenMod Platform SDK. It enables you to add to your apps framework level features - whether it's creating quick custom tiles, profiles, alarms via the CM DeskClock - all using a set of useful APIs. Why should you use it? So your apps can take full advantage of the extra functionality available for them to use. In fact, one of my own projects, Quickile, uses the Custom tiles package, to create custom tiles for apps. Here is a quick snippet of some of the Tile-generation part of the code:
{% highlight java linenos %}
CustomTile tile = new CustomTile.Builder(this)
    .setLabel(title)
    .setOnSettingsClickIntent(settings) //A pendingIntent is used for the action
    .setContentDescription("Quickile developed by Manas Rawat (cyource)")
    .setIcon(icon) //Bitmap/+Drawable set
    .setOnClickIntent(pending) //A pendingIntent is used for the action
    .hasSensitiveData(true) //If the tile can be shown in the lock screen or not
    .build();
CMStatusBarManager.getInstance(this).publishTile(id, tile);
{% endhighlight %}
<br>
The full code can be accessed at the <a href="https://github.com/cyource/cyapps_Quickile">github repo</a>. All you need to do to access the SDK's packages is add this line to your /app ```build.gradle```:
{% highlight gradle linenos %}
compile 'org.cyanogenmod:platform.sdk:4.0.1' //Use the latest version, rather than 4.0.1
{% endhighlight %}
<br>
Check out the Platform SDK's offical documentations and official GitHub repository for more information.