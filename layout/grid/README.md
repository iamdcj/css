# CSS Grid

The grid layout module is a two-dimensional layout system specifically designed to solve common layout problems often seen in web user-interfaces.

It can handle two-dimensional layouts, that is, both rows _and_ columns can be manipulated when developing grid-based layouts. This differs to the [`flex`](../flex) layout system, which only handles one-direction layouts; columns _or_ rows.

### **When to Use**

Like `flex`, `grid` is a tool for laying-out content is a certain way, and based on what you need to achieve `grid` could be the right tool for the job.

A good rule of thumb is to reach for `grid` whenever you need to align on both the x and the y axes, otherwise [`flex`](../flex) should do the job.

### Explicit vs. Implicit Grid

If the developer doesn't _explicitly_ configure the grid layout, i.e. doesn't stipulate the rows and/or columns, the browser will implicitly generate an implicit grid layout.

### **Basic Setup & Terminology**

All `grid` powereder layouts consist of two main things; a [grid container](./structure/_container), and at least one [grid item](./structure/item) within the container.

```
<section class="grid-container">
  <div class="grid-item>
  <div class="grid-item>
  <div class="grid-item>
</section>
```

**The above is the starting point of all `grid` powered layouts**, which contains:

- **grid container**
  - > **grid-items**.

---

#### References

- [Complete Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
