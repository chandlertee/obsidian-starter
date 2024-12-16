---
periodic: weekly
---
# <% tp.file.title %>

**Prev Week:** **[[<% tp.date.now("YYYY-[W]ww", -7, tp.file.title, "YYYY-[W]ww") %>]]**
**Next Week:** **[[<% tp.date.now("YYYY-[W]ww", +7, tp.file.title, "YYYY-[W]ww") %>]]**
**Month:** **[[<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-[W]ww") %>]]**
___
## Quest Prep ⚔️
#### This Month's Adventures
```dataview
task 
from "Journal/Monthly/<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-[W]ww") %>"
```
#### Quests 🏹
**What can I do this week to advance this month's Adventures?**
- [ ] <% tp.file.cursor() %>
#### Allies 🛡️
 **Who or what can help me this week?**  
- 
#### Traps 👹
**What obstacles or distractions should I watch out for?**  
- 

___
## Long Rest 🌙
#### Wisdom 📚
**What did I learn this week?**  
- 
#### Boons ⚡
**What gave me energy or helped me?**  
- 
#### Loot 🏆
**What were my wins this week?**  
- 
#### Monsters 🐉
**What were the toughest challenges I faced? How did I handle them?**  
- 
#### Growth 🌱
**What can I improve next week?**  
- 
#### Blessings 🌟
**What am I grateful for this week?**  
- 

___
## Daily Notes
- [[<% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 2, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 3, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 4, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 5, tp.file.title, "YYYY-[W]ww") %>]]
- [[<% tp.date.now("YYYY-MM-DD", 6, tp.file.title, "YYYY-[W]ww") %>]]

___
## Notes Created This Week
```dataview
list 
where file.cday >= date("<% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-[W]ww") %>") 
and file.cday < date("<% tp.date.now("YYYY-MM-DD", 7, tp.file.title, "YYYY-[W]ww") %>") 
and file.name != "<% tp.file.title %>"
sort file.cday desc, file.ctime desc
```
