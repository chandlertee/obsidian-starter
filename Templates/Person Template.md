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

## Mentions
```dataview
TABLE without id
file.link as "Note", file.cday as "Date"
FROM !"Templates" AND !"Meetings"
where contains(file.outlinks, [[]])
SORT file.cday DESC
```

## Tasks
```dataview
task
where contains(text, "<% tp.file.title %>")
```

## Meetings
```dataview
TABLE without id
file.link as "Meeting", file.cday as "Date"
FROM "Meetings" 
where contains(file.outlinks, [[]])
SORT file.cday DESC
```
