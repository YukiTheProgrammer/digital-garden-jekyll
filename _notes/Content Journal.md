---
title: "Content Journal"
---
<%*
const DOI = await tp.system.prompt("DOI?")
const title = await tp.system.prompt("Title?")
const APA = await tp.system.prompt("APA?")
const MLA = await tp.system.prompt("MLA?")
const filetitle = title
%>
---
tags: media/journal
doi: "<% DOI %>"
title: "<% title %>"
---
# <% filetitle %>
### Quick Summary:
<% tp.file.cursor() %>
### Basic:
<% filetitle %>
### APA:
<% APA %>
### MLA:
<% MLA %>

### Reminds me of:

### Mentioned in the following notes:
```dataview
list from [[<% filetitle %>]]
```

<% await tp.file.move("/Media/Journals/" + filetitle) %>