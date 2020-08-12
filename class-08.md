
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

- **CSS Frameworks**:its provid the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.