---
periodic: weekly
---
# <% tp.file.title %>

**Prev:** [[<% tp.date.now("YYYY-[W]ww", -7, tp.file.title, "YYYY-[W]ww") %>]]   **Next:** [[<% tp.date.now("YYYY-[W]ww", +7, tp.file.title, "YYYY-[W]ww") %>]]   **Month:** [[<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-[W]ww") %>]]

## Focus
- <% tp.file.cursor() %>

## Daily Notes
- [[<% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 2, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 3, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 4, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 5, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 6, tp.file.title, "YYYY-[W]ww") %>]]

## Reflection
**What did I learn this week?**
- 

**Wins:**
- 

**Next week:**
- 

## Notes Created This Week
```dataview
list 
where file.cday >= date("<% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-[W]ww") %>") 
and file.cday < date("<% tp.date.now("YYYY-MM-DD", 7, tp.file.title, "YYYY-[W]ww") %>") 
and file.name != "<% tp.file.title %>"
sort file.cday desc, file.ctime desc
```
