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
A 1–3 sentence plain-language summary (first lines appear in previews).

## When

- Start: YYYY-MM-DD
- End: YYYY-MM-DD
- Time of day / season: optional

## Where

- Primary location: [[Place name]]
- Other locations: [[Place2]], nearby regions

## Key figures

- [[Person A]] — role/brief note
- [[Person B]] — role/brief note

## Cause  
Short statement of immediate trigger(s).

## Course  
Bulleted sequence of the main actions/events (keep to the essentials).

## Outcome  
Short statement of the immediate result.

Consequences / Long-term effects

- Political:
- Cultural:
- Magical / supernatural:
- Economic:

## Evidence / Sources

- Source short name or artifact: note/link
- Oral tradition: summary

## Related

- [[Battle note / Law / Treaty]]
- #timeline or link to parent event