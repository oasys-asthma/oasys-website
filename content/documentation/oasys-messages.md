---
title: "Oasys messages"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Oasys messages"
---

Oasys often shows a message, when something has gone wrong or to provide extra information.

The descriptions below give some extra information about some of these messages.

If you have some new question which wasn't explained well here please get in touch via the [contact](/contact) page. We will update the descriptions when this happens.

### The Oasys web server has been updated

"The Oasys web server has been updated and will no longer work with this version of Oasys. Please download the latest version of oasys using the link below."

If you receive this error then we have released a new version of the Oasys Server that your current version of Oasys cannot work with. Please [install the latest version of Oasys](/install).

There is no need to worry, none of your records or personal details will be lost. Apologies for the inconvenience, we will try to make breaking changes as rarely as possible.

### Unexpected error

If this happens then there is a problem with Oasys or with the data, please contact us via the [Contact](/contact) page to sort things out.

### Could not open record

The Oasys server always expects to be able to open a record. However there may well be unforseen circumstances where this does not happen. The following error message can be returned by the Oasys server.

- Unexpected Error: Oasys cannot find this record in the database

Our very sincere apologies for this. Unfortunately the company which host The Oasys Server had a problem and lost all of our data, including all of the backups, despite us paying for a bare metal backup service. We managed to find a backup from another source but we still lost about 6 months worth of data, from March 2015 to July 2015. You are almost certainly receiving this message because you are trying to open a record that has been lost. Once again, we are very sorry about this. We are now doing our own backups on top of the ones our hosts do, and are now hosting in Microsoft Azure.

### Could not save record

If you can connect to the Oasys Server it should be possible to save any record. However there may be unforseen circumstances where this does not happen. The following error messages can be returned by the Oasys server. If one of these happens then there is a problem with Oasys or with the record, please contact us via the [Contact](/contact) page to sort things out.

- File caused an unknown error during opening. The error returned was: ...
- Invalid XML: serialspirometryrecord node missing.
- Invalid XML: demographic node missing.

### Record Saved Successfully

When a record is saved successfully the Oasys Server will sometimes return a message with some information / warnings that you may wish to do something about. The messages that can be returned are explained below.

#### Cannot save the patient details file, unable to save record: ...

This message is returned when the Oasys client cannot save the patient details file. There will be an error message with some more information as to why it could not be saved. The record will have been saved on the internet in this case but any changes to the patients personal details will not have been saved. You can click on "Edit - Options" and then on the "Internet" tab to tell Oasys where the patient details file is stored. We have seen the following problems cause this error

- The patient details file is on a network drive that is no longer available
- The patient details file is on a usb stick that is not plugged in
- The patient details file is in a location that the current user does not have permission to use.

#### Unusual problems

The following errors can be returned in exceptional conditions. Your record has still been largely saved but some data may be missing. If one of these happens then there is a problem with Oasys or with the record, please contact us via the [Contact](/contact) page to sort things out.

Cannot convert Pef reading (...) for blow ...
(and similar messages for FEV1, FEV3 etc)

Invalid work exposure found in file for work period starting at ... Work Exposure reset to ...

Invalid XML ...