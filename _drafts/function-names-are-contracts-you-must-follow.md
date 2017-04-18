---
layout: post
title:  "Function Names are Contracts you must follow"
<!--date:   2017-04-04 04:46:39 +0000-->
categories: programming
---
# quote
# frequency is high
Imagine this scenario: you are hungry and go to the local shopping centre. You 
choose the donuts and cola. Typiclly not the healthiest of options, but that's
besides that point. You go to the cashier pay for your goodies. She asks you
whether you like the receipt and you say yes. She prints one out and gives it
to you. But what you didn't know is that she sent emails to everyone about
what you bought, unbeknownist to you. Quite rude, I think!

But this happens time and time again! This is what I see:
``` perl
sub do_something {
    do_expected_things();
    
    do_something_else();
}
```

In this basic example, the function is telling use that it is "do_something",
but in reality it is doing more than that. It's actually doing something else.
I have a real world example where, I came across a function that created end
user reports. Cool, I needed to use that, so I made a call to it. What a
mistake. What the function name didn't tell me
# it's annoying
It really annoys me
# example of poor function
# example of better function
# conclusion