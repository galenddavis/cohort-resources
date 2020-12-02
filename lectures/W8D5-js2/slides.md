# W8D5

### JavaScript II

![JavaScript-shade](https://i.redd.it/h7nt4keyd7oy.jpg)
---

## Today's Topics

+ Ruby vs ES5 vs ES6
+ Class Syntax
+ `call`, `apply`, `bind`
+ `arguments` object
+ Module Pattern
+ Callbacks
+ Event Loop

---


## [Ruby & JavaScript comparison chart](https://appacademy.github.io/curriculum/language_comparison/index.html)
#### _look back at it_

---

![buh-bye](https://media.giphy.com/media/UQaRUOLveyjNC/giphy.gif)
#### bye bye ruby


---

## Back to the topic at hand...

![JavaScript](https://i.ytimg.com/vi/sZDjqTnfiGA/maxresdefault.jpg)

---

## Ways to call a function

* Function Style: `fun(arg1, arg2)`
* Method Style: `obj.method(arg1, arg2)`
* Constructor Style: `new`

---
# Quick Demo - Functions
---

## Class Syntax

* JavaScript uses prototypal inheritance
* class definition in ES5:
  * any function can be a class constructor
  * explicitly set keys on `prototype`
  * syntax is very different from Ruby
* class definition in ES6: syntactic sugar
  * creates same prototype structure as ES5
  * a more familiar, user-friendly syntax
  * adds [extra features](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) that are beyond our scope today

---

# Demo - Class Syntax

![class-demo](http://wwonline.net/wp-content/uploads/2015/04/Mobile-Technology-In-The-Classroom.png)


---

## Ways to call a function

* Function Style: `fun(arg1, arg2)`
* Method Style: `obj.method(arg1, arg2)`
* Constructor Style: `new`
##### NEW!
* Apply: `func.apply(newContext, [args])`
* Call: `func.call(newContext, arg1, arg2)`
* Bind: `obj1.func.bind(newContext)(arg1,arg2)`

---
## Binding

* ensure our context is what we want it to be
* `bind()` returns a **function**
* Note: different from `call` and `apply` which **invoke** the function

---
# Demo - Call, Apply, and Bind
![call styles joke](https://66.media.tumblr.com/bd889e9ab3bb01c2c465f22aff49c9fb/tumblr_mpnqbjIxwk1sqlkr5o1_1280.jpg)


---

## Arguments

* Functions happily accept more or fewer arguments than expected
* omitted arguments are set to `undefined` (if they have no default)
* Accessing extra arguments:
  * ES5: array-like `arguments` variable
  * ES6: rest/spread operator: `...`

---

### Some different ways to convert `arguments` into an Array:

+ ES6: `Array.from(arguments)`
+ ES5: `Array.prototype.slice.apply(arguments)`
+ Lazy ES5: `[].slice.apply(arguments)`
+ 😮 ES6: `[...arguments]`

---

## Arguments Clinic

![monty-python-argument-clinic](https://multimedia-english.com/recursos/contenidos/5b332af4cb618cc94c765a42085f1422.jpg)


---

# Pop Quiz!
## [*Kahoooooot*](https://create.kahoot.it/details/w5d5-callbacks-quiz-1/580fb3b6-2570-44d1-8ea5-79f791b68bfb)

---

![hangin-on](https://media.giphy.com/media/eBCnpuRGBhQGY/giphy.gif)

---

## Module Pattern

* allows us to split our code into multiple files
  * like ruby's `require` and `require_relative`
* Two steps: exporting & importing

---

### Modules Demo

![space-station-module](http://www.21stcentech.com/wp-content/uploads/2013/11/Zarya-module.jpg)

---

## Let's Talk about Callbacks!

![thatd-be-great-callback](https://media.makeameme.org/created/if-you-could-phpoic.jpg)

---

## Callbacks

* Functions that are passed to other functions as arguments
* Allow us to build in asynchronicity into our programs

![customer-callback-system](https://www.infosearchbpo.com/bpo-news/wp-content/uploads/call-back-system.jpeg)

---

### Demo Time!

![cute-puppy-callback](https://memegenerator.net/img/instances/58926517/just-waiting-for-you-to-call-me-back.jpg)


---

## Event Loop

* Asynchronous functions schedule work to be done in the background
  * i.e. timers, AJAX requests, events
* Callbacks are invoked when action ready to occur & stack is empty
* [Event Loop Visualization](http://latentflip.com/loupe)


**read the demo**

---

## Pop Quiz!

#### [hoot hoot](https://create.kahoot.it/details/w5d5-callbacks-quiz-2/aae9c829-64e6-4e43-a68f-efd8ef52167c)

---

![the-light](https://media.giphy.com/media/xlGYf1RUbYYes/giphy.gif)

---

# Thanks!

![JavaScript](https://stackify.com/wp-content/uploads/2017/08/Javascript-vs-Typescript-793x397.jpg)