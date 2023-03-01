---
---

<%*
const title = await tp.system.prompt("Title?")
const creator = await tp.system.prompt("Creator?")
const url = await tp.system.prompt("Url?")
const filetitle =  title + " by " + creator
%>
---
tags: media/video
title: "<% title %>"
creator: "<% creator %>"
url: "<% url %>" 
---
# <% filetitle %>
### Quick Summary:
<% tp.file.cursor() %>
### Reminds me of:

### Mentioned in the following notes:
```dataview
list from [[<% filetitle %>]]
```
<% await tp.file.move("/Media/Videos/" + filetitle) %>
