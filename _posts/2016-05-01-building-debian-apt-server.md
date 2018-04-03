---
layout: post
title:  "Building Debian APT Server"
info: "Building Debian APT Server."
tech: "Debian, Bash, APT, aptly"
type: Penta
---

## Project Period & Property
Designed and developed by myself and takes about 2 weeks.


## Background
Debian provides APT server as a repository for uploading and downloading packages.  
This APT server is supported by multiple mirror servers, but when the distribution becomes EOL, the server disappears.  
Of course, you can get packages from an archived server, but not all packages.  
So I built an APT server in-house, mirrored the external package server, took a snapshot and managed it.  


## Check
- Reviewing libraries to build APT server.
  - reprepro and ftparchive, aptly, etc...
  - Considering the purpose and technical difficulty, aptly was appropriate.


## Technical Summary
- Building APT server using [aptly](https://www.aptly.info/).
- Build mirror server with aptly and snapshot management.
- Separate the accounts of Linux server, build mrror server and in-house package upload server.
- Develop upload script to make package management easy for in-house upload server.



## Content
I built a server with Debian, and installed aptly and related libraries.  
And I split up the accounts and made it possible to upload in-house packages with 80 ports in one account.  
In other accounts, I mirrored the external APT server to port 8080, created a snapshot and served it.  
Finally, I created a script to make it easy to upload files to in-house APT server.  
This allows you to process package uploads and server updates at once.
