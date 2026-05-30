---
periodic: monthly
---
# <% tp.file.title %>

**Prev:** [[<% tp.date.now("YYYY-MM", -1, tp.file.title, "YYYY-MM") %>]]   **Next:** [[<% tp.date.now("YYYY-MM", +31, tp.file.title, "YYYY-MM") %>]]

## Focus
- <% tp.file.cursor() %>

## Weeks
- [[<% tp.date.now("YYYY-[W]ww", 0, tp.file.title, "YYYY-MM") %>]]
- [[<% tp.date.now("YYYY-[W]ww", 7, tp.file.title, "YYYY-MM") %>]]
- [[<% tp.date.now("YYYY-[W]ww", 14, tp.file.title, "YYYY-MM") %>]]
- [[<% tp.date.now("YYYY-[W]ww", 23, tp.file.title, "YYYY-MM") %>]]

## Reflection
**What did I learn this month?**
- 

**Wins:**
- 

**Next month:**
- 

## Notes Created This Month
```dataview
list 
from !"Templates"
where dateformat(file.cday, "yyyy-MM") = "<% tp.date.now("yyyy-MM", 0, tp.file.title, "YYYY-MM") %>"
sort file.cday desc, file.ctime desc
```
