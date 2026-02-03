---
title: "Setting the interpretation as recommended"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "How to enable to recommended interpretation in Oasys"
---

The "Scores" part of the [Oasys Report](/documentation/oasys-report) (on the [conclusions](/documentation/conclusions) page) will sometimes show a warning if the "interpretation" is not as recommended. This is not a big problem and you can happily ignore it. If you want to correct the situation click on the "Set as recommended" button next to the text. See the documentation on [Pseudo Day Interpretation](/documentation/pseudo-day-interpretation) for more information

Oasys will try and set the interpretation and if everything works fine the report will update and the warning will be removed. If there are problems Oasys will show a message with the problems and solutions. Possible messages are listed below. When you have made the changes, click the "Set as recommended" button again.

> Oasys needs to know which type of peak flow meter the patient used. Please click "View - Patient Demographics" to type this in and try again.

Some older meters used non linear scale. Thus a reading of 200 was not exactly double that of 400. Oasys corrects these readings so that they are linear (like modern meters). In order to make sure that the readings are linear, Oasys needs to know the type of meter used. If you do not know the type of meter then you will not be able to correct the problem. See the help on [patient demographics](/documentation/patient-demographics) for more information on entering the type of meter. Setting the meter to "Other Linear" is a good default if you're not sure.

> The events ("Wake Up", "Start Work" etc) are not in the correct order. Please click "View - Data Sheet" to make corrections. The record must start with a "Wake Up" event and finish with a "Go To Bed" Event. Once in the data sheet you can click on "Additional - Go to next invalid event" and Oasys will show you roughly where the problem is. Keep doing this until the "Additional - go to next invalid event" option is greyed out and then try again.

In order to "Pseudo Day Interpret" a record Oasys needs to know when the patient sleeps and works. This is all typed in using the [data sheet](/documentation/data-sheet). The record must start with a "Wake up" (W) and end with a "Go to bed" (B). All other events must follow in a logical order. For example a "Start work" can't come after a "Go to bed", as the patient is still asleep! The data sheet can take you to the problem events by clicking on "Additional - Go to next invalid event". Note that Oasys often takes you to the event after the problem, so you should always look at the previous event as well.

> In order to perform "Pseudo Day Interpretation" Oasys needs to have readings within 90 minutes of waking up. This record does not have enough of these. This is not an issue that can be fixed, so its best not to worry about it. The results are nearly as good even without the "Pseudo Day Interpretation".

Oasys needs a certain number of waking readings to "Pseudo Day Interpret" a record. If there are not enough of these then there is nothing that can be done. When instructing patients to perform serial peak flow records be sure to emphasize the importance of taking readings shortly after waking up.