CSS rulesets are applied to a document by the browsers in order to affect the appearance of the webpage.

These rulesets make-up a stylesheet, and these rules determine how the page will look in the browser.

ANATOMY
A CSS ruleset is made up of the following:

- A Selector: this selects the HTML elements you want to apply styles to.
- Parentheses: a pair of curly braces which follow the selector
- Declarations: all style declarations live within the curly braces, forming a declaration block, and consist of the following
  - A property: the property is tell the browser what you are styling (these are predefined in the CSS spec)
  - A value: the value is assigned to the property, and if valid will determine how the content is displayed
  - A semicolon: this signifies the end of the style declaration

EXAMPLE
The following example of a CSS ruleset consists of a selector which targets all paragraphs(<p>) in the document, and the color property, which possesses a value of red:

p {
color: red;
}

https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Syntax
