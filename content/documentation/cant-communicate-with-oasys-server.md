---
title: "Cannot communicate with Oasys server"
date: 2026-01-22T00:00:00+01:00
draft: false
description: "Problems communicating with the Oasys server"
---

Sometimes Oasys can't communicate with the server, which it needs to do to open records, save records, and so on.

There are only really three reasons why this can happen:

  1. You cannot connect to the internet.
  2. Your firewall is blocking the connection.
  3. The "Url of the Oasys server" is incorrect.
  4. The Oasys server or database is having a problem.

You can use the [connection checker](/documentation/connection-checker) to help work out which one of these is the problem.

### You cannot connect to the internet

In this case the solution is simple, and you need to reconnect to the internet!

### Your firewall is blocking the connection

The Oasys program works fine with the standard Windows Firewall and N3, the NHS Network, but this is still probably the most common problem, especially in strict IT environments, which are common in healthcare settings, for obvious reasons.

If you are asked to allow oautil.exe access in the firewall then please do so. If you still have problems then please talk to your IT department, and let them know they are welcome to get in touch with us via the [Contact](/contact) page to talk things through. 

### The "Url of the Oasys server" is incorrect

It is possible that you have the wrong url for the Oasys Server. We try to change this as rarely as possible, but we do still need to change it sometimes (2 times in 15 years currently).

You can see what the value should be on the [URL of the Oasys Server](/documentation/oasys-server-url) page. Go to the [oasys options](/documentation/oasys-options) and make sure that this value is entered in the "URL of the Oasys Server" box.

If the Url of the Oasys server changes we will email everybody who has used Oasys in the last year to let them know.

### The Oasys server or database is having a problem

This is a rare event, but can happen. You can try again in a few minutes. It is exceedingly rare for the server to be down for any serious length of time, so if you experience this for a long time please contact us via the [Contact](/contact) page to sort things out.

### What about saving my work?

If you cannot connect to the Oasys server you will not be able to open or create any records.

However any records you have open will automatically be saved locally when you to save them, and will be saved to the Oasys server next time you log in.

See [saving local backups](/documentation/saving-local-backups) for more details.
