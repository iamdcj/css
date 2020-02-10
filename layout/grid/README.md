# CSS Grid

The grid layout module is a two-dimensional layout system specifically designed to solve common layout problems often seen in web user-interfaces.

It can handle two-dimensional layouts, that is, both rows _and_ columns can be manipulated when developing grid-based layouts. This differs to the `flex` layout system, which only handles one-direction layouts; columns _or_ rows.

### Basic Setup

All grid layouts start by creating a grid container/wrapper - this is accomplished using the `display: grid` declaration.

**HTML**

```
<section class="grid-container"> ... </section>
```

**CSS**

```
.grid-container {
  display: grid
}
```

All direct descendants of the `.grid-container` automatically become 'grid-items'.

**The above is the starting point of all `grid` powered layouts.**

---

#### References

- [Complete Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
