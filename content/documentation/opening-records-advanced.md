---
title: "Opening records in advanced mode"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Exploring more powerful options to open records in Oasys"
---

The "Opening Records" window defaults to opening in "Simple" mode, where it shows all your records in a long list and you can just click on the record that you want to open. If you work with a large number of records this list can become a bit cumbersome, in this case, click on the "Advanced" button and the window will convert into advanced mode. In this mode you can search for records using the methods below. 

![](images/oasys_open_from_internet_2010.gif)

### Searching for records

Searching by Patient ID

- Click on the "PID" tab
- Enter all or part of a patient id
- Click "Go"
- Matching records are found from your patient details file

Searching by Name

- Click on "Name" tab.
- Enter all or part of the first name
- Enter all or part of the surname
- Click "Go"
- Matching records are found from your patient details file
- If you have entered a surname and a first name then only patients that match both names will be found.

Searching by Company

- Click on the "Company" tab
- Enter all or part of the company name
- Click "Go"
- Matching records are found from your patient details file

Searching for a list of Patient ID's

- Click on "PID List"
- Enter a list of Patient IDs, separated by spaces, tabs, or returns (if you have a list in a word or excel document you should just be able to paste it in).
- Click "Go"
- Matching records are found from your patient details file

Searching by Date

- Click on "Date"
- Enter a start date and an end date
- Click "Go"
- Matching records are found from your patient details file

Searching for records you have entered

- Click on "Mine"
- Click "Go"
- Records you have created are found from the Oasys Server and returned
- Information from your patient details file is matched up with these records and displayed
- Records that have "no data" for the name and id exist in the database but not in your patient details file. You will not be able to open these records. You will need to find the patient details file that you were using when you created these records in order to open them. This could happen if you are working on a different computer from usual.

### Creating a list of records

By default Oasys creates a new list of records every time you do a search (this is the "Start a new list" option in the middle of the window).

If you click "Add to list" any results from subsequent searches will be added to the list of results.

If you click "Remove non matching items from list" the list will only show records that are already in the list and that are returned by the next search.

If you click "Remove matching items from list" the list will only show records that are already in the list but are not returned by the next search.

This probably sounds a bit confusing, so here is a quick example.

- Patient "1" has 10 records, one a year for 10 years.
- You search by patient id and the 10 records are listed
- You click "Remove non matching items from list"
- You search by date for 01/01/2003 to 01/01/2005
- The list now shows the 2 records for this patient in 2003 and 2004 (these two records were returned by the search and were in the list, everything else was not returned by the search and were hence "non matched" and were removed).
- You could do the opposite by clicking on "Remove matching items from list" instead, which would give you all records except the ones in 2003 and 2004.

### Actually opening the records

To open a single record in the list you can double click it, or single click it and then click "Open".

You can select multiple records in the list by left dragging an area with the left mouse button or by holding down Shift or Ctrl while single clicking. This is standard Windows behaviour. To open all the selected files click "Open". The screenshot below shows 3 selected records.
