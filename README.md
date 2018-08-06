### Primitive Types and Type Conversions

## Index
* [Learning Objective](#learning-objective)
* [Code Snippet](#code-snippet)
* [Studying The Snippet](#studying-the-snippet)


___

## Learning Objective
 Consider JavaScript's Data Primitives, Type Conversions(aka Coercion) and Operators
 * Data Primitive Types Covered: Boolean, Number and Null.
 * Operators: typeof and void.
 
[TOP](#index)

___
 
## Code Snippet

[PyTut Link](http://www.pythontutor.com/javascript.html#code=var%20result%3B%0Avar%20number%20%3D%2010%3B%0A%0Aresult%20%3D%20typeof%20Boolean%20%28void%20%28number.toString%28%29%29%20%2B%20String%28null%29%29.valueOf%28%29%3B%0A%0Aconsole.log%28result%29%3B&curInstr=4&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

````js
var result;
var number = 10;

result = typeof Boolean (void (number.toString()) + String(null)).valueOf();

console.log(result);

````

[Repl.it Link](https://repl.it/@Joaoviana/CodeSnippet)
````js
var result;
var number = 10;

result = typeof Boolean (void (number.toString()) + String(null)).valueOf();
number.toString();
// s0 : (String, '10')
String(null);
// s0 : (String, 'null')
void('10');
// s1: (undefined, undefined)
(undefined+ 'null').valueOf();
// s2: (string, 'undefinednull')
Boolean ('undefinednull');
//s3: (Boolean, true)
typeof true;
//s4 (string, 'boolean')
````
[TOP](#index)

## Studying The Snippet

Step-by-Step Explanation:
 1. s0 : number.toString() converts number variable 10 to a string '10' ; String(null) converts it to string 'null'
 2. s1 : void operator makes variable undefined - it acts as a 'dissociation' of its passed value
 3. s2 : valueOf() returns the primitive value of a Number; however, it is taking 'undefinednull' string as an argument.
 4. s3 : Boolean Primitive takes in a string and returns true.
 5. s4 : typeof true is string 'Boolean'
 
Head over again to the Repl.it link to see the Parsons 'reshuffle' method. Try to organise the declarations to reach to reach the same goal. 
[TOP](#index)

