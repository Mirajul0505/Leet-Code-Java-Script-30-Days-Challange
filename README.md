**Java Script Problame Solving**

In this project we are solving 1000 Java Script Provlame.


**Problame No-01: Write a function createHelloWorld. It should return a new function that always returns "Hello World"**

                var createHelloWorld = function() {
                    return function(...args) {
                        return "Hello World";
                    };
                };
                const f=createHelloWorld();
                console.log(f());

**Alternative**:

                const createHelloWorld=()=>()=>"Hello World";
                const e=createHelloWorld();
                console.log(e());

**Problame 02: Given an integer n, return a counter function. This counter function initially returns n and then returns 1 more than the previous value every subsequent time it is called (n, n + 1, n + 2, etc).**

                var createCounter = function(n) {
                      let value=n-1;
                    return function() {
                        return ++value; 
                    };
                };
                 const counter = createCounter(9);
                 console.log(counter());
                 console.log(counter());
                 console.log(counter());

 **Problame No-03: Write a function createHelloWorld. It should return a new function that always returns "Hello World"**
       
                    var HelloWorld = function() {
                        
                        return function(...args) {
                            return "Hello World";
                        };
                    };
                     
                      const f=HelloWorld();
                    console.log(f());

 **Alternative:**

                    const createHelloWorld=()=>()=>"Hello World";
                    const m=createHelloWorld();
                    console.log(m());  

 **Problame 04: Given an integer n, return a counter function. This counter function initially returns n and then returns 1 more than the previous value every subsequent time it is called (n, n + 1, n + 2, etc).**
  
                    var createCounter = function(n) {
                          let value=n-1;
                        return function() {
                          
                            return ++value;
                        };
                    };
                    
                     const counter = createCounter(9);
                     console.log(counter());
                     console.log(counter());
                     console.log(counter());



**Provlame-05:Write a function expect that helps developers test their code.It should take in any value val and return an object with the following two functions.toBe(val) accepts another value and returns true if the two values === each other.If they are not equal, it should throw an error "Not Equal".notToBe(val) accepts another value and returns true if the two values !== each other.If they are equal, it should throw an error "Equal".**

 **Solution:**
    
                    function x(){
                            const val=34;
                            const n=32;
                           function e(a,b){
                                if(a===b){
                                    return {result:true};
                                 }else{
                                    return {Error:"Not Equal"};
                                }
                            };
                           
                            function f(c,d){
                                    if(c!==d){
                                        return {Error:"Not Equal"};
                                    }else{
                                        return {result:true};
                                    }
                                }; 
                            return {
                                eResult:e(val,n),
                                fResult:f(val,n),
                            };
                     };
                     const output=x();
                    console.log(output);
                     
**Alturnative:**
                    
                    const val=32;
                    const n=32;
                    function e(){
                        function a(x,y){
                            return x===y ? {rasult:true}:{rasult:"dont Matcj=h"};
                        };
                        function b(k,l){
                            return k!==l ? {result:"dont match"}:{result:true};
                        };
                        return{
                            aRasult:f(val,n),
                            bRasult:b(val,n),
                        }
                    };
                    const res=e();
                    console.log(res)
                    
**problem 06: write a js function to find the sum of two number**
**solution:**
                    
                    function sum(x,y){
                        return (x+y);
                    }
                    console.log(sum(19,11));
                    
