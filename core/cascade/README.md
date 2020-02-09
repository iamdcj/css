# The Cascade

It is an algorithm built into the browser engine which determines which styles should be applied to an element based on the rules declared in the various stylesheets active in a web-page.

In most case websites ship with at least one engineered authored stylesheet, however this is not the only stylesheet at play when you load a page;

- **[User-agent Stylesheet](../types-of-stylesheets/user-agent)** - browser's default baseline styles.
- **[Author Stylesheet](../types-of-stylesheets/author)** - engineer authored styles.
- **[User Stylesheet](../types-of-stylesheets/user)** - styles added by the user, often for accessibility purposes.

The above stylesheets could, and often will, contain conflicting rulesets, as a result the browser needs to determine which declarations should be applied to a given element based on the multiple sources at play.

### **How it works**?

The following describes at a high-level the different procedures taken by the cascade algorithm.

- **ASSESS** - The engine will assess all the various stylesheets present when the page is loading.
- **FILTER** - filter the rulesets from each source that are intended for a given element.
- **SORT** - sorts the filtered rules based on their importance and their source;
  - **SOURCE** - what type of stylesheet does the ruleset come from, e.g. is it from the user-agent, the developer or the user?
  - **IMPORTANCE** - does the declaration have an `!important` statement present?
- **APPLICATION** - once the cascade has determined which declaration should be applied, it will apply the style to the element.

##### **Cascade Priority Order** (highest to lowest);

The stylesheet origin and declaration importance determine which style gets applied to an element, the following order is used to determine the winner when the cascade discovers competing declarations;

1. [User Stylesheet](../types-of-stylesheets/user) `!important`
2. [Author Stylesheet](../types-of-stylesheets/author) `!important`
3. [Author Stylesheet](../types-of-stylesheets/author)
4. [User Stylesheet](../types-of-stylesheets/user)
5. [User-agent Stylesheet](../types-of-stylesheets/user-agent)

If the cascade can determine a winner based on the origin and importance, then it moves on to the next conflict.

**No outright winner**

If the cascade mechanism fails to determine the correct declaration due to it having the same source and level of importance, it will call on the [specificity](../specificity) mechanism to decide the winner.

---

Reference
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade)
[Nicolas Gallagher](http://nicolasgallagher.com/css-cascade-specificity-inheritance/)
[Specification](https://www.w3.org/TR/CSS2/cascade.html)
[Understanding the cascade](https://blog.logrocket.com/how-css-works-understanding-the-cascade-d181cd89a4d8/)
