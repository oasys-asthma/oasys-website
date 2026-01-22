---
title: "Green-pages.eco (first analysis)"
date: 2022-06-12T13:06:19+01:00
draft: false
description: "First Analysis of carbon emissions for green-pages.eco by Green Pages"
---

## Core metrics

The current carbon emissions calculations for websites are early stage, and mostly use very generic assumptions. The only inputs to the calculation are transfer size, and whether the server uses renewable energy or offsets. All the other aspects of the calculation use global averages.

For this reason, it is more useful to focus on the core metrics, which do directly correlate with emissions, even though they don't all effect the current carbon calculation. They are also easy to compare, so that you can make changes to the website, and verify that there is an improvement.

The "Second Load" numbers are usually smaller, as some things are already cached from the "First Load".

| Client      | Total transfer size | Average transfer size | Total CPU (benchmarked) | Average CPU (benchmarked) |
| ----------- | ------------------- | --------------------- | ----------------------- | ------------------------- |
| First Load  | 0.045 Mb            | 0.006 Mb              | 6                       | 0.8                       |
| Second Load | 0.027 Mb            | 0.004 Mb              | 3                       | 0.4                       |
| Mobile      | 0.046 Mb            | 0.007 Mb              | 4                       | 0.6                       |

| Server      | Average Time (benchmarked) | Total Time (benchmarked) |
| ----------- | -------------------------- | ------------------------ |
| First Load  | 30                         | 4                        |
| Second Load | 25                         | 4                        |

| Page Count | Power Usage Efficiency (PUE) of server | Server Utilisation |
| ---------- | -------------------------------------- | ------------------ |
| 7          | -                                      | >16%               |

## {{<co2>}} metrics

This website is new, and at the time of writing, doesn't have enough analytics to be useful, so we don't know how many times each page is loaded, which means we don't know how much carbon is emitted.

Instead we can calculate the emissions for each page in the website being viewed once. These calculations are very approximate, the core metrics are more actionable.

|             | {{<co2>}} (kilograms) |
| ----------- | --------------------- |
| First Load  | 0.016                 |
| Second Load | 0.01                  |
| Mobile      | 0.016                 |

## Discussion

### Website

This website is very well optimised, and has extremely good metrics, roughly 1000 times better than the average web site. It is a simple website, and goes further than most websites will want to, sacrificing some design goals along the way (there are no custom fonts, limited images and the css and javascript is simple and lightweight). However, it still looks professional, is easy to use, and is hopefully good inspiration for what is possible.

### Embodied carbon

Hardware obsoletion is the primary driver of embodied carbon that we can control.

The website has very low CPU usage on the client, and can be used with a wide range of browsers going back to 2020. Even though this is quite recent, it still covers the vast majority of users today, because even devices much older than this have updated to use the latest versions (even Chrome 94 is only used for 0.77% of visits). This means that it will run well on older hardware and isn't driving obsoletion.

| Browser | Oldest supported version |
| ------- | ------------------------ |
| Firefox | 74 (2020)                |
| Chrome  | 80 (2020)                |
| Opera   | 67 (2020)                |

The website is static, and just serves text files. This means that it will run well on virtually any hardware and web server software.

### Website host / data center

The website is hosted by Cloudflare, which has a global content delivery network (CDN), and so wherever a user is in the world, the data will not have to travel very far. They are also extremely efficient and are a certified Green Web Host.

There is no data for the Power Usage Efficiency of their data centers / the data centers they use, but they do claim a server utilisation of greater that 16%, although again, the actual figure isn't given.

[The climate and cloudflare](https://blog.cloudflare.com/the-climate-and-cloudflare/) blog post is an interesting summary of this.

The cloudflare blog also has a [sustainability section](https://blog.cloudflare.com/tag/sustainability/), with all the details of their sustainability efforts.
