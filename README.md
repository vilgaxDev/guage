

[![demo](https://github.com/thlorenz/d3-gauge/raw/master/assets/gauge-demo.gif)]

```js
var d3gauge = require('d3-gauge');

var gauge = d3gauge(document.getElementById('simple-gauge'));
gauge.write(39);
```

**Note:** please make sure to [include the appropriate `css`](#styling) in your page, otherwise all you'll see is a big black
circle.

## Installation

    npm install d3-gauge
## Try it

```sh
npm explore d3-gauge
npm run demo
```

## API

####gauge (el[, opts])*

Creates a gauge appended to the given DOM element.

@name Gauge
@function
**params:**

- 

*Object* the gauge with a `write` method

**Note:** have a look at the [default opts](https://github.com/thlorenz/d3-gauge/blob/master/defaults/simple.js)

###*gauge.write = function(value, transitionDuration)*

Writes a value to the gauge and updates its state, i.e. needle position, accordingly.
@name write
@function
**params:**

- value *Number* the new gauge value, should be in between min and max
- transitionDuration *Number* (optional) transition duration, if not supplied the configured duration is used

## Styling

## License

MIT
