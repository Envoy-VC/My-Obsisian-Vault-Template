---
type: dashboard
description: Collection of My Notebooks
banner: "![[notebook-banner.jpg]]"
banner_y: 0.34334
banner_icon: 📔
---
---
**Tags**:: #dashboard
**Links**::[[📰 Dashboard]]

---


<span
  style="
    font-size: 64px;
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
  ">NOTEBOOKS</span>
  

```dataview
TABLE description AS "Description"
FROM #notebook
where file.name != "📓 New Notebook"
```
