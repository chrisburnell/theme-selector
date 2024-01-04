# `theme-selector`

A Web Component for setting a website theme using a select element.

**[Demo](https://chrisburnell.github.io/theme-selector/demo.html)** | **[Further reading](https://chrisburnell.com/article/web-component-theme-selector/)**

## Examples

General usage example:

```html
<script type="module" src="theme-selector.js"></script>

<theme-selector>
  <button>Button</button>
</theme-selector>
<style>
  theme-selector:not(:defined) {
    display: none;
  }
</style>
```

## Features

This Web Component allows you to: TODO

- Check for… TODO

## Installation

You have a few options (choose one of these):

1. Install via [npm](https://www.npmjs.com/package/@chrisburnell/theme-selector): `npm install @chrisburnell/theme-selector`
1. [Download the source manually from GitHub](https://github.com/chrisburnell/theme-selector/releases) into your project.
1. Skip this step and use the script directly via a 3rd party CDN (not recommended for production use)

### Usage

Make sure you include the `<script>` in your project (choose one of these):

```html
<!-- Host yourself -->
<script type="module" src="theme-selector.js"></script>
```

```html
<!-- 3rd party CDN, not recommended for production use -->
<script
  type="module"
  src="https://www.unpkg.com/@chrisburnell/theme-selector@1.0.0/theme-selector.js"
></script>
```

```html
<!-- 3rd party CDN, not recommended for production use -->
<script
  type="module"
  src="https://esm.sh/@chrisburnell/theme-selector@1.0.0"
></script>
```

## Credit

With thanks to the following people:

- [David Darnes](https://darn.es) for creating this [Web Component repo template](https://github.com/daviddarnes/component-template)
