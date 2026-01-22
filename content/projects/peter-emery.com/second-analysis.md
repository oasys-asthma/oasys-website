---
title: "Peter-emery.com (second analysis)"
date: 2022-10-21T13:06:19+01:00
draft: false
description: "Second Analysis of carbon emissions for peter-emery.com by Green Pages"
---

At this point, it was decided that it would be better to rewrite the website from scratch, instead of incrementally improving the existing one. The website was custom built, and expensive to maintain, so moving to an off the shelf website template (from Fabrik.io) reduces this maintenance cost, and should come with current best practice out of the box.

## Core metrics

The current carbon emissions calculations for websites are early stage, and mostly use very generic assumptions. The only inputs to the calculation are transfer size, and whether the server uses renewable energy or offsets. All the other aspects of the calculation use global averages.

For this reason, it is more useful to focus on the core metrics, which do directly correlate with emissions, even though they don't all effect the current carbon calculation. They are also easy to compare, so that you can make changes to the website, and verify that there is an improvement.

The "Second Load" data transfer is smaller, as much of the website is already cached from the "First Load". The CPU values are benchmarked.

Changes from the first analysis are shown in brackets, with green for an improvement and red for a deterioration.

You can read our [Methodology](/methodology) for more information about how these numbers are calculated.

|             | Total Transfer Size                    | Average Transfer Size                    | Total CPU Client                  | Average CPU Client                    |
| ----------- | -------------------------------------- | ---------------------------------------- | --------------------------------- | ------------------------------------- |
| First Load  | 12.2 Mb ({{<improvement text="83%">}}) | 0.68 Mb ({{<deterioration text="10%">}}) | 63 ({{<improvement text="69%">}}) | 3.5 ({{<deterioration text="106%">}}) |
| Second Load | 0.2 Mb ({{<improvement text="93%">}})  | 0.01 Mb ({{<improvement text="58%">}})   | 49 ({{<improvement text="74%">}}) | 2.7 ({{<deterioration text="69%">}})  |
| Mobile      | 10.8 Mb ({{<improvement text="85%">}}) | 0.60 Mb ({{<improvement text="5%">}})    | 52 ({{<improvement text="68%">}}) | 2.9 ({{<deterioration text="107%">}}) |

| Page Count                        | Power Usage Efficiency (PUE) of server | Server Utilisation |
| --------------------------------- | -------------------------------------- | ------------------ |
| 18 ({{<improvement text="85%">}}) | 1.15                                   | -                  |

These metrics show huge improvements over the old website, which is mostly down to there being fewer pages (18 instead of 121). The caching and the mobile transfer size is improved, which you would expect when using a standard template. The average transfer size has increased a little, mostly due to the standard template using javascript inefficiently. The CPU usage on the client has increased a lot, also mostly due to uneccesarily complicated CSS.

## {{<co2>}} metrics

The website currently doesn't yet have useful analytics, so we don't know how many times each page is loaded, which means we don't know how much carbon is emitted.

Instead we can calculate the emissions for each page in the website being viewed once. These calculations are very approximate, the core metrics are more actionable.

|             | {{<co2>}} (kilograms)               |
| ----------- | ----------------------------------- |
| First Load  | 4.4 ({{<improvement text="83%">}})  |
| Second Load | 0.08 ({{<improvement text="92%">}}) |
| Mobile      | 3.8 ({{<improvement text="86%">}})  |

These metrics also show huge improvements over the old website, which is also nearly all down to there being fewer pages.

## Discussion

### Website

The website uses a standard template from Fabrik.io, which is specifically aimed at creative websites.

Fabrik states that it optimises and "right sizes" images, and it seems to do a good job of this, with smaller images being used for smaller screen sizes. It uses lossless compression, which is not as good, but probably appropriate for the graphic centric creative websites it is aimed at. It uses the ".jpg" format, and could probably improve by moving to a more modern format, such as ".webp".

Fabrik states that it handles a lot of hosting complexities efficiently, such as a Content Delivery Network (CDN), site caching, load balancing and similar. This all sounds good, but it is hard to know how well this is done / how effective it is.

The Fabrik template does use a lot of javascript, some of which is not used at all, and most of which could be designed out. It does however download standard scripts from well known locations, so there is a reasonable chance that users will already have this script in their browser cache. The size of the scripts and the execution of them in the browser contribute to the website not loading as quickly as it could do.

The website shows a picture of the start, middle and end of each video, to make it easier for people to decide whether they want to watch the video or not, which will result in less wasted time and energy.

### Embodied carbon

Hardware obsoletion is the primary driver of embodied carbon that we can control.

The CPU usage on the client has increased, and is largely unnecessary. The website can be still used with a wide range of older browsers. This means that it will run well on older hardware and isn't driving obsoletion.

The details of the server are unknown, but it is very likely to be static pages. It is likely that this will run well on older hardware and isn't driving obsoletion.

### Website host / data center

The Website is ultimately hosted by [Amazon EU (Ireland)](https://www.thegreenwebfoundation.org/directory/#698), which [self declares that it either uses renewable energy for its hosting, or offsets](https://www.thegreenwebfoundation.org/green-web-check/?url=https%3A%2F%2Fwww.peter-emery.com). Amazon finances / owns a large amount of renewable energy in Ireland and elsewhere.

This data center has a [Power Usage Efficiency](https://en.wikipedia.org/wiki/Power_usage_effectiveness) of 1.15, which is good.

The website is primarily UK based, so hosting in Ireland makes sense.

## Reccomendations

### Add a robots.txt file to stop robots

There are many programs (or 'bots') that will visit all the pages on your website. Some of these are useful (like Google), some are comparable with spam, and some are actively trying to cause problems.

These bots can make up a significant fraction of your total website traffic, 50% is a commonly quoted figure.

You can add a robots.txt file to indicate which bots are welcome and which are not. Not all bots will respect this file, but reputable ones will.

https://sustainablewww.org/principles/block-unwanted-and-spammy-bots-with-robotstxt-and-speed-up-your-website

### Contact Fabrik

Using a standard template from Fabrik.io is a good idea, and transfers most of the problems away from you and on to Fabrik. This makes sense, as the template is used by many people, and is paid for, so Fabrik have the time, motivation and money to make sure that the problems are solved.

The template from Fabrik is pretty good. It does a decent job of client side caching and it correctly sizes images for different size displays, so less data is transferred to mobile phones and tablets.

However, it transfers and executes a lot of uneccesary javascript, which slows down the page load time, reduces the Google lighthouse score (which means the site performs less well in Google searches), and increases the carbon emissions. The css is also larger and more complicated that it needs to be.

Fabrik is aimed at creative websites, where probably these things have traditionally not been the primary concern. It would be worth contacting Fabrik to let them know that you care about these things, and to ask them to improve.
