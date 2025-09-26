---
title: Event - Full Template
draft: true
---
<%* setTimeout(() => { // Get the path to the new file 
const newFile = tp.file.find_tfile(tp.file.path(true)) // Process the frontmatter 
app.fileManager.processFrontMatter(newFile, (frontmatter) => { // Add a new field 
frontmatter.title = tp.file.title
frontmatter.draft = false
// Or delete the properties you don't want 
 }) }, 300) %>
 ###### Up: [[index|Home Page]] | [[Timeline]] | [[Development Stages MOC]]

# <% tp.file.title %> 

> [!info]
> - significance: One-line summary of why it matters
> - Alternate name 
> - location: [[Place name]] # optional, prefer a link 
> - date: YYYY-MM-DD # best single-date identifier for the file  
> - start: YYYY-MM-DD # optional  
> - end: YYYY-MM-DD # optional 

## Overview
A 1–3 sentence plain-language summary (
- Location
- Key Figures
- Cause
- Outcome
- Evidence / Sources

## Related

- Full Event it is related too
