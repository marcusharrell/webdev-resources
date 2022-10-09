[JavaScript Variables](https://www.developer.com/languages/javascript/javascript-variables/)
# WTF are Variables?
[Variables are containers for storing data (storing data values).](https://www.w3schools.com/js/js_variables.asp)

[Here is a great analogy further explaining variables using a real world example](https://javascript.info/variables#a-real-life-analogy)


In this example, x, y, and z, are variables, declared with the var keyword:

```
var x = 5;
var y = 6;
var z = x + y;
// 11 
```

In this example, x, y, and z, are variables, declared with the let keyword:

```
let x = 5;
let y = 6;
let z = x + y;
// 11
```



Below are undeclared variables. 
*(Undeclared variables mean that the variable does not exist in the program at all!)*




### How to Declare and Set a JavaScript Variable

Before we get into the business of declaring and setting a variable in JavaScript, we should establish that there are two variable scopes in JavaScript: local and global.

Local variables are declared inside a function or block using the const, let, or var keywords and are accessible only within that function or block:

```
function aFunction() {
  var myLocalVar = 99; //local variable  
  console.log(myLocalVar); //99 
}

//ReferenceError: myLocalVar is not defined
console.log(myLocalVar); 
```
Meanwhile, global variables are those that are declared without the const, let, or var keywords or explicitly added to the global window object. As you would expect, once declared, global variables are accessible from anywhere in the script. They can be declared outside the function or explicitly added to the window object:
```
globalVar = 'I am global!';

function aFunction() {
  var myLocalVar = 99; //local variable  
  console.log(myLocalVar); //99 
  //Inside aFunction: I am global!
  console.log('Inside aFunction: ' + globalVar);
  window.anotherGlobalVar = 4.5;
}
aFunction();

//Outside a function: I am global!
console.log('Outside a function: ' + globalVar); 

//anotherGlobalVar = 4.5
console.log('anotherGlobalVar = ' + anotherGlobalVar);
```
