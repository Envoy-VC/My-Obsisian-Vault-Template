---
type: dashboard
description: A Dashboard for all the Reading Items
banner: "https://images.unsplash.com/photo-1507842217343-583bb7270b66?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1590&q=80"
banner_y: 0.14001
banner_icon: 📚
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

## 📚 Curating A Reading List
Reading is one of the best ways to gather knowledge from multiple sources - reading can be books - in physical and electronic form, magazines, blog posts and articles.

---

## Planned List
This list contains items not yet processed - to remove them from this list set their status to "planned"
```dataview
table author as "Author", format as "Format"
from #reading
where file.name != "📙 New Reading Item"
and status = "planned"
```

---

## In Progress List
Items that are current in progress of being read and reviewed
```dataview
TABLE
	author AS "Author"
from #reading
where file.name != "📙 New Reading Item"
and status = "in-progress"
```

---

## Done
A list of all your finished items
```dataview
table author as "Author", format as "Format", rating as "Rating"
from #reading
where file.name != "📙 New Reading Item"
and status = "done"
```
