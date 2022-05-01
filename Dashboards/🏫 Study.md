---
banner: "https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
banner_icon: 🏫
type: dashboard
description: My Study Dashboard
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

## Dashboard Info

You can [[👩‍🌾 Gardening Tips/🪴 Sowing Your Garden/🎯  Create Custom Dashboards|🎯 Create Custom Dashboards]] easily using the `dataview` plugin and SQL-like query language.

---

## All Current Dashboards
```dataview
table description as "Description" 
where type = "dashboard"
sort file.name ASC
```