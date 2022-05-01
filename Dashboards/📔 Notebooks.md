---
type: dashboard
description: Collection of My Notebooks
banner: "![[notebook.jpg]]"
banner_y: 0.34334
banner_icon: 📔
---
---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---


# Notebooks

```dataview
TABLE description AS "Description"
FROM #notebook
where file.name != "📓 New Notebook"
```
