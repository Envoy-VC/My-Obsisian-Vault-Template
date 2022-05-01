---
type: dashboard
description: A Dashboard containing all todo lists
banner: "![[backlog.jpg]]"
banner_y: 0.52333
banner_icon: 🪵
---


---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

# Welcome to 🪵 Backlogs


## 🪵 Current Backlog
Your entire backlog is visible
```dataview
table file.ctime as "Planted at" 
from "Backlog"
sort file.ctime DESC
```