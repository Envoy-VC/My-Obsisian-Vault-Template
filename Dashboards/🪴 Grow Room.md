---
type: dashboard
description: Dashboard for the Seed Box
banner: "![[grow-room-banner.jpg]]"
banner_y: 0.63666
banner_icon: 🤯
---

---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---

  <div
  style="
    width: 100%;
    text-align: center;
    background-image: linear-gradient(45deg, #553c9a, #ee4b2b);
    font-size: 48px;
    font-weight: 800;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    color: transparent;
    background-clip: text;
    -webkit-background-clip: text;
  "
>
  WELCOME TO
</div>

<div
  style="
    width: 100%;
    font-size: 64px;
    text-align: center;
    border: 1px dashed #dfdcd8;
    color: #fff;
    background-image: linear-gradient(
      to right,
      #23966c,
      #faaa54,
      #e23b4a,
      #db0768,
      #360670
    );
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande',
      'Lucida Sans', Arial, sans-serif;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  ">🪴 Grow Room</div>
  

---

## 🌱 Seed Box

```dataview
table type as "Type", file.ctime as "Planted at", file.mtime as "Last Manicured"
from "Seed Box"
sort file.ctime DESC
limit 5
```

---
---
