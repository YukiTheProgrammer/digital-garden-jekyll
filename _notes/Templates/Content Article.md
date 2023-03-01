---
---

<%*
const URL = await tp.system.prompt("URL?")
const title = await tp.system.prompt("Title?")
const author = await tp.system.prompt("Author?")
const APA = await tp.system.prompt("APA?")
const MLA = await tp.system.prompt("MLA?")
const filetitle = title + ' by ' + author
%>
---
tags: media/article
url: "<% URL %>"
title: "<% title %>"
author: "<% author%>"
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

<% await tp.file.move("/Media/Articles/" + filetitle) %>