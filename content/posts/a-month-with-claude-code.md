+++
draft = true
date = 2025-07-25T09:37:49-07:00
title = "A Month With Claude Code"
description = ""
slug = ""
authors = []
tags = []
categories = []
externalLink = ""
series = []
+++

After a month on sabbatical, I decided to dive into Claude Code with the $20/month Pro plan. Here's what I learned from using it across various projects.

![Daily Usage](/ccusage-daily.png)

![Project Breakdown](/ccusage-projects.png)

*Usage data via [ccusage](https://github.com/ryoppippi/ccusage) - though once you're on a subscription plan, claude code itself will no longer report costs through /costs.*

```console
> /cost
  ⎿  With your Claude Max subscription, no need to monitor cost — your subscription includes Claude Code usage
```

## From Coder to Tech Lead

The biggest shift? I'm no longer writing code—I'm directing it. Claude Code feels like managing a capable junior developer across multiple projects, from large applications like my [activity tracker](https://github.com/PureSin/activity-tracker) (will do a review of the code in a later post) to quick scripts automating some simple tasks.

## Two Quick Wins: Automating tasks

I needed to automate two simple tasks:
- Monitor YouTube for expected videos
- Check websites for inventory updates

Instead of my usual Python + cron on my local computer, Claude suggested Cloudflare Workers. Within minutes, I had TypeScript scripts using the YouTube API and web scraping libraries, complete with email notifications. Cost? About $1 each to create (website/youtube-checker) and basically free to run daily.

## The Reality Check

It's not perfect. Both large and small projects had their share of suboptimal code and logical bugs. But here's the thing—reviewing and tweaking Claude's work is far faster than writing from scratch. I can focus on architecture and requirements while Claude handles implementation details.

The workflow works surprisingly well: I act as product manager, Claude codes, I review and refine. I also get to do other things and multitask. So I could be running errands around the house or reading and just checking Claude whenever it's ready. 

## On Session Limits and Reliablity

I did at one point run into a reliability [issue](https://github.com/anthropics/claude-code/issues/3891) where Claude will crash, and it was quickly fixed. 

A popular topic online has been one talking about reaching the session limit, which can be done pretty quickly on the $20/month Pro plan. But even people on the $100-$200/month plan are finding they reach it pretty quickly, especially when using Opus 4. The Pro Plan itself doesn't support Opus 4 yet, so I can't speak to how well it works vs. on it. Talking from friends that have access to Opus, they really like it and find it much better for tricky tasks. 

## Overall

Overall, I think this is a really great tool. I love using it from the terminal. I think having this tool or like Gemini COI (or any of the other COI tools) will let me work on side projects a lot quicker, especially the small stuff that I would've never sat down to bother to do. 

