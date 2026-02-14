---
title: "Pseudo day interpretation"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Pseudo day interpretation / pre processing in Oasys"
---

In basic terms, Oasys looks at a patient's peak flow readings on work days to see if they are worse than their days off. This seems to make a lot of sense.

{{< middle-section-1 >}}

However, if you work in the afternoons then you will take many readings before work. These readings clearly cannot be made any worse by the work on that day, so maybe these should be analysed differently?

Oasys has an option to "Day Interpret" a record into "Pseudo Days", this option is on by default for a record and is recommended. This is entered in the [Interpretation Options](/documentation/choosing-the-interpretation).

{{< /middle-section-1 >}}

Oasys converts / pre processes days into "Pseudo Days". Each Pseudo day is only allowed to contain readings which are subject to an exposure at work, or those which are not. It cannot contain both.

In addition each Pseudo Day must contain a reading within 90 minutes of waking up. These readings are usually the lowest of the day and can bias the results if they are missing. Oasys can copy these readings from nearby days if required.

{{< middle-section-2 >}}

See the [Pseudo Day Interpretation Specification](/documentation/pseudo-day-interpretation-specification) page for more details.

This contains some common examples of how the pseudo day interpreter works, which are fairly easy to understand. It also contains the full specification for the pseudo day interpreter if you want to delve deeper.

{{< /middle-section-2 >}}

If Pseudo Day Interpretation is turned off, Oasys simply compares readings on days at work with readings on days away from work.