**problem 07: write a js function to find the product of two number**
**solution:**

                       function product(x,y){
                          return (x*y);
                       }
                       console.log(product(20,9
                       
                       
**problem 08: write a js function to find the modulas of two number**
**solution:**

                     function reminder(a,b){
                        return (a%b);
                     }
                     console.log(product(20,9));
                     

**problem 09: write a js function to find the deferance of two number**
**solution:**
                  
                    function defferance(x,y){
                        return (x-y);
                    }
                    console.log(defferance(20,19));


**Provlam-10: Write a JavaScript function to check if a number is positive, negative or zero**
**solution:**
 
                    function e(n,n,n){
                        if(n>0){
                            return "This is a positive Number";
                        }
                        else if(n<0){
                            return " This Is a Nagitive Number";
                        }else{
                            return "It Is a Zero";
                        }
                        
                    }
                    console.log(e(0,));

**Problem-11: Write a JavaScript function to check if a number is odd or even**
**solution:(Common code for problame 11 to )** 

                    function oddOrEven(n){
                        if (n % 2===0){
                            return "This Is a Odd Number";
                        } else {
                            return "this Is A Even number";
                        }
                    };
                    console.log(oddOrEven(100000000000));

**Provlame-12: Write a JavaScript function which returns the number of even or odd numbers in an array**
**solution:**
 
                    const array=[334,245,3535,546,56,243,6574,4543,234,4656,4645,858,800];
                    
                    function number(n){
                        if(n%2===0){
                            return(n + " is Even Number ");
                        }else{
                            return(n +" is odd Number ");
                        }
                    }
 
**Using for loop**

                    for(let i=0; i<array.length;i++){
                        number(array[i]);
                        console.log(number(array[i]));
                    }

**Alturnative:  Using forEatch loop**

                    array.forEach(function(element,index,array){
                    
                        let result=number(element,index,array);
                        console.log(result);
                        console.log(index);
                        console.log(array);
                    });
**Result push in a new array**
                    let result = [];
                    array.forEach(function(index){
                        result.push(number(index));
                    
                    });
                    console.log(result.length);
                    console.log(result);
**ES6 Methode:**
                    let num=[];
                    array.forEach(index=>{num.push(number(index))});
                    console.log(num);


**Using  for...of loop**

                    for(let e of array){
                       let result = number(e);
                       console.log(result);
                    };


                    let digit={ key:[] };
                    for(let x of array){
                        digit.key.push(number(x));
                    };
                    console.log(digit);

**Using While Loop**

                    let newVal=[];
                    let i=1;
                    while(i<=15){
                        newVal.push(number(i));
                        i++;
                    }
                    console.log(newVal);


**Problem-13: Write a JavaScript function to calculate the square of a number**
**solution:**
                    
                    function squareNumber(n){
                        return (n*n);
                    }
                    console.log(squareNumber(10000000000));

**Problem-14: Write a JavaScript function to concatenate two strings**
**solution:**
                    let str1="Abdur";
                    let str2="Rahaman"
                     function concatenate(){
                        return `${str1} ${str2}`;
                     }
                     console.log(concatenate());
**Problem-15: Write a JavaScript function to find the biggest number among 3 numbers.**
**solution:**
                     function check(a,b,c){
                        if (a>b){
                            return a;
                        }else if (c>a){
                            return c;

                        }else{
                            return b;
                        }
                     }
                     console.log(check(113,32,9));


******String To Array Convartion Using Defferent Methode:******

**Common Code:** 
                    
                    let str="Hellow Worldddgg!";
                    let arr=str.split("");
                    
**Using for loop:** 
    
               
                   let b=[];
                   for(let i=0; i<arr.length; i++){
                           b.push(arr[i].toUpperCase());
                   };
            
                   console.log(b);
                   
        
**Using Map() Methode:**


                   let newArray=arr.map(function (value){
                          return value.toUpperCase();
                   });
                   console.log(newArray);
                   
        
**Using ES6 Methode:**

        
                   let newArrES6 =arr.map((value)=>value.toUpperCase());
                   console.log(newArrES6);
               
        
**Using forEah loop:**


                   let c=[];
                   arr.forEach(function (e){
                          c.push(e.toUpperCase());
                    })
                    console.log(c);
                  
            
**ES6 Methode:**


                     let d=[];
                     arr.forEach((x)=>d.push(x.toLowerCase()));
                     console.log(d);
              
              
                     // Using for...fo loop
                     let f=[];
                     for(value of arr){
                            f.push(value.toLowerCase());
                     }
                     console.log(f);

                     
              
**Using While loop:**


      
                     let h=[];
                     let i=0;
                     while(i<arr.length){
                            h.push(arr[i].toUpperCase());
                            i++;
                     } 
                     console.log(h);


/*  problame 05:Given an integer array arr and a mapping function fn, return a new array with a transformation applied to each element.
    The returned array should be created such that returnedArray[i] = fn(arr[i], i).
    Please solve it without the built-in Array.map method. */

  
       ** Using forEach loop**

1.
        
                    let arr=[1,2,3,4];
                    let returnedArray=[];
                    function fn(){
                        let increment=parseInt(arr);
                        arr.forEach(function(arr,i){
                           increment +=1;
                           returnedArray.push(increment);
                          
                        }); 
                       
                    }
                    fn();
                    console.log(returnedArray);





2 



                    let arra=[1,2,3,4];
                      let newArra=[];
                      let map=function (arr){
                              arr.forEach(function(element,i){
                               element=element+1;
                              // element=element+1;
                             newArra.push(element);
                      
                          }); 
                          
                      };
                      
                      map(arra);
                      console.log(newArra);



3

                      
                      let oldArray=[5,6,7,8,9,10];
                      let returnNewArray=[];
                      let customMap=function(ara,index){
                          ara.forEach(function(element,index){
                              let value = element+1;
                              returnNewArray.push(value);
                          })
                      }
                      customMap(oldArray);
                      console.log(returnNewArray);



                **Using For Loop **


1


                        let array=[4,5,6,7];
                        let newArray=[];
                        
                        function c(i){
                          
                            for(let i=0; i<array.length;i++){
                                let count = array[i];
                                count=count+1;
                                 newArray.push(count);
                            }
                        }
                        c();
                        console.log(newArray);



2   



                      let val=[1,3,5,7,14];
                      let newVal=[];
                      let customFunction=function(parameter){
                      for(let i=0;i<parameter.length;i++){
                          let value=parameter[i];
                          value =value+1;
                          newVal.push(value);
                      }
                      };
                      customFunction(val);
                      console.log(newVal);



3


                      
                       let array=[1,2,3,4];
                      var map = function(arr,fn) {
                          let returnedArray=[];
                          
                          for(let i=0; i<arr.length; i++){
                              let callback=fn(arr[i],i)
                              returnedArray.push(callback);
                          }
                         
                          return returnedArray;
                      };
                      
                       let result =map(array, (n)=>n+1);
                       console.log(result);

                      

                                          





