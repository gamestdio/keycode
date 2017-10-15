# @gamestdio/keycode

Use human key names instead of keycode numbers for your keyboard bindings.

**1.7kb minified**

## Warning

The [`which`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/which) and [`keyCode`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/keyCode) properties are in the process of being deprecated by the browsers.

You would rather use the new [`key`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key) or [`code`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/code) attributes in `KeyboardEvent` instead. By the time of this writing, IE/Edge doesn't support either `KeyboardEvent.key` or `KeyboardEvent.code` yet.

## Usage example

```typescript
import { Keycode } from "keycode.js";

document.addEventListener('keyup', function(e) {
  if (e.code == Keycode.Enter) {
    console.log("User pressed ENTER key")
  }
})
```

## License

MIT
