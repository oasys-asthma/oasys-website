---
title: "Sharing patient details"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Sharing patient details in Oasys"
---

No personal details are ever sent to or stored on the Oasys Server. Instead Oasys stores all personally identifiable information about patients locally. It is stored in a file called the "Patient Details File". All the non identifiable data is stored on the Oasys website. See the section on [Data Protection](/documentation/data-protection) for more information.

The default location for this file is "My Documents\oasyspatientdetails.opd". If you only work on one computer and you do not need to give anyone else access to your records then the default will work well.

If you work with a number of people and everyone needs to be able to access the Oasys records then you will need to share the patient details file.

We recommend that you place the patient details file on a network location that is shared by all users. Every user will then need to enter this location in the [oasys options](/documentation/oasys-options) so that Oasys knows where to find the file.

If you already have a patient details file then you can copy it to this new location. If not just set the desired location in the options and Oasys will create the file the first time that it needs to use it.

You can [export](/documentation/exporting-patient-details) and [import patient details](/documentation/importing-patient-details) if you need to combine patient details files (for example, if there is a merger, or a new starter uses their own patient details file before becoming aware of a shared one.)