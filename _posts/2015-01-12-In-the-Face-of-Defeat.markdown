---
layout: post
title:  "In the Face of Defeat"
date:   2015-01-12 21:35
categories: blog january
---

The results are in for the qualifying round of the Facebook Hacker Cup. Unfortunately, my code did not pass some of the test cases provided. To be honest, I am slightly dejected with the fact that had I been more resilient with testing my code, I would have had a better chance at moving towards the next round. Nevertheless, what's done is done and I am here to share what I could have done better with my code.

I will post my code for the problem later, but here is the major mistake that I found:


```
char[] digit = new char[num.length()];
```

and these two lines:

```
char[] copy = digit; 
```

```
char temp = digit[j];
```

I made the detrimental mistake of creating the line ```char[] copy = digit;``` and thus made my code fail the test cases. Instead, I should have created a new char array by invoking the line ```char[] copy = new char[num.length()]``` and then add to the array character by character like I did for the digit array. This silly mistake costed me participation into the first round, but this should serve more as an eye-opener for me than anything else.

Sadly, I could have caught all of this with slightly more awareness and simple testing. In the end, I ended up regretting not considering more general cases to test and only tested the special cases. On the other hand, I decided to rush the testing phase of the coding and failed. As a lesson, testing should come while programming, not after.

Adimwit