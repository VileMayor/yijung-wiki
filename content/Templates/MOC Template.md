---
title: MOC Template
draft: true
aliases:
---
<%* setTimeout(() => { // Get the path to the new file 
const newFile = tp.file.find_tfile(tp.file.path(true)) // Process the frontmatter 
app.fileManager.processFrontMatter(newFile, (frontmatter) => { // Add a new field 
frontmatter.title = tp.file.title
frontmatter.draft = false
// Or delete the properties you don't want 
 }) }, 300) %>###### Up: <%* tR += '[[' + 'index' + ']]' %> | <%* tR += '[[' + 'Development Stages MOC' + ']]' %>
---

# <% tp.file.title %>

## **Heading**

### *Subheading*

---

