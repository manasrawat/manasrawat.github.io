---
layout: post
title:  "The Magic of Magisk"
date:   2017-07-16 00:00:00 +0000
category: android
comments: true
---
Xposed is a framework for Android that allows modules to be installed, which take customisation to a level beyond that of even custom ROMs, such as RR and CM, and theme engines, such as Substratum and CMTE. However: it modifies system files and isn't yet avaliable for devices running Nougat. Thus, enter **Magisk**.

![](/res/posts/magisk.jpg "Xposed++")

Now... what's Magisk? Magisk is very much like Xposed - but rather than being a system-modifying framework, it's a *systemless* interface that can layer modules over it **without** modifying system files. It also enables systemless rooting, with its own version of SuperUser built-in. Thus, when a new build of a ROM is flashed - the Magisk modules don't need reconfiguring. In fact, it even has modules of Systemless Xposed Frameworks - Xposed can be used within Magisk! 

Magisk does everything Xposed does, but better (systemlessly), and is avaliable for more devices (i.e. those with Nougat too). It comes built in with RR, serving as its root manager - but it can be downloaded for multiple ROMs! To get it, visit the [XDA thread](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445).

