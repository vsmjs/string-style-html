# string-style-html

Converts a *string* and a simple '*style*'-instructions string,
to *HTML* code that has styling tags inserted.

This functionality is used by both vsm-autocomplete and vsm-box,
which is why it is a separate package.


## Examples

```
const stringStyleHtml = require('string-style-html');

console.dir( stringStyleHtml('cdc2', 'i') );
// => '<i>cdc2</i>'.

console.dir( stringStyleHtml('Ca2+', 'u2-4') );
//   Offsets of the indexes: '0123'.
// => 'Ca<sup>2+</sup>'.

console.dir( stringStyleHtml('HCO3-', 's3;u4') );
//   Offsets of the indexes: '01234'.
// =>'HCO<sub>3</sub><sup>-</sup>'.
```


## Specification

The full specification and more examples are in
[stringStyleHtml.test.js](stringStyleHtml.test.js).