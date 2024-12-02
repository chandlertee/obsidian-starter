---
name: {{name}}
role: {{role}}
team: {{team}}
location: {{location}}
tags: [person, team]
last_updated: {{date:YYYY-MM-DD}}
meetings: []
---
## Details
- **Role:** {{role}}
- **Team:** {{team}}
- **Location:** {{location}}
- **Interests:** {{interests}}
- **Pets:** {{pets}}
- **Preferred Pronouns:** {{pronouns}}

## Recent Meetings
```dataview
table date, type, notes
from "Meetings"
where contains(participants, "{{name}}")
sort date desc
