# jquery-amd

An AMD compatiable [jQuery](https://github.com/jquery/jquery), which address the problem that AMD do not have a inherent `window` with a `document`. A creation of a mockup of `window` with a `document` is needed and handled.

## Installation

### Node.js

```
npm install jquery-amd
```

### AMD

Follow the instruction of the environments you are using.

## How to use

### Node.js

```
var jq = require('jquery-amd');
var window = ... // use some window and dom mockup tool, like Noddom, jsdom etc.
var $ = jq(window);
```

### AMD

```JavaScript
define(['jquery'], function(jq){
    ...
    var window = ...; // use some window and dom mockup tool, like Noddom, jsdom etc.
    var $ = jq(window);
    ...
});
```

## Authors and Contributors

+ Jianwei Liu

## License

jquery-amd is released under the [MIT license](http://www.opensource.org/licenses/MIT).
