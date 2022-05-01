---
banner: ""
effectiveness: 
name : <% tp.date.now("DDMMYYYY") %>
feelings: 
---

<% await tp.file.move("/Daily Log/" + tp.file.title) %>
<% await tp.file.rename(tp.date.now("DDMMYYYY")) %>

<% tp.web.random_picture("3840x2160", "landscape,nightcity,space") %>

---

**Tags**:: #daily
**Links**::[[📓 Daily Note]]

---

# <% tp.date.now("DDMMYYYY") %>

## Effectiveness : 
## H20💦 (bottles) :
## Tasks Done : 
## 🌈 I feel : 
## 🗓 Date : <% tp.date.now("Do MMMM YYYY") %>
---
```button
name Add to-do
type append text
action - [ ]
```
^button-m066

---
## Anything About Today...


---
---
