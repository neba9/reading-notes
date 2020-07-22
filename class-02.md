# Text

- most **web site** is made up of text. It is the most common way of conveying information to the visitor. For that reason, it makes sense to pay some attention to how it is formatted. How your format your text has a huge influence on how your page looks and, more importantly, how easily people can read it.

- When creating a web page, you add tags ```(known as markup)``` to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

1. **Structural markup**: the elements that you can use to describe both headings and paragraphs.

- example:-**heading tag** HTML has six levele of heading.Browsers display the contents of headings at different sizes.

- **pargraphs tag** To create a paragraph, surround the words that make up the paragraph with an opening ```<p> tag and closing </p>``` tag. By default, a browser will show each paragraph on a new line.

2. **Semantic markup**: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation ```(and who said it)```, the meaning of acronyms, and so on.

- example:- **stront** The use of the ```<strong>``` element indicates that its content has strong importance.

- **em**:- The ```<em>``` element indicates emphasis that subtly changes the meaning of a sentence.

# CSS

- **css**:- is Cascading Style Sheets,for describing the presentation of Web pages, including colors, layout, and fonts.css rule contain two parts: a selector and a declaration.

- **Selector**: indicate which elementes the rule applies to.the same rule can apply to more than one element if you separate the element names with commas.

- **Declaration**: indicate how the elements referred to in the selector should be styled.declaration are split into two parts ```(a property snd a value)``` and are saparated by a colon.


-example: ``` p {```
    ```font-family: arial;}```

```h1, h2, h3 {```
    ```font-family: Arial;```
    ```color:yellow;}```

- this rule indicates that all h1,h2,h3 elements should be shown in the typeface,in a yellow color.

- **properties**:indicate the aspects of the element you want to change.for example, color,font,width,height and border.

- **values**: specify the settings you want to use for the chosen properties.for examples, if you want to specify a color property then the value is the color you want the text in these elements to be.

# JavaScript instraction

- **A script** is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **statement**. Statements should end with a semicolon.

- A statement is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon.

- Some statements are surrounded by curly braces; these are known as code blocks. The closing curly brace is not followed by a semicolon.

### COMMENTS
- You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code. two types of comments

1. **MULTI-LINE COMMENTS**: To write a comment that stretches over more than one line, you use a multi-line comment, starting with the /* characters and ending with the * / characters. Anything between these characters is not processed· by the JavaScript interpreter.

2. **SINGLE-LINE COMMENTS**:In a single-line comment, anything that follows the two forward slash characters I/ on that line will not be processed by the JavaScript interpreter. Singleline comments are often used for short descriptions of what the code is doing.

## WHAT IS A VARIABLE?

- **Variable** means anything that can vary. JavaScript includes variables which hold the data value and it can be changed anytime. JavaScript uses reserved keyword var to declare a variable. A variable must have a unique name.

- var is an example of what programmers call a key word.the javaScript interpreter known that this keyword is used to creat a variable.in order to use the variabel, you must give it a name.```(its claaed identifier)```. if variable name is more than one word ti is usually written in a camelCase.

- example: ```var quantity = 3 ;``` this example has variable name, assignment opretor and variable value.

### DATA TYPES

-  Data type indicates characteristics of data. It tells the compiler whether the data value is numeric, alphabetic, date etc., so that it can perform the appropriate operation.JavaScript distinguishes between numbers,
strings, and true or false values known as Booleans.

- **NUMERIC DATA TYPE**: The numeric data type handles numbers.Ex 0.75

- Ex: ```var price;```
      ```var quantity;```
      ```var total;```

      ```price= 5;```
     ``` quantity= 14;```
      ```total= price * quantity;```

     ```var el = document.getElementById('cost);```
     ```el.textContent ='$' + total;```



- **STRING DATA TYPE**: The strings data type consists of letters and other characters.Ex 'Hi, Ivy!'

- Ex: ```var username;```
      ```var message;```
      ```username = 'Molly';```
      ```message = 'See our upcoming range';```
      ```var elName = document.getElementByld{'name');```
      ```elName .textContent = username;```
      ```var elNote = document .getElementByld( 'note');```
      ```elNote .textContent = message;```

- **BOOLEAN DATA TYPE**: Boolean data types can have one of two va lues: true or false.Ex true

- Ex: ```var inStock;```
      ```var shipping;```

      ```inStock = true;```
      ```shipping= fa l se;```
      
      ```var elStock = document.getElementByld('stock');```
     ```elStock.className = inStock;```

     ```var el Ship = document .getElementByid('shipping');```
     ```elShip.className = shipping ;```

## ARRAYS

- **An array** is a special type of variable. It doesn't just store one value; it stores a list of values.Arrays are especially helpful when you do not know how many items a list will contain because, when you create the array, you do not need to specify how many values it will hold.

- ex: ```var colors;```
      ```colors ['white', 'black', ' custom '];```
      ```var el document.getElementByld('col ors');```
      ```el . textContent = col ors[O];```