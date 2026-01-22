---
title: "Peter-emery.com (first analysis)"
date: 2022-06-12T13:06:19+01:00
draft: false
description: "First Analysis of carbon emissions for peter-emery.com by Green Pages"
---

## Core metrics

The current carbon emissions calculations for websites are early stage, and mostly use very generic assumptions. The only inputs to the calculation are transfer size, and whether the server uses renewable energy or offsets. All the other aspects of the calculation use global averages.

For this reason, it is more useful to focus on the core metrics, which do directly correlate with emissions, even though they don't all effect the current carbon calculation. They are also easy to compare, so that you can make changes to the website, and verify that there is an improvement.

The "Second Load" data transfer is smaller, as much of the website is already cached from the "First Load". The CPU values are benchmarked.

You can read our [Methodology](/methodology) for more information about how these numbers are calculated.

|             | Total Transfer Size | Average Transfer Size | Total CPU Client | Average CPU Client |
| ----------- | ------------------- | --------------------- | ---------------- | ------------------ |
| First Load  | 72.7 Mb             | 0.62 Mb               | 203              | 1.7                |
| Second Load | 2.8 Mb              | 0.024 Mb              | 185              | 1.6                |
| Mobile      | 74.3 Mb             | 0.63 Mb               | 163              | 1.4                |

| Page Count | Power Usage Efficiency (PUE) of server | Server Utilisation |
| ---------- | -------------------------------------- | ------------------ |
| 121        | -                                      | -                  |

## {{<co2>}} metrics

The website currently doesn't have any analytics, so we don't know how many times each page is loaded, which means we don't know how much carbon is emitted.

Instead we can calculate the emissions for each page in the website being viewed once. These calculations are very approximate, the core metrics are more actionable.

|             | {{<co2>}} (kilograms) |
| ----------- | --------------------- |
| First Load  | 26                    |
| Second Load | 1                     |
| Mobile      | 27                    |

## Discussion

### Website

The website is already well designed, easy to navigate, and easy to search for. Images are usually loaded on demand, saving transfer size when they aren't required. The site is a Progressive Web App, which improves caching and hence reduces data transfer. As with everything though, when you take a long and detailed look there are improvements that can be made.

### Embodied carbon

Hardware obsoletion is the primary driver of embodied carbon that we can control.

The website has modest CPU usage on the client, and can be used with a wide range of older browsers. This means that it will run well on older hardware and isn't driving obsoletion.

The details of the server are unknown, but it appears to be static pages or simple php scripts. It is likely that this will run well on older hardware and isn't driving obsoletion.

### Website host / data center

