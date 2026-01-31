---
title: "Oasys options"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Oasys options"
---

To enter / view the options click on "Edit - Options". A new window will open with a list of tabs across the top for the various sections.

![](/assets/images/oasys_options_2010.gif)

### Internet

The "Patient Details File" contains the location of your patient details file. This defaults to "My Documents\oasyspatientdetails.opd". If you work alone and on the same computer then you do not need to change this.

If you work with others then you need to share your patient details file with the team. If you work on many computers then you either need to have the patient details file where it can be accessed from all the computers or you need to carry it with you on an encrypted USB stick.

See the section on [Sharing your patient details file](/documentation/sharing-patient-details) for more information.

You can enter a new location for your patient details file here or click on the "..." button to browse.

todo add link to url of the oasys server
The Oasys client also needs to know where to find the Oasys Server. Please see URL of the Oasys Server to find out what this should be. Oasys comes pre installed with the correct value so you should not have to do anything. We do not plan on changing this often / at all. If it does need to be changed for some reason then we will let you know.

### Printing

If you print the report and the pages come out in the wrong order then tick the "Print in reverse order" box and everything should work out.

If you are having trouble printing click on "High Compatibility Printing". This stops Oasys using some of the fancier features that most modern printers have so should work better with older printers.

### Analysis

The options in this section are generally not very interesting to new users so feel free to skip this section. We thought we'd leave them in just in case anybody wanted to use them.

todo add link to daily graph
The Daily Graph of the [Oasys report](/documentation/oasys-report) shows the Oasys scores for each complex (these are the horizontal lines near the top with a number between 1 and 4 in the middle). These can be shown / hidden by clicking "Hide complex scores on the Daily PEF Graph".

todo add link to time of day and time from waking
The Mean 2-Hourly Time OF Day and Time From Waking graphs of the [Oasys report](/documentation/oasys-report) show the 95% standard error of the mean for each point. If you find this distracting it can be shown / hidden by clicking on "Hide Error Bars on Hourly Graphs".

### Serial Plot

These options are quite complicated and we don't recommend use of the serial plot so this section could be skipped as well.

todo add link to serial plot
The Serial Plot (View - Serial plot) shows every measurement that the patient has recorded along with the date and time. It can be very big and very long. The options here allow you to control the size of the graph both on the screen and when printed.

The "On Screen" values control the size of the graph on the screen, and also when printed unless "Use Printer Scaling" is ticked. The "When Printed" values control the size of the graph when printed as long as "Use Printer Scaling" is ticked.

When shown on screen Oasys will divide the serial plot into as many separate graphs as necessary and show them one above the other. "Centimetres per day (X Scale)" controls how wide each day will appear. "Centimetres per Reading (Y Scale)" controls the height of each division (20 l/min). "Days per graph" controls how many days to put on each graph before starting a new graph underneath.

todo add link to serial plot
See the Serial Plot help for more details on this and some examples.

When printed "Days per Page Width" controls how wide each day will appear. Oasys will autosize the days so that the right number fit on the page, so the actual size will depend on the size and orientation of the paper. "Graphs per Page height" controls how high each 20 L/min division will be. Oasys will autosize this in the same way as the days.
