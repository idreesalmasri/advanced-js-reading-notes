##JS callback functions
1-In JavaScript, functions are objects.
2-we can pass functions as parameters to other functions and call them inside the outer functions.
3-a function that is passed to another function as a parameter is a callback function.
4-also we use callback functions for events declerations.

called asynchronous programming:JavaScript runs code sequentially in top-down order. However, there are some cases that code runs (or must run) after something else happens and also not sequentially.

when the callback function has no name and a function definition without a name in JavaScript is called as an “anonymous function”.

you can also write the same callback function as an arrow function.

##JavaScript | Promises
-Promises are used to handle asynchronous operations in JavaScript.
-Events were not good at handling asynchronous operations.

-Promises are the ideal choice for handling asynchronous operations in the simplest manner. They can handle multiple asynchronous operations easily and provide better error handling than callbacks and events.

-Promises do provide a better chance to a user to read the code in a more effective and efficient manner especially it that particular code is used for implementing multiple asynchronous operations. 

-###Benefits of Promises:
* Improves Code Readability.
* Better handling of asynchronous operations.
* Better flow of control definition in asynchronous logic
* Better Error Handling

###A Promise has four states:
* fulfilled: Action related to the promise succeeded.
* rejected: Action related to the promise failed.
* pending: Promise is still pending i.e. not fulfilled or rejected yet.
* settled: Promise has fulfilled or rejected.

Promise Consumers: Promises can be consumed by registering functions using 
* then() 
then() is invoked when a promise is either resolved or rejected. It may also be defined as a career which takes data from promise and further executes it successfully.
* catch()
catch() is invoked when a promise is either rejected or some error has occurred in execution. It is used as an Error Handler whenever at any step there is a chance of getting an error.
Applications :
* Promises are used for asynchronous handling of events.
* Promises are used to handle asynchronous http requests.


##Async/Await Function
Async:
functions will always return a value. It makes sure that a promise is returned and if it is not returned then javascript automatically wraps it in a promise which is resolved with its value.

Await:
Await function is used to wait for the promise. It could be used within the async block only. It makes the code wait until the promise returns a result. It only makes the async block wait.

##Test-Driven Development
Testing:Testing is the process of ensuring a program receives the correct input and generates the correct output and intended side-effects.

Manual Testing:Manual testing is the process of checking your application or code from the user’s perspective. Opening up the browser or program and navigating around in an attempt to test functionality and find bugs.

Automated Testing:Automated testing, on the other hand, is writing code that checks to see if other code works. Contrary to manual testing, the specifications remain constant from test to test. The biggest advantage is being able to test many things much faster.

summery:
* Testing is verifying our application does what it should.
* There are two types of tests: manual and automated
* Tests assert that your program will behave a certain way. Then the test itself proves or disproves that assertion.