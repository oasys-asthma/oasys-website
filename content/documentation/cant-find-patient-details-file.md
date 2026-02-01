---
title: "Cannot find the patient details file"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Problems reading and writing patient details in Oasys"
---

Oasys stores all personally identifiable information about patients on each users local computer. It is stored in a file called the "Patient Details File".

Oasys creates a patient details file the first time it runs, containing 4 example patients, so you will not normally see these messages unless you change the default options.

The location of your patient details is set in the [Oasys Options](documentation/oasys-options) and defaults to "My Documents\oasyspatientdetails.opd". If you store your patient details file somewhere else (on a network share for example) then set the location in the options.

If Oasys needs to access the patient details file but cannot it will show you a message. You will normally get the chance to cancel whatever you are doing at this point, so that you can change the options if you need to.

If you set the patient details file to something that doesn't exist in the options, then Oasys will create the file next time it needs to change it, and will show you a message beforehand.

If something has gone wrong and you end up with multiple patient details file, you can combine them by [exporting patient details](/documention/exporting-patient-details) and [importing patient details](/documentation/importing-patient-details).