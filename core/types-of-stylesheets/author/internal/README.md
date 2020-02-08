# Internal Stylesheets

Internal stylesheets are styles which reside in the `<head />` of an HTML document, and not loaded from an external stylesheet file.

Internal stylesheets are not render blocking, making them the place [critical rendering path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css) styles.

--

### Examples

This example consists of standard document markup, and within the `<head />` element an internal stylesheet is defined:

```
<!doctype html>
<html>
  <head>
    <style>
      p {
        color: red;
      }
    </style>
  </head>
  <body>
  ...
```
