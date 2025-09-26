---
title: Magic Item Template
draft: true
aliases:
---
<%* setTimeout(() => { // Get the path to the new file 
const newFile = tp.file.find_tfile(tp.file.path(true)) // Process the frontmatter 
app.fileManager.processFrontMatter(newFile, (frontmatter) => { // Add a new field 
frontmatter.title = tp.file.title
frontmatter.draft = false
// Or delete the properties you don't want 
 }) }, 300) %>###### Up: <%* tR += '[[' + 'Adventure MOC#Magic Items' + '|' + 'Magic Items' + ']]' %> | <%* tR += '[[' + 'Development Stages MOC' + ']]' %>

# <% tp.file.title %>

---Example
_Wondrous Item, Common_

This small, unremarkable leather pouch is similar in appearance to a Bag of Holding. Its interior defies the temporal flow of its surroundings, existing in a bubble that time passes around. Objects placed inside the bag do not experience the passing of time. It can hold up to 25 pounds of weight and 7.5 cubic feet of volume. 

---

#### See Also