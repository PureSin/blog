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

I've been on sabbatical for about a month now, and part of that is using some of the time to try out new coding tools. The most popular of which is Claude Code, so I signed up for the Claude Code Pro ($20/month) plan and then coding with it. Here are two screenshots that show the usage across different projects and by day over the last month. 

![Daily Costs](/ccusage-daily.png)

![Per Project Costs](/ccusage-projects.png)

Cost data via https://github.com/ryoppippi/ccusage. This tool lets you calculate the costs for cloud usage based on tokens. Once you subscribe to a plan, the tool itself no longer tells you the cost. 

```console
> /cost
  ⎿  With your Claude Max subscription, no need to monitor cost — your subscription includes Claude Code usage
```

Some thoughts on working with Claude Code.
I think first I'm behaving more like a tech lead and just guiding junior engineers across a variety of projects. The projects can range from large (the biggest one is this activity tracker, which is a personal version of a to-do app) to really small one-off projects. For example, there are two small tasks I wanted to automate:
- Checking YouTube for a video that I'm expecting
- Checking a website for some inventory to be available
Both of which I could have automated myself using Python scripts and just set it up as a cron job on my computer, but with Claude's help, I can kind of just give them the requirements, acting more like a PM, and have it offer suggestions. In which case it suggests that I use Cloudflare's Workers and use that to cron so I don't have to run the computer myself. With some input, it was able to quickly build pretty simple TypeScript using a few libraries that will check the web page and send me an email or check YouTube using YouTube API and send me an email, and it only costs about a dollar each to generate.

Not that it was error-free, right? In both the larger activity tracker project and some of these smaller scripts, there were times where either didn't write optimal code or had small logical bugs. It's small enough that I can just quickly review it and suggest fixes or small style or API changes to make it easier to use. But the main thing is it's so easy now to build these things since I'm not the one actually doing the programming, I'm able to hand them off and just review and maybe do small tweaks. And the results worked very well. 

https://github.com/PureSin/activity-tracker