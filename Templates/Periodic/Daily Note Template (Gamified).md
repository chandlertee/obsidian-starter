---
periodic: daily
---
# <% tp.file.title %>

**Prev Day:** **[[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]]**  
**Next Day:** **[[<% tp.date.now("YYYY-MM-DD", +1, tp.file.title, "YYYY-MM-DD") %>]]**  
**Week:** **[[<% tp.date.now("YYYY-[W]ww", 0, tp.file.title, "YYYY-MM-DD") %>]]**  
___
## Campfire Prep 🔥
#### Inspiration 📜
<% tp.web.daily_quote() %>
#### Blessings 🌟
**What am I grateful for today?**  
- <% tp.file.cursor() %>
#### This Week's Quests
```dataview
task 
from "Journal/Weekly/<% tp.date.now("YYYY-[W]ww", 0, tp.file.title, "YYYY-MM-DD") %>"
```
#### Today's Encounters 🏹
**What can I do today to advance this week's Quests?**  
  - [ ] 
#### Allies 🛡️
 **Who or what can help me today?**  
- 
#### Traps 👹
**What obstacles or distractions should I watch out for?**  
- 

___
## Field Notes 📝
- 

___
## Long Rest 🌙
#### Wisdom 📚
**What did I learn today?**  
- 
#### Boons ⚡
**What gave me energy or helped me?**  
- 
#### Loot 🏆
**What were my wins today?**  
- 
#### Monsters 🐉
**What were the toughest challenges I faced? How did I handle them?**  
- 
#### Growth 🌱
**What can I improve tomorrow?**  
- 

___
## Notes Created Today
```dataview
list 
where file.cday = date("<% tp.file.title %>") and file.name != "<% tp.file.title %>"
sort file.ctime desc
```
