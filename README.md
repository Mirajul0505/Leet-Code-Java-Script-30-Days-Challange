# Leet-Code-Java-Script-30-Days-Challange
In this project we are solving 35 Java Script Provlame.That is a newlly uploaded LeetCode weabsite as challange.


**Problame No-01: Write a function createHelloWorld. It should return a new function that always returns "Hello World"**

Solution:              
var createHelloWorld = function() {
    return function(...args) {
        return "Hello World";
    };
};
const f=createHelloWorld();
console.log(f());_

**Alternative**:

const createHelloWorld=()=>()=>"Hello World";
const e=createHelloWorld();
console.log(e());_

**Problame 02: Given an integer n, return a counter function. This counter function initially returns n and then returns 1 more than the previous value every subsequent time it is called (n, n + 1, n + 2, etc).**

var createCounter = function(n) {
      let value=n-1;
    return function() {
        return ++value; 
//**preiectrment mense value add before its return .PreIncrement Define ++i .**//
    };
};
 const counter = createCounter(9);
 console.log(counter());
 console.log(counter());
 console.log(counter());
