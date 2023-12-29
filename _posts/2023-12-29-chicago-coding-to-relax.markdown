---
layout: post
title: $PATH home from Chi-town
date: 2023-12-29 16:10 -0600
---

## site.time

#### So I've been in Chicago the last few days...

... with family and some ppl they were hanging out with. Good enough time even though it was cold, wet, and rainy the entire time.

I found myself at a starbux on the last day here charging my devices for the ride home. I had some time to kill so I decided to dork around with Ember a bit more. Not sure productive, but I did end up playing around with my M1 Mac running Sonoma 14.2.1.

The problem was that every time I opened a new terminal window I would get this really long loading sequence like the OS was getting sourced multiple times? Or _maybe I just need to update my theme so that I don't see all the OS directory jumping_.

I spent a bit trying to modify my OS $PATH environment variable [with the help of this article](https://towardsdatascience.com/my-path-variable-is-a-mess-e52f22bfa520), but there is a lot of stale info on updating the $PATH for OSX running new mac silicon (the M* series, which I have the M1 from 2021).

I got rid of some NVM (node version manager) binaries to trim down the $PATH a bit, but there is still RVM (ruby version manager, which I need to get rid of in favor of a better supported package), PYENV (for python environment management, which I'm told is _not_ the way to install and manage Python), a few Ruby libraary binaries (again that need to get removed).

I thougth the process woudld be as simple as:

> echo $PATH
> export $PATH = ""
> export $PATH = "{{replace this handlebars-style syntax with the colon(:) separated list of directories to source}}"

but I kept running into errors that felt like I was approaching this from the wrong angle. Once I get home I'll have to dig into some Sonoma docs for apple osx and see why I am just hitting blockers here.

I accomplished what I wanted though, I distracted myself for 45 minutes while I drank some coffee and charged my devices for the drive back home.

Now into the dark, dear friends...