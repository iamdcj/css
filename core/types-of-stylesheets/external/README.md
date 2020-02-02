# External Stylesheets

External stylesheets are stylesheets which are loaded into the document from an external stylesheet file(.css).

External stylesheets are linked to in the head of a document, using the <link /> element.

### Why use them?

External stylesheets are the most popular form of authored stylesheet; they provide separation of concerns by abstracting the stylesheet from the markup.

Stylesheets block page rendering.

--

### Example

This example consists of standard document markup, and within the head element an external stylesheet is loaded via the link element (w/ relationship attribute)

```
<!doctype html>
<html>
  <head>
    <link href=“/styles.css” rel="stylesheet"> />
  </head>

  <body>
  ...
```
