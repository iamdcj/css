# minmax

The `minmax` unit provides a powerful, function-like syntax for stipulating the narrowest and widest widths a grid item can be.

This feature allows us to build responsive layouts without always reaching for media queries.

```
grid-template-columns: 1fr minmax(200px, 2fr);
```

The above snippet uses `minmax` to set the second column width to:

- `min`: a minimum of `200px`
- `max`: a maximum of `2fr`
