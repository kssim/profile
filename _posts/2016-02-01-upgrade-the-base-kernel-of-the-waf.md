---
layout: post
title: Upgrade the base kernel of the Web Firewall 
info: Upgrading the Debian-based kernel. 
tech: Debian, Kernel, C, Quilt
type: Penta 
---

## Project Period & Property
Designed and developed by myself and takes about 3 months.


## Background
We were using Debian 6 as the base kernel in our Web Firewall.  
By the way, Debian 6 was EOL in February 2016.  
So, We were working on changing the base kernel to Debian 8.   


## Check
- Apply changes made in Debian 6 based kernel to Debian 8.
- Major changes in Debian 8.
- Easier deployment of modified base kernels.


## Technical Summary
- Change the OS of the Web Firewall based on kernel 3.16
- Apply the patches of existing customized kernel and fix conflicts (use quilt)
- Create an ISO image to deploy the modified kernel (using debian-installer, simple-cdd, debian-cd, APT server)


## Content
TBD
