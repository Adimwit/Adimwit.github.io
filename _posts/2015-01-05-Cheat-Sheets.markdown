---
layout: post
title:  "Cheat Sheets"
date:   2015-01-05 19:00
categories: blog january
---

The internet is an amazing tool powered by search engines to help you find what you need. Today, I used the Google search engine to find out how to "add images in Markdown" (the exact keywords I used) and stumbled upon a Markdown Cheatsheet created by adam-p on github! The post provides a table of contents for just about anything you would stumble upon on a daily basis in Markdown.

Github Cheatsheet link: [Markdown Cheatsheet][cheatsheet]

The first topic that caught my eye wasn't images, it was the topic right below it called "Code and Syntax Highlighting". From the Jekyll  code snippets provided, I can write ruby-code snippets with "% highlight ruby %" which highlight code in this example provided by Jekyll:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}


Or I can write code snippets without the highlighting:

```
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```

I would only use the above code box for 1 line codes as it seems "\n" and any other way that I have tried does not work.

Getting back on track, I found out that there are two ways to add images using Markdown: Inline-style and reference-style. I have a preference for the way my code is structured, so having a reference-style image suits my tastes. It makes it easier to edit code when you know where something is instead of looking for it within the code.

Some code for reference-style images:

```
![refImage][image]
```

Then I can place this code anywhere I want (usually at the bottom):

```
[image] http://cdn.screenrant.com/wp-content/uploads/the-simpsons-renewed-season-24-25.jpg "The image has text!"
```

The outcome?

![refImage][image]

The image has text when you hover over it? GASP!

Well, that's all for today. Much thanks to adam-p for creating this and uploading it!

Adimwit

[image]: http://cdn.screenrant.com/wp-content/uploads/the-simpsons-renewed-season-24-25.jpg "The image has text!"

[cheatsheet]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
