---
layout: post
title:  "Diary Entry"
date:   2017-05-19
categories: programming, life, personal
---
Diary entry for May 19th, 2017

First one of it's kind. Nothing too fascinating as it's main purpose is to note down things that I've learnt throughout the day.
Typically it will be about development (good, bad and the ugly), but sometimes it will be life stuff.

Enjoy.

### Jekyll

Currently I'm using Jekyll for my blog. It's easy to learn, uses Markdown, and it can be hosted on Github Pages.
I haven't been using it for very long and I was surprised at smart it was.
Something probably everyone knows is that you can add subdirectories in your *\_drafts*, and it will be picked up but Jekyll and generate a post.
I'm thinking that this is the same for all the folders, which I will experiment on later.

It makes things so easy because I can encapsulate everything into it's own folder structure and it should leave everything clean

### Google Drive

Speaking of clean, I've noticed that my Google Drive has become a little messy.
See, in real life, you wouldn't really call my work station "clutter free". And I'm ok with this.
Strangely though, I need to have the folders and desktop on my all my computers to be clutter free.



# Notes
* 6:30 alarm
* Checking Pinterest
* Start diary entries
* Found out that you can add folders in the *\_drafts* folder and it will still show up when you serve it on Jekyll
* Sort out Google Drive folders
  * Cluttered workspace frustrates me
* Website is running slow
  * Ran google insights to check where it can be improved
  * Mobile: 64/100
    * Need to remove render blocking js and css
      * jquery
  * Focus is Mobile experience so will need to remove, or at least, move to footer
  * Added a plugin - "Script to Footer" that moved scripts to footer
    * Mobile: 75/100
  * Enabled WP Super Cache
    * Mobile: 65/100
    * Odd, but it's complainging about images, so I need to fix those
  * Disabled Jetpack (I don't use it anyway)
    * Mobile: 64/100
    * I think it's the images
