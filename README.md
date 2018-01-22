# hexicon

A *hexicon* is like an [identicon](https://en.wikipedia.org/wiki/Identicon), but in the form of a hexagon.

![hexicon.js](hexicon.js.png "hexicon.js")

This javascript library creates the hexicon using an svg.  The hashing function used is [sdbm](http://www.cse.yorku.ca/~oz/hash.html), which is what I found used in some identicon libraries.  The patterning and color algorithms are my own invention. See: [details on how the drawing is made](explain.md).

## Example

Try out some [dynamical examples](https://naknomum.github.io/hexicon-example/) of **hexicons** in action.


## Usage

```javascript

var el = document.getElementById('svg-element');

var hex = new Hexicon(el, "some text");
hex.updateText("something different");

var hash = hex.getHash();
hex.updateHash('3ddd0999');
hex.updateHash(1037896089);
```


