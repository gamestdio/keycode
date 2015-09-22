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
