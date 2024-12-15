---
periodic: weekly
---
# <% tp.file.title %>

**Prev:** **[[<% tp.date.now("YYYY-[W]ww", -7, tp.file.title, "YYYY-[W]ww") %>]]**
**Next:** **[[<% tp.date.now("YYYY-[W]ww", +7, tp.file.title, "YYYY-[W]ww") %>]]**
**Month:** **[[<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-[W]ww") %>]]**

___
## Battle Prep ⚔️
#### Main Quests 🏹
**What can I do this week to advance this month's Epic Quests?**
- [ ] <% tp.file.cursor() %>
#### Side Quests 🗡️
**What can I do to support my Main Quests?**
- [ ] 
#### Allies 🛡️
 **Who or what can help me this week?**  
- 
#### Enemies 👹
**What obstacles or distractions should I watch out for?**  
- 

---
## Save Point ⏳ 
#### XP 🎮
**What did I learn or improve upon this week?**  
- 
#### Power-Ups ⚡
**What gave me energy or helped me?**  
- 
#### Achievements 🏆
**What were my wins this week?**  
- 
#### Boss Fights 🐉
**What were the toughest challenges I faced? How did I handle them?**  
- 
#### Level Up ✨
**What do I want to focus on leveling up next week?**
- 
#### Gratitude 💖
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

---
## Notes Created This Week
```dataview
list 
where file.cday >= date("<% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-[W]ww") %>") 
and file.cday < date("<% tp.date.now("YYYY-MM-DD", 7, tp.file.title, "YYYY-[W]ww") %>") 
and file.name != "<% tp.file.title %>"
sort file.cday desc, file.ctime desc
```
