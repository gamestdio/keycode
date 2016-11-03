**DEPRECATION WARNING**

The [`which`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/which) and [`keyCode`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/keyCode) properties are being deprecated by the browsers. Even though it still might work, the usage is not encouraged anymore.

You would rather use the new [`key`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key) or [`code`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/code) attributes in `KeyboardEvent`.

keycode.js
===

Use human key names instead of keycode numbers for your keyboard bindings.

**1.7kb minified**

Usage example
---

```javascript
var Keycode = require('keycode.js')

document.addEventListener('keyup', function(e) {
  if (e.which == Keycode.ENTER) {
    console.log("User pressed ENTER key")
  }
})
```

License
---

MIT
