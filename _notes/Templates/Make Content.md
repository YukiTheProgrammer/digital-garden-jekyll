---
---

<%* 
const mediatype = await tp.system.suggester(["Album","Article","Book","Film","Journal","Video"], ["Album", "Article","Book","Film","Journal","Video"])

await tp.file.create_new(tp.file.find_tfile("Templates/Content " + mediatype),"","True")
%>