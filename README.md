# `theme-selector`

A Web Component for setting a website theme using a select element.

**[Demo](https://chrisburnell.github.io/theme-selector/demo.html)** | **[Further reading](https://chrisburnell.com/article/web-component-theme-selector/)**

## Examples

General usage example:

```html
<script type="module" src="theme-selector.js"></script>

<theme-selector>
    <select autocomplete="off">
        <optgroup label="Select a theme">
            <option value="light">
                Light
            </option>
            <option value="dark">
                Dark
            </option>
            <option value="other">
                Other
            </option>
        </optgroup>
    </select>
</theme-selector>
<style>
    theme-selector:not(:defined) {
        display: none;
    }
</style>
```

Example using a custom storage key:

```html
<script type="module" src="theme-selector.js"></script>

<theme-selector data-key="color-scheme">
    <select autocomplete="off">
        <option value="light">
            Light
        </option>
        <option value="dark">
            Dark
        </option>
    </select>
</theme-selector>
<style>
    theme-selector:not(:defined) {
        display: none;
    }
</style>
```

Example using a custom dark theme key:

```html
<script type="module" src="theme-selector.js"></script>

<theme-selector data-dark-theme="white-on-black">
    <select autocomplete="off">
        <option value="black-on-white">
            Black on White
        </option>
        <option value="white-on-black">
            White on Black
        </option>
    </select>
</theme-selector>
<style>
    theme-selector:not(:defined) {
        display: none;
    }
</style>
```

Example with a custom transition class and duration to keep the class applied:

```html
<script type="module" src="theme-selector.js"></script>

<theme-selector data-transition-class="transitioning" data-transition-duration="100">
    <select autocomplete="off">
        <option value="light">
            Light
        </option>
        <option value="dark">
            Dark
        </option>
    </select>
</theme-selector>
<style>
    theme-selector:not(:defined) {
        display: none;
    }
</style>
```

Example targeting a specific element to apply the theme to:

```html
<script type="module" src="theme-selector.js"></script>

<theme-selector data-root-element=".content">
    <select autocomplete="off">
        <option value="light">
            Light
        </option>
        <option value="dark">
            Dark
        </option>
    </select>
</theme-selector>
<style>
    theme-selector:not(:defined) {
        display: none;
    }
</style>
```

## Features

This Web Component allows you to use a select element to control user-preferred theming across your website by setting a data attribute against the root element (or a defined selector query). Additionally saves the preference to local storage so that it can be applied on new page loads and maintained between user visits.

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
- [Andy Bell](https://piccalil.li/) for writing the article, [Create a user controlled dark or light mode](https://piccalil.li/tutorial/create-a-user-controlled-dark-or-light-mode/), which served as the initial inspiration and basis for building my own theming setup and eventually became this Web Component
