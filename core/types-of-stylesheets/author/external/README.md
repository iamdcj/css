# External Stylesheets

External stylesheets are stylesheets which are loaded into the document from an external file(`.css`). External stylesheets are the most popular form of authored stylesheet; _they provide separation of concerns by abstracting the stylesheet from the markup_.

External stylesheets are linked to in the `<head />` of a document, using the `<link />` element.

**Stylesheets block page rendering; the browser will stop building the document when it encounters and external stylesheet reference.**

--

### Example

This example consists of standard document markup, and within the head element an external stylesheet is loaded via the link element:

```
<!doctype html>
<html>
  <head>
    <link href=“/styles.css” rel="stylesheet"> />
  </head>

  <body>
  ...
```
