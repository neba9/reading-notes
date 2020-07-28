
# HTML Links

- **links**: are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

- You will commonly come across the following types of links:

- Links from one website to another

- Links from one page to another on the same website You can use a shorthand known as a relative URL.

- Links from one part of a web page to another part of the same page

- Links that open in a new browser window

- Links that start up your email program and address a new email to someone

- Ex: ```<a href="http://www.imbd.com">IMDB</a>```

- Links are created using the ```<a>``` element.

- The ```<a>``` element uses the href attribute to indicate the page you are linking to.

- The text between the opening ```<a> tag and closing </a>``` tag is known as link text.

- If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.

- You can create links to open email programs with an email address in the "to" field.

- You can use the id attribute to target elements within a page that can be linked to.

- **Directory Structure**:On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.

# CSS Layout

- how to control where each element sits on a page and how to create attractive page layouts.

-CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

- Ex: Block-level elements start on a new line Examples include:
```<h1> <p> <ul> <li>```

- Inline elements flow in between surrounding text Examples include:
```<img> <b> <i>```

- **Containing Elements**: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.EX: the header ```<div> elements contian logo & nav  onther <div>``` main content of the page, body & footer.

- **Controlling the Position of elements**:CSS has the following positioning schemes that allow you to control the layout of a page: normal flow,relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

- **Normal Flow**:position:static, In normal flow, each block-level element sits on top of the next one.
- ```h1{```
  ```background-color:blue;```
  ```padding:10px;}```

- **Relative Positioning**: moves an element in relation to where it would have been in normal flow.
- ```p.example{```
  ```position: relative;```
  ```top:10px;```
  ```left:100px;}```
- **Absolute positioning**:When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page. ```(They act like it is not there.)```
- **Fixed positioning** is a type of absolute positioning that requires the position property to have a value of fixed.

- **Floating El ements**:The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

- **Clearing Floats**:The clear property allows you to say that no element (within the same containing element) should touch the left or righthand
sides of a box. It can take the following values:

- EX:```clear {clear:left;}```

- **Screen Sizes**:Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

- **Screen Resolution**:Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

- **Page Sizes**:Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

- **Fixed Width Layouts**:Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
- Ex:```body {```
     ```width: 960px;``
     ```margin: 0 auto;}```

- **Liquid Layouts**:Liquid layout designs stretch and contract
as the user increases or decreases the size of their browser window. They tend to use percentages.
- Ex: ```body {```
      ```width: 90%;```
      ```margin: 0 auto;}```

- **Layout Grids**:Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them position items on a page, and the same is true for web designers.

- **CSS Frameworks**:its provid the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch

# Functions

- **Functions**:let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).

- this example has key word function , function name, and code block 

- Ex:```function sayHello(){document.write('Hello!')};```

- to call we use : ```sayHello();```

- function store the code required to perform a spesific task,and that the script can ask the function to perform that task whenever neede.

- **Calling a function**: having declaration the functio, you can then execute all of the statments between its curly braces with just one line of code.this is known as calling the function. 

- we can call the same function as many times as we want within the same javaScript file.

- sometimes a function needs specific information to perform its task.in such cases,when you declare the function you give it parameteres.inside the function ,the parameters act like variables.

- Ex:```function getArea(width, height){```
     ```return width * height;}```

- this function will calculate and return the area of a rectangle.it needs the rectangle width and height, each time you call the function these values could be different.

- calling function that need information.when you call a function has parametres, you spesify the values it should use in the parentheses that follow its name.he values are called arguments,they can be provided as values or as variables.

1. arguments as values

- ```getArea(3, 5);```

2. arguments as variables

- ```wallwidth =3;```
  ```wallHeight = 5;``
  ```getArea(wallWidth, wallHeight);```

- function can return more than one vvalue using an array.ex this function calculate the area and volume of a box.

- ```Ex: function getSize(widyh, height, deptj){```
  ```var area = width * height;```
  ```var volume = width * height * depth;```
  ```var sizes = [area, volume];```
  ```return size;```
```}``
```var areaOne = getSize(3, 2, 3)[0];```
```var volumeOne = getsize(3, 2, 3)[1];```

- areaOne var holds 3*2.the area is the first value in the sizes array
- volumeOne var holds 3*2*3.the volume is the second value in the size array.

- **ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS**:

- **function declaration** creates a function that you can ca ll later in your code. It is the type of function you have seen so far in this book.you
must give it a name, so these are known as named functions.Below, a function called area() is declared,

- Ex: ```function area (width, height)```
      ```return width * height;};```
      ```var size= area(3, 4) ;```

- the interpreter always looks for variables and function declarations before going through each section of a script, line-by -line.

- **FUNCTION EXPRESSION**:If you put a function where the interpreter would expect to see an expression, then it is treated as an expression, and it is known as a function expression.name is usually omitted.A function with no name is called an anonymous function.Below, the function is stored in a variable called area.

- Ex: ```var ar ea = f unction(width, height) {```
      ```return width * height;} ;```
      ```var size = area(3, 4) ;```

- the function is not processed until the interpreter gets to that statement. This means you cannot call this function before the interpreter has discovered it. It also means that any code that appears up to that point could potentially alter what goes on inside this function

- **VARIABLE SCOPE**:The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's **scope**.

- **LOCAL VARIABLES**:When a variable is created inside a function using the var keyword, it can only be used in that function. It is called a local variable or function-level variable. It is said to have local scope or function-level scope.It cannot be accessed outside of the function in which it was declared. Below, area is a local variable
- Local variables are only remembered during the period of time that a function is being executed

- **GLOBAL VARIABLES**:If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope. In the example shown, wa 11 Size is a global variable.
- Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded.

- Ex: ```function getArea(width, height)```
      ```var area = width * height;```
      ```return area;```
      ```var wallSize = getArea(3, 2);```
     ```document. write(wa 11 Si ze);```