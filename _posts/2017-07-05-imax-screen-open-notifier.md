---
layout: post
title: IMAX Screen Open Notifier
info: Create bots that send slack notifications when the theaters begin to book.
tech : "Python, HTML, Slack API, HTML parse"
---

## Project Period & Property
Designed and developed by myself and takes about 1 week.  
It's a toy project.  


## Background
There was a lot of competition to make reservations at large multiplexes that show IMAX.  
Because it is the largest IMAX movie theater in Korea, seats and reservations were fierce.  
So I made a feature that would let me know if IMAX reservations were avaliable.  


## Check
- How to check the IMAX ticket reservation time.
  - Does not provide any additional functions on the multiplex homepage.
  - So must parse html directly.
- How to notify to me.
  - Set to notify via slack API.


## Technical Summary
- Periodic monitoring work.
- HTML parsing.
- Slack API interlock.


## Content
Periodically check the reservation status on the multiplex homepage.  
Parses the query results to see if there are new reservations.  
If available, send a notification via slack API.  
