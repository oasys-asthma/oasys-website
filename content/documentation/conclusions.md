---
title: "Oasys report conclusions"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "The conclusions section of the Oasys report"
---

Click on the "Conclusions" tab of the [Oasys report](/documentation/oasys-report) to access the Conclusions part of the report.

### Patient Details

todo add link to setting interpretation as recommended probably 
This section shows the name, patient id, dates of the record, peak flow meter used, level of exposure, workplace, jobs, predicted peak flow, treatments and agents. Most of this is entered in the [patient demographics](/documentation/patient-demographics) window. It also shows the "Interpretation". We recommend [Pseudo Day Interpretation](/documentation/pseudo-day-interpretation) and it is the default, however it is not always possible, see the Setting the "interpretation" as recommended page for more details.

### Quality


This section starts off by stating whether the record is of optimal quality for Oasys and quotes the published specificity and sensitivity for the level of quality. Click to view the [paper that defines sensitivity and specificity for the different levels of quality](/assets/pdfs/eopefdqodsasioa.pdf).

The quality for the ABC score and timepoint score follow.

If the record is "sloping" (either improves or deteriorates throughout the record) Oasys will tell you how much the record is sloping in L/Min/Day. The Oasys scores do not work very well with high angles of slope. We remove any records with a >5 L/Min/Day slope from our research projects and we are reluctant to diagnose records with more than 2 or 3 L/Min/Day. Oasys can only detect an average slope, and sometimes records are sloping for good reasons. For example a patient on holiday for 2 weeks followed by work for 2 weeks would be expected to slope downwards during the record if he was worse at work. Some human decision making is required here.

todo add link to number preference
Oasys checks the record for number preference, to detect rounding to the nearest 50 or 25. If the patient has made up a large number of readings this can usually be spotted by eye. Oasys displays number preference graphs to help with this. See the section on number preference for more information.

Oasys checks the record for signs of respiratory tract infections. These are shown on the [Daily Graph](/documentation/daily-graph) and can be excluded from the record or commented on by [adding a comment](/documentation/adding-comments). The dates of any possible respiratory tract infections are shown on the report.

The detecting of infections is not perfect, it should be used as a guide that something should be checked, rather than a definitive answer in itself.

Oasys shows the number of reading outliers. These are readings outside of the 95% confidence interval for the record. These should all be checked if possible. If the record has been entered by hand it is possible that typing errors have been made. If the record has been downloaded from an electronic meter it is possible that friends and family of the patient "had a go" with the meter. Readings that are found to be wrong should be corrected or removed. Note that records will always have some perfectly valid readings outside of the confidence interval. This function just highlights readings that are worth checking. These readings are shown in bold on the [data sheet](/documentation/data-sheet) and can be removed from there. Once all readings have been checked click on "Check All" to indicate that you have done so. A new form will pop up allowing you to enter some comments.

### Diurnal Variation

We don't think that diurnal variation is a very useful measure, but other people do so we have included it. The top line of this table shows whether the denominator for the diurnal variation is the predicted peak flow or the mean of all the readings in the record. The rows show the minimum, mean and maximum diurnal variation for each type of day. The table below shows higher diurnal variation on days at work.

![](/assets/images/oasys_diurnal_variation_table.gif)

### Work Exposures

If you have added multiple work exposures to the record then Oasys will add a table with some information about them. The mean of all peak flows for a particular exposures is subtracted from the mean of all peak flows on days off (we think this is the best measure to use when there is only a small amount of data to analyse). The higher the number the more likely that a particular exposure is causing a problem. The value is shown as a percentage of the predicted peak flow if it is available or in L/Min otherwise. A value of >3.3% of predicted or >15L/Min is indicative of occupational asthma, as long as there is enough data. The number of work days for each exposure is also shown so that you can make this judgement. If there are some exposures that do not seem to be causing any problem you should go to the [Interpretation Options](/documentation/choosing-the-interpretation) and untick these exposures. Oasys will reanalyse the record calling these rest days (they are not rest days, but they are unexposed days).

The example below shows two exposures which both appear to be a problem, although there is not that much data for each. This would suggest that the patient is exposed to the same causative agent in both locations, which could provide a clue as to what the problem agent is.

![](/assets/images/oasys_work_exposure_table.gif)

### Scores

Oasys first displays any opinions that have been entered for the record. Although the Oasys scores are very good, they should not replace the expert opinion, which is why any opinions are shown first. This is particularly important when there are confounding factors which have not been taken into account by the computer scoring. See the section on [adding opinions](/documentation/adding-opinions) to find out how to do this.

The Oasys-2 score for the record is then shown, in bold, along with a percentage chance of occupational asthma based on the score and the quality of the record. This is a summary of information already in the Quality section. We think its important!

Following this a warning is shown if there is no predicted peak flow for the record. You should enter the predicted peak flow if you can (this involves knowing the sex, height and age of the patient and is entered from the [patient demographics](/documentation/patient-demographics)).

Following this the various Oasys scores are listed, along with the percentage chance of occupational asthma based on the score and quality. Click to view the published papers defining these percentages for the [ABC score](https://journal.chestnet.org/article/S0012-3692(09)60117-3/abstract) and the [Timepoint Score](https://thorax.bmj.com/content/64/12/1032?keytype=ref&ijkey=C6PCKKBVIubUcoD).

