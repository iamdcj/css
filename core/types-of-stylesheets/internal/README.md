# Internal Stylesheets

Internal stylesheets are styles which are part of the document, and not loaded from an external stylesheet file.

Internal stylesheets are typically set into the document head.

### Why use them?

They are typically used for critical rendering path styles, or inject by third-party libraries.

--

### Examples

This example consists of standard documemt markup, and within the head element an internal stylesheet is defined

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
