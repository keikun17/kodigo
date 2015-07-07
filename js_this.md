## ES5 values of `this`

- Within `foo.methodName`, the value of `this` is `foo`.
- Function calls :
```
var this = 'something'
functionName = function() { return this }
functionName() // 'something'
```
- When using `new` (ex. `var foo = new Foo()`), the value of 'this' inside the definition is `foo`
- Force `this` value with `apply`, `call`, `bind`
