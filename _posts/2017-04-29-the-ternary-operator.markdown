---
layout: post
title:  "The Ternary Operator"
date:   2017-04-29 00:00:00 +0000
category: code
description: "If only I found about it before..."
comments: true
---
If/Else If/Else statements. The code that everyone hates but has to use. Since I started programming, in nearly every single project of mine, I had to use these messy, clunky statements. However, a few weeks ago, I came across something I wish I did a long time ago. Some may call it the conditional operator. Others may refer to it as inline if. But everyone (who uses it anyway - I'm sure many coders do, but the aim of this post is to get more people to) knows it as the "ternary operator".

{% highlight csharp linenos %}
var input = ReadLine().ToLower();
if (input == "hello") {
  WriteLine("Hola");
} else if (input == "hi") {
  WriteLine("Bonjur") {
} else {
  WriteLine("Bye");
}
{% endhighlight %}

Some people probably won't have a problem with that snippet of code initially. But then they'll realise, that there are 132 characters for this simple function - and that's not even counting spaces! Now, let's make it better:

{% highlight csharp linenos %}
var input = ReadLine().ToLower();
WriteLine(input == "hello" ? "Hola" : input == "hi" ? "Bonjur" : "Bye");
{% endhighlight %}

90 characters. Using the tenary operator made this snippet 42 characters smaller. Now, some people may think that smaller code doesn't make it better (it does to some extent, in all honesty) - and they're correct. I agree. What makes coder better isn't quantity - but quality. But we aren't writing an essay here - we're writing code. And in the context of programming - let's face it: quantity makes quality (less quantity -> more quality, that is). Now, this snippet is tiny - but when someone is making a large project - it'll be better for if their code is neater and easier to get around.