# The Cascade

It is an algorithm built into the browser engine which determines which styles should be applied to an element based on the rules declared in the various stylesheets active in a web-page.

In most case websites ship with at least one engineered authored stylesheet, however this is not the only stylesheet at play when you load a page;

- User-Agent Stylesheet - browser's default baseline styles.
- Authored Stylesheets - engineer authored styles.
- User Stylesheet - styles added by the user, often for accessibility purposes.

The above stylesheets could, and often will, contain conflicting rulesets, as a result the browser needs to determine which declarations should be applied to a given element based on the multiple sources at play.

### How the cascade does its thing?

The following describes at a high-level the different procedures taken by the cascade algorithm.

- ASSESS - The engine will assess all the various stylesheets present when the page is loading.
- FILTER - filter the rulesets from each source that are intended for a given element
- SORT - sorts the filtered rules based on their important and their source;
- IMPORTANCE - does the declaration have an `!important` statement present?
- SOURCE - what is the origin of a particular rule, e.g. is it from: the user-agency, the developer or the user?

##### Cascade Order (highest to lowest);

1. User Stylesheet !important
2. Author Stylesheet !important
3. Author Stylesheet
4. User Stylesheet
5. User-agent Stylesheet

#### No outright winner

If the cascade cannot successfully choose a declaration due to the it having the same source and importance, it will utilise the specificity mechanism to decide the winner

---

https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade
http://nicolasgallagher.com/css-cascade-specificity-inheritance/
https://www.w3.org/TR/CSS2/cascade.html