keycode.js
===

Use constants instead of plain number/string values for your keyboard bindings.

Codes extracted from [KeyboardEvent.code](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/code).

**1.7kb minified**

Usage example
---

```typescript
import { Keycode } from "keycode.js";

document.addEventListener('keyup', function(e) {
  if (e.code == Keycode.Enter) {
    console.log("User pressed ENTER key")
  }
})
```

License
---

MIT
