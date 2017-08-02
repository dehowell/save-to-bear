# save-to-bear

Bookmarklet for saving the current page to Bear. To save the bookmarklet, go to:

[https://dehowell.github.io/save-to-bear/][1]

[1]: https://dehowell.github.io/save-to-bear/

This is the whole thing, unminified:

```javascript
function saveToBear() {
  var bearUrl =  'bear://x-callback-url/grab-url?url=' + encodeURIComponent(window.location);
  window.location.href = bearUrl;
};
```
