---
title: Dataview - Alphabetical - MOC List Template
draft: true
aliases:
---

# Dataview - Alphabetical - MOC List Template

<%*  
const activeFile = app.workspace.getActiveFile();  
if (!activeFile) throw new Error("No active file open.");

let fileBase = (typeof activeFile.basename === "string") ? activeFile.basename : null;  
if (!fileBase) {  
fileBase = activeFile.name.replace(/.[^/.]+$/, "");  
}

const fileText = await app.vault.read(activeFile);  
const allLines = fileText.split("\n");

const headings = [];  
for (let i = 0; i < allLines.length; i++) {  
const line = allLines[i];  
const match = line.match(/^\s*(#{1,6})\s*(.+?)\s*$/);  
if (match) {  
headings.push({  
text: match[2],  
level: match[1].length,  
line: i  
});  
}  
}

let chosenHeading = null;  
if (headings.length > 0) {  
const displays = headings.map(h => `${"#".repeat(h.level)} ${h.text}`);  
const values = headings.map(h => h.text);  
chosenHeading = await tp.system.suggester(displays, values, "Pick a heading (top → bottom)");  
} else {  
chosenHeading = await tp.system.prompt("No headings found in this file. Enter heading text to search for:");  
}

if (!chosenHeading) throw new Error("No heading selected.");

const safeHeading = chosenHeading.replace(/]]/g, "] ]");  
const linkTarget = fileBase + "#" + safeHeading;

tR += '%% DATAVIEW_PUBLISHER: start\n';
tR += '```dataview\n'; tR += 'list from ""\n'; tR += 'where contains(file.outlinks, [[' + linkTarget + ']])\n'; tR += 'sort file.name asc\n'; tR += '```\n';  
tR += '%%\n';  
tR += '%% DATAVIEW_PUBLISHER: end %%\n';
%>