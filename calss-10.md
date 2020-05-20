# learn how to find the errors in your code
### The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope. 
- Each time a script enters a new execution context, there are two phases of activity: 
1. PREPARE
   - The new scope is created
   - Variables, functions, and arguments are created
   - The value of the this keyword is determined 
2. EXECUTE
   - Now it can assign values to variables
   - Reference functions and run their code
   - Execute statements 

## ***In the interpreter, each execution context has its own va ri ables object.It holds the variables, functions, and parameters available within it.Each execution context can also access its parent's v a ri ables object.*** 
#### If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code. 
- Error objects can help you find where your mistakes are and browsers have tools to help you read them. 
> PROPERTY DESCRIPTION
1. name Type of execution
2. message Description
3. fileNumber Name of the JavaScript file
4. lineNumber Line number of error
> OBJECT
1. Error :Generic error - the other error are all based upon this error
2. Syntax Error :Syntax has not been followed
3. ReferenceError Tried to reference a variable that is not declared/within scope
4. TypeError:An unexpected data type that cannot be coerced
5. Range Error: Numbers not in acceptable range
6. URI Error: encodeURI ().decodeURI(),and similar methods used incorrectly
7. EvalEr r or: eva l () function used incorrectly 

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
#### ***The JavaScript console will tell you when there is a problem with a script,where to look for the problem, and what kind of issue it seems to be. ***

## MORE CONSOLE METHODS
1. conso1e.info() can be used for general information
2. console.warn() can be used for warnings
3. console.error() can be used to hold errors 
4. console.group () method to group the messages together. 

# BREAKPOINTS 
### You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time. 

## COMMON ERRORS 
1. GO BACK TO BASICS 
2. MISSED/ EXTRA CHARACTERS 
3. DATA TYPE ISSUES 

> If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback. 


