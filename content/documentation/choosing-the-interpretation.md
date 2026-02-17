---
title: "Choosing the interpretation"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "How to choose how Oasys pre processes the record before analysis"
---

Oasys "Interprets" / pre processes the raw serial peak flow data before analysis. The default options will rarely need changing.

If you do wish to change the "Interpretation" options then click "Edit - Interpretation" and a new window will pop up.

![](images/oasys_interpretation_options_2010.gif)

### Exclude Marked Ranges

Oasys allows you to remove parts of a record (for example, if the patient is ill for 3 days of a 4 week record, it is possible to remove these 3 days). See the section on [adding comments](/documentation/adding-comments) for more details on how to do this.

Oasys does not actually delete the peak flow measurements, but instead "Marks" them. During the "Interpretation" these marked ranges are temporarily removed to do the analysis. If you would like to look at the results with these ranges included then make sure that this box is unticked. This can be useful to see how much effect the illness (in this example) is having on the results.

{{< middle-section-1 >}}

### Pseudo Day Interpret

Oasys uses [Pseudo Day Interpretation](/documentation/pseudo-day-interpretation) to pre process / group all readings into "Pseudo Days", where the peak flow measurements in a Pseudo Day are either all subjected to the work exposure, or all not subjected to the work exposure. Each Pseudo Day must also include a reading within 90 minutes of waking up, as this is usually the lowest reading of the day and can bias the results (although this value can be copied from nearby days). More details are available on the dedicated Pseudo Day Interpretation Page.

We recommend the use of Pseudo Day Interpretation, where possible. However you can turn it off by unticking the "Pseudo Day Interpret" box.

{{< /middle-section-1 >}}

### Work Exposures

Oasys recommends that you indicate any variation in exposures that a patient may have whilst at work. For example a patient could be working in multiple locations (say the office and the factory) and be exposed to different agents in these places. Alternatively a patient could work in one location but do multiple jobs (say welding and paint spraying). These are entered on the [patient demographics](/documentation/patient-demographics) window and the [data sheet](/documentation/data-sheet).

The [Oasys report](/documentation/oasys-report) will always include some analysis of the different exposures in a record, however the bulk of the report only analyses the ticked work exposures. Any exposures that are not considered to be exposed to the suspected causative agent should be unticked in this list.