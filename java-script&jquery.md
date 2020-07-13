# How JavaScript makes web pages more interactivs.


- **JavaScript**:-allows to make web pages more interactive ba accessing and modifying the content and markup used in a web page while it sis being viewed in a browser.

1. **ACCESS CONTENT**:-you can use JavaScript to select any element, attribute, or text from an HTML page. For example: Select the text inside all of the ```<hl>``` elements on a page.

2. **MODIFY CONTENT**:- You can use JavaScript to add elements, attributes, and text to the page, or remove them. For example:Add a paragraph of text after the first ```<hl>``` element.

3. **PROGRAM RULES**:- You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page. For example:A gallery script could check which image a user clicked on and display a larger version of that image.

4. **REACT TO EVENTS**:-You can specify that a script should run when a specific event has occurred. For example, it could be run when: A button is pressed,  A link is clicked (or tapped) on, A cursor hovers over an element,Information is added to a form, An interval of time has passed, A web page has finished loading.

### Script:-
- is a series of instructions that a computer can follow to achieve a goal.To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.

- Start with the big picture of what you want to achieve, and break that down into smaller steps.

1. **DEFINE THE GOAL**:- First, you need to define the task you want to achieve. You can think of this as a puzzle for the computer to solve.

2. **DESIGN THE SCRIPT**:- To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle. This can be represented using a flowchart. You can then write down individual steps that thecomputer needs to perform in order to complete each individual task (and any information it needs to perform the task), rather like writing a recipe that it can follow.

3. **CODE EACH STEP**:- Each of the steps needs to be written in a programming language that the compu ter
understands. In our case, this is JavaScript. As tempting as it can be to start coding straight away, it pays to spend time designing your script before you start writing it.

- **Designing a script**:- tasks:-once you know the goal of your script,you can work out the indivitual tasks neede to achieive it.This high-level view of the tasks can be represented using a flowchart.

- Each individual task may be broken down into a sequence of steps. When you are ready to code the script,these stepes can then be translated into individual lines of code.


## EXPRESSIONS and OPERATORS

- An **expression** evaluates into (results in) a single value. Broadly speaking there are two types of expressions.

1. **EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE** In order for a variable to be useful, it needs to be given a value. As you have seen, this is done using the assignment operator (the equals sign). 
```var color = 'beige';``` The value of co 1 or is now beige.

2. **EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE**
You can perform operations on any number of individual values (see next page) to determine a single value. For example: ```var area = 3 * 2;``` The value of area is now 6.

- **opreters**:-Expressions rely on things called operators; they allow programmers to create a single value from one or more values. list fo opreters

- **ASSIGNMENT OPERATORS**:-Assign a value to a variable
```color = 'beige';``` The value of co 1 or is now beige.

- **ARITHMETIC OPERATORS**:-Perform basic math
```area = 3 * 2;``` The value of area is now 6.

- **STRING OPERATORS**:- Combine two strings
```greeting= 'Hi 1 + 'Mol ly';``` The value of greeting is now Hi Molly.

- **COMPARISON OPERATORS**:-Compare two values and return true or fa 1 se
```buy = 3 > 5;``` The value of buy is fa 1 se.

- **LOGICAL OPERATORS**:-Combine expressions and return true or fa 1 se
```buy= (5 > 3) && (2 < 4);``` The value of buy is now true.


## Functions
- Functions consist of a series of statements that have been grouped together becouse they perform a spesific task. 

- basic functins has :- ```function sayHello(){```
                          ```document.write('Hello!');```
                         ``` }```

- if diifrent part of a script need to perform the same task, you do not need to reapet the same satementes multibel time -you use a function to do it.```(and reuse the same code)```

- **calling a function**:-having declared the function, you can then excute all of the statements between its curly braces just one line of code.

- if a function needs information to work,you indicate what it need to know in parentheses after the function name.parametres are used to like var within the function. 

- example:- ```function getArea(width, height)```
                   ```{return width * height;```
                   ```}```