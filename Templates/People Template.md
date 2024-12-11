---
name: <% tp.file.title %>
role: 
team: 
location: 
tags: [person]
meetings: []
created: <% tp.file.creation_date() %>
modified: <% tp.file.last_modified_date() %>
---
# <% tp.file.title %>
## Details
- **Preferred Pronouns:** 
- **Interests:** 
- **Pets:** 

---
## Meetings
```dataview
list
from "Meetings"
where contains(participants, "<% tp.file.title %>")
sort file.cdate desc, file.ctime desc
```

 