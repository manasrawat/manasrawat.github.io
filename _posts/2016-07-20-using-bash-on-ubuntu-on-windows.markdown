---
layout: post
title:  "Using Bash on Ubuntu on Windows"
date:   2016-07-20 00:00:00 +0000
category: general
description: "The pros and cons of the Windows Subsystem for Linux's unix shell"
comments: true
---
Back in March, starting with Windows Insider Build something-something-something-somthing-something, Microsoft released the Windows Subsystem for Linux, which is, as it's name states, well, a Windows Subsystem for Linux. That name really did a good job of explaining it and also works pretty well, unlike project codenames of some other stuff.. (cough, "Nougat", cough). However long ago it came out, it was only recently that I re-opted back into the Insider Program after leaving it a year ago, to check out this new software.
<br>
<br>
The apt-get package manager was fairly easy-to-use, and this 'native' Bash worked better with Git, Jekyll, Bundler and Ruby than I had ever been able to, with Git Bash. Within a few hours, I had ditched their Windows variations in favour of their Linux ones. I even got rid of Windows programs such as HexChat in favour of the command-line based Irssi. Unlike Cygwin, which recompiles some existing Linux packages to make them runnable on Windows, or VMs, Linux binaries run directly from Windows via WSL - without being recompiled or launched from a virtual environment. Not only is it faster, but it also saves MUCH more space. However, WSL-Bash doesn't come without some downsides.
{% highlight sh linenos %}
bundle exec jekyll build
bundle exec jekyll serve --force_polling
{% endhighlight %}
<br>
Unfortunatley, inotify isn't really supported that well - yet. So this means I have to use the more 'expensive' method of viewing change locally, via forcing polling. Another minor problem is the fact that it's case sensetive - but that doesn't really bother me much. But what does bother me, is the fact I'm unable to access directories of WSL directly - and though via some *ways* I can, I still can't change any WSL-files (changes made to files under the WSL AppData directory aren't reflected) - this limits the ammount to which I can customize apps, ie Irssi notifcations and creating permenant WSL-environmental variables. Oh, and another plus of WSL that I forgot to mention, is running GUI Linux apps via a third-party X Server, with me using Xming. I haven't really required GUI Linux apps *yet*, but it's nice to just have it setup - knowing your PC is now capable of running them.
<br>
<br>
Overall, I'm pretty impressed with what Microsoft and Canonical have managed to put together from the remnants of the failed Windows Bridge for Android, Project Astoria. I look forward to seeing what they'll add to WSL, and how they'll improve it - first of all, though, I hope they enable access to the Linux directories...