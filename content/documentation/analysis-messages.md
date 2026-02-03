---
title: "Analysis warnings and errors"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Warnings and errors in the Oasys analysis"
---

Oasys will sometimes display one or more of the following messages when analysing a record (in order to show The [Oasys Report](/documentation/oasys-report) for example). Please read on for some more details about these messages.

### The events (W, S, E, B) for this patient are not in the correct order. Please return to the Data Sheet and make corrections.

If the events for a record (Wake Up, Start Work, End Work and Go To Bed) are missing or are not in the correct order Oasys will not be able to [Pseudo Day Interpret](/documentation/pseudo-day-interpretation) the record. Incorrect waking events will mean that The []"2 Hourly" Time from Waking Graphs](/documentation/time-from-waking-graphs) will not be accurate. Incorrect work events mean that Oasys will not be able to analyse the differences between work and days off properly (which is the basis for all the Oasys scores and the diagnosis of occupational asthma). If this is the problem open The Data Sheet and make corrections. Records must start with a Wake Up event and finish with a Go To Bed Event. The [data sheet](/documentation/data-sheet) page has more information about finding and correcting events that are in the wrong order.

### There is no data for this patient for this interpretation.

This can happen if no data has yet been entered for a patient, or if the entire record has been excluded (see [adding comments](/documentation/adding-comments) for excluding all / part of a record).

### The record has more than 2000 days (ie. more than 5 years long).

Displaying the report would cause Oasys to go very slowly so Oasys doesn't do it. If you "Pseudo Day Interpret" the record any gaps in the record will be removed so you won't see this message. If the record really is this long please split it into separate records.

It takes a long time to draw The [Daily Maximum, Minimum and Mean Graph](/documentation/daily-graph) for very long records so Oasys will not analyse records that are 5 years long or more. This is not a limit that we expect to be a practical problem! It can happen if you have mistakenly put in a reading in 1899 (the dawn of time from the point of view of Oasys) and then added readings with the correct date. If this record is Pseudo Day Interpreted Oasys will cut out the (roughly 100 year) gap between these readings and it will not be a problem. If the record is Solar interpreted then Oasys would display every day of this time frame on the daily graph. To fix this problem simply correct the problem readings. In the very unlikely scenario that you have a record which has more than 5 years of data please split the record into two. This can be done by creating a new record for the same patient and then using the data sheet to copy and paste the readings and events.

### The record has an unfeasibly large range of values (from [...] to [...]).

This would cause Oasys to go very slowly so is not allowed. Please return to the [data sheet](/documentation/data-sheet) to make corrections.

It also takes a long time to draw the graphs for extremely large variations in peak flow. This will never be a practical consideration (a range of 2000 l/min is allowed) and must be due to a problem with the data, please return to the the Data Sheet to modify the offending readings. Blows outside the 95% confidence interval for the record are shown in bold in the data sheet so are easy to spot.

### Could not day interpret this file. There are no [rest / work] waking readings. The solar interpretation is used instead.

[Pseudo Day Interpretation](/documentation/pseudo-day-interpretation) requires each Pseudo Day to have a waking reading. If there is no waking reading then one can be copied from a nearby day. If there are no waking readings to copy then Oasys cannot Pseudo Day Interpret the record. The record can still be analysed and this message is just for information, there is nothing that can be done about it. When asking patients to perform serial peak flow records it is important to stress the need to do a blow as soon after waking up as possible, and always within 90 minutes.

### The interpretation is not as requested. The interpretation used is shown on the toolbar and in the interpretation window.

This warning is shown when Oasys tries to Pseudo Day Interpret a record (which is the default) but is unable to do so, this could be because the events are in the wrong order, or there were no waking readings. In this case Oasys will use Solar "Interpretation" instead. The "interpretation" is shown on the status bar of the program (at the bottom right of the main window in Oasys) and on the [Choosing the "Interpretation" window](/documentation/choosing-the-interpretation). If you have fix the problem that is stopping Oasys from Pseudo Day Interpreting the record you will need to return to the Choosing the "Interpretation" window and tick the "Pseudo Day Interpret" box again.