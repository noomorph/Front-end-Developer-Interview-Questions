#Front-end Job Interview Questions

### General Questions:

* Can you describe your workflow when you create a web page?
* How would you optimize a websites assets/resources?
  * Looking for a number of solutions which can include:
    * File concatenation, minification, CDN, caching, etc…
* Name 3 ways to decrease page load. (perceived or actual load time)
* How would you create a simple slideshow page?
  * Bonus points if it does not use JS.
* What tools do you use to test your code's performance?
  * Profiler, JSPerf, Dromaeo
* What is FOUC? How do you avoid FOUC?

### HTML-Specific Questions:

* What's a `doctype` do?
* What's the difference between standards mode and quirks mode?
* How do you serve a page with content in multiple languages?
* What are `data-` attributes good for?
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?
* Describe the difference between cookies, sessionStorage and localStorage.

### JS-Specific Questions

* Explain event delegation, event bubbling
* Explain how `this` works in JavaScript
* Explain how prototypal inheritance works
* How do you go about testing your JavaScript?
* What are `undefined` and `undeclared` variables?
* What is a closure, and how/why would you use one?
* What's a typical use case for anonymous functions?
* How do you organize your code? (module pattern, classical inheritance?)
* Difference between:
```
function Person(){} var person = Person() var person = new Person()
```
* What's the difference between `.call` and `.apply`?
* Explain AJAX in as much detail as possible
* Explain how JSONP works (and how it's not really AJAX)
* What's the difference between an "attribute" and a "property"?
* Why is extending built in JavaScript objects not a good idea? Why good idea?
* What is the difference between `==` and `===`?
* Explain how you would get a query string parameter from the browser window's URL.
* Explain the same-origin policy with regards to JavaScript.
* Make this work:
```
[1,2,3,4,5].duplicate(); // [1,2,3,4,5,1,2,3,4,5]
```
* Why is it called a Ternary expression, what does the word "Ternary" indicate?

### JS-Code Examples:

```
"i'm a lasagna hog".split("").reverse().join("");
```
Question: What value is returned from the above statement?
**Answer: "goh angasal a m'i"**

```
( window.foo || ( window.foo = "bar" ) );
```
Question: What is the value of window.foo?
**Answer: "bar"**
only if window.foo was falsey otherwise it will retain its value.

```
var foo = "Hello"; (function() { var bar = " World"; alert(foo + bar); })(); alert(foo + bar);
```
Question: What is the outcome of the two alerts above?
**Answer: "Hello World" & ReferenceError: bar is not defined**

```
var foo = [];
foo.push(1);
foo.push(2);
```
Question: What is the value of foo.length?
**Answer: `2`

```
var foo = {};
foo.bar = 'hello';
```
Question: What is the value of foo.length?
**Answer: `undefined`

### jQuery-Specific Questions:

* Explain "chaining".
* Explain "deferreds".
* Name 4 different values you can pass to the jQuery method.
  * Selector (string), HTML (string), Callback (function), HTMLElement, object, array, element array, jQuery Object etc.
* What is the effects (or fx) queue?
* What is the difference between `.bind()`, `.live()`, and `.delegate()`?
* What is the difference between `$` and `$.fn`? Or just what is `$.fn`.
* Optimize this selector:
```javascript
$(".foo div#bar:eq(0)")
```

### ExtJS-Specific Questions:

* What are pros and cons sides of ExtJS?
* Structure of Ext JS 4 application
* How to access Dom element using ExtJS? … Component?
* What is purpose of Ext.Element?
* What is xtype?
* How to reduce time for initial page loading in ExtJS?
* How to customize look'n'feel?
* How to handle event for a Ext JS component? Describe several approaches.
* What is purpose and responsibility of controllers?
* What is model? What functionality does model have? (Active Record, validation, associations, getters, setters, isDirty, id)
* What is store? How it works?
* What is the purpose of load() in store?
* What's difference between load() and loadData()?
* What are layout managers?
* How grids in ExtJS work?
    * Purpose of renderer in grid panel?
    * Paging toolbars
    * Cell and row editing

### CSS-Specific Questions:

* Describe what a "reset" CSS file does and how it's useful.
* Describe Floats and how they work.
* What are the various clearing techniques and which is appropriate for what context?
* Explain CSS sprites, and how you would implement them on a page or site.
* What are your favourite image replacement techniques and which do you use when?
* CSS property hacks, conditionally included .css files, or... something else?
* What are the different ways to visually hide content (and make it available only for screen readers)?
* Have you used or implemented media queries or mobile specific layouts/CSS?
* Any familiarity with styling SVG?
* How do you optimize your webpages for print?
* What are the advantages/disadvantages of using CSS preprocessors? (SASS, Compass, Stylus, LESS)
  * If so, describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
  * Webfonts (font services like: Google Webfonts, Typekit etc.)

### Optional Questions:

* explain `Function.prototype.bind`?
* Describe a strategy for memoization (avoiding calculation repetition) in JavaScript.
* What is the arity of a function?
```
(function (a, b, c) {}).length
arguments.length
```
* Have you ever used JavaScript templating?
  * If so, what libraries have you used? (Mustache.js, Handlebars etc.)
* Explain "hoisting". What will the following function log?
```
(function () { c=5; var c; console.log(c); })()
```
* (+) CSS selector priority
* What's your favorite feature of Internet Explorer?
