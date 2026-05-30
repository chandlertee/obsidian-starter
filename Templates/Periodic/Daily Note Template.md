---
periodic: daily
---
# <% tp.file.title %>

**Prev:** [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]]   **Next:** [[<% tp.date.now("YYYY-MM-DD", +1, tp.file.title, "YYYY-MM-DD") %>]]   **Week:** [[<% tp.date.now("YYYY-[W]ww", 0, tp.file.title, "YYYY-MM-DD") %>]]

## Focus
- <% tp.file.cursor() %>

## Notes
- 

## Reflection
**What did I learn today?**
- 

**Wins:**
- 

**Tomorrow:**
- 

## Notes Created Today
```dataview
list 
where file.cday = date("<% tp.file.title %>") and file.name != "<% tp.file.title %>"
sort file.ctime desc
```
