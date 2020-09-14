## Routing 
refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.
These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method. In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function.

![](https://d33wubrfki0l68.cloudfront.net/a22bb45df146d43b57f2f6c90182d19e7394cd96/d6e10/assets-jekyll/blog/express-middleware-examples/middleware-30b3b30ad54e21d8281719042860f3edd9fb1f40f93150233a08165d908f4631.png)
## Terms
- Middleware : functions that have access to the request object (req), the response object (res), and the next middleware function in the - application’s request-response cycle.

- Request Object : what retrieves the values that the client browser passed to the server during an HTTP request.

- Response Object : communicates between the server and the output which is sent to the client.

- Application Middleware : software that provides services beyond those provided by the operating system to enable the various components of a distributed system to communicate and manage data.

- Routing Middleware : determining how an application responds to a client request to a particular endpoint.

