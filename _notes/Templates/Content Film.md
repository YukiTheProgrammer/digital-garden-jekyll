---
---

<%*
const title = await tp.system.prompt("Title?")
const year = await tp.system.prompt("Year?")
const filetitle =  "(" + year + ") " +  title
%>
---
tags: media/film
title: "<% title %>"
year: "<% year %>" 
---
# <% filetitle %>
### Quick Summary:
<% tp.file.cursor() %>

### Reminds me of:

### Mentioned in the following notes:
```dataview
list from [[<% filetitle %>]]
```
<% await tp.file.move("/Media/Films/" + filetitle) %>
