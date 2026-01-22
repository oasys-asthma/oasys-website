---
title: "Methodology"
date: 2022-06-12T13:06:19+01:00
draft: false
description: "Methodology that Green Pages uses to analyse websites for carbon emissions"
---

## Drivers of carbon emissions

**Unnecessary clicks**: Good website user experience, copy writing and search optimisation can all result in people spending less time browsing the web looking for information, and visiting less pages that don’t meet their needs.

**Images**: Images are usually the dominant factor in the size of a web page, and resizing them on the client uses CPU.

**Videos**: When videos are present they tend to be the dominant factor in the size of a web page.

**Javascript**: Javascript adds to the size of a web page, and uses CPU on the client to run.

**Fonts**: Custom fonts are often a surprisingly large contribution to the page size.

## Carbon emissions from websites

It is extremely hard to calculate an accurate number for all of the carbon emissions for a website, but it is relatively easy to reason about the sources of the emissions, and hence to optimise.

### Embodied / Embedded Carbon

Embodied carbon (otherwise referred to as "Embedded Carbon") is the amount of carbon emitted during the creation and disposal of a device, and is significant.

For example, a 2019 R640 Dell Server has an amortized embodied carbon cost of 320 kg CO2eq/year, which is around 40% of its annual carbon emissions (depending on the greenness of the electricy used to power it).

There is no good proxy for these emissions, but using hardware for longer is the best way to reduce it. Most hardware does not break, but becomes obsolete as it cannot run increasingly demanding software, so making a website less demanding (on the server and on the client) is the primary driver.

### Networking / data transfer

The internet is a series of switches, routers, and servers.

When you transfer data across the internet, you are sending that data through many devices, and each one of those has embodied carbon and is consuming electricity. As a result, any data you send or receive over the internet emits carbon.

The amount of data you transfer, and the distance you transfer it, are very good proxies for the amount of emissions that will result.

### Electricity usage

The server running a website, as well as the devices that are viewing the website will be consuming electricity.

Modern data centers publish a Power Usage Efficiency, or PUE. The PUE is determined by dividing the amount of energy entering the data centre by the amount of energy used to run the computers inside it. This then highlights the amount of energy being wasted on non-computational activities such as cooling. The typical PUE for a data centre is around 1.67, meaning that for every 1.67 watts going into the data centre, only 1 watt is being used to power the computing systems. High efficiency data centres can have a PUE as low as 1.11.

The CPU usage the client uses while rendering a page, or the server uses while serving a page are good proxies for the amount of emissions that will result.

### Carbon intensity

The carbon intensity of electricity is a measure of how much carbon emissions are produced per kilowatt-hour of electricity consumed.

The carbon intensity changes all the time, and for example will go down when it is windy and there is more wind power available. A website doesn't have easy control over this and many of the other factors involved.

Choosing a data center with good green credentials, or in a region with low average carbon intensity is best way to improve this.

### Server Utilisation

The more you utilize a computer, the more efficient it becomes at converting electricity to useful computing operations. For example, a server running at 50% utilisation might use 180W, but doubling its utilisation to 100% only might only increase this to 200W.

Choosing a well run, optimised data center with good green credentials is the best way to improve this.

## Core metrics

The current carbon emissions calculations for websites are early stage, and mostly use very generic assumptions. The only inputs to the calculation are transfer size, and whether the server uses renewable energy or offsets. All the other aspects of the calculation use global averages.

For this reason, it is more useful to focus on the core metrics, which do directly correlate with emissions, even though they don't all effect the current carbon calculation. They are also easy to compare, so that you can make changes to the website, and verify that there is an improvement.

### Client Metrics

These metrics are calculated for both the first time a user visits a page, and for subsequent visits. When loading a web page for a second (or later) time, a lot of the content should already exist in the cache, so the Second Load metrics are a good indicator of how well the caching is set up for the site.

Mobile phones, and devices with smaller screens, don't require high resolution images or videos, so the transfer size to these should generally be smaller. This has an oversized effect on carbon emissions, as mobile network is more carbon intensive than normal broadband / fibre.

**Transfer Size**: The more data that is transferred, the greater the carbon emissions, as discussed above in [Networking / data transfer](#networking--data-transfer)

**Transfer Distance**: The more distance that data is transferred, the greater the carbon emissions, as discussed above in [Networking / data transfer](#networking--data-transfer)

**CPU**: The more CPU usage, the more carbon emissions, from [electricity usage](#electricity-usage) and [embodied carbon](#embodied--embedded-carbon)

### Server metrics

Aside from CPU usage, server metrics are mostly out of our control, but we can still choose a data center that has good metrics.

**Power Usage Efficiency (PUE)** is directly related to [electricity usage](#electricity-usage) and is published by all the major cloud vendors (except Amazon), and quite a few independent vendors as well.

**[Server utilisation](#server-utilisation)** is directly related to [electricity usage](#electricity-usage), and is currently hard to find, but the companies running data centers will already know it, so it should be commonly available soon (especially if we ask for it before choosing a data center).

**CPU**: The more CPU usage, the more carbon emissions, from [electricity usage](#electricity-usage) and [embodied carbon](#embodied--embedded-carbon)

## co2 metrics

The calculation of carbon emissions comes from https://sustainablewebdesign.org/calculating-digital-emissions/, which in turn comes from [Perspectives on Internet Electricity Use in 2030, Anders S.G. Andrae, June 2020](https://www.researchgate.net/publication/342643762_New_perspectives_on_internet_electricity_use_in_2030).

This calculation only takes in to account the page size, and whether or not the host is using green energy, or offsets. For everything else it uses global average values.

Energy per visit in kWh (E) = Data Transfer in GB x 0.81 kWh/GB

This breaks down as follows:

- Consumer device energy (52%)
- Network energy (14%)
- Data center energy (15%)
- Production energy (19%)

Carbon Emissions are calculated from the energy, by multiplying by 442 g/kWh (global average carbon intensity) or or 50 g/kWh (approximate carbon intensity for renewable energy).

The CPU usage and the data transfer size are calculated using [sitespeed.io](https://www.sitespeed.io/), which in turn uses Chrome. This also calculates the [CPU benchmark](https://www.sitespeed.io/documentation/sitespeed.io/cpu-benchmark/), which is used to normalise the CPU usage, so that analysis done on different computers (or the same computer under differing load) can be usefully compared.
