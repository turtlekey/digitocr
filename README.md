Just one script for ocr the digit(s), recieving the canvas element, the img element, or the img uri.

```html
<!DOCTYPE html>
...
<script src="digitocr.js"></script>
...
<canvas id="digit"></canvas>
<img src="digit.jpg" />
...
<script>
  let ocr = new DigitOcr(document.querySelector("canvas");
  // or
  let ocr = new DigitOcr(document.querySelector("img");
  // or
  let ocr = new DigitOcr("digit.jpg");

  ocr.getDigit().then(value => console.log(value));
</script>
</html>
```

