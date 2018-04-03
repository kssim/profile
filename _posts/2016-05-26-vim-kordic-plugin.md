---
layout: post
title: vim-korDic plugin
info: The vim plugin is a program that translates English words into Korean.
tech: "Python, Vim, vim-nox, HTML parse"
type: Toy
---

## Project Period & Property
Designed and developed by myself and takes about 1 month.  
It's a toy project.  


## Background
When I use vim, I often have to translate English into Korean.  
So, I created a plugin for vim so that I could translate it into simple command in vim.  


## Check
- How to create to a vim plugin.  
  - There were serveral ways, but using vim-nox was the simplest.  
  - Using vim-nox did not develop native plugins for vim.  
    - So I need additional packages and some functional limitations, but this is negligible.  


## Technical Summary
- Create a Python plugin available in vim using vim-nox.  
- Translate the words I want to search for on web, which provides dictionary services.  
- Parses translated words from the web and displays a new window on vim's screen.  
- The HTML parsing library depends on the version of Python, so implemented to support all.  


## Content
Develop vim plugin in Python using vim-nox.  
Python queries the protal site for word searches and parses the query results.  
Display the results fo the search in a new window of vim.  

It's simple to use. Place the cursor on the word you want to search for, and type the command to translate the word.  


## Link 
[vim-korDic github](https://github.com/kssim/vim-korDic)
