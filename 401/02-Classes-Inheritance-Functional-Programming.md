![packegs](https://miro.medium.com/max/2732/1*n04DXe4L4d-1zhDE2EtUQA.jpeg)
### Why would you want to run JavaScript code outside of a browser?
- make use interact with database and can be used to create RESTful APIs. So we can use the JS to write the backend coding on the server side. like C# and python.

### What is the difference between a module and a package?
_by the stack over flow:_
- A module is a single JavaScript file that has some reasonable functionality. A package is a directory with one or more modules inside of it and a package.

_by the npm docs_
- A *package* is a file or directory that is described by a `package.json` file. A *module* is any file or directory in the `node_modules` directory that can be loaded by the Node.js require() function.

* Note: Since modules are not required to have a package.json file, not all modules are packages. Only modules that have a package.json file are also packages.

### What does the node package manager do?
- Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node. js packages in your application. It is also an online repository for open-source Node.

_And we can mention more things that included in the npm docs as following:_
* Adapt packages of code for your apps, or incorporate packages as they are.
* Download standalone tools you can use right away.
* Run packages without downloading using npx.
* Share code with any npm user, anywhere.
* Restrict code     to specific developers.
* Create Orgs (organizations) to coordinate package maintenance, coding, and * developers.
* Form virtual teams by using Orgs.
* Manage multiple versions of code and code dependencies.
* Update applications easily when underlying code is updated.
* Discover multiple ways to solve the same puzzle.
* Find other developers who are working on similar problems and projects.

### ways of export module:
1. anonymous function
> module.exports = function (msg) { console.log(msg);};

so you can use it now :
>var msg = require('./Log.js'); msg('Hello World');

2. Export Function as a Class
```
module.exports = function (firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = function () { 
        return this.firstName + ' ' + this.lastName;
    }
}
```
and now can be used as following:
```
var person = require('./Person.js');

var person1 = new person('James', 'Bond');

console.log(person1.fullName());
```
