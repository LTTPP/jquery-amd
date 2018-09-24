# jquery-amd

An AMD compatiable [jQuery](https://github.com/jquery/jquery), which supports the case that do not have a inherent `window` with a `document`. A creation of a mockup of `window` and `document` is needed and handled.

## Installation

```
npm install jquery-amd
```

## How to use

```JavaScript
define(['path/to/jquery'], function(jq){
    ...
    var window = ...; // use some document generation tool, like Noddom, [jsdom](https://github.com/jsdom/jsdom) etc.
    var $ = jq(window);
    ...
});
```

## Authors and Contributors

+ Jianwei Liu

## License

jquery-amd is released under the [MIT license](http://www.opensource.org/licenses/MIT).
