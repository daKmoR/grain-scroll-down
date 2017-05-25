[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/daKmoR/grain-scroll-down)
[![Polymer Version](https://img.shields.io/badge/polymer-v2-blue.svg)](https://www.polymer-project.org)

# \<grain-scroll-down\>

Adds an element that allows the user to scroll down.

## Demo
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="grain-scroll-down.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<grain-scroll-down>
  click me to scroll down 100%
</grain-scroll-down>
```

## Installation

```sh
$ bower install --save daKmoR/grain-scroll-down
```

## Getting Started

Import the package.

```html
<link rel="import" href="/bower_components/grain-scroll-down/grain-scroll-down.html">
```

## PolyFill SmoothScroll

Unfortunately Smooth Scroll is still not widely available.
But you can easily use a Polyfill like https://github.com/iamdustan/smoothscroll

Example for loading only if needed.
```js
(function() {
  'use strict';
  // load polyfill for smoothscroll if needed
  let scrollBehaviorSupported = ('scrollBehavior' in document.documentElement.style);
  if (!scrollBehaviorSupported) {
    let script = document.createElement('script');
    script.async = true;
    script.src = '../bower_components/smoothscroll/dist/smoothscroll.js';
    script.onload = onload;
    document.head.appendChild(script);
  }
})();
```


*For more information, see the API documentation.*

## Working on the Element

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed.
* View the Element via `polymer serve`
* Run tests via `polymer test`
