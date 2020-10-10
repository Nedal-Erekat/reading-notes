# WHAT IS AN OBJECT? 

#### A set of variables and functions to creat a model of a somthing. In an object variables known as proparites and functions as methods.

## creating an Object:
#### literal notaion, the following show the general way to creat an object:- 

> `var` name of oject `= {`
> proparity_name(key) `:` value `,`
> method_name`: function(){`
> code...
> `}`
> `};`

## accessing an Object and dot notaion:
#### You can access by this:-
var anyName=objectName.proparityName/method;


# The Document Object Model (DOM):
#### specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.   
### THE DOM TREE IS A MODEL OF A WEB PAGE As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes. 
#### WORKING WITH THE DOM TREE Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
> get El ement Byld (),
> getElementsByClassName(),
2. Use its text content, child elements, and attributes. 
#### DOM queries may return one element, or they may return a Nodelist,which is a collection of nodes. 
### NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element). 

## GET/UPDATE ELEMENT CONTENT
####  how to access/update element content. Your choice of techniques depends upon what the element contains. 
#### When you select a text node, you can retrieve or amend the content of it using the `node Value` property. 

## CROSS-SITE SCRIPTING`(XSS)` ATTACKS 
#### If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise, an attacker could gain access to your users' accounts. 

- DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes. 
- Whenever a DOM query can return more than onenode, it will always return a Nadel i st. 
- From an element node, you can access and update its content using properties such as textContent and i nnerHTML or using DOM manipulation techniques. 


 

