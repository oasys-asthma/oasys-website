---
title: "Pseudo day interpretation specification"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Specification for pseudo day interpretation / pre processing in Oasys"
---

### Primary Aim

The primary aim of day interpretation is to create pseudo days in which all the peak flow readings are either all exposed or all non-exposed. Additionally each pseudo day must contain exactly one waking reading.

The key concept is that a patient can feel the effects of exposure after being exposed but cannot possibly feel the effects before exposure. Hence a waking reading for a work pseudo day needs to be after the exposure, i.e. from the following day.

{{< middle-section-1 >}}

### Secondary Aims

This method of day interpretation was produced after discussion with experts and tries to agree with an expert interpretation. The rules are complex and not easily readable. Hence the application of the rules in various situations is described below.

{{< /middle-section-1 >}}

### Night shifts

When a patient goes on to a night shift from resting there is often a large time between them waking up and going to work. The rules will make a rest pseudo day out of this time if it is long enough (which is common).

When a patient goes on to a night shift from a day shift there is often a large time between the end of exposure from the day shift and the start of exposure on the night shift. The rules will make a rest pseudo day out of this time if it is long enough (which is common).

When a patient comes off a night shift (at say 6am) there is usually a period awake on that day after they have woken up (at say 11am), some of which may still be affected from the night shift exposure. The rules make a rest pseudo day from the time when it is likely that readings are unaffected by exposure until the patient returns to bed, but only if this time is long enough (which does happen but is not so common).

{{< middle-section-2 >}}

### Working

When a patient is working a constant shift for a number of days all readings are normally said to be exposed. The rules usually create work pseudo days from one time of starting work to the next.

{{< /middle-section-2 >}}

### Resting

When a patient is resting for a number of days all readings are said to be non-exposed. The rules create rest pseudo days from after a waking reading through to after the next waking reading.

Please read the full [day interpretation specification (pdf)](/assets/pdfs/oasys-day-interpretation.pdf) for more details.