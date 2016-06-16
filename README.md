# RequireJSES6Class
Demo of RequireJS AMD module with ES6 (ES2015) Class with timing check in browser code.

 * This is a demo of modules asynchronously loading classes in the browser. 
 * Server code (node.js) has it's own module loader.
 * Code is from RequireJS intro demo from http://requirejs.org/docs/start.html
 * Constructor-based and ES2015 'class' based (object definitions) are in modules loaded by RequireJS
 * Added timing test code.  Timing tests should be written in their own modules.
 * Asyncronous Module. ES2015 'import' and 'export' is not implemented yet in browsers.  This is June 2016

Here is a class with a getter and setter:
```javascript
es6c: class ES6C {
			constructor(abc)
			{
				this.abc = abc;  // uses 'set' method
			}
			set abc(abcv)  // define 'set' method
			{
				this.vabc = abcv
			}
			get abc()  // define 'get' method
			{
				return this.vabc;
			}
		}
```
It is defined in the module 'lib/print.js' in the define statement.
It is loaded in 'app/main.js' with a require statement.
  
 