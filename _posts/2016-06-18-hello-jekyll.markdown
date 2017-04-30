---
layout: post
title:  "Hello Jekyll"
date:   2016-06-18 00:00:00 +0000
category: general
comments: true
---
The first thing I thought of when I first heard Jekyll was jelly - because it's instinct. I knew it was related to technology, but I still thought of Jelly. I don't know why - I was just told by some friends about how it was a useful static-site generator for blogs, and worked especially well with ones hosted on GitHub pages. I had no interest in blogging at that time, so I didn't take much interest. 
<br>
<br>
*A few months later*...
<br>
<br>
I got into blogging. I decided to develop my own blog - but back then, I had only just started HTML. I was always an object-orientated programmer - my "coding arsenal" includes programming languages such as The 3 Cs (C, C++, C#), Java, JS, Python - in addition to markup and styling languages. So when I wanted to make my blog - I didn't have the skills required to use Jekyll, so I decided to use Blogger.
{% highlight js linenos %}
if (!bloggerIsCool) {
  while (true) {
    alert("baaad");
  }
}
{% endhighlight %}
Blogger. It was once the world's largest blogging platform for, well, blogging. Creative name? Check - must've taken forever. Fully customizable? Check. I wish. Don't take me wrong - I love a lot of what Google makes. Search? Obviously. Gmail? Pretty neat. Android & Play - Who doesn't? Now, I attempted to use as much HTML I knew in my first blog. It went well. Until it kept adding back junk such as comments, scripts and other stuff I didn't need. Useless code was being forced upon my blog - and very soon, I didn't feel like blogging.
<br>
<br>
For a long time, I didn't blog. I was bored of it, had many other commitments -  I knew where my priorities were - thus, I had a hiatus on coding as well. However, Half-term then flew by that was when I had a LOT of free time. So then it clicked - By then, my HTML & CSS skills had advanced by a good amount, so that got me thinking - should I give Jekyll a shot?
<br>
<br>
For some of my free time during the one week holiday, I got out my laptop, setup Ruby, Bundler, the required Gems - and Jekyll was all set. I stated earlier that I like some of Google's work - well, I forgot to mention that I absolutley ADORE Material Design, and had known about mdl (material design lite for websites) for ages - I knew that, if I applied it to my blog, some peope would think of it as too mobile-like - but this was my blog, and I definitley going to add it. After adding it's dependancy html tag to my blog's head - then came the fun part. For about two or three days of the holidays, I coded a good amount around an hour a day before the end of year exams came. Another 2 weeks hiatus.
<br>
<br>
Yesterday, I got out my computer - and finished the PC layout of the blog. I was pretty pleased with myself. Th next day - today - I wrapped up the mobile layout, and then pushed the blog to GitHub. I then proceeded to add my custom domain to it (I didn't really fancy the .github.io subdomain too much - still grateful for it though) and also link it to a CloudFlare certificate. I did have some bits and bobs to fix before fully publishing it live; but one bit after I did that took forever to fix: the favicon. I kept trying different combinations of html tags - but none of them worked - none at all, until when one of them worked (I just contradicted myself)...
{% highlight html linenos %}
<link rel="shortcut icon" type="image/png" href="[[site.url]]/favicon.png">
<!--Note: [ = {-->
{% endhighlight %}
That... worked. It worked everywhere - apart from IE. So I used a png instead, and it worked - but then I found out it didn't work in Firefox. I then 'experimented' a little by removing ```'[[site.url]]'``` - and it... worked. I apologise to all the Firefox users - I just can't be asked to fix it now - but I'm pretty satisifed my blog's done  - even more so due to the fact that on top of the base Jekyll theme *(update: rewrote the blog in Januray 2017 without mdl)*, I coded it. I coded my own blog.