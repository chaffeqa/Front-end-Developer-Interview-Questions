#Front-end Job Interview Questions



#### Discussion Questions:

* Why do we concatinate all javascript files and css files into a single one?
* Why is Gzipping important?
* What does CORS stand for and what issue does it address?
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
* What's the difference between inline and inline-block?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What tools and techniques do you use debugging JavaScript code?
* Explain the following request and response headers:
  * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * ETag
  * X-Frame-Options



#### Coding Questions:

*Write the commands to clone the repository `git@github.com:chaffeqa/nuthin.git`, add a file `file.txt` with contents `Hello`, commit it, and push it back up to `origin/master`.*

    Answer:
    |
    |
    |
    |
    |
    |
    |

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```


*Question: What is the value of `window.foo`?*
```javascript
( window.foo || ( window.foo = "bar" ) );
```

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```


*Question: What is the result of the following code?*
```javascript
var fullname = 'John Doe';
var obj = {
   fullname: 'Colin Ihrig',
   prop: {
      fullname: 'Aurelio De Rosa',
      getFullname: function() {
         return this.fullname;
      }
   }
};
console.log(obj.prop.getFullname());
var test = obj.prop.getFullname;
console.log(test());
```

*Question: What will be printed on the console?*
```javascript
(function() {
   var a = b = 5;
})();
console.log(b);
```

*Question: What will be printed on the console?*
```javascript
function meth1(){
  return 1;
}
function meth2(input){
  return 2 + input;
}
function result(arg1, cb){
  var result = typeof(cb) == "function" && cb(arg1)
  return result
}
console.log('a'+result(1,meth1()))
console.log('b'+result(1,meth1))
console.log('C'+result(1,meth2))
```

*Question: What will be printed on the console?*
```javascript
var d = (function f(f, d){
  return {f: typeof f(), d: typeof(d) };
})(function(){ return 1; });
console.log(d)
```
