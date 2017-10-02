Another LightBox
===

[An example][example]

Getting started
---

### Step 1: Download
- [Download lightbox.js][download-js].
- [Download lightbox.css][download-css].

### Step 2: Process files
Rename lightbox.scss -> lightbox.css (current file doesn't contain sass logic)

### Step 3: Include files

```html
<!-- Include lightbox.js -->
<script src="/path/to/lightbox.js"></script>

<!-- Include the styles -->
<link rel="stylesheet" href="/path/to/lightbox.css" />

<!-- Create a container (optional) element and anchor elements as sources. -->
<div id="gallery">
  <a href="path/to/image-large-01.jpg"><img src="path/to/image-small-01.jpg" /></a>
  <a href="path/to/image-large-02.jpg"><img src="path/to/image-small-02.jpg" /></a>
  <a href="path/to/image-large-03.jpg"><img src="path/to/image-small-03.jpg" /></a>
</div>
```

### Step 4: Create a new `LightBox` object, passing anchor elements

```javascript
window.addEventListener('load', function(){
  var lightBox = new LightBox(document.querySelectorAll('#gallery a'));
});
```

Methods
---

### openViewer() ###
Opens the lightbox viewer starting with the first element.

```javascript
window.addEventListener('DOMContentLoaded', function(){
  var lightBox = new LightBox(document.querySelectorAll('#gallery a'));

  lightbox.openViewer();
});
```

[download-js]: https://github.com/nielsriekert/lightbox.js/tree/master/src/lightbox.js
[download-css]: https://github.com/nielsriekert/lightbox.js/tree/master/src/lightbox.scss
[example]: http://judolosser.nl/fotoalbum/avondvierdaagse/
