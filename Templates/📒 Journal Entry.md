---
banner: ""
type: journal
description: My Personal Journal
name: <% tp.date.now("DD-MM-YYYY") %>
topic: 
---

---
**Tags**:: #journal
**Links**:: [[📒 Journal]]

---

<% await tp.file.move("/Journal/" + tp.file.title) %>

---

## Back to [[📒 Journal]]