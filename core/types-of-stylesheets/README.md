# Stylesheet Varieties

There are a number of different stylesheets that can be loaded into a webpage, thus becoming part of the cascade - some stylesheets are automatically added by the browser, others are added by the engineer, or the end-user;

- [**User-Agent**](user-agent) (_M_) - the browser provided stylesheets.
- [**Author**][user] - stylesheets created by a developer;
  - [**Internal**](internal) (_H_) - developer generated stylesheets written in the `<head />` of the document.
  - [**External**](external) (_H_) - developer generated stylesheets written in a separate file, loaded into the `html` document.
  - [**Inline**](inline) (_M_) - developer generated styles, directly added to an element via the `style` attribute.
- [**User**](*H*) - end-user generated stylesheets loaded into the browser, usually for accessbility purposes.

##### Key

- **(_M_)** - Added by a machine
- **(_H_)** - Added by a human
