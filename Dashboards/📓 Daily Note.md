---
banner: "![[daily log.jpg]]"
banner_y: 0.43
banner_icon: 🖋️
type: dashboard
description: A Dashboard for Daily Logs
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

# 🖋 Daily Log

```button
name New
type command
action Create new note
color purple
```
^button-s2mb

---

```dataview
TABLE WITHOUT ID
	("[[" + name + "]]") AS "File",
	effectiveness AS "Effectiveness",
	feelings AS "🌈 I feel"
	
FROM "Daily Log"
SORT file.name DESC
```
