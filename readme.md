minifier
========

A simple tool for minifying CSS/JS without a big setup.

Feature highlights
------------------

- It minifies JS and CSS
- It reworks URLs in CSS from the original location to the output location.
- It automatically resolves `@import` statements in CSS.


How to install
--------------

There are no way to install it atm. Instead, pull it from github and create an alias.

I know, I know, this is not optimal. But it needs to work before it needs to be pretty :).


How to run
----------

Running it is simple:

	minifier [--out path/to/put/file] path/to/file

If the output parameter is not set, it will place a file next to the original,
with the suffix `.min`.

For example, `minifier script.js` will output `script.min.js`, whereas
`minifier --output out.js script.js` will output `out.js`.


Running the tests
-----------------

After installing from [github](https://github.com/fizker/minifier), simply run
`npm test`.

Alternatively, the `runAllTests.js` script will also execute the tests.

Inside the `test/` folder, there is a script called `prepareManualTests.js`.
This will run the script against the css-files inside `test/manual/css/`,
which provides a real-world example of the CSS minification tools.

The manual tests can be seen by opening `test/manual/index.html` in a browser
after executing `prepareManualTests.js`.


Credits
-------

In no particular order:

- [sqwish](https://github.com/ded/sqwish) for minifying CSS files.
- [uglify-js](https://github.com/mishoo/UglifyJS) for minifying JS files.
- [commander](https://github.com/visionmedia/commander.js) for command-line
  interaction.
- [mocha](https://github.com/visionmedia/mocha), [chai](http://chaijs.com),
  [sinon](http://cjohansen.no/sinon/) and
  [sinon-chai](https://github.com/domenic/sinon-chai) for testing home-brewed
  logic.
