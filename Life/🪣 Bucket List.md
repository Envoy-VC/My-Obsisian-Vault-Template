---
banner: "![[bucket list.jpg]]"
banner_icon: 🪣
type: dashboard
description: My Bucket List
banner_y: 0.52667
---

---
**Tags**:: #dashboard #life 
**Links**::[[⚛️ Life]]

---

# Bucket List

```dataview
TABLE
	why AS "Why?",
	stage AS "Status"
FROM #bucket-list 
where file.name != "🪣 New Bucket List"
```
