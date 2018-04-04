---
layout: post
title: Windows 7 Driver Development for VPN 
info: Developing a driver to use a VPN protocol developed in-house.
tech: C, WDK, NDIS, TCP, WinDBG 
type: Ento
---

## Project Period & Property
Designed and developed by myself and takes about 3 months.


## Background
New development needed to use Windows 7 build-in VPN protocol based on Windows XP.  
When the VPN client is run, the drivers wrap the packets according to the internal VPN protocol and send them to the VPN server.  
Therefor, it is necessary to develop a function to wrap the packet from the driver to the VPN server according to the protocol.  


## Check
- How to implement network driver in Windows 7.
  - Developed by referring to NDIS example of WDK.
    - In Windows XP there was a passthru example for DDK.
    - But, it was changed to WDK after Vista, and the passthru example disappeared.
  - Segment processing for packets exceeding MSS size for TCP.
- How to test and debug using network drivers.
  - Remote debugging with WinDBG is possible because the system may hang when testing the driver.
  - If the VPN client is not working, I should treat it so that it does not wrap packets.


## Technical Summary
- Developed network driver for Windows 7.
- When wrapping packets with the VPN protocol, be careful not to exceed the MSS size.
- In the normal case, the packet is not wrapped.
- Register the callback function appropriately to avoid system panic.


## Content
TBD
