---
layout: post
title:  "Programmer's Log - June 5th, 2017"
date:   2017-06-05
categories: log programming life
---
{% include affiliate-disclaimer.md %}

# Intro

Today is the start of another work week. Monday... Yay...
First day back from what ended up close to 2 weeks off. Week one, whole family
sick with the flu, so I was kind of on leave. Week two, birthday week! A
traditional I plan to have forever on.

As per every morning, I'm up at around 6:30 AM and I'm hacking away at my laptop.
Today's morning session was a continuation of last night's discovery of Ruby [Prawn][1].
I like it because it's easier to learn than the current methods I've been using in Perl and Python
and it gives me the chance to learn a different language.

# Ruby: Prawn

I continued learning during my lunch break, where I got a little more familiar
with Prawn Table. Because I'm currently creating puzzles for my website,
[puzzlesbynilo.com][2], and also selling hard copies on [Amazon][3] (My Affiliate Link),
making tables in a PDF is very important. Pretty much most puzzles are set out
in a grid of some sort.

Currently, I am using my primary language, Perl, and my secondary, Python, to
generate the puzzles and to output pdfs for upload to my website and Amazon. But,
what I've found is that it is very clunky and it isn't easy to configure. I also
tried a Python solution, but I found that even worse.

Anyway, what I learnt in my lunch hour was how to generate a basic 3x3 table,
with center text alignment within each cell and move it around in it's own
bounding box. Then I was able to move said bounding box around the page whilst
keeping the table in place in reference to the bounding box. It is very
flexible and very easy to configure.

The next part was use JSON to configure the settings of the table, from its (x,y)
positions, width, height, to its text align and valign. It was going well until
I tried to set align and valign. Since the Prawn Table module required the use
of symbols, and JSON doesn't store symbols just text, I had to convert the keys
and values into symbols. This was done by using the function .to_sym. Note that
this can only be used on strings, as I found out while trying to make integers symbols.

# Work

While at work, I typically use Perl to make company contracts. Though I'm not too
sure why it was initially chosen to begin with, I think it would have been due
to it's ability to manipulate strings and regular expression capabilities. I
think it's a pretty powerful language, although, I think there are other languages
that could be used instead. Topic for another day.

As it's my first day back since I took leave, I was expecting to hit the ground
running. Which I did. Loads of emails to sort through, status and handover meetings
during the day and a full day of work on top of all that. Typical Monday work day.

Going through my duties during the day, I began to question the saying: *if it ain't
broke, don't fix it*. Now I suppose it seems like there's nothing wrong
with the saying, but the more I think about it, the more I think that it's
deeply flawed.

These questions pop up in my mind:
* Though a program does run from start to finish, but is poorly written, shouldn't
you fix it?
* If the program runs extremely inefficiently, shouldn't you fix it?
* Does upgrading a program mean you are fixing it?

I feel like this mentality is at the heart of a lot of problems. Only acting
when the failure occurs, instead of acting when a potential problem is spotted.

# Conclusion

To sum up the day: I've learnt that Ruby Prawn does pdf generation way better
than Perl or Python (highly subjective), I wish I didn't have to go back to work today
and I like asking the hard question

Until next time.

Nilo

[1]: http://prawnpdf.org/api-docs/2.0/index.html "Prawn PDF"
[2]: https://puzzlesbynilo.com "Puzzles By Nilo"
[3]: http://amzn.to/2rMPr9f "Amazon Search - Nilo Ballener (My Affiliate link)"
