# Error checks in node  
## Undici

```js

function isErrorLike (object) {
    return object instanceof Error || (
      object?.constructor?.name === 'Error' ||
      object?.constructor?.name === 'DOMException'
    )
}
```
