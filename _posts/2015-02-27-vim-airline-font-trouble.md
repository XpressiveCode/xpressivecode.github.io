---
layout: post
title: "Vim Airline Font Trouble?"
description: ""
category: 
tags: [vim, vim-airline]
---
{% include JB/setup %}

<a href="https://github.com/bling/vim-airline" target="_blank">Airline</a> is a great plugin if you're working in vim. It provides a "lean & mean status/tabline for vim". It works really well with other plugins, such as <a href="https://github.com/scrooloose/syntastic" target="_blank">syntastic</a>, <a href="https://github.com/scrooloose/nerdtree" target="_blank">nerdtree</a> and <a href="https://github.com/tpope/vim-fugitive" target="_blank">fugitive</a> (to name but a small few). 

Here is a demo of what it looks like

<img src="https://github.com/bling/vim-airline/wiki/screenshots/demo.gif" />

Notice the nice chevrons, or the nice branch icon next to the git branch name?

If you're like me, you might not have had the correct font installed that would allow those characters to show up. 

The quick fix for me was to:

- Install the free powerline font, <a href="https://github.com/powerline/fonts" target="_blank">here</a> (clone the repo and run the install.sh)
- Now go to your terminal preferences, find your font and select `Source Code Pro for Powerline`. 

If you're using iterm2, you will go to Preferences > Profiles > Text and update the `Non-ASCII Font`. You don't need to update your `Regular Font` option.

