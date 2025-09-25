---
title: New and Recent Files
draft: false
aliases:
---

###### Up: [[index]] | [[Development Stages MOC#**Low Priority**]]

---

# [[New and Recent Files]]

## New Files

%% DATAVIEW_PUBLISHER: start
```dataview
    TABLE dateformat(file.ctime, "MM/dd/yy") + " - " + dateformat(file.ctime, "hh:mm a") as "Last Modified"
    FROM ""
    SORT file.ctime DESC
    LIMIT 10

```
%%
%% DATAVIEW_PUBLISHER: end %%

## Recent Files

%% DATAVIEW_PUBLISHER: start
```dataview
    TABLE dateformat(file.mtime, "MM/dd/yy") + " - " + dateformat(file.mtime, "hh:mm a") as "Last Modified"
    FROM ""
    SORT file.mtime DESC
    LIMIT 10

```
%%
%% DATAVIEW_PUBLISHER: end %%

### *Subheading*

---

