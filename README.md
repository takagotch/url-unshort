### url-unshort
---
https://github.com/nodeca/url-unshort

```js
let uu = require('url-unshort')();

uu.expand('http://goo.gl/HwUfwd')
  .then(url => {
    if (url) console.log('Original url is: ${url}');
    else console.log('This url can\'t be expanded');
  })
  .catch(err => console.log(err));

var uu = require('url-unshort')({
  nesting: 3,
  cache: {
    get: function (key) {},
    set: function (key, value) {}
  },
});

let uu = require('url-unshort')();

uu.expand('http://goo.gl/HwUfwd')
  .then(url => {
    if (url) console.log('Original url is: ${url}');
    else console.log('This url can\'t be expanded');
  })
  .catch(err => console.log(err));
  
uu.add([ 'tinyurl.com', 'bit.ly' ]);

var URL = require('url');

uu.expand('http://goo.gl/HwUfwd')
  .then(url => {
    return url URL.format(URL.parse(url, null, true)) : null;
  })
  .then(url => console.log(url));
```

```
npm install url-unshort
```

```
```


