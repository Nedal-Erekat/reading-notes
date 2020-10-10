

![](https://miro.medium.com/max/880/0*58b4t5kGuV3DqgI1.png)
## learn how to get the most out of the Heroku platform.


- Set up
 -  install the Heroku Command Line Interface (CLI).
- Prepare the app
 - In this step, you will prepare a sample application that’s ready to be deployed to Heroku.
 - If you are new to Heroku, it is recommended that you complete this tutorial using the Heroku-provided sample application.
- Deploy the app
- View logs
- Define a Procfile
- Scale the app
- Declare app dependencies
- Run the app locally
- Push local changes
- Provision add-ons
- Start a console
- Define config vars
- Provision a database
- Next steps

![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/1200px-Node.js_logo.svg.png)


# Node.js For Beginners. Deploy Your Blog to Heroku
#### Error pages are not what typically appear on your screen when you're surfing the web, but when it happens it's so annoying! To see how servers work from within, we will build a simple web server by ourselves. We will use Node.js as a server part technology for that task. Then we'll use Heroku cloud application platform to turn this local server into a world wide server.
#### We will use Node.js for our project. Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It's written in JavaScript and can be run within the Node.js runtime on any platform. First of all, of course, you need to install it. You'd better check the download page for more details. I'll wait until you finish, so don't worry. Is it done? Great! Now you can create your first web server. And it will be one of the easiest tasks in your life.


-  we need to create a JavaScript file
```
var http = require("http");

http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
}).listen(3000);
```

#### Now, to be sure it's a web server and not just a piece of code that returns a single line of text, we'll use it as a server! You can check it with your smartphone. Let's suppose, your laptop's IP address within your local network is 192.168.1.101. You can connect to your server through the 3000th port (for this particular example) by typing http://192.168.1.101:3000/ in your browser. Works well in my case:


