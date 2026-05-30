---
periodic: monthly
---
# <% tp.file.title %>

**Prev Month:** **[[<% tp.date.now("YYYY-MM", -1, tp.file.title, "YYYY-MM") %>]]**
**Next Month:** **[[<% tp.date.now("YYYY-MM", +31, tp.file.title, "YYYY-MM") %>]]**
**Weeks:** **[[<% tp.date.now("YYYY-[W]ww", 0, tp.file.title, "YYYY-MM") %>]]**, **[[<% tp.date.now("YYYY-[W]ww", 7, tp.file.title, "YYYY-MM") %>]]**, **[[<% tp.date.now("YYYY-[W]ww", 14, tp.file.title, "YYYY-MM") %>]]**, **[[<% tp.date.now("YYYY-[W]ww", 23, tp.file.title, "YYYY-MM") %>]]**
**Quarter:** **[[<% tp.date.now("YYYY-[Q]Q", 0, tp.file.title, "YYYY-MM") %>]]**
___
## Adventure Prep ⚔️
#### This Quarter's Campaigns
```dataview
task
from "Journal/Quarterly/<% tp.date.now("YYYY-[Q]Q", 0, tp.file.title, "YYYY-MM") %>"
```
#### Adventures 🏹
**What can I do this month to advance this quarter's Campaigns?**
- [ ] <% tp.file.cursor() %>
#### Allies 🛡️
 **Who or what can help me this month?**  
- 
#### Traps 👹
**What obstacles or distractions should I watch out for?**  
- 

___
## Long Rest 🌙
#### Wisdom 📚
**What did I learn this month?**  
- 
#### Boons ⚡
**What gave me energy or helped me?**  
- 
#### Loot 🏆
**What were my wins this month?**  
- 
#### Monsters 🐉
**What were the toughest challenges I faced? How did I handle them?**  
- 
#### Growth 🌱
**What can I improve next month?**  
- 
#### Blessings 🌟
**What am I grateful for this month?**  
- 
