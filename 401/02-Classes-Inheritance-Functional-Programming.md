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

> module.exports = function (firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = function () { 
        return this.firstName + ' ' + this.lastName;
    }
}

and now can be used as following:

> var person = require('./Person.js');
    var person1 = new person('James', 'Bond');
    console.log(person1.fullName());


- Node.js: is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside of a web browser.

- V8 Engine: is Google’s open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and in Node. js, among others. It implements ECMAScript and WebAssembly, and runs on Windows 7 or later, macOS 10.12+, and Linux systems that use x64, IA-32, ARM, or MIPS processors.

- module: is a single JavaScript file that has some reasonable functionality.

- package: is a directory with one or more modules inside of it.

- ecosystem: is a managed lifecycle and dependency injection for the application components.

- node package manager (npm): is an online repository for the publishing of open-source Node.js projects and a command-line utility for interacting with said repository that aids in package installation, version management, and dependency management.

- server: is a computer program or a device that provides functionality for other programs or devices, called “clients”.

- interpreter: is the same as the complier but an interpreter directly executes the instructions in the source programming language while a compiler translates those instructions into efficient machine code.

- environment: refers to the state of a computer, determined by a combination of software, basic hardware, and which programs are running. For example, if a program is running in a Windows environment, it means that the program is utilizing the Windows operating system.

- compiler: is a program that translates code written in a high-level programming language (like JavaScript or Java) into low-level code (like Assembly) directly executable by the computer or another program such as a virtual machine.