# Hoisting Exercises

What is logged in each of these code blocks? Answer it **without** actually running the code on a computer.

#### 1

```js
var test = "initial value"
var f = function () {
    test = "new value"

    if (test) {
        test += " and more!"
    } else {
        var test = "It begins here"
    }
}
f()
console.log("Test: " + test)
```


#### 2

```js
var test = "initial value"
var f = function () {
    test = "new value"

    if (test) {
        test += " and more!"
    } else {
        test = "It begins here"
    }
}
f()
console.log("Test: " + test)
```
#### 3

```js
var test = "initial value"
var f = function () {
    test += "new value"

    if (test) {
        test += " and more!"
    } else {
        var test = "It begins here"
    }
    return test
}
console.log(f())
```

#### 4
```js
var test = "initial value"
for (var i = 0; i < 5; i++) {
    test = "new value"

    if (test) {
        
        test += " and more!"
    } else {
        var test = "It begins here"
    }
}

console.log("Test: " + test)
```


#### 5
```js
var test = "initial value"
var f = function () {
    test = "new value"

    if (test) {
        test += " and more!"
    } else {
        test = "It begins here"
    }
    g()
}
var g=function(){
	var test="newnew value"
}
f()
console.log("Test: " + test)
```

#### 6
```js
var test = "initial value"
var f = function () {
    test = "new value"

    if (test) {
        test += " and more!"
    } else {
        var test = "It begins here"
    }
    g()
}
var g=function(){
	test="newnew value"
}
f()
console.log("Test: " + test)
```

#### 7
```js
var test = "initial value"
var f = function () {
	g()
    test = "new value"

    if (test) {
        test += " and more!"
    } else {
        test = "It begins here"
    }
}
var g=function(){
	test="newnew value"
}
f()
console.log("Test: " + test)
```

