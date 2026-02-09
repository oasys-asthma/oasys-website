---
title: "Entering spirometry / peak flow readings"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "How to enter spirometry and event readings in Oasys using the Data Sheet"
---

The data entry sheet is used to enter peak flow readings, times of waking, starting work, ending work and sleeping and the type of exposure whilst at work. The data sheet is opened by clicking 'View - Data Sheet'. The graphs on the right hand side of this window require downloaded graph data from an electronic meter, and currently, all the ones Oasys supports have been discontinued.

![](/assets/images/oasys_open_from_internet_2010.gif)

{{< middle-section-1 >}}

### Importing readings from Electronic meters

If you are using a meter that Oasys supports then the readings can be read in automatically and all you have to do is enter the Event Times (see below).

To import the readings click on the button at the bottom left of the data sheet. A new window will appear. Click on "Import readings ...".

See [Importing Readings from the eMini Wright](/documentation/e-mini-wright) for more details.

{{< /middle-section-1 >}}

### I have made a mistake, do I really need to type it all in again?

No! See the "Copy / Paste etc" section below. Events and readings can be copied and pasted separately in case they are out of sync. Gaps can be inserted into records if you have missed a day. The entire record can be moved to a new start date if this is wrong. Gaps can be removed from records if this is a problem.

{{< middle-section-2 >}}

### Entering the Peak Flow Measurements

Peak flow readings are entered simply by typing in the peak flow in the required box. If the "x 10" box is ticked then any readings under 60 or 90 will be multiplied by 10. This means that only two digits of the three need to be entered in almost all cases. Eg 56 as opposed to 560.

With practice hand entry is quick. It is designed to be done with the numeric key pad on the right hand side of a conventional keyboard. The right hand enters the numbers for the readings and presses the "Enter" or "+" keys to enter events (see below). The left hand presses the arrow keys to go to the time of the next reading / event.

{{< /middle-section-2 >}}

### Suspect Measurements

If you suspect that a reading is incorrect it is possible to exclude the reading from the analysis. You can still see the reading in the data sheet. Click on the reading and then click on "Additional - Exclude / Comment on Blow". A new window will appear where you can enter your name and a comment, along with the status for the blow. If you set the status to "Checked and Bad" the reading will be excluded from the analysis.

Readings where the status has been set or that have a comment are displayed in italics in the datasheet. Readings that will be excluded are in Italics and Strikethrough.

{{< middle-section-3 >}}

### Entering Event Times (working, sleeping)

The Symbols (![](/assets/images/WakeUp16.ico), ![](/assets/images/StartWork16.ico), ![](/assets/images/EndWork16.ico), ![](/assets/images/GoToBed16.ico))  are used to signify the "Waking Up", "Starting Work", "Ending Work" and "Going To Bed" events.

Events are entered by pressing the plus key or the enter key in the required box. Oasys automatically puts in the next logical event (Eg. after going to bed the next event must be to wake up). If this is not the desired event then press plus or enter again until the correct event is shown, or until the event is removed (if you wish to delete it).

Oasys doesn't like it when the events for a record are in the wrong order and it will show you lots of nasty messages. A record must start with a "Wake Up" Event and continue until a "Go To Bed" event. An "End Work" can only come after a "Start Work", a "Wake Up" can only come after a "Go To Bed" and so on. Oasys can tell you which events it doesn't like. Click on the "Additional" button and then click on "Go To Next Invalid Event" from the menu that pops up. The screen and cursor will move to the next event that Oasys doesn't like. Often the real problem is with the event before this one so be sure to look at that one as well. Repeat this until the events are all in the correct order.

{{< /middle-section-3 >}}

### Navigation

The up and down arrow keys move forward and backward one hour. Page Up goes forward one hour and Page Down goes forward two hours. Holding down Ctrl and a number will jump to the next hour (eg "Ctrl - 9" will move forward to the next 9 o' clock, am or pm depending on the current position). Navigating past the end of the screen will cause the screen to move forward one day, the reverse is true moving before the start of the screen.

The buttons in the bottom left corner of the screen can be used to go to the start of the record, go back a week, go back a day, go forward a day, go forward a week and go to the end of the record.

{{< middle-section-1 >}}

### Work Exposures

Each period at work can be given a particular exposure, which Oasys will analyse separately. For example if a patient spends some time working in the office and some time on the factory floor it would be sensible to analyse these two separately, as the exposures are probably different. This can also be true of a patient doing two different types of job in the same area.

Whenever a "Start Work" event is entered it is automatically assigned the default exposure. If this is not applicable then click on the up and down arrows by the work exposure description (at the bottom left of the window) to select the correct one. You can also hold down the "Ctrl" key and press the up and down arrow keys to change the work exposure. Changing the work exposure can only be done having when youy are "inside" a work period. This exposure continues until the next "End Work" event. If a patient has two (or more) exposures in the same shift add an "End Work" to mark the end of one exposure and a "Start Work" to mark the start of the new exposure.

Work exposures are added / modified / removed from the [patient demographics](/documentation/patient-demographics).

The screenshot earlier shows two different work exposures, one marked in blue and the other with orange. The first day is also orange but has been selected for copy / paste (see below) so is shown in a darker shade.

{{< /middle-section-1 >}}

### Copy / Paste etc

You can select portions of the record by holding down the left mouse button while dragging the cursor. The screen will move forwards and backwards if you go off the end of the screen. You can also highlight by holding down "Shift" while using the keyboard arrow keys. The selected part of the record will go a darker colour, as in the screenshot below.

Once you have made a selection you can copy it "Edit - Copy", cut it "Edit - Cut" or delete it "Edit - Delete". When cutting or deleting you can choose to remove readings, events or both. You can also specify whether readings and events after the selection (if any) should stay where they are or be shifted back to take up the space being vacated.

Once you have something on the clipboard you can paste ("Edit - Paste"). The records will go in at the current point. You can choose to paste readings, events or both. You can also specify whether any readings and events after the current point should stay where they are or be moved forward to make way for the pasted data.

If the start date of the record is wrong click on "Additional" and then "Move / Set start date" from the menu that pops up. Enter a new date and the entire record will be moved to start at this point. This is particularly useful if you forget to enter the start date of the record initially.

You can also "Additional - Insert Hour" to shift everything after the current point forward by an hour. Similar things can be done for "Delete Hour", "Insert Day" and "Delete Day".

### Fiddly Stuff

Readings and events are usually entered to the nearest hour, but can be put in more precisely if required, using the triangular button to the left of the readings and to the right of the events. Simply click on the grey triangle next to the reading or event and drag it up and down to set the time.

If "Overlap" is shown in a box (only "Overl" is initially visible) then there is more than one reading within the hour. Holding the mouse over the box will list the readings. When this happens with events (waking up, going to bed, starting work, stopping work) the WSEB symbol is shown (![](/assets/images/OverlapEvents16.ico)). Holding the mouse over the symbol will display list all these events.

Readings shown in bold are outside of the 95% confidence interval for the record. Note that as more readings are added to a record the 95% confidence interval will change so it is best to review these readings once you have finished typing in the data.

If there is a gap in the record where the patient has not taken any readings you can add a discontinuity and Oasys will effectively ignore it. This is only worth doing for gaps that are a day long or more. To do this add a "Wake Up" event at the start of the gap. Than move to the next hour down and click "Additional - Insert Discontinuity", then add a "Go To Bed" event at the end of the gap. The discontinuity is marked using the (![](/assets/images/Discontinuity16.ico)) symbol.
