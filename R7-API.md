# web servers( “Web Services” or "APIs")
* A web page is a “representation” of a resource. Resources are just concepts. URLs--those things that you type into the browser...
* Those URLs tell the browser that there's a concept somewhere. A browser can then go ask for a specific representation of the concept. 
* computers can use those same protocols to send messages back and forth to each other.

# SuperAgent
#### SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!


> http: This part tells the browser what protocol to use.
```
 request
   .post('/api/pet')
   .send({ name: 'Manny', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });
   ```