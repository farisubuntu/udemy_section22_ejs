> udemy_section22_ejs
> this is my notes for the section 22 of udemy course

```shell
# first install:
$ mkdir app1 && cd app1
$ npm init -y # change index.js to app.js
$ npm install express ejs nodemon --save
```
### To getstarted:

- for getstarted with `EJS`: [ejs.co]
- Using `EJS` with `express` : [https://github.com/mde/ejs/wiki/Using-EJS-with-Express]


## Using EJS with Express

install EJS:

`$ npm install ejs`

> This assumes a views directory containing an index.ejs page.

**views/index.js**

```js
let express = require('express');
let app = express();

app.set('view engine', 'ejs');

app.get('/', (req, res) => {
  res.render('index', {foo: 'FOO'});
});

app.listen(4000, () => console.log('Example app listening on port 4000!'));
```
