---
layout: post
title:  Windows XP based driver and client maintenance
info: Windows XP based driver and client maintenance 
tech: C, DLL, HSSP, WinAPI, DDK, NDIS
type: Ento
---

## Project Period & Property
Improvements and bug fiexs for about 10 months.


## Background
"ENTO Networks" used Windows XP based client as its main product.  
Until the next version development, we had to improve and maintain the product.  
 

## Check
- HSSP (Hot Stand by Switching Protocol).
  - A proprietary protocol for communication between the driver and the client.
  - Check speed with VPN server to help switch to faster VPN line.
  - Proper algorithms are needed to prevent wasted switching.
- How to test and debug using network drivers.
  - Remote debugging with WinDBG is possible because the system may hang when testing the driver.
  - If the VPN client is not working, I should treat it so that it does not wrap packets.


## Technical Summary
- Register the callback function appropriately to avoid system panic.
- Improved HSSP algorithm.


## Content
TBD
