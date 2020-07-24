
# LISTS

- **ListsHTML**: provides us with three different types:

1. **Ordered lists**: are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.

- Ex: ```The ordered list is created with the <ol>``` element. Each item in the list is placed between an opening ```<li> tag and a closing </li>``` tag. (The li stands for list item.)

2. **Unordered lists**: are lists that begin with a bullet point, rather than characters that indicate order.

Ex: The unordered list is created with the ```<ul> element.Each item in the list is placed between an opening <li> tag and a closing </li>``` tag. (The li stands for list item.)

3. **Definition lists**: are made up of a set of terms along with the definitions for each of those terms. 

Ex: The definition list is created with the ```<dl>``` element and usually consists of a series of terms and their definitions.Inside the ```<dl> element you will usually see pairs of <dt> and <dd> elements.<dt> This is used to contain the term being defined (the definition term). <dd>``` This is used to contain the definition.

- **nested lists**: You can put a second list inside an ```<li>``` element to create a sublist or nested list.

# Boxes

- By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the **height and width** properties.The most popular ways to specify the size of a box are to use pixels percentages, or ems.

- **Limiting Width**: Some page designs expand and shrink to fit the size of the user's screen.
- **min-width**:property specifies the smallest size a box can be displayed at when the browser window is narrow,
- **max-width**: property indicates the maximum width a box can stretch to when the browser window is wide.

# Border, Margin and Padding

- Every box has three aveilable properties that can be adjusted to control its appearance.

- **Boredr**:Every boxes has a border evenif it is not visible or is specified to be 0 pixels wide.the borde separates the edge of one box from anather.Border: has different property.border-width, border-style, border-color.  

- **Margin**: Margin sit outsite the edge of the berder. you can set width of a margin to create a gap between the border of two adjacent boxes.

- The margin property controls the gap between boxes. Its value
is commonly given in pixels, although you may also use percentages or ems.

- You can specify values for each side of a box using:
     
     - margin-top
     - margin-right
     - margin-bottom
     -  margin-left


-**Padding**: Padding is the space between the border of a box and any content contained within it.adding padding can increase the readability of its contents.
- The padding property allows you to specify how much space should appear between the content of an element and its border.You can specify different values for each side of a box using:
     
     - padding-top
     - padding-right
     - padding-bottom
     - padding-left

### Centering content

- If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto.

- Ex: ```body { text-align: center;}```

### Hiding Boxes visibility

- The visibility property allows you to hide boxes from users but It leaves a space where the element would have been.This property can take two values:
**hidden** This hides the element.**visible** This shows the element.

# if else statmentes: 

- The if else statments checks a condition.if it resolves to **true** the first code block is excuted.if the condition resolves to **false**the second code block is runinstead.

- Ex: ```if (score >=50){congratulate();```
       ```}else {```
         ```encourage();```
       ```};```

- Here you can see that an if ...else statement allows you to provide two sets of code:
1. one set if the condition evaluates to **true**

2. another set if the condition is **false**

# Loops

- Loops:check a condition.if it returns,a code block will run.then the condition will be checked again if it still returns ture,the code block will run again.it repeats untik the condition returns false.Thre are three common types of loops.

1. For Loops:if you need torun code a spesific number of times,we useit,in the for loop the condition is usually a counter which is used to tell how many times the loop should run.

2. While Loop: if you do not know how many times the code should run,we useit,the condition can be somthing other than a counter,and the code will continue to loop for as long as the condition is true.

3. Do While Loop: is very similar to the while loop,but has one key difference :it will always run the statments inside the curly braces at least once,even if the condition evaluates to false.

-Ex: ```for (var i = 0; i < 10 ; i++){```
  ```document.write(i);```
```}```
- var i = 0; initialization ceart a variable and set it to 0.
- i < 10; condition loop should continue to run until the counter reaches a spesified number. 
- i++: update every time the loop has run the statmentes in the curly braces,it adds one to the counter.
