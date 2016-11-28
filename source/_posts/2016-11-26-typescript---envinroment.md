---
layout: post
title: "TypeScript - environment setup"
permalink: typescript-environment
date: 2016-11-26 22:49:27
comments: true
description: "TypeScript - environment"
keywords: "typescript environment"
categories:
- typescript

tags:
- typescript
- environment

---
<p>Ok, so You decided to work, learn or just try TypeScript, congratulations. Before You start..
You should know what TypeScript is not understandable by browser, so You need to compile files before.</p>

<h3>WebStorm</h3>

In WebStorm, TypeScript code is transpiled into JavaScript using the built-in TypeScript compiler.
Just open WebStorm | Preferences and fallow the instruction from official site.
<a href="https://www.jetbrains.com/help/webstorm/2016.3/transpiling-typescript-to-javascript.html">WebStorm compiler</a>

<h3>npm</h3>


{% highlight javascript %}
npm install -g typescript
{% endhighlight %}

Then create some ts file, for example first.ts

{% highlight javascript %}
function greeter(person: string) {
    return "Hello, " + person;
}

var user = "Jane User";

document.body.innerHTML = greeter(user);
{% endhighlight %}

Compile the file with npm in console

{% highlight javascript %}
tsc first.ts
{% endhighlight %}

Seems to be working just fine, try changing person: string - > to person: number and lets see what happen.

Ok, enough for now, we are not suppose to learn TS (TypeScript) now just to compile.



