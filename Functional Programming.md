
# Functional Programming:-

- In computer science, functional programming is a programming paradigm, a style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

- It uses pure functions, where pure functions are the functions that act only on their parameters and return the value obtained by performing the operations on parameter

- Use Immutable data : An immutable data is an data whose state cannot be modified after it is created. 

- Easily able to create data structures insted of modifying ones which is already exist


## Benifits:-

- Reduce occurance of bugs in program 

- Easy to execute and debug

- Allow Parallel processing
	

## Limitations:-

- Not easy and difficult to understand for beginner

- Writing pure functions are easy but combining them with rest of application and I/O operations is the difficult task. 




# Functional Programming in Javascript:-

- We can assign functions to vaiables

- And they can be used in objects, arrays and as a argument to other functions and can be returned by functions


## Higher Order Functions:-
	
- HOF are the functions which accept functions as a arguments or return functions.


#### CONST is used in JavaScript which is used to enforce Immutability on variables.

#### OBJECT.ASSIGN() is a key to create objects in JavaScript

#### CONCAT() is used to append anything in array in FP, generally we use push() which mutates the original array
	
```
a = [1, 2]
b = [1, 2].concat(3)
b = [1, 2, 3]
```

### FILTER() used  for removing an item from an array: instead of using pop() and splice(), which modify the original array

```
const d = a.filter((v, k) => k < 1)
// d = [1]
```


## Pure Function:-

- Never changes any of the parameters that get passed to it by reference

- The return value of a pure function is not influenced by anything else than its input parameters

- During its execution, a pure function does not change anything outside of its


## Data Transformations:-

As in Functional Programming the data is immutable, then you might think how data is changed?

***Simple: Data is changed by creating copies.***

Functions in particular change the data by returning new copies of data.


## Following are the functions which are used to chnage the data

#### ARRAY.MAP():-

If we call Array.map() on any array, It will crete an new array which will contain the result of operation performed in the original array.

```
const a = [1, 2, 3]
const b = a.map((v, k) => v * k)
// b = [0, 2, 6]

```

#### ARRAY.REDUCE():-

If we call Array.reduce() on any array, It will allow us to transform that array on anything else, including a function, a boolean, an object.

```
const a = [1, 2, 3]
const sum = a.reduce((partial, v) => partial + v, 0)
<!-- // sum = 6 -->
```
	
## RECURSION:-

Recursion is a key topic in functional programming. when a function calls itself, it’s called a recursive function.

The classic example of recursion is the Fibonacci sequence (N = (N-1 + N-2)) calculation, here in its 2^N totally inefficient (but nice to read) solution:

```
var f = (n) => n <= 1 ? 1 : f(n-1) + f(n-2)
```

## COMPOSITION:-

Composition is another key topic of Functional Programming, a good reason to put it into the “key topics” list.

***Composition is how we generate a higher order function, by combining simpler functions***

- common way to compose functions in plain JavaScript is to chain them:

```
obj.doSomething()
.doSomethingElse()
```

- or, also very widely used, by passing a function execution into a function

```
obj.doSomething(doThis())
``` 