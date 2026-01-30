---
title: "Editing patient demographics"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Editing patient demographics in Oasys"
---

To enter / view the patient demographics click on "View - Patient Demographics". A new window will open with a list of tabs across the top for the various sections.

![](/assets/images/oasys_patient_demographics_2010.gif)

### Patient Information

Click on the "Patient Info" tab for data about the patient. Only the gender, race and age are sent to the Oasys server. The patient id, name, DOB and height are considered to be personally identifiable so are not sent.

Please enter the patient id, name, date of birth (age is calculated automatically, but can be entered if you don't know the date of birth but do know the age), and the height, race and sex. If the age, sex and height are known click on "Calculate Predicteds" and Oasys will calculate the predicted peak flow.

Oasys calculates the predicted peak flow using the ECCS (European Community for Coal and Steel) regression equations contained in the ARTP/BTS guidelines for the Measurement of Respiratory Function.

### Record Information

Click on the "Record Info" tab for data about this peak flow record. This information is stored on the Oasys Server as it is not personally identifiable.

Choose the type of peak flow meter. If it is not listed choose "Other" and enter the name in the "Meter Name (if Other)" box. If you are not sure "Other linear" is a good default.

Add respiratory related treatments (which could include beta blockers). Please use generic names where possible. Clicking on the "Add" button will pop up a list of treatments. If the one you want is not on the list then click "Other" (at the bottom of the pop up list of treatments) and enter it by hand.

todo add link
You can specify whether there are any confounding factors in the record (such as treatment change, respiratory tract infection etc) if you have checked for this. We advise you to add a comment to a record if you know of any confounding factors (see Adding Comments from the Oasys Report).

Oasys always plots its graphs at the same scale. This is so that users can easily recognise patterns. If the patient's PEF varies a lot you can click on "Show graphs at half normal scale". The scale will be smaller and the graphs will have a watermark so that it is very obvious that the scale has been changed.

### Information about the Workplace

Click on the "Workplace" tab for data about the workplace, including jobs and exposures. This information (apart from the Workplace) is stored on the Oasys Server so please do not enter any details that would identify an individual. This is not likely but there could be occasions where a job / agent is so rare that it is only used by a handful of people.

Please enter a list of Jobs that the patient is doing in this record using the nearby "Add", "Rename" and "Remove" buttons.

Please enter a list of exposures (if there is more than one during the record) using the nearby "Add", "Rename" and "Remove" buttons. For example a patient could be working in multiple locations (say the office and the factory) and be exposed to different agents in these places. Alternatively a patient could work in one location but do multiple jobs (say welding and paint spraying). If you enter different exposures Oasys will analyse them separately.

Please enter the level of exposure. For new records this will usually be "Original". A company will often try to reduce exposure for effected individuals, by providing extraction or by moving the worker to a different location. In this case the exposure would be "Decreased".

Please enter the likely causative agents present in the workplace using the nearby "Add", "Edit" and "Remove" buttons. This does not have to a definitive list but more of a "best guess". For example an office worker will probably be exposed to "cleaning fluids". A paint sprayer will probably be exposed to isocyanates. A solderer will probably be exposed to rosin etc. See adding / editing agents for more details.

If you get confirmation that a particular agent is the cause of a patients occupational asthma we would greatly appreciate you editing the agent to indicate this. Results of Specific IgE tests and Specific Bronchial / Inhalation Challenges also very welcome.

### Information about the peak flow readings

Click on the "Readings" tab for data about the peak flow readings.

You can enter the predicted peak flow by hand here if you know it. Alternatively if the date of birth, sex and height have been entered you can click on "Calculate Predicteds" and Oasys will do it for you. Note that it is usually easier doing this from the "Patient Info" tab.