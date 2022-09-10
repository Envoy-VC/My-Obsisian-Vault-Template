---
banner: "https://images.unsplash.com/photo-1507494924047-60b8ee826ca9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1073&q=80"
banner_icon: 
type: dashboard
description: anything stupid that comes to my mind!!
banner_y: 0.52
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

<div
  style="
    width: 80%;
    height: 100px;
    font-size: 64px;
    background: rgb(26,0,36);  
background: linear-gradient(90deg, rgba(26,0,36,0.3267682072829131) 0%, rgba(74,9,121,0.427608543417367) 0%, rgba(246,0,255,0.7105217086834734) 100%);
    padding-left: 16px;
    border-radius: 16px;
  "
>
  🧠 brain dump
</div>

---

```dataview
TABLE Idea AS "Idea", file.mtime AS "Last Modified"
FROM #brain-dump
WHERE file.name != "🧠 New brain dump"
```

---
