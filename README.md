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

***Note:***

      👉 দুটো result বাইরে দরকার হলে object return করো আর sequence দরকার হলে array return            করো শুধু debug করতে চাইলে console.log করো
      👉 ফাংশনের আউটপুট forEach-এ ব্যবহার করতে হলে, callback-এর ভিতরে ফাংশন কল করে তার             return ভ্যালু দিয়ে কাজ করতে হবে
      👉 return করে সরাসরি পাওয়া যাবে না।
      👉 শুধু লুপ চালানোর জন্য forEachব্যাবহার করো। forEach কোনো কিছু return নেয় না বা দেয় না ।             কিন্তু তুমি ফাংশনের আউটপুট নিয়ে forEach–এর ভেতরে কাজ করতে পারো
      👉 ফাংশনের আউটপুট নিয়ে নতুন array তৈরি করতে map ব্যাবহার করো। 
          map নিজেই ফাংশনের return ভ্যালু নিয়ে array বানায়। element সবসময় array-এর আসল                 মানটাই হবে। return করা ভ্যালু দিয়ে element পরিবর্তন হয় না।
      👉 শর্ত অনুযায়ী বাছাই করতে filter ব্যাবহার করো।
      👉
      👉
      👉
      👉
      👉
      👉
      👉
      👉
      👉
