# The `min-content` Unit

The `min-content` unit will expand a box to the 'natural' size of its containing content.

### Text

If we take a chunk of text, place it within an element

```
<p>I am David Christian Jones. I do the codes.</p>
```

then cap the width of the element to an arbritrary size:

```
p {
  width: 200px;
}
```

the content will break based on width of its wrapping element

```
----------------
I am David Christian Jones.
I do the codes.
----------------
```

If we adjust the pixel value to `min-content`;

```
p {
  width: min-content;
}
```

the width of the paragraph will shrink to the size of the longest word;

```
----------
I am
David
Christian
Jones.
I do the
codes.
----------
```
