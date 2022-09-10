---
type: dashboard
description: My Personal Journal
banner: "![[journal-banner.jpg]]"
banner_y: 0.26334
banner_icon: 📒
---
---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

<div style="
background-image: url(https://i.ibb.co/fd79Dc8/texture.png);
background-repeat: repeat;
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
font-size: 120px;
font-weight: 800;
font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
text-align: center;"
>JOURNAL</div>

---

```dataview
TABLE name AS "Date",topic AS "Topic"
from #journal 
where file.name != "📒 Journal Entry"
SORT name DESC
```
---
---

