---
layout: post
title:  "How I built this"
date:   2016-07-09 21:50:32 +0100
categories: general
description: "How I developed this blog, and what I used to do so"
---
aFirst of all, as Jekyll (the static site generator that this blog is powered by) is written in Ruby, I had to install that onto my computer, along with the required "gems" - the libraries that this blog needs. In order to aid me in the latter part - I used the Bundler package manager to install the required Jekyll dependencies. I then generate a "generic" Jekyll blog locally, I had to create a Gemfile in order to 'describe' the required Ruby dependencies that will be used in my blog.

{% highlight ruby  %}
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
gem 'nokogiri', '~> 1.6.8.rc2'
{% endhighlight  %}
