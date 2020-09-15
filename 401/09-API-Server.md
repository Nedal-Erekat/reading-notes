# API

#### The parameters of the callback function are:

1. req, the request object.
1. res, the response object.
1. next, indicating the next middleware function.
1. The value of the name parameter.
1. The name of the parameter.

- Routing:refers to how an application’s endpoints (URIs) respond to client requests.
- Route Prefixing: Route grouping is a concept to make the route function that receive same prefix of different requests.
- request body: data sent by the client to your API.
- Request “Query” :the values that the client browser passed to the server during an HTTP request
- Request “Params” : is a combination of the keys/values you’ll find in Request.Querystring , Request.Form , Request.Cookies , Request.ServerVariables

* Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.