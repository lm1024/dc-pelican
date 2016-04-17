layout: post
title: Technical debt for whole systems
author: devcurmudgeon
date: 2016/03/19

<b>"It ain't what you don't know that gets you into trouble. It's what you know for sure that just ain't so."</b> [Mark Twain]

If you've been in involved in large-scale software projects over the last few
decades you've probably learned the hard way that upgrading the platform (operating system, libraries etc) mid-project can lead to a world of unexpected pain:

* APIs and ABIs change
* it turns out your project had hidden dependencies on stuff that is now
  deprecated
* and the exciting new stuff that led you to accept the upgrade
    * exposes problems you didn't know you had, and/or
    * doesn't quite work as expected, and/or
    * isn't quite ready for primetime.

As a result, the folk wisdom is to resist platform upgrade as long as possible. Let's push it back to the integration phase. Let's get the delivery
out first and do that as a maintenance release.

All of which makes perfect sense for traditional embedded projects.

Unfortunately, for many large-scale or complex Linux-based systems involving connected devices, this battle-hardened strategy is <b>proving to be disastrous</b>.

<i>"Backporting all these patches is taking forever... We're finally ready to roll out into production but the LTSI kernel we built on is already EOL... 
We had to upgrade the kernel, but it was a nightmare!"</i>

For everyone who's spent recent years learning to combine "Agile" practices with building on a "Baseline" and "Board Support Package", here's the heads-up:

<b>Connected devices are going to require constant security updates from now on.</b>

If you choose a "hardened platform" you'll be backporting fixes and updates, and as time passes those backports will just get harder and more expensive. So I propose a simple guideline to help folks cope in the world we are now in:

** Treat any delta your project carries versus mainline as technical debt. The bigger the patchsets for your BSP, OS and middleware, the more you'll be paying in maintenance over the lifetime of the project. **


It's called upstream for a reason. Streams *flow*, and in 2016 the flow of
software change is already a flood. 

In the real world, faced with a torrent of onrushing water... you wouldn't choose to be on a fixed platform, waiting to be be engulfed. 

You'd have a better chance going with the flow ... on a boat.
