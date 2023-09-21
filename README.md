# doughbeat

doughbeat is a very minimal bytebeat livecoding editor.

You can use it here: https://felixroos.github.io/doughbeat/

To understand how it works, read my blog post series:

- https://loophole-letters.netlify.app/buffers/
- https://loophole-letters.netlify.app/real-time-synthesis/
- https://loophole-letters.netlify.app/real-time-synthesis2/

## Usage

It is very simple, you just have to write a `dsp` function that takes time as its only argument.
Example:

```js
function dsp(t) {
  return (110 * t) % 1;
}
```

This is a simple square wave...

## Credits

- [htmlbytebeat](https://github.com/greggman/html5bytebeat)
- [wavepot](http://wavepot.com/) inspired the `dsp` function (before it was just a `t` expression)
