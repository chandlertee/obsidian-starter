---
company: 
team: 
role: 
location: 
email:
aliases:
---
# [[<% tp.file.title %>]]

## Details
- **Preferred Pronouns:** 
- **Interests:** 
- **Pets:** 

## Notes
- 

```dataview
table rows.Details as "Mentions"
from !"Templates"
where contains(log, "<% tp.file.title %>")
flatten log as Details
where contains(Details, "<% tp.file.title %>")
group by file.link as Note
sort rows.file.day desc
```
___

### Tasks
```dataview
task
where contains(text, "<% tp.file.title %>")
```
---

## Meetings
```dataview
TABLE without id
file.link as "Meeting", file.cday as "Date"
FROM "Meetings" 
where contains(file.outlinks, [[]])
SORT file.cday DESC
```
