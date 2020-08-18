
# Debugging

-  **debugging**:is the process of finding and resolving bugs within computer programs, software, or systems.

- **EXECUTION CONTEXTS**:The JavaScript interpreter uses the concept of execution contexts.There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

- Every statement in a script lives in one of three execution contexts:
1. **GLOBAL CONTEXT**:Code that is in the script, but not in a function.There is only one global context in any page.

2. **FUNCTION CONTEXT**:Code that is being run within a function.Each function has its own function context.

3. **EVAL CONTEXT (NOT SHOWN)**:Text is executed like code in an internal function called eval.

- **VARIABLE SCOPE**:The first two execution contexts correspond with the notion of scope.

- **GLOBAL SCOPE**:If a variable is declared outside a function, it can be used anywhere because it has global scope.If you do not use the var keyword when creating a variable, it is placed in global scope.

- **FUNCTION-LEVEL SCOPE**:When a variable is declared within a function,it can only be used within that function. This is because it has function-level scope.

- **The tasck**:the javaScript interpreater processes one line of code at atime.when a statmenet needs data from another function,it stacks(or piles) the new function on top of the current task.

- Each time a script enters a new execution context, there are two phases of activity:

1. **Prepare**:
- The new scope is created
- Variables, functions, and arguments are created
- The value of the this keyword is determined

2. **Execute**:
- Now it can assign values to variables
- Reference functions and run their code
- Execute statements.

- ### Error objects

- **Error objects**: can help you find where your mistakes are and browsers have tools to help you read them.

- When an Error object is created, it will contain the
following properties:
- **property                description**
  name                    Type of excution
  massage                 Descripion
  fileNumber              name of the javaScript
  line number             Line number of error

- There are seven types of built-in error objects in JavaScript. You'll see them on the next two pages:

- **object               Description**
1. **Error**:Generic error - the other errors are all based upon this error.
2. **Syntax Error**:Syntax has not been followed.
3. **Ref erenceError**:Tried to reference a variable that is not declared/within scope.
4. **TypeError**: An unexpected data type that cannot be coerced
5. **Range Error**:Numbers not in acceptable range.
6. **URI Error**: encodeURI ().decodeURI(),and similar methods used incorrectly.
7. **Eval Error**:eval () function used incorrectly.

- #### How to deal with errors

- Now that you know what an error is and how the browser treats them, there are two things you can do with the errors.

1. **DEBUG THE SCRIPT TO FIX ERRORS**:If you come across an error while writing a script(or when someone reports a bug), you will need to debug the code, track down the source of the error,and fix it.

2. **HANDLE ERRORS GRACEFULLY**:You can handle errors gracefully using try, catch, throw, and fina1ly statements.

- **WRITING FROM THE SCRIPT TO THE CONSOLE**:Browsers that have a console have a console object, which has several
methods that your script can use to display data in the console.The object is documented in the Console API.

- **More console Methodos**:To differentiate between the
types of messages you write to the console, you can use three different methods.

1. conso1e.info() can be used for general information.
2. console.warn() can be used for warnings.
3. console.error() can be used to hold errors.

- In browsers that support it, the console. table () method lets you output a table showing:Obects,arrays  that contain other objects or arrays.

- Using the **console. assert()** method, you can test if a condition is met, and write to the console only if the expression evaluates to false.

- **HANDLING EXCEPTIONS**:If you know your code might fail, use try, catch, and finally.Each one is given its own code block.

- **TRY**:First, you specify the code that you think might throw an exception within the try block.

- **CATCH**:If the try code block throws an exception, catch steps in with a alternative set of code.

- **FINALLY**:The contents of the fina11y code block will run either way - whether the try block succeeded or failed.

