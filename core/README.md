# Core CSS

The core functionality of CSS is concerned with taking the various [stylesheets](./types-of-stylesheets) loaded into a page, and assigning the correct styles to the targeted elements in the document.

### Sorting and Applying

The browser engine has a number of built-in mechanisms which determine what styles get applied to a given element based on the rules of the language;

- [**Cascade**](./cascade); determines which styles are applied to elements based on the variety of [stylesheets](./types-of-stylesheets/) loaded into the page.
- [**Specificity**](./specificity); provides the cascade with a comprehensive conflict resolution by deciding which ruleset contains the most specific selector(s)
- [**Inheritance**](./inheritance); if a particular property hasn't been explicitly added to an element, the inhertiance mechanism will set the value based on its ancestors declarations, dependant on _that_ particular property.
