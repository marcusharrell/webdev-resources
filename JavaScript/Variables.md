[JavaScript Variables](https://www.developer.com/languages/javascript/javascript-variables/)
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
