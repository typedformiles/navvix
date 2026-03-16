---
layout: post
title: "Building a moOde Audio Remote Display with a Raspberry Pi3"
date: 2026-03-15
---

I found an old Raspberry Pi3B in a drawer last week, and set about a little project aided by Claude Code to make a remote display for my home moOde Audio player.

If you're not familiar with [moOde](https://moodeaudio.org/) I recommend checking it out, it's an audiophile operating system for the Raspberry Pi range of SBCs and does an amazing job for me as a headless device connected to my main amplifier, housing a collection of around 4k FLAC and mp3 files I have.

I usually control moOde using a mobile or tablet via the local hostname, but wanted to have some "Now Playing" art available and thought the Pi3 with a 4" screen would be perfect for this.

<img src="/assets/images/moode-display.jpg" alt="moOde remote display showing Now Playing on a Raspberry Pi with 4 inch screen" style="max-width: 400px;">

It wasn't all plain sailing getting this setup, I learned pretty quickly that nuances in PiOS operating system version cause a lot of issues when dealing with older boards like this, but we got there in the end! The github Repo is public [here](https://github.com/typedformiles/moode_remote) if you're inclined to do something similar.

The screen is touch so this can also be used as a remote so play, pause, skip and control volume... but mostly it's just a nice way to see what's playing!
