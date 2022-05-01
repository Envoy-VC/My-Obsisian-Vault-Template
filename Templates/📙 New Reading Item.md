---
type: reading
description: A basic structure for a reading source such as a book or article
---

---
**Tags**:: #reading
**Links**:: [[📚 Reading]]
**Format**:: <% tp.system.suggester(["Book", "E-Book", "Article", "Blog Post", "PDF", "Custom"], ["Book", "E-Book", "Article", "Blog Post", "PDF", ""]) %>
**Author**:: 
**ISBN**::
**Status**::


---
<% await tp.file.move("/Library/" + tp.file.title) %>
### Summary
<!-- Enter a brief summary of the book here, this can be copied from a website or a picture from a book jacket -->

### Questions
<!-- What Questions do you want answered by this book? Do you have any assumptions about what you might learn? -->

### Notes
<!-- Notes made from reading -->

### Quotes
<!-- Quotes that can be used later -->

### Conclusions
<!-- Any conclusions drawn from the book -->