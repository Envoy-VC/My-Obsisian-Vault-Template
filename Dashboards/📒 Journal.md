---
type: dashboard
description: My Personal Journal
banner: "![[journal.jpg]]"
banner_y: 0.26334
banner_icon: 📒
---
---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

## Journal

```dataview
TABLE name AS "Date",topic AS "Topic"
from #journal 
where file.name != "📒 Journal Entry"
SORT name DESC
```
