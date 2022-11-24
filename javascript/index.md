# Javascript `Journey`
- [Execute some javascript code](#execute-some-javascript-code-in-the-browser)
- [Execute some javascript with nodejs](#execute-some-javascript-code-with-nodejs)

### Execute some javascript code in the browser

You can start your javascript journey and try to run some javascript code simply by doing it on a browser (Firefox, Chrome, Edge, Safari ...).

On chrome browser open a new tab and press <kbd>F12</kbd>.

Then you select the console tab, et voilà a command like window is opened where you can type your javascript code who will be executed immediately when you hit <kbd>Enter</kbd>.

``` js
let a = 5, b = 5;
const c = a + b;
console.log(c);
```

### Execute some javascript code with nodejs

Nodejs is a JavaScript runtime built on Chrome's V8 JavaScript engine, and can run JavaScript code directly on the command line or by executing the code inside a javascript file.

After installing nodejs and adding it to the OS environment so it can be accessed from the console or command line.

Like in the browser, you can type your javascript code who will be executed immediately when you hit <kbd>Enter</kbd>.

``` js
let str = 'THIS IS NODE JS';
console.log(str);
```

Or by creating a javascript file `file.js` with some code inside and executing it by running :

```
node file.js
```