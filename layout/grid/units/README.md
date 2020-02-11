# The 'fr' Unit

The `fr` unit is a fraction unit; it asssess the number of items in a `grid` container, and determines the fractional size for each item based on the container width.

**CSS**
We state that we would like three columns, each a `fr`action wide.

```
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

**HTML**
We have three items in our grid container

````
<div class="grid">
  <div class="grid-item">David</div class="grid-item">
  <div class="grid-item">Stephanie</div>
  <div class="grid-item">Nole</div>
</div>```
````

**Result**
The engine will layout our items based on the above code - in this example we have three elements; all grid items will be 1/3 of the total space

```
------
[][][]
------
```
