# Leet-Code-Java-Script-30-Days-Challange
In this project we are solving 35 Java Script Provlame.That is a newlly uploaded LeetCode weabsite as challange.


**Problame No-01: Write a function createHelloWorld. It should return a new function that always returns "Hello World"**

Solution:              
_var createHelloWorld = function() {
    return function(...args) {
        return "Hello World";
    };
};
const f=createHelloWorld();
console.log(f());_

**Alternative**:

__const createHelloWorld=()=>()=>"Hello World";
const e=createHelloWorld();
console.log(e());_


