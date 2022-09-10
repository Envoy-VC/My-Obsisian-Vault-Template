---
banner: "https://images.unsplash.com/photo-1501785888041-af3ef285b470?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80"
banner_icon: ✈
type: dashboard
description: My travel Guide.
banner_y: 0.36334
---

---
**Tags**:: #dashboard
**Links**:: [[⚛️ Life]]

---


<div style="
background-image: url(https://i.ibb.co/PMR2St6/wave.png);
background-repeat: repeat;
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
font-size: 120px;
font-weight: 800;
font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
text-align: center;
letter-spacing: 8px;"
>TRAVEL</div>
---

```dataview
TABLE Destination,Start-Date AS "Start Date", End-Date AS "End Date", Duration, Status
FROM #travel
WHERE file.name != "✈ New Travel Entry"
```




