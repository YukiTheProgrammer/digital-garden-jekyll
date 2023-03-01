# Indexes


## Film
```dataview
table title, year
from #media/film 
sort title asc
where file.name != "Content Film"
```
## Album
```dataview
table title, artist, year
from #media/album 
sort title asc
where file.name != "Content Album"
```
## Video
```dataview
table title, creator
from #media/video  
sort title asc
where file.name != "Content Video"
```
## Book
```dataview
table title, author
from #media/book 
sort title asc
where file.name != "Content Book"
```
## Journal
```dataview
table title, author
from #media/journal  
sort title asc
where file.name != "Content Journal"
```
## Article
```dataview
table title, author
from #media/article
sort title asc
where file.name != "Content Article"
```
