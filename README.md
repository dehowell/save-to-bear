# save-to-bear

Bookmarklet for saving the current page to Bear. To save the bookmarklet, go to:

[https://dehowell.github.io/save-to-bear/][1]

[1]: https://dehowell.github.io/save-to-bear/

And then drag this link to your browser's bookmarks toolbar:

<a id="bookmarklet" href="javascript:(function saveToBear(){var bearUrl='bear://x-callback-url/grab-url?url='+encodeURIComponent(window.location);window.location.href=bearUrl})();">Save to Bear</a>

This is the whole thing, unminified:

```javascript
function saveToBear() {
  var bearUrl =  'bear://x-callback-url/grab-url?url=' + encodeURIComponent(window.location);
  window.location.href = bearUrl;
};
```
