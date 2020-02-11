# The `max-content` Unit

The `max-content` unit will expand a box to the 'natural' size of its containing content.

### Text

If we take a chunk of text, place it within an element

```
<p>I am David Christian Jones. I do the codes.</p>
```

then cap the width of the element to an arbritrary size:

```
p {
  width: 50px;
}
```

the content will break based on width of its wrapping element

```
----------------
I am David
Christian Jones.
 I do the codes.
----------------
```

If we adjust the pixel value to `max-content`;

```
p {
  width: max-content;
}
```

the width of the paragraph will grow to the largest size possible based on the text within;

```
-------------------------------------------
I am David Christian Jones. I do the codes.
-------------------------------------------
```
