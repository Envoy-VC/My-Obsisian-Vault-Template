---
type: dashboard
description: Dashboard for the Seed Box
banner: "![[grow-more.jpg]]"
banner_y: 0.63666
banner_icon: 🤯
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

## Welcome to 🪴 Grow Room

The 🪴 Grow Room is your inbox on current 🪵 Backlog Items, and [[🌱  Seeds]] you have created but not yet curated.

---

## 🪵 Current Backlog
Your entire backlog is visible
```dataview
table file.ctime as "Planted at" 
from "Backlog"
sort file.ctime DESC
```

---

## 🌱 Seed Box - 5 Latest Items
🤨 Should these still be here?
```dataview
table type as "Type", file.ctime as "Planted at", file.mtime as "Last Manicured"
from "Seed Box"
sort file.ctime DESC
limit 5
```

## 🌱 Seed Box - All Items
All Items in the Seed Box
```dataview
table type as "Type", file.ctime as "Planted at", file.mtime as "Last Manicured"
from "Seed Box"
sort file.mtime DESC
```

