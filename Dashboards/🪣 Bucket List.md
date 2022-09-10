---
banner: "![[bucket-list-banner.jpg]]"
banner_icon: 🪣
type: dashboard
description: My Bucket List
banner_y: 0.24
---

---
**Tags**:: #dashboard #life 
**Links**::[[⚛️ Life]]

---

<div style="
background-image: url(https://i.ibb.co/nkZsx7p/Untitled-design-1.png);
background-repeat: repeat;
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
font-size: 120px;
font-weight: 800;
font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
text-align: center;"
>BUCKET LIST</div>
---

```dataview
TABLE
	why AS "Why?",
	stage AS "Status"
FROM #bucket-list 
where file.name != "🪣 New Bucket List"
```
---
---
