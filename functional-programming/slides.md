---
theme: academic
coverAuthor: Qianhe Chen
hideInToc: true
---

# Functional Programming

---
layout: table-of-contents
hideInToc: true
---

# Table of Contents

---

# Imperative Programming

In computer science, imperative programming is a programming paradigm of software that uses statements that change a program's state. In much the same way that the imperative mood in natural languages expresses commands, an imperative program consists of commands for the computer to perform. Imperative programming focuses on **describing how a program operates step by step**, rather than on high-level descriptions of its expected results.

```mermaid
graph LR
A[买鸡蛋和西红柿]-->B[切西红柿]-->C[打鸡蛋]-->D[炒鸡蛋]-->E[炒西红柿]-->F[混合鸡蛋]-->G[西红柿炒鸡蛋]
```

---

# Declarative programming

In computer science, declarative programming is a programming paradigm—a style of building the structure and elements of computer programs—that expresses the logic of a computation without describing its control flow.

```mermaid
graph LR
A[来一份西红柿炒鸡蛋]-->B(((BLACK BOX)))-->C[西红柿炒鸡蛋]
```

---

# Functional Programming

In computer science, **functional programming is a programming paradigm where programs are constructed by applying and composing functions.** 

In functional programming, **functions are treated as first-class citizens**, <u>*meaning that they can be bound to names (including local identifiers), passed as arguments, and returned from other functions, just as any other data type can.* </u>This allows programs to be written in a declarative and composable style, where small functions are combined in a modular manner.

Functional programming has its roots in academia, **evolving from the lambda calculus.**

```mermaid
graph LR
A[[购买]]-->B[[处理]]-->C[[炒制]]-->D[西红柿炒鸡蛋]
```

* First-class and higher-order functions
* Pure functions
* Referential transparency

---

# λ Calculus

Lambda calculus (λ-calculus), originally created by Alonzo Church, is the world’s smallest programming language. Despite not having numbers, strings, booleans, or any non-function datatype, **lambda calculus can be used to represent any Turing Machine!**<sup>1</sup>

|Name|Syntax|Example|Explanation|
|---|---|---|---|
|Variable|`<name>`|`x`|a variable named “x”|
|Function|`λ<parameters>.<body>`|`λx.x`|a function with parameter “x” and body “x”|
|Application|`<function><variable or function>`|`(λx.x)a`|calling the function “λx.x” with argument “a”|

The most basic function is the identity function: `λx.x` which is equivalent to $f(x) = x$. The first “x” is the function’s argument, and the second is the body of the function.


<Footnotes separator>
  <Footnote :number=1><a href="https://learnxinyminutes.com/docs/lambda-calculus/" rel="noreferrer" target="_blank">Lambda Calculus</a></Footnote>
</Footnotes>

---

# Pure Functions

Pure functions (or expressions) have **no side effects (memory or I/O)**. This means that pure functions have several useful properties, many of which can be used to optimize the code:

* If the result of a pure expression is not used, it can be removed without affecting other expressions.
* If a pure function is called with arguments that cause no side-effects, the result is constant with respect to that argument list (sometimes called referential transparency or idempotence), i.e., **calling the pure function again with the same arguments returns the same result**. (This can enable caching optimizations such as memoization.)
* If there is no data dependency between two pure expressions, their order can be reversed, or they can be performed in parallel and they cannot interfere with one another (in other terms, the evaluation of any pure expression is thread-safe).
* If the entire language does not allow side-effects, then any evaluation strategy can be used; this gives the compiler freedom to reorder or combine the evaluation of expressions in a program (for example, using deforestation).

---

## Side Effect of Function

In computer science, an operation, function or expression is said to have a side effect if it **modifies some state variable value(s) outside its local environment**, which is to say if it has any observable effect other than its primary effect of returning a value to the invoker of the operation. <u>Example side effects include modifying a non-local variable, modifying a static local variable, modifying a mutable argument passed by reference, performing I/O or calling other functions with side-effects.</u> In the presence of side effects, a program's behaviour may depend on history; that is, the order of evaluation matters. Understanding and debugging a function with side effects requires knowledge about the context and its possible histories.

---

```python
x = 0
def setx(n):
    global x
    x = n
setx(3)
assert x == 3
setx(3)
assert x == 3
```

```python
def abs(n):
    return -n if n < 0 else n
assert abs(abs(-3)) == abs(-3)
```

```python
def hello(name: str):
  print('hello ', name)
  return 'hello ' + name
```

```python
def hello(name: str):
  return 'hello ' + name
```

---

## the function return values are identical for identical arguments

A function is a special relationship between values: Each of its input values gives back exactly one output value.

|![](https://www.mathsisfun.com/sets/images/function-sets.svg)|![](https://www.mathsisfun.com/sets/images/relation-not-function.svg)|
|---|---|

<Footnotes separator>
  <Footnote><a href="https://www.mathsisfun.com/sets/function.html" rel="noreferrer" target="_blank">Function</a></Footnote>
</Footnotes>

---
layout: two-cols
---

## Why Pure Functions

* Determinacy
* No Side Effect

### Benefit

* Cacheable

::right::

```javascript
const squareNumber = memoize(x => x * x);

squareNumber(4); // 16

squareNumber(4); // 16, returns cache for input 4

squareNumber(5); // 25

squareNumber(5); // 25, returns cache for input 5
```

```javascript
const memoize = (f) => {
  const cache = {};

  return (...args) => {
    const argStr = JSON.stringify(args);
    cache[argStr] = cache[argStr] || f(...args);
    return cache[argStr];
  };
};
```

---
layout: two-cols
hideInToc: true
---

## Why Pure Functions

* Determinacy
* No Side Effect

### Benefit

* Cacheable
* Portable

::right::

```javascript
// impure
const signUp = (attrs) => {
  const user = saveUser(attrs);
  welcomeUser(user);
};

// pure
const signUp = (Db, Email, attrs) => () => {
  const user = saveUser(Db, attrs);
  welcomeUser(Email, user);
};
```

---
hideInToc: true
---

## Why Pure Functions

* Determinacy
* No Side Effect

### Benefit

* Cacheable
* Portable
* Testable


---
layout: two-cols
hideInToc: true
---

## Why Pure Functions

* Determinacy
* No Side Effect

### Benefit

* Cacheable
* Portable
* Testable
* Reasonable

::right::

```javascript
const { Map } = require('immutable');

// Aliases: p = player, a = attacker, t = target
const jobe = Map({ name: 'Jobe', hp: 20, team: 'red' });
const michael = Map({ name: 'Michael', hp: 20, team: 'green' });
const decrementHP = p => p.set('hp', p.get('hp') - 1);
const isSameTeam = (p1, p2) => p1.get('team') === p2.get('team');
const punch = (a, t) => (isSameTeam(a, t) ? t : decrementHP(t));

punch(jobe, michael); // Map({name:'Michael', hp:19, team: 'green'})
```

---
hideInToc: true
---

## Why Pure Functions

* Determinacy
* No Side Effect

### Benefit

* Cacheable
* Portable
* Testable
* Reasonable
* Parallel
