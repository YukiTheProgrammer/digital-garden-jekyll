#alpha #unprocessed
# A<% tp.date.now("YYYYMMDD")%><% tp.date.now("HHmm")%>
<% await tp.file.rename("A"+tp.date.now("YYYYMMDD")+tp.date.now("HHmm")) %>
### Notes: 
<% await tp.file.cursor() %>
### Beta Note: [[<% (await tp.file.create_new(tp.file.find_tfile("Templates/Beta"),"B"+ tp.date.now("YYYYMMDD")+tp.date.now("HHmm"))).basename %>]]
