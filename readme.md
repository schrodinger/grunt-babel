# NOTE: This is a temporary repository to test LiveDesign upgrade to babel@7 before its official release.

# grunt-babel [![Build Status](https://travis-ci.org/babel/grunt-babel.svg?branch=master)](https://travis-ci.org/babel/grunt-babel)

> Use next generation JavaScript, today, with [Babel](https://babeljs.io)

*Issues with the output should be reported on the Babel [issue tracker](https://github.com/babel/babel/issues).*


## Install

```
$ npm install --save-dev grunt-babel @babel/core @babel/preset-env
```


## Usage

```js
require('load-grunt-tasks')(grunt); // npm install --save-dev load-grunt-tasks

grunt.initConfig({
	babel: {
		options: {
			sourceMap: true,
			presets: ['env']
		},
		dist: {
			files: {
				'dist/app.js': 'src/app.js'
			}
		}
	}
});

grunt.registerTask('default', ['babel']);
```


## Options

See the Babel [options](https://babeljs.io/docs/usage/options), except for `filename` which is handled for you.


## License

MIT © [Sindre Sorhus](https://sindresorhus.com)
