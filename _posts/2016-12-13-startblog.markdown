---
bg: "tools.jpg"
layout: post
title:  "You Don't Know JS: startblog & Beyond"
crawlertitle: "About startblog"
summary: "What's new in startblog"
date:   2016-12-13 20:09:48 +0700
categories: posts
tags: ['startblog']
author: redVi
---
연습으로 만든것 테스트 한것 가장 많이 사용되는 레이아웃 같은데 잘되야 되지 않을까 ?

Before you dive into this book, you should have a solid working proficiency over JavaScript up to the most recent standard (at the time of this writing), which is commonly called ES5 (technically ES 5.1). Here, we plan to talk squarely about the upcoming startblog, as well as cast our vision beyond to understand how JS will evolve moving forward.

If you are still looking for confidence with JavaScript, I highly recommend you read the other titles in this series first:

Up & Going: Are you new to programming and JS? This is the roadmap you need to consult as you start your learning journey.

- Up & Going
- Scope & Closures
- this & Object Prototypes
- Types & Grammar
- Async & Performance

[![railroad]({{ site.images }}/rails.jpg)]({{ site.images }}/rails.jpg)

If you've already read all those titles and you feel pretty comfortable with the topics they cover, it's time we dive into the evolution of JS to explore all the changes coming not only soon but farther over the horizon.

## `let` Declarations

However, we can now create declarations that are bound to any block, called (unsurprisingly) *block scoping*. This means all we need is a pair of `{ .. }` to create a scope. Instead of using var, which always declares variables attached to the enclosing function (or global, if top level) scope, use `let`:

{% highlight js %}
var a = 2;

{
    let a = 3;
    console.log( a );   // 3
}

console.log( a );       // 2
{% endhighlight %}
