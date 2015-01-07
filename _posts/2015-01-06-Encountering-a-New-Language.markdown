---
layout: post
title:  "Encountering a New Language"
date:   2015-01-06 15:14
categories: blog january
---

Today, I decided to take a good look at the CSS files that compose my blog. Having no prior experiences with CSS, I am subjected to the nuances between languages that I've come to know (mostly object-oriented programming languages) and a language geared towards web development. At this stage of my learning, I can now ask myself "What do I do when I encounter a new language"?

Opening a file called _base.scss, I am left startled by the massive differences between what I knew and some CSS code lying in front of me. Fortunately, they are all in the same 26 letters and 50 or so characters that I've seen and used. I outline here steps I took to begin comprehending what I saw:

<h1>Syntax</h1>

I first look for code that uses syntax I can recognize.

Code such as 
```
/** Reset some basic elements */
```
tell me that what I am reading is a comment even if I do not know what ```/**``` and ```*/``` mean.

When I came across 
```
$spacing-unit / 2
```
I immediately recognized that ```$spacing-unit``` is an integer variable, and thus the register ```$``` character must represent variables. Further analysis led me to a file called main.scss that held most of those variables used in the base.scss file, suggesting that these variables acted as global variables.

These are a few of what I could analyze solely based on prior knowledge of other languages. The ```{``` and ```}``` characters used also helped me to identify bodies of code.

<h1>Changing Values</h1>

I experiment by changing values (integers are easiest to manipulate) one at a time and seeing what effect it has on the code.

Here is some code from _layout.scss:


<pre><code>.site-nav {  
    float: right;  
    line-height: 56px;  
    etc...
</code></pre>

By changing ```56px``` to ```20px``` I notice the position of the "About" shift vertically upwards. Thus, line-height controls vertical positioning. If I change ```right``` to ```left```, the "About" on the top right is repositioned to the top left.

Of course, this works much better when you can visually see the changes take place. I cannot claim to know exactly what ```line-height``` is, but I have a general idea.

<h1>Keyword LookUp</h1>

Most of the time, changes to variables does not visually change the code. Even moreso are code that employ the language's own features.

As an example:

<pre><code>.post-list {
    margin-left: 1;
    list-style: none;

    > li {
        margin-bottom: 1px; //space between the links
    }
}
</code></pre>

At first glance, ```list-style``` isn't as intuitive as it looks. However, a quick search reveals that ```list-style``` controls what form the bullet points will take shape in. At the home page, my posts are bulleted as circles (this may change with time). I used most of my time deciphering some of the smaller code and making comments in the code itself to remind myself what they do.


<br>

I feel like I've written too much for one post so I will end it here. The excitement of learning something new can turn minutes of browsing into hours of analyzing.

Adimwit