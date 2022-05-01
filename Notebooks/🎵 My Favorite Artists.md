---
banner: "![[music.jpg]]"
banner_y: 0.75333
banner_icon: 🎵
description: My Favourite Artists
---

---
## 🎵 My Favorite Artists
#notebook

---

```dataview
TABLE
	album AS "Favorite Album/Single",
	genre as "Genre"
FROM #artist 
SORT file.name ASC
where file.name != "📔 New Artist"
```
## Go Back to [[📔 Notebooks]]