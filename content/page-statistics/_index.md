---
title: "Page statistics"
date: 2022-06-12T13:06:19+01:00
draft: false
description: "Description of the metrics that are shown at the bottom of every page on green-pages.eco"
---

Some metrics are displayed at the bottom of every page on this website, read on for some details about how these are calculated.

This site is very well optimised, and has extremely good metrics, roughly 1000 times better than the average web site. It is a simple website, and goes further than most websites will want to, sacrificing some design goals along the way (there are no custom fonts, limited images and the css and javascript is simple and lightweight). However, it still looks professional, is easy to use, and is hopefully good inspiration for what is possible.

## Transfer size

Transfer size is calculated using the [Performance interface](https://developer.mozilla.org/en-US/docs/Web/API/Performance) of your browser.

There is a lack of standards in the performance interface, and different browsers measure it differently. Device Atlas have an [interesting blog post](https://deviceatlas.com/blog/measuring-page-weight) about it.

It uses the `transferSize`, which is the size of the data as it is transferred across the internet. This data should be compressed on the server and uncompressed in your browser, so this value should be less than the size of the files.

It should include all files included as part of rendering the page, including scripts and stylesheets.

The images on this website are "lazy loaded". If they are off the bottom of the page initially, then they are only loaded when you scroll down to see them. The size of these images (once loaded) is included in the **Transfer size**.

If you look at this website on an Android phone and are in **Battery saver** mode, lower quality images will be displayed, and hence the **Transfer Size** will be lower.

The **Transfer size** takes in to account anything that is already in your browser cache, so the second time you view a page this number will be lower. If you want to see the original value you can [hard refresh](/hard-refresh) the page.

## Load time

Load time is also calculated using the [Performance interface](https://developer.mozilla.org/en-US/docs/Web/API/Performance) of your browser.

It is calculated as the time from [Navigation Start](https://developer.mozilla.org/en-US/docs/Web/API/PerformanceTiming/navigationStart) (when you click on a link or type in a url) to [Dom Complete](https://developer.mozilla.org/en-US/docs/Web/API/PerformanceTiming/domComplete) (which more or less means that the browser has finished showing the page).

## co2

The co2 calculation is very broad brush, and uses global average values for everything apart from the **Transfer Size**. Estimating carbon emissions from websites is at a very early stage, and all of the current calculations are like this. You can read our [Methodology](/methodology) for more information about emissions and how to optimise.

It is assumed that each Gigabyte of **Transfer Size** uses 0.81 Kilowatt Hours of energy.

It uses the global average value of 442 grams of CO2 per Kilowatt Hour of energy.

These numbers come from [calculating-digital-emissions](https://sustainablewebdesign.org/calculating-digital-emissions/), which in turn comes from [Perspectives on Internet Electricity Use in 2030, Anders S.G. Andrae, June 2020](https://www.researchgate.net/publication/342643762_New_perspectives_on_internet_electricity_use_in_2030).

Some calculators work out whether the server for a website is hosted on a "Green" data center / server, and then use a different value for the "grams of CO2 per Kilowatt Hour of energy". This is a reasonable thing to do, but we don't, as there is huge variation in this number and a lot of "Green" data centers use Carbon Offsets, which are frequently ineffective.