It lookes like Website is hosted by [ionos / 1&1](https://www.ionos.com/), which [self declares that it either uses renewable energy for its hosting, or offsets](https://www.thegreenwebfoundation.org/green-web-check/?url=https%3A%2F%2Fwww.peter-emery.com).

I couldn't find a Power Usage Efficiency (PUE) value for Ionos, or an representative Server Utilisation.

### Vimeo

The videos on the website don't start automatically, so will only be streamed by a user when they actually want to watch them.

Hosting videos on a specialist platform is a good idea, as they have the scale and expertise to optimise the hosting and streaming of videos.

Vimeo are just getting started with Environmental Social and Governance issues, and bought some carbon offsets for the first time in 2021. They are currently laying the groundwork for a formal sustainability policy that will seek to mitigate their greenhouse gas emissions on a long-term basis.

https://investors.vimeo.com/static-files/3ab0dbb9-e0da-4a97-974e-e5f9e1a3ac05

### Analytics

There are no analytics for the site, which means some number crunching isn't worthwhile.

It isn't possible to work out how far data is transferred over the network, as we don't know the final destination.

We don't know how often pages are viewed, so we don't know how much data is transferred, nor can we decide which pages are most important and should be optimised first.

## Reccomendations

### Add analytics

It is very difficult to optimise something you can't measure, and adding analytics will enable this measuring, and lead to further recommendations, such as moving the website near where its users are, or using a Content Delivery Network (CDN) to reduce the transfer distance between the website and the user.

[Cabin](https://withcabin.com/) provides privacy and carbon conscious web analytics, and they have a free tier that would be suitable.

You can pay $19 per month and it will additionally estimate the carbon footprint of your website based on usage data. Like all current website carbon calculators this only uses transfer size and whether or not the server buys renewable energy to make this estimate, but it is still useful.

### Add a robots.txt file to stop robots

There are many programs (or 'bots') that will visit all the pages on your website. Some of these are useful (like Google), some are comparable with spam, and some are actively trying to cause problems.

These bots can make up a significant fraction of your total website traffic, 50% is a commonly quoted figure.

You can add a robots.txt file to indicate which bots are welcome and which are not. Not all bots will respect this file, but reputable ones will.

https://sustainablewww.org/principles/block-unwanted-and-spammy-bots-with-robotstxt-and-speed-up-your-website

### Delete content which isn't human reachable

There is quite a lot of content on the website that isn't reachable by clicking on links, but is reachable by computer.

This content doesn't have any benefit, and does add to the carbon footprint, as it is still downloaded by bots.

Some examples:

- https://www.peter-emery.com/author/appleboxdesigns/page/5
- https://www.peter-emery.com/photography-and-ideas/page/2
- https://www.peter-emery.com/work/photography/little-deaths-04

### Contact Vimeo

Vimeo are in charge of some of the emissions for this site, and have recently started a sustainability journey. It would be worth asking them to publish numbers detailing carbon emissions (or other metrics) for each video, which you could then use. This would be useful advocacy, and would enable you to make informed decisions about video content.

### Data Center

I couldn't find any stats on Ionos, your website host, about their Power Usage Efficiency (PUE), Server Utilisation or whether they used renewable energy in their data centers.

The website is hosted in Germany, and I imagine that most of the users are in the UK.

The three major cloud providers all have tools to estimate the carbon cost of your cloud infrastructure.

It would be worth thinking about transferring to a different host, or contacting Ionos and asking about PUE, Server Utilisation and renewable energy.

### Sign the Sustainable Web Manifesto

The [Sustainable Web Manifesto](https://www.sustainablewebmanifesto.com/) is a public declaration of a shared commitment to create a sustainable internet.

### Use server caching (if pages are dynamically created)

It is inefficient to generate a page every time someone visits it. I am not sure if this is happening on your website, but I will be able to tell once I have access to the serer.

Caching technologies like Varnish pre-generate static versions of each page so that the server overhead can be significantly reduced for most visitors.

It can be complicated to set up, but is sometimes provided off the shelf.

It is also probably the case that the website doesn't need to dynamically generate pages, and can use static pages instead.

### Optimise images

The images on the website are already a sensible size, but some of them are still downscaled in the browser, which creates more work for the CPU, and means that more data is being transferred than required. This can be fixed by sending images that are exactly the size that is desired in the browser.

There are modern image formats designed for the web, that do a better job of compression than traditional formats such as .jpg.

### Set cache-control headers

The cache-control header tells the browser how long to cache a page (or image or similar) on the website for, which allows the browser to use it's cache instead of downloading from your website again.

Nearly everything already has the cache-control header set, but there are a few places where it could be usefully added such as https://www.peter-emery.com/.

### Reduce page size and javascript

There is some scope to reduce the overall size of the pages.

The site only uses a small amount of javascript, but a much larger amount is downloaded, mostly because a small part of a large library is being used.

Some of the javascript is downloaded before the page renders (which slows it down), and could be switched to downloading afterwards.

There is also scope to reduce the size of the styles and custom fonts.

### Reduce mobile page size

Mobile screens are smaller than desktops, so it usually makes sense to send smaller versions of images to them, which reduces the transfer size.

Mobile phones often have slower network speed, and the carbon cost of transferring on the mobile network is higher, so it makes sense from these points of view as well.

However, on this website the average transfer size is bigger for mobile than it is for desktop.

This is because on some pages the desktop view shows 3 columns of images, and the mobile only shows 1.

This might dissapear once the unreachable pages have been deleted. If not, these images should be lazy loaded, so that they are only downloaded if the user scrolls down to them. This will ensure that the mobile pages always have a smaller transfer size than the desktop pages.

### Implementing the recommendations

The reccomendations are in a rough order of difficulty / value, and many of them can be done easily without any special expertise.

However, some will require work from a web developer or similar. We would be happy to help with this if you are interested.
