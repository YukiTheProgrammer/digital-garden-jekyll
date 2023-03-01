---
---

<%*
const title = await tp.system.prompt("Title?")
const tag = await tp.system.suggester(["idea", "term"], ["idea", "term"]) 
%>
#gamma/<% tag %> #seedling
# <% title %>
<% await tp.file.rename(title) %>
### Notes:
<% await tp.file.cursor() %>
### Related to:
1. 
### Sources:
1. 
### Mentioned in:
```dataview
list from [[<% title %>]]
```
### Beta Notes:
1. 

