---
title: "Creating a new record"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Creating a new record in Oasys"
---

To create a new serial peak flow record click "File - New Record (on Oasys Server)". A new wizard will open to guide you through the various sections.

![](images/oasys_new_internet_record_2010.gif)

### Choosing the patient

First of all enter the start date of the record on this step. There are no problems if this is left out, although it can make things confusing. If you need to you can change it later from the data sheet by clicking on "Additional - Move / Set Start Date"

A list of patients from your patient details file is shown. If you have already entered a previous record for the patient then click on the patient in the list. The list can be sorted by ID, First name and surname by clicking on the headings. You can also type in a name or patient id and the list will go to the next match as you type.

If the list is unexpectedly empty, or the patient is not in the list and you think it should be, then there is probably an issue with your patient details file. See [sharing your patient details](/documentation/sharing-patient-details) for more information.

If this is the first record for the patient then click on "This is the first record I have entered for this patient".

If you choose an existing patient some information is automatically be copied into the new record. The name, id, date of birth, height and workplace will all be copied in from your patient details file. The jobs, causative agents, treatments, race, sex and level of exposure are copied from the previous record.

{{< middle-section-1 >}}

### Warnings

If you have chosen an existing patient Oasys may add some warnings for things you may want to check. For example if jobs have been added from a previous record it is a good idea to check that these are still the same. If there are no warnings the wizard will skip this step.

{{< /middle-section-1 >}}

### Patient Demographics

The patient demographics are available on the "Patient Info", "Record Info", "Workplace" and "Reading" steps. Please see the help on the [Patient Demographics](/documentation/patient-demographics) window for more details about these as they are (nearly) identical.

When you have finished entering the demographic details for the record click on "Finished" to create the record.