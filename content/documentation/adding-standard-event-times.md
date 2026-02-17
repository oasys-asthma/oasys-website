---
title: "Adding standard event times"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "How to add routine event times in Oasys (wake up, start work, end work, go to bed)"
---

If you are entering a record where the event times (waking up, starting work, ending work and going to bed) are always the same then Oasys can add the events automatically for you. Note that it is usually easier to enter the events by hand.

For example a patient might always start work at 9am and always finish work at 5pm and always work Monday to Friday.

To start click on "Tools - Add standard event times", a new window will open with a list of tabs across the top for the various sections.

![](images/oasys_add_standard_event_times_2010.gif)

The options default to adding no events, so you must set some of the options for something to happen.

Note that there is no undo function in Oasys yet so it is worth checking that everything looks right before adding the events.

{{< middle-section-1 >}}

### General

This tab has options for adding events when some of the events have already been entered. If you have not yet entered any events you can ignore these options.

"Always add Events" will add the events you specify to every day, even if there already is an event for that day. This could result in getting two of the same events on the same day, which you would need to correct in the data sheet.

If a patient ends work at 5pm on every day apart from Fridays (when it is 4pm) you could enter the end work events on Fridays and then "Add Standard Event Times". Clicking on "Only add an event if the day does not already have one" will stop Oasys from adding another end work event on Fridays.

If a patient works 9am - 5pm every day but takes a one week holiday during the record, you could enter the Wake Up and Go To Bed events for the holiday and then "Add Standard Event Times". Ask Oasys to add Start Work and End Work events only (more on this later) and click on "Only add events if there are no other events for this day". Oasys will add Start Work and End Work events for all days except the holiday.

You can "Add Standard Event Times" more than once for complicated scenarios.

{{< /middle-section-1 >}}

### Work Days

Clicking on "Add work days to certain days of the week" allows you to tick which days Oasys should add Start Work and End Work events to.

Clicking on "Add work events in a pattern" is for patients that work a certain number of days, and then have a certain number of days off. For example, many of our patients work a 4 days on, 3 days off pattern. "Consecutive Work Days" controls how many days a patient works for before having a break (4 in the example). "Consecutive Rest Days" controls how many days off a patient has (3 in the example). Having 5 "Consecutive Work Days" and 2 "Consecutive Rest Days" would correspond to a standard Monday to Friday working pattern.

If you have added multiple work exposures in the patient demographics you can specify which exposure Oasys should use when adding work events. Simply type in the name of the work exposure in the box at the bottom. If you wish to add more than one exposure you can "Add Standard Event Times" twice and use different options.

{{< middle-section-2 >}}

### Wake Up

Tick "Add Wake Events" to tell Oasys to add Wake Up events, at the time specified by the "At this time" box. If "Remove Existing Wake Events" is ticked any existing Wake Up events will be removed.

{{< /middle-section-2 >}}

### Start Work

Tick "Add Start Work Events" to tell Oasys to add Start Work events, at the time specified by the "At this time" box. Ticking the "Or after the wake event if it is later" will force Oasys to move the Start Work event after the Wake Up event, even if this means changing the default time specified in the "At this time" box.

If "Remove Existing Start Work Events" is ticked any existing Wake Up events will be removed.

{{< middle-section-3 >}}

### End Work

Tick "Add End Work Events" to tell Oasys to add End Work events, at the time specified by the "At this time" box. If "Remove Existing End Work Events" is ticked any existing End Work events will be removed.

{{< /middle-section-3 >}}

### Go To Bed

Tick "Add Go To Bed Events" to tell Oasys to add Go To Bed events, at the time specified by the "At this time" box. If "Remove Existing Go To Bed Events" is ticked any existing Go To Bed events will be removed.
