# hexicon

A *hexicon* is like an [identicon](https://en.wikipedia.org/wiki/Identicon), but in the form of a hexagon.

![hexicon.js](https://raw.githubusercontent.com/naknomum/hexicon/master/hexicon.js.png "hexicon.js")

This javascript library creates the hexicon using an svg.  The hashing function used is [sdbm](http://www.cse.yorku.ca/~oz/hash.html), which is what I found used in some identicon libraries.  The patterning and color algorithms are all my own, but it is (obviously) based on rotational symmetry.  I can explain it in more detail if anyone is curious.

## Example

Try out some [dynamical examples](https://naknomum.github.io/hexicon-example/) of **hexicons** in action.


## Usage

```javascript

var el = document.getElementById('svg-element');

var hex = new Hexicon(el, "some text");

hex.updateText("something different");
```


