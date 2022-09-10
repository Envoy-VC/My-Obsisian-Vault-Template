---
banner: "![[daily-log-banner.jpg]]"
banner_y: 0.43
banner_icon: 🖋️
type: dashboard
description: A Dashboard for Daily Logs
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

  <div
    style="
      background-image: linear-gradient(45deg, #553c9a, #ee4b2b);
      font-size: 72px;
      font-weight: 800;
      font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
      color: transparent;
      background-clip: text;
      -webkit-background-clip: text;
    "
  >
    DAILY LOG
  </div>

---

<span
  style="
    font-size: 48px;
    text-shadow: 1px 0px 1px #ccc, 0px 1px 1px #eee, 2px 1px 1px #ccc,
      1px 2px 1px #eee, 3px 2px 1px #ccc, 2px 3px 1px #eee, 4px 3px 1px #ccc,
      3px 4px 1px #eee, 5px 4px 1px #ccc, 4px 5px 1px #eee, 6px 5px 1px #ccc,
      5px 6px 1px #eee, 7px 6px 1px #ccc;
    font-weight: bold;
    color: #a8a095;
  ">SEPTEMBER</span>



```dataview
TABLE
	file.cday AS "Created At"
	
FROM "Daily Log"
WHERE file.cday.month = this.file.mtime.month
SORT file.ctime DESC
```

---

<span
  style="
    font-size: 48px;
    text-shadow: 1px 0px 1px #ccc, 0px 1px 1px #eee, 2px 1px 1px #ccc,
      1px 2px 1px #eee, 3px 2px 1px #ccc, 2px 3px 1px #eee, 4px 3px 1px #ccc,
      3px 4px 1px #eee, 5px 4px 1px #ccc, 4px 5px 1px #eee, 6px 5px 1px #ccc,
      5px 6px 1px #eee, 7px 6px 1px #ccc;
    font-weight: bold;
    color: #a8a095;
  ">AUGUST</span>


```dataview
TABLE
	file.cday AS "Created At"
	
FROM "Daily Log"
WHERE file.cday.month + 1 = this.file.mtime.month
SORT file.ctime DESC
```
---
---


