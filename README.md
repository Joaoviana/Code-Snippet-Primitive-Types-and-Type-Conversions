### Primitive Types and Type Conversions

## Index
* [Learning Objective](#learning-objective)
* [Study Snippet](#study-snippet)

___

## Learning Objective
 Considering type conversions and how primitive types influence the outcome of an integer variable, such as:
  * Boolean, void, null, typeof
  * toString(), String() and valueOf()
 
[TOP](#index)

___
 
## Study Snippet
//add declaration of operators, types etc

[PyTut Link](http://www.pythontutor.com/javascript.html#code=var%20result%3B%0Avar%20number%20%3D%2010%3B%0A%0Aresult%20%3D%20typeof%20Boolean%20%28void%20%28number.toString%28%29%29%20%2B%20String%28null%29%29.valueOf%28%29%3B%0A%0Aconsole.log%28result%29%3B&curInstr=4&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

````js
var result;
var number = 10;

result = typeof Boolean (void (number.toString()) + String(null)).valueOf();

console.log(result);

````

[Repl.it Link](https://repl.it/@Joaoviana/UnimportantNaivePdf)
````js
var result;
var number = 10;

result = typeof Boolean (void (number.toString()) + String(null)).valueOf();
number.toString();
// s0 : (String, '10')
String(null);
// s0 : (String, 'null')
void('10')
// s1: (undefined, undefined)
void(undefined+ 'null').valueOf()
// s2: (undefined, 'undefined)
Boolean (undefined)
//s3: (Boolean, false)
typeof false;
//s4 (string, 'boolean')
````
[TOP](#index)
