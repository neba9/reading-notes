
# WHAT IS AN OBJECT?

- Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

- If a **variable** is part of an object, it is called a **property**. Properties tell us about the object, such as the name of a hotel or the number of rooms it has.Each individual hotel might have a different name and a different number of rooms. 

- If a **function** is part of an object, it is called a **method**. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms.

- ex: ```var:'Quay',{```
      ```rooms:40,```
      ```booked: 24,```
      ```gym: true,```
      ```roomTyoe: ['twin', 'double', 'suite'],```

      ```checkAvaility: fubction() {```
      ```return this.room -this.booked;```
      ```}```
      ```};```

- Above you can see a **hotel** object. The object contains the following key/value pairs:
**PROPERTIES**: KEY VALUE
                **name** string
                **rooms** number
                **booked** number
                **gym** Boolean
                **room** Types array

**METHODS**: **checkAvailability** function

- Programmers use a lot of name/value pairs:
1. **HTML** uses **attribute** names and values.

2. **CSS** uses **property** names and values.

3. In JavaScript:
  
  - **Variables** have a name and you can assign them a value of a string, number, or Boolean.

  - **Arrays** have a name and a group of values. (Each item in an array is a name/value pair because it has an index number and a value.)

  - **Named functions** have a name and value that is a set of statements to run if the function is called.

  - **Objects** consist of a set of name/value pairs (but the names are referred to as keys).

- to access the properties or methods of an object using **dot** notation.we can also access properties usnig square brackets.

- to access a property or method of an object you use the name of the object,followed by a petiod,then the name of the property or method you want to access,this is known as **dot notation**.

- the period is known as the **member opretator**.the property or method on its right is a member of the object on its left. here, two variables are created to hold the hotel name and number of vacant rooms.

```var hotelName = hotel.name;```
```var roomsFree = hotel.checkAvailablitiy();```

- you can also access the properties of an object but not its method using ssquare brackt syntax.this time the object name is followed by square brackets, and the property name is inside them.

- Ex: ```var hotelName = hotel['name'];```

- **CREATING OBJECTS USING LITERAL NOTATION**

```var hotel = {```
```name: 'Quay',```
```rooms : 40,```
```booked: 25,```
```checkAvailability: function() {```
```return this.rooms - this.booked;```
```}```
```} ;```
```var elName = document .getElementByld('hotelName');```
```elName.textContent =hotel .name;```
```var elRooms = document.getElementByid{'rooms');```
```elRooms .textContent = hotel .checkAvailability();```

# Document Object Model(DOM):

- The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

- The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.It is implemented by all major browser makers, and covers two primary areas:

1. **MAKING A MODEL OF THE HTML PAGE**:When the browser loads a web page, it creates a model of the page in memory.The DOM specifies the way in which the browser should structure this model using a **DOM tree**.

2. **ACCESSING AND CHANGING THE HTML PAGE**:The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser.

- As a browser loads a web page, it creates a model of that page.The model is called a DOM tree, and it is stored in the browsers' memory. It consists of **four main types of nodes**.

1. **THE DOCUMENT NODE**:At the top of the tree a document node is added; it represents the entire page (and also corresponds to the document object,

2. **ELEMENT NODES**:HTML elements describe the structure of an HTML page. (The ```<h l > - <h6>``` elements describe what parts are headings; the ```<p>```tags indicate where paragraphs of text start and finish; and so on.)

3. **ATTRIBUTE NODES**:The opening tags of HTML elements can carry attributes and these are represented by attribute
nodes in the DOM tree.

4. **TEXT NODES**:Once you have accessed an element node, you can then reach the text within that element. This is
stored in its own text node.

- Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser.

- **WORKING WITH THE DOM TREE**:Accessing and updating the DOM tree involves two steps:

1. Locate the node that represents the element you want to work with.

2. Use its text content, child elements, and attributes.

- methods that find element in the DOM tree are calleed DOM queries.when you neeed to work with an element more than once,you should use a variable to store jthe resalt of this query.

- Ex: ```var itemOne = getElementById('one');```

- DOM queries may return one element, or they may return a Nodelist,which is a collection of nodes.

- getElementById()and querySelectr() acn both search an entire document and return individual elements.both use a similar syntax.

- Ex:```document.getElementById('one')```

- **document** refers to the document **object**,you always have to access individual element via the document object.

- **getElementById()**: **method** indicates thas you wwant to fin an element of its od attribute.

- **member oprator(.)**: the dot notation indicate that the method (on the right) is being  applied to the node on the left of the period.

- **parameter('one')**: the method needs to know thw value of the id attribute on the element you want.it is the parameter of the method.

- There are two ways to select an element from a Nodelist:

1. **The item() method**:Nodelists have a method called item() which will return an individual node from the
Node list. You specify the index number of the element you want as a parameter of the method (inside the parentheses)

- Ex:```var elements = document.getElementsByClassName     ('hot')```
```if (element.length >= 1){```
  ```var firstItem = element.item(0);```
```}```

2. **array syntax**:Both require the index number of the element you want.you can access individual nodes using a square bracket syntax using a square bracket syntax similar to that used to access individual item that follow the nedelist.

- Ex: ```var elements = document.getElementsByClassName('hot');```
```if (elements.length >= 1){```
  ```var firstItem = element[0];```
```}```

- **LOOPING THROUGH A NODELIST**:If you want to apply the same code to numerous elements,looping through a Nodelist is a powerful technique.JAVASCRIPT It involves finding out how many items are in the Nodelist, and then setting a counter to loop through them, one-by-one.

- Ex: ```var hotItems = document.querySelector All(,li.hot');```
```if (hotItems.length > 0) {```

```for (var i=0; i<hotItems.length; i++>){```
```hotItems[i].className = 'cool';```
```}```
```}```

