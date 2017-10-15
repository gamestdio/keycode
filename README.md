# @gamestdio/keycode

Use human key names instead of keycode numbers for your keyboard bindings.

**1.7kb minified**

## Warning

The [`which`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/which) and [`keyCode`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/keyCode) properties are in the process of being deprecated by the browsers.

After mainstream adoption, you would rather use the new [`key`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key) or [`code`](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/code) attributes in `KeyboardEvent`.

By the time of this writing, IE/Edge still doesn't support the new `KeyboardEvent.key` / `KeyboardEvent.code` API. See: https://caniuse.com/#feat=keyboardevent-code

## Usage example

```typescript
import Keycode from "@gamestdio/keycode";

document.addEventListener('keyup', function(e) {
  if (e.which == Keycode.ENTER) {
    console.log("User pressed ENTER key")
  }
})
```

## License

MIT
