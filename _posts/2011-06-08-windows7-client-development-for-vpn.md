---
layout: post
title: Windows 7 Client Development for VPN 
info: Develop a client to connect to a VPN server. 
tech: C#, DLL, HSSP, .NetFramework, UAC
type: Ento
---

## Project Period & Property
Designed and developed by myself and takes about 2 months.


## Background
I needed to re-create the client based on .NetFramework to create a VPN client on Windows 7.  
New client has improved VPN line switching algorithm on Windows XP based client.  


## Check
- Efficient programming method based on .NetFramework.
  - Develop client using C#.
  - Delegate the driver-related part to the .NetFramework.
- User access control after Windows Vista.
  - Since Windows Vista, the UAC policy has been added so the program does not automatically run with administrator privilieges.
  - I need administrator priviliege to communicate with the driver and modify network settings.
  - Modifying the manifest file to elevate permissions after build.
- HSSP (Hot Stand by Switching Protocol).
  - A proprietary protocol for communication between the driver and the client.
  - Check speed with VPN server to help switch to faster VPN line.
  - Proper algorithms are needed to prevent wasted switching.


## Technical Summary
- Develop Windows 7 client using C# and .NetFramework.
- Modify manifest file to bypass UAC policy.
- Developed "Hot Stand by Switching Protocol".


## Content
TBD
