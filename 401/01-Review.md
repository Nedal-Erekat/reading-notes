Readings: Node Ecosystem, TDD, CI/CD


1. Array map() Method
    > The map() method creates a new array with the results of calling a function for every array element. calls the provided function once for each element in an array, in order. and this method does not change the original array.

    ```
    array.map(function(currentValue, index){code}
    ```

2. Array reduce() Method
    > The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in single output value. Your reducer function's returned value is assigned to the accumulator, whose value is remembered across each iteration throughout the array, and ultimately becomes the final, single resulting value.

    ```
    array.reduce(function(total, currentValue, currentIndex, arr), initialValue)
    ```
3. superagent() Method
- use superagent() to fetch data from a URL and log the result:

>  normal Promise .then() syntax
```
superagent.get('https://swapi.dev/api/people/')
  .then( data => {
    console.log(data.body);
  })
```

> async / await syntax
```
async function cities (name){
  let result= await superagent.get(`https://geocode.xyz/${name}?json=1`)
  console.log(result.body)
}
```

4. promises 
#### Promises are one way to manage Asynchronous actions. Like a callback, a promise allows you to execute some code and “move on”, allowing for that code to take as long as it needs to run.
#### A promise says, “Hey, Javascript, you go ahead and do some work. I don’t care how long it takes and I’m going to go ahead and keep working … but let me know when you’re done .then() give me the data and let me deal with it myself”

5. Are all callback functions considered to be Asynchronous? 
#### Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous, for example, Array's forEach.For a function to be asynchronous it needs to perform an asynchronous operation. 

## Node.js
Node.js is an open source server environment and Node.js uses asynchronous programming!
> A common task for a web server can be to open a file on the server and return the content to the client.

- Here is how Node.js handles a file request:
 
1. Sends the task to the computer's file system. 
1. Ready to handle the next request. 
1. When the file system has opened and read the file, the server returns the content to the client.

- What Can Node.js Do?
1. Node.js can generate dynamic page content
1. Node.js can create, open, read, write, delete, and close files on the server
1. Node.js can collect form data
1. Node.js can add, delete, modify data in your database

## npm (Node package manager) 
#### These are libraries built by the awesome community which will solve most of your generic problems. npm (Node package manager) has packages you can use in your apps to make your development faster and efficient.

