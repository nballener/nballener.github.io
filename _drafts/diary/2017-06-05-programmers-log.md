---
layout: post
title:  "Programmer's Log"
date:   2017-06-05
categories: programming, life, personal
---
{% include affiliate-disclaimer.md %}

Today is the start of another work week. Monday... Yay...
First day back from what ended up close to 2 weeks off. Week one, whole family sick with the flu, so I was kind of on leave. Week two, birthday week! A traditional I plan to have forever on.

As per every morning, I'm up at around 6:30 AM and I'm hacking away at my laptop.
Today's morning session was a continuation of last night's discovery of Ruby [Prawn][1].
I like it because it's easier to learn than the current methods I've been using in Perl and Python
and it gives me the chance to learn a different language.

I continued learning during my lunch break, where I got a little more familiar
with Prawn Table. Because I'm currently create puzzles for my website,
[puzzlesbynilo.com][2], and also selling hard copies on [Amazon][3] (My Affiliate Link),
making tables in a PDF is very important. Pretty much most puzzles are set out
in a grid of some sort.

Currently, I am using my primary language, Perl, and my secondary, Python, to
generate the puzzles and to output pdfs for upload to my website and Amazon. But,
what I've found is that it is very clunky and it isn't easy to configure. I also
trying a Python solution, but I found that even worse.

Anyway, what I learnt in my lunch hour was how to generate a basic 3x3 table,
with center text alignment within each cell and move it around in it's own
bounding box. Then I was able to move said bounding box around the page whilst
keeping the table in place in reference to the bounding box. It is very
flexible and very easy to configure.

The next part was use JSON to configure the settings of the table, from its (x,y)
positions, width, height, to its text align and valign. It was going well until
I tried to set align and valign. Since the Prawn Table module required the use
of symbols, and JSON doesn't store symbols just text, I had to convert the keys
and values into symbols.

This was done by using the function .to_sym. Note that this can only be used on
strings, as I found out while trying to make integers symbols.

# Outline
* RUBY: Prawn
* Prawn::table
  * quick example
  * table position
  * table cell width/height
  * JSON to_sym
* will use ruby from now on to create pdfs
* WORK:
  * back from leave
  * hit the ground running
* QUESTION:
  * why fix something that isn't broken? what if it was broken when it was made?
* THOUGHTS:
  * I choose to be language agnostic as I believe each language can have it's own strengths and uses
  * sometimes people get stuck in the one language when there are other languages more suited
  * example: I do my puzzle logic in perl and python, but when it comes down to creating pdfs, I'm going to switch to ruby. not because I stopped liking the previous languages, I just feel that ruby (at the time of writing this) is a better tool for pdf generation. Will this change in the future? of course. Same with all tooling.

[1]: http://prawnpdf.org/api-docs/2.0/index.html "Prawn PDF"
[2]: https://puzzlesbynilo.com "Puzzles By Nilo"
[3]: http://amzn.to/2rMPr9f "Amazon Search - Nilo Ballener (My Affiliate link)"
