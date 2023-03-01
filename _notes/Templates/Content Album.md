---
---

<%*
const title = await tp.system.prompt("Title?")
const artist = await tp.system.prompt("Artist?")
const year = await tp.system.prompt("Year?")
const filetitle = "(" + year + ") " + title + " by " + artist 
%>
---
tags: media/album
title: "<% title %>"
artist: "<% artist %>"
year: <% year %>
---
# <% filetitle %>
### Quick Summary:
<% await tp.file.cursor() %>
### Reminds me of:

### Mentioned in the following notes:
```dataview
list from [[<% filetitle %>]]
```

<% await tp.file.move("/Media/Albums/" + filetitle) %>