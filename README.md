# Image-JPEG-Convert
Image JPEG Convert is Image format convert to JPEG.

It is used WebWorker. If WebWorker is busy, use main thread or delayed.

## How To Use
```html
<script type="text/javascript" src="./jpeg.js" defer></script>
<!--Load script-->
<!--If you want save network, use jpeg.min.js.-->
```

```javascript
const jpeg = new JPEG();

jpeg.start(file, {
    success(result) {
        // result type is blob.
    },
    error(err) {
        // When work rejected.
    }
});
